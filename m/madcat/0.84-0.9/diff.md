# Comparing `tmp/madcat-0.84.tar.gz` & `tmp/madcat-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madcat-0.84.tar", last modified: Mon Jun 26 18:36:52 2023, max compression
+gzip compressed data, was "madcat-0.9.tar", last modified: Fri Feb 10 23:56:18 2023, max compression
```

## Comparing `madcat-0.84.tar` & `madcat-0.9.tar`

### file list

```diff
@@ -1,270 +1,121 @@
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.109577 madcat-0.84/
--rw-r--r--   0 amitosi    (501) staff       (20)      190 2023-06-26 18:36:52.109398 madcat-0.84/PKG-INFO
--rw-r--r--   0 amitosi    (501) staff       (20)     1367 2023-03-22 15:02:11.000000 madcat-0.84/README.md
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.064995 madcat-0.84/chester/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.84/chester/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.065905 madcat-0.84/chester/cleaning/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.84/chester/cleaning/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1726 2023-02-14 11:01:28.000000 madcat-0.84/chester/cleaning/cleaner_handler.py
--rw-r--r--   0 amitosi    (501) staff       (20)     8913 2023-02-14 11:10:19.000000 madcat-0.84/chester/cleaning/cleaning_func.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.066185 madcat-0.84/chester/data/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-16 07:01:02.000000 madcat-0.84/chester/data/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.066396 madcat-0.84/chester/data_loader/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.84/chester/data_loader/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      693 2023-02-10 12:03:58.000000 madcat-0.84/chester/data_loader/webtext_data.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.066745 madcat-0.84/chester/feature_analyzing/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.84/chester/feature_analyzing/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     7767 2023-02-12 13:00:40.000000 madcat-0.84/chester/feature_analyzing/feature_correlation.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.068283 madcat-0.84/chester/feature_stats/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/feature_stats/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6113 2023-05-28 15:36:04.000000 madcat-0.84/chester/feature_stats/categorical_stats.py
--rw-r--r--   0 amitosi    (501) staff       (20)      214 2023-02-08 10:13:48.000000 madcat-0.84/chester/feature_stats/feature_stats.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5521 2023-02-14 12:45:27.000000 madcat-0.84/chester/feature_stats/numeric_stats.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2152 2023-03-21 07:33:39.000000 madcat-0.84/chester/feature_stats/text_stats.py
--rw-r--r--   0 amitosi    (501) staff       (20)     7292 2023-02-20 17:02:27.000000 madcat-0.84/chester/feature_stats/time_series_stats.py
--rw-r--r--   0 amitosi    (501) staff       (20)      646 2023-02-14 14:21:02.000000 madcat-0.84/chester/feature_stats/utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.069852 madcat-0.84/chester/features_engineering/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.84/chester/features_engineering/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2222 2023-02-05 11:09:58.000000 madcat-0.84/chester/features_engineering/bag_of_words.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2218 2023-03-07 08:09:18.000000 madcat-0.84/chester/features_engineering/corex.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6275 2023-03-07 06:57:19.000000 madcat-0.84/chester/features_engineering/fe_nlp.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4745 2023-03-21 07:33:39.000000 madcat-0.84/chester/features_engineering/feature_handler.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3355 2023-03-07 07:20:49.000000 madcat-0.84/chester/features_engineering/features_handler.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1970 2023-02-05 11:09:58.000000 madcat-0.84/chester/features_engineering/tfidf.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.072423 madcat-0.84/chester/features_engineering/time_series/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-15 07:10:16.000000 madcat-0.84/chester/features_engineering/time_series/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1829 2023-02-17 09:22:41.000000 madcat-0.84/chester/features_engineering/time_series/cyclic_features_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4455 2023-02-16 13:45:22.000000 madcat-0.84/chester/features_engineering/time_series/event_counter.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1909 2023-02-27 19:09:23.000000 madcat-0.84/chester/features_engineering/time_series/feature_elimination_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5324 2023-02-16 14:23:15.000000 madcat-0.84/chester/features_engineering/time_series/frequencies_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5317 2023-02-18 11:46:20.000000 madcat-0.84/chester/features_engineering/time_series/get_time_freqeuency_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4379 2023-02-16 14:20:54.000000 madcat-0.84/chester/features_engineering/time_series/moving_metric_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4129 2023-02-16 10:20:17.000000 madcat-0.84/chester/features_engineering/time_series/static_features_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4907 2023-02-20 16:14:11.000000 madcat-0.84/chester/features_engineering/time_series/ts_feature_extraction.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1013 2023-02-17 13:51:59.000000 madcat-0.84/chester/features_engineering/time_series/ts_features_extraction.py
--rw-r--r--   0 amitosi    (501) staff       (20)      379 2023-02-17 14:38:52.000000 madcat-0.84/chester/features_engineering/time_series/ts_utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.072770 madcat-0.84/chester/model_analyzer/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.84/chester/model_analyzer/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)    11364 2023-02-19 08:56:08.000000 madcat-0.84/chester/model_analyzer/model_analysis.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.073652 madcat-0.84/chester/model_monitor/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/model_monitor/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      887 2023-02-10 12:10:10.000000 madcat-0.84/chester/model_monitor/calculate_scores_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6324 2023-02-14 17:08:34.000000 madcat-0.84/chester/model_monitor/error_prediction.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4656 2023-02-14 16:36:28.000000 madcat-0.84/chester/model_monitor/model_boostrap.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.074185 madcat-0.84/chester/model_training/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.84/chester/model_training/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3427 2023-02-05 19:57:36.000000 madcat-0.84/chester/model_training/data_preparation.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2149 2023-02-11 16:14:05.000000 madcat-0.84/chester/model_training/model_utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.075013 madcat-0.84/chester/model_training/models/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.84/chester/model_training/models/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.077652 madcat-0.84/chester/model_training/models/chester_models/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/model_training/models/chester_models/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1977 2023-02-11 10:13:40.000000 madcat-0.84/chester/model_training/models/chester_models/base_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2160 2023-02-10 12:10:10.000000 madcat-0.84/chester/model_training/models/chester_models/base_model_utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.078144 madcat-0.84/chester/model_training/models/chester_models/baseline/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/model_training/models/chester_models/baseline/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1012 2023-02-12 12:18:36.000000 madcat-0.84/chester/model_training/models/chester_models/baseline/baseline_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3519 2023-02-10 12:10:10.000000 madcat-0.84/chester/model_training/models/chester_models/baseline/baseline_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1965 2023-02-12 12:18:36.000000 madcat-0.84/chester/model_training/models/chester_models/best_baseline_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1522 2023-02-10 12:10:10.000000 madcat-0.84/chester/model_training/models/chester_models/best_catboost.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1769 2023-02-10 12:10:10.000000 madcat-0.84/chester/model_training/models/chester_models/best_linear_regression.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1917 2023-02-14 15:09:08.000000 madcat-0.84/chester/model_training/models/chester_models/best_logistic_regression.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2782 2023-02-14 15:25:23.000000 madcat-0.84/chester/model_training/models/chester_models/best_model.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.078542 madcat-0.84/chester/model_training/models/chester_models/catboost/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/model_training/models/chester_models/catboost/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1176 2023-02-10 12:10:10.000000 madcat-0.84/chester/model_training/models/chester_models/catboost/catboost_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)    10528 2023-03-11 11:42:24.000000 madcat-0.84/chester/model_training/models/chester_models/catboost/catboost_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1750 2023-02-10 12:10:30.000000 madcat-0.84/chester/model_training/models/chester_models/hp_generator.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.079147 madcat-0.84/chester/model_training/models/chester_models/linear_regression/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/model_training/models/chester_models/linear_regression/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2429 2023-02-17 12:12:20.000000 madcat-0.84/chester/model_training/models/chester_models/linear_regression/linear_regression.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6891 2023-02-10 12:10:10.000000 madcat-0.84/chester/model_training/models/chester_models/linear_regression/linear_regression_utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.079741 madcat-0.84/chester/model_training/models/chester_models/logistic_regression/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/model_training/models/chester_models/logistic_regression/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2542 2023-02-14 15:54:46.000000 madcat-0.84/chester/model_training/models/chester_models/logistic_regression/logistic_regression_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6637 2023-02-10 12:10:10.000000 madcat-0.84/chester/model_training/models/chester_models/logistic_regression/logistic_regression_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2040 2023-02-05 11:09:58.000000 madcat-0.84/chester/model_training/models/cv_training.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4764 2023-02-05 11:09:58.000000 madcat-0.84/chester/model_training/models/lstm.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1155 2023-02-10 12:20:48.000000 madcat-0.84/chester/model_training/models/scoring.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.080347 madcat-0.84/chester/post_model_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/post_model_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)    12668 2023-02-23 10:52:06.000000 madcat-0.84/chester/post_model_analysis/post_model_analysis_class.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1492 2023-02-11 16:14:05.000000 madcat-0.84/chester/post_model_analysis/post_regression.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.081502 madcat-0.84/chester/pre_model_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/pre_model_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)    15538 2023-03-11 12:30:17.000000 madcat-0.84/chester/pre_model_analysis/categorical.py
--rw-r--r--   0 amitosi    (501) staff       (20)    15136 2023-03-21 11:25:00.000000 madcat-0.84/chester/pre_model_analysis/numerics.py
--rw-r--r--   0 amitosi    (501) staff       (20)     9856 2023-02-19 19:27:25.000000 madcat-0.84/chester/pre_model_analysis/target.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3383 2023-02-20 16:04:59.000000 madcat-0.84/chester/pre_model_analysis/time_series.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.082098 madcat-0.84/chester/preprocessing/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.84/chester/preprocessing/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5096 2023-02-14 11:12:55.000000 madcat-0.84/chester/preprocessing/preprocessing_func.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1661 2023-03-07 06:13:34.000000 madcat-0.84/chester/preprocessing/preprocessor_handler.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.083224 madcat-0.84/chester/run/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-08 09:40:57.000000 madcat-0.84/chester/run/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1786 2023-02-11 11:52:10.000000 madcat-0.84/chester/run/chapter_titles.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2779 2023-02-08 21:21:02.000000 madcat-0.84/chester/run/feature_attention_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)    16206 2023-03-21 07:53:41.000000 madcat-0.84/chester/run/full_run.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5035 2023-03-21 07:33:39.000000 madcat-0.84/chester/run/user_classes.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.084077 madcat-0.84/chester/run_manual_chester/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 13:32:50.000000 madcat-0.84/chester/run_manual_chester/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3638 2023-05-29 14:23:09.000000 madcat-0.84/chester/run_manual_chester/bad_data.py
--rw-r--r--   0 amitosi    (501) staff       (20)      602 2023-06-10 12:20:58.000000 madcat-0.84/chester/run_manual_chester/bad_data2.py
--rw-r--r--   0 amitosi    (501) staff       (20)    19306 2023-03-21 07:53:41.000000 madcat-0.84/chester/run_manual_chester/manual_run.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.086512 madcat-0.84/chester/text_stats_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/text_stats_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1261 2023-02-14 11:53:21.000000 madcat-0.84/chester/text_stats_analysis/common_words.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3708 2023-03-07 08:42:30.000000 madcat-0.84/chester/text_stats_analysis/corex_topics.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4446 2023-03-21 07:33:39.000000 madcat-0.84/chester/text_stats_analysis/data_quality.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3466 2023-02-14 12:12:27.000000 madcat-0.84/chester/text_stats_analysis/key_sentences.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3663 2023-02-14 12:20:36.000000 madcat-0.84/chester/text_stats_analysis/keywords_extraction.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1951 2023-02-14 14:04:54.000000 madcat-0.84/chester/text_stats_analysis/sentiment.py
--rw-r--r--   0 amitosi    (501) staff       (20)    10355 2023-03-21 07:33:39.000000 madcat-0.84/chester/text_stats_analysis/smart_text_analyzer.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4118 2023-03-21 07:33:39.000000 madcat-0.84/chester/text_stats_analysis/text_summary.py
--rw-r--r--   0 amitosi    (501) staff       (20)      526 2023-02-11 16:14:05.000000 madcat-0.84/chester/text_stats_analysis/word_cloud.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5304 2023-02-19 09:26:17.000000 madcat-0.84/chester/util.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.086939 madcat-0.84/chester/utils/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.84/chester/utils/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.087520 madcat-0.84/chester/zero_break/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.84/chester/zero_break/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)       89 2023-02-05 11:09:58.000000 madcat-0.84/chester/zero_break/get_or_else.py
--rw-r--r--   0 amitosi    (501) staff       (20)     8952 2023-03-21 11:17:36.000000 madcat-0.84/chester/zero_break/problem_specification.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1694 2023-03-11 12:21:56.000000 madcat-0.84/chester/zero_break/text_detector.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.089135 madcat-0.84/databots/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-26 15:33:22.000000 madcat-0.84/databots/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.089726 madcat-0.84/databots/brainstorming/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-25 16:47:58.000000 madcat-0.84/databots/brainstorming/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      826 2023-03-26 16:04:03.000000 madcat-0.84/databots/brainstorming/code_review.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1514 2023-03-26 16:57:50.000000 madcat-0.84/databots/brainstorming/task_extends.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.090234 madcat-0.84/databots/code_development/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-25 15:32:25.000000 madcat-0.84/databots/code_development/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1014 2023-03-26 17:41:52.000000 madcat-0.84/databots/code_development/develop.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1585 2023-03-26 17:17:47.000000 madcat-0.84/databots/code_development/error_handling.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.090819 madcat-0.84/databots/code_health/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-25 11:26:20.000000 madcat-0.84/databots/code_health/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      639 2023-03-26 17:04:27.000000 madcat-0.84/databots/code_health/clean_not_code.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3561 2023-03-26 17:44:28.000000 madcat-0.84/databots/code_health/code_organization.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.091054 madcat-0.84/databots/code_restructure/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-26 15:32:56.000000 madcat-0.84/databots/code_restructure/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.091253 madcat-0.84/databots/code_to_file/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-23 10:11:18.000000 madcat-0.84/databots/code_to_file/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      616 2023-03-25 10:59:25.000000 madcat-0.84/databots/code_to_file/code_to_file.py
--rw-r--r--   0 amitosi    (501) staff       (20)      896 2023-03-26 12:22:14.000000 madcat-0.84/databots/ex1.py
--rw-r--r--   0 amitosi    (501) staff       (20)      696 2023-03-26 12:33:33.000000 madcat-0.84/databots/example.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1451 2023-03-26 17:42:37.000000 madcat-0.84/databots/from_scratch.py
--rw-r--r--   0 amitosi    (501) staff       (20)      297 2023-03-27 09:13:40.000000 madcat-0.84/databots/games.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.091678 madcat-0.84/databots/modify_code/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-26 09:30:00.000000 madcat-0.84/databots/modify_code/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      893 2023-03-26 15:05:07.000000 madcat-0.84/databots/modify_code/code_modification.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1374 2023-03-26 16:34:10.000000 madcat-0.84/databots/modify_file.py
--rw-r--r--   0 amitosi    (501) staff       (20)      801 2023-03-28 12:20:39.000000 madcat-0.84/databots/pg.py
--rw-r--r--   0 amitosi    (501) staff       (20)      383 2023-03-25 16:51:45.000000 madcat-0.84/databots/utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.094091 madcat-0.84/diamond/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-27 12:32:41.000000 madcat-0.84/diamond/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.094429 madcat-0.84/diamond/data_augmentation/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-27 13:11:53.000000 madcat-0.84/diamond/data_augmentation/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     9190 2023-03-10 09:26:49.000000 madcat-0.84/diamond/data_augmentation/augmentation.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.094769 madcat-0.84/diamond/face_detection/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-08 15:04:20.000000 madcat-0.84/diamond/face_detection/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2932 2023-03-21 07:33:39.000000 madcat-0.84/diamond/face_detection/face_image_.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.095439 madcat-0.84/diamond/image_caption/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-04 08:54:21.000000 madcat-0.84/diamond/image_caption/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2612 2023-03-21 07:33:39.000000 madcat-0.84/diamond/image_caption/image_caption_class.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1800 2023-03-04 15:58:09.000000 madcat-0.84/diamond/image_caption/utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.095939 madcat-0.84/diamond/image_data_info/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-27 12:42:29.000000 madcat-0.84/diamond/image_data_info/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      476 2023-03-01 17:18:05.000000 madcat-0.84/diamond/image_data_info/image_info.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.096325 madcat-0.84/diamond/image_object_detection/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-07 17:14:36.000000 madcat-0.84/diamond/image_object_detection/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3029 2023-03-21 07:33:39.000000 madcat-0.84/diamond/image_object_detection/image_object_class.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4767 2023-03-21 07:33:38.000000 madcat-0.84/diamond/manual_run.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2437 2023-03-21 07:33:38.000000 madcat-0.84/diamond/manual_run2.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1539 2023-03-10 09:08:39.000000 madcat-0.84/diamond/manual_run3.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2756 2023-03-21 07:33:39.000000 madcat-0.84/diamond/manual_run4.py
--rw-r--r--   0 amitosi    (501) staff       (20)      322 2023-03-21 07:33:39.000000 madcat-0.84/diamond/manual_run5.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.097204 madcat-0.84/diamond/model_training/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-27 14:51:50.000000 madcat-0.84/diamond/model_training/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1335 2023-03-02 19:46:53.000000 madcat-0.84/diamond/model_training/best_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)      529 2023-02-28 17:45:14.000000 madcat-0.84/diamond/model_training/model_results.py
--rw-r--r--   0 amitosi    (501) staff       (20)     8691 2023-03-21 07:33:39.000000 madcat-0.84/diamond/model_training/train_single.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.097604 madcat-0.84/diamond/post_model_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-28 15:22:38.000000 madcat-0.84/diamond/post_model_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5917 2023-03-05 16:01:12.000000 madcat-0.84/diamond/post_model_analysis/post_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4714 2023-03-21 07:33:39.000000 madcat-0.84/diamond/run.py
--rw-r--r--   0 amitosi    (501) staff       (20)    10986 2023-03-21 07:33:39.000000 madcat-0.84/diamond/user_classes.py
--rw-r--r--   0 amitosi    (501) staff       (20)      667 2023-03-03 19:00:26.000000 madcat-0.84/diamond/utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.097889 madcat-0.84/example_notebooks/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-11 13:38:57.000000 madcat-0.84/example_notebooks/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2981 2023-03-11 15:08:39.000000 madcat-0.84/example_notebooks/main.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.098710 madcat-0.84/madcat.egg-info/
--rw-r--r--   0 amitosi    (501) staff       (20)      190 2023-06-26 18:36:52.000000 madcat-0.84/madcat.egg-info/PKG-INFO
--rw-r--r--   0 amitosi    (501) staff       (20)     8135 2023-06-26 18:36:52.000000 madcat-0.84/madcat.egg-info/SOURCES.txt
--rw-r--r--   0 amitosi    (501) staff       (20)        1 2023-06-26 18:36:52.000000 madcat-0.84/madcat.egg-info/dependency_links.txt
--rw-r--r--   0 amitosi    (501) staff       (20)      347 2023-06-26 18:36:52.000000 madcat-0.84/madcat.egg-info/requires.txt
--rw-r--r--   0 amitosi    (501) staff       (20)       58 2023-06-26 18:36:52.000000 madcat-0.84/madcat.egg-info/top_level.txt
--rw-r--r--   0 amitosi    (501) staff       (20)       38 2023-06-26 18:36:52.109627 madcat-0.84/setup.cfg
--rw-r--r--   0 amitosi    (501) staff       (20)      559 2023-06-26 18:36:43.000000 madcat-0.84/setup.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.099186 madcat-0.84/tamtam/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 07:37:31.000000 madcat-0.84/tamtam/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.100365 madcat-0.84/tamtam/ab_feature_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-23 10:02:44.000000 madcat-0.84/tamtam/ab_feature_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      541 2023-02-23 10:19:25.000000 madcat-0.84/tamtam/ab_feature_analysis/ab_catboost.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1923 2023-03-21 07:53:41.000000 madcat-0.84/tamtam/ab_feature_analysis/ab_feature_analysis_class.py
--rw-r--r--   0 amitosi    (501) staff       (20)      348 2023-02-23 10:19:25.000000 madcat-0.84/tamtam/ab_feature_analysis/ab_partial_plot.py
--rw-r--r--   0 amitosi    (501) staff       (20)      402 2023-02-23 10:19:25.000000 madcat-0.84/tamtam/ab_feature_analysis/ab_tree_class.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.100762 madcat-0.84/tamtam/ab_info/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 07:44:45.000000 madcat-0.84/tamtam/ab_info/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4011 2023-02-23 21:52:11.000000 madcat-0.84/tamtam/ab_info/ab_class.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.101286 madcat-0.84/tamtam/allocation_calculation/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 13:01:46.000000 madcat-0.84/tamtam/allocation_calculation/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1937 2023-02-22 14:13:02.000000 madcat-0.84/tamtam/allocation_calculation/bias_class.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.101702 madcat-0.84/tamtam/delta_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-23 07:37:32.000000 madcat-0.84/tamtam/delta_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6199 2023-02-23 21:48:17.000000 madcat-0.84/tamtam/delta_analysis/delta_class.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2517 2023-02-23 21:45:56.000000 madcat-0.84/tamtam/manual_run.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.102105 madcat-0.84/tamtam/metrics_correlation/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 14:27:03.000000 madcat-0.84/tamtam/metrics_correlation/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2350 2023-02-23 14:45:57.000000 madcat-0.84/tamtam/metrics_correlation/metric_class.py
--rw-r--r--   0 amitosi    (501) staff       (20)      964 2023-02-23 14:45:57.000000 madcat-0.84/tamtam/run.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.102507 madcat-0.84/tamtam/user_class/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 07:41:13.000000 madcat-0.84/tamtam/user_class/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1895 2023-02-23 11:53:41.000000 madcat-0.84/tamtam/user_class/user_class.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.103136 madcat-0.84/tamtam/utils/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 10:08:15.000000 madcat-0.84/tamtam/utils/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)       54 2023-02-22 16:12:56.000000 madcat-0.84/tamtam/utils/column_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)       59 2023-02-22 16:24:31.000000 madcat-0.84/tamtam/utils/utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.105442 madcat-0.84/udi/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-21 07:33:39.000000 madcat-0.84/udi/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1678 2023-03-22 08:19:21.000000 madcat-0.84/udi/manual_run.py
--rw-r--r--   0 amitosi    (501) staff       (20)      935 2023-03-21 13:38:45.000000 madcat-0.84/udi/manual_run2.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1433 2023-03-22 14:50:20.000000 madcat-0.84/udi/manual_run3.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1429 2023-03-22 08:49:57.000000 madcat-0.84/udi/manual_run4.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2064 2023-03-22 08:36:39.000000 madcat-0.84/udi/run.py
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-21 07:33:39.000000 madcat-0.84/udi/speech_recognition.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.105644 madcat-0.84/udi/speech_to_text/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-22 08:14:49.000000 madcat-0.84/udi/speech_to_text/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1704 2023-03-22 13:44:37.000000 madcat-0.84/udi/speech_to_text/speech_to_text_class.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.107000 madcat-0.84/vis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-08 09:59:19.000000 madcat-0.84/vis/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.107396 madcat-0.84/vis/frames_to_video/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-16 07:43:50.000000 madcat-0.84/vis/frames_to_video/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1066 2023-03-16 07:44:29.000000 madcat-0.84/vis/frames_to_video/video_creator_class.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.107823 madcat-0.84/vis/grayscale/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-16 06:48:58.000000 madcat-0.84/vis/grayscale/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1827 2023-03-16 09:22:35.000000 madcat-0.84/vis/grayscale/grayscale.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1100 2023-03-21 07:33:39.000000 madcat-0.84/vis/manual_run.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.108239 madcat-0.84/vis/object_video_tracker/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-21 07:33:39.000000 madcat-0.84/vis/object_video_tracker/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1761 2023-03-21 07:33:39.000000 madcat-0.84/vis/object_video_tracker/object_tracker.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.108538 madcat-0.84/vis/reversed_order/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-16 07:58:09.000000 madcat-0.84/vis/reversed_order/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1537 2023-03-16 09:22:04.000000 madcat-0.84/vis/reversed_order/video_revereser.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2601 2023-03-21 07:33:39.000000 madcat-0.84/vis/run.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3340 2023-03-16 07:27:30.000000 madcat-0.84/vis/user_classes.py
--rw-r--r--   0 amitosi    (501) staff       (20)      667 2023-03-03 19:00:26.000000 madcat-0.84/vis/utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.108804 madcat-0.84/vis/video_data_info/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-08 09:59:45.000000 madcat-0.84/vis/video_data_info/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      713 2023-03-21 07:33:39.000000 madcat-0.84/vis/video_player.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-06-26 18:36:52.109031 madcat-0.84/vis/video_zoom/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-16 08:19:21.000000 madcat-0.84/vis/video_zoom/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2480 2023-03-16 09:22:53.000000 madcat-0.84/vis/video_zoom/zoom_class.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.950087 madcat-0.9/
+-rw-r--r--   0 amitosi    (501) staff       (20)      187 2023-02-10 23:56:18.949776 madcat-0.9/PKG-INFO
+-rw-r--r--   0 amitosi    (501) staff       (20)     1104 2023-02-05 11:20:57.000000 madcat-0.9/README.md
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.922741 madcat-0.9/chester/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.9/chester/__init__.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.923426 madcat-0.9/chester/cleaning/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.9/chester/cleaning/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1387 2023-02-10 12:03:58.000000 madcat-0.9/chester/cleaning/cleaner_handler.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     8715 2023-02-10 12:03:58.000000 madcat-0.9/chester/cleaning/cleaning_func.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.923838 madcat-0.9/chester/data_loader/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.9/chester/data_loader/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      693 2023-02-10 12:03:58.000000 madcat-0.9/chester/data_loader/webtext_data.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.924236 madcat-0.9/chester/feature_analyzing/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.9/chester/feature_analyzing/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     7484 2023-02-10 12:03:58.000000 madcat-0.9/chester/feature_analyzing/feature_correlation.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.926368 madcat-0.9/chester/feature_stats/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/feature_stats/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5006 2023-02-10 12:03:58.000000 madcat-0.9/chester/feature_stats/categorical_stats.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      214 2023-02-08 10:13:48.000000 madcat-0.9/chester/feature_stats/feature_stats.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5153 2023-02-10 16:34:35.000000 madcat-0.9/chester/feature_stats/numeric_stats.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      633 2023-02-10 12:03:58.000000 madcat-0.9/chester/feature_stats/text_stats.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      151 2023-02-05 11:09:59.000000 madcat-0.9/chester/feature_stats/utils.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.928319 madcat-0.9/chester/features_engineering/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.9/chester/features_engineering/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2222 2023-02-05 11:09:58.000000 madcat-0.9/chester/features_engineering/bag_of_words.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2000 2023-02-05 11:09:58.000000 madcat-0.9/chester/features_engineering/corex.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5806 2023-02-08 16:47:51.000000 madcat-0.9/chester/features_engineering/fe_nlp.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3758 2023-02-10 12:03:58.000000 madcat-0.9/chester/features_engineering/feature_handler.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3220 2023-02-10 12:03:58.000000 madcat-0.9/chester/features_engineering/features_handler.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1970 2023-02-05 11:09:58.000000 madcat-0.9/chester/features_engineering/tfidf.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.928735 madcat-0.9/chester/model_analyzer/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.9/chester/model_analyzer/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    11337 2023-02-10 14:33:32.000000 madcat-0.9/chester/model_analyzer/model_analysis.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.929855 madcat-0.9/chester/model_monitor/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/model_monitor/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      887 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_monitor/calculate_scores_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5573 2023-02-10 23:39:51.000000 madcat-0.9/chester/model_monitor/error_prediction.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4328 2023-02-10 23:39:36.000000 madcat-0.9/chester/model_monitor/model_boostrap.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.930518 madcat-0.9/chester/model_training/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.9/chester/model_training/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3427 2023-02-05 19:57:36.000000 madcat-0.9/chester/model_training/data_preparation.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2133 2023-02-10 12:20:53.000000 madcat-0.9/chester/model_training/model_utils.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.931535 madcat-0.9/chester/model_training/models/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.9/chester/model_training/models/__init__.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.933571 madcat-0.9/chester/model_training/models/chester_models/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/model_training/models/chester_models/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1866 2023-02-09 10:51:53.000000 madcat-0.9/chester/model_training/models/chester_models/base_model.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2160 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/base_model_utils.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.934649 madcat-0.9/chester/model_training/models/chester_models/baseline/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/model_training/models/chester_models/baseline/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      948 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/baseline/baseline_model.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3519 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/baseline/baseline_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1963 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/best_baseline_model.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1522 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/best_catboost.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1769 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/best_linear_regression.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1909 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/best_logistic_regression.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2782 2023-02-09 10:53:47.000000 madcat-0.9/chester/model_training/models/chester_models/best_model.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.935195 madcat-0.9/chester/model_training/models/chester_models/catboost/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/model_training/models/chester_models/catboost/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1176 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/catboost/catboost_model.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    10018 2023-02-10 23:12:00.000000 madcat-0.9/chester/model_training/models/chester_models/catboost/catboost_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1750 2023-02-10 12:10:30.000000 madcat-0.9/chester/model_training/models/chester_models/hp_generator.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.935786 madcat-0.9/chester/model_training/models/chester_models/linear_regression/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/model_training/models/chester_models/linear_regression/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2437 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/linear_regression/linear_regression.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     6891 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/linear_regression/linear_regression_utils.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.936473 madcat-0.9/chester/model_training/models/chester_models/logistic_regression/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/model_training/models/chester_models/logistic_regression/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2435 2023-02-07 14:13:26.000000 madcat-0.9/chester/model_training/models/chester_models/logistic_regression/logistic_regression_model.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     6637 2023-02-10 12:10:10.000000 madcat-0.9/chester/model_training/models/chester_models/logistic_regression/logistic_regression_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2040 2023-02-05 11:09:58.000000 madcat-0.9/chester/model_training/models/cv_training.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4764 2023-02-05 11:09:58.000000 madcat-0.9/chester/model_training/models/lstm.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1155 2023-02-10 12:20:48.000000 madcat-0.9/chester/model_training/models/scoring.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.937195 madcat-0.9/chester/post_model_analysis/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/post_model_analysis/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    10055 2023-02-10 23:34:42.000000 madcat-0.9/chester/post_model_analysis/post_model_analysis_class.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1472 2023-02-10 12:22:11.000000 madcat-0.9/chester/post_model_analysis/post_regression.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.938235 madcat-0.9/chester/pre_model_analysis/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/pre_model_analysis/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    12849 2023-02-10 23:54:28.000000 madcat-0.9/chester/pre_model_analysis/categorical.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    13655 2023-02-10 23:55:29.000000 madcat-0.9/chester/pre_model_analysis/numerics.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2623 2023-02-10 23:44:23.000000 madcat-0.9/chester/pre_model_analysis/target.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.939547 madcat-0.9/chester/preprocessing/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.9/chester/preprocessing/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4927 2023-02-10 12:26:51.000000 madcat-0.9/chester/preprocessing/preprocessing_func.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1474 2023-02-10 11:56:52.000000 madcat-0.9/chester/preprocessing/preprocessor_handler.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.941260 madcat-0.9/chester/run/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-08 09:40:57.000000 madcat-0.9/chester/run/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1450 2023-02-10 12:03:58.000000 madcat-0.9/chester/run/chapter_titles.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2779 2023-02-08 21:21:02.000000 madcat-0.9/chester/run/feature_attention_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    10783 2023-02-10 22:46:35.000000 madcat-0.9/chester/run/full_run.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2621 2023-02-09 10:53:22.000000 madcat-0.9/chester/run/user_classes.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.941834 madcat-0.9/chester/run_manual_chester/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 13:32:50.000000 madcat-0.9/chester/run_manual_chester/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     7373 2023-02-10 09:55:58.000000 madcat-0.9/chester/run_manual_chester/manual_run.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.946847 madcat-0.9/chester/text_stats_analysis/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/text_stats_analysis/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1075 2023-02-10 22:54:25.000000 madcat-0.9/chester/text_stats_analysis/common_words.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2800 2023-02-10 23:14:03.000000 madcat-0.9/chester/text_stats_analysis/corex_topics.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3870 2023-02-10 23:50:35.000000 madcat-0.9/chester/text_stats_analysis/data_quality.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3301 2023-02-10 12:30:34.000000 madcat-0.9/chester/text_stats_analysis/key_sentences.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3468 2023-02-10 12:30:34.000000 madcat-0.9/chester/text_stats_analysis/keywords_extraction.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1744 2023-02-10 16:36:36.000000 madcat-0.9/chester/text_stats_analysis/sentiment.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     8525 2023-02-10 12:30:34.000000 madcat-0.9/chester/text_stats_analysis/smart_text_analyzer.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      510 2023-02-10 16:36:06.000000 madcat-0.9/chester/text_stats_analysis/word_cloud.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3532 2023-02-10 12:31:19.000000 madcat-0.9/chester/util.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.947313 madcat-0.9/chester/utils/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-0.9/chester/utils/__init__.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.948591 madcat-0.9/chester/zero_break/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-0.9/chester/zero_break/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)       89 2023-02-05 11:09:58.000000 madcat-0.9/chester/zero_break/get_or_else.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     6933 2023-02-10 12:31:19.000000 madcat-0.9/chester/zero_break/problem_specification.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1565 2023-02-10 12:31:19.000000 madcat-0.9/chester/zero_break/text_detector.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-02-10 23:56:18.949515 madcat-0.9/madcat.egg-info/
+-rw-r--r--   0 amitosi    (501) staff       (20)      187 2023-02-10 23:56:18.000000 madcat-0.9/madcat.egg-info/PKG-INFO
+-rw-r--r--   0 amitosi    (501) staff       (20)     4231 2023-02-10 23:56:18.000000 madcat-0.9/madcat.egg-info/SOURCES.txt
+-rw-r--r--   0 amitosi    (501) staff       (20)        1 2023-02-10 23:56:18.000000 madcat-0.9/madcat.egg-info/dependency_links.txt
+-rw-r--r--   0 amitosi    (501) staff       (20)      308 2023-02-10 23:56:18.000000 madcat-0.9/madcat.egg-info/requires.txt
+-rw-r--r--   0 amitosi    (501) staff       (20)        8 2023-02-10 23:56:18.000000 madcat-0.9/madcat.egg-info/top_level.txt
+-rw-r--r--   0 amitosi    (501) staff       (20)       38 2023-02-10 23:56:18.950142 madcat-0.9/setup.cfg
+-rw-r--r--   0 amitosi    (501) staff       (20)      559 2023-02-10 23:56:10.000000 madcat-0.9/setup.py
```

### Comparing `madcat-0.84/chester/cleaning/cleaning_func.py` & `madcat-0.9/chester/cleaning/cleaning_func.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import re
 import string
 import unicodedata
 from typing import List
 
 import pandas as pd
 
-from chester.util import get_stopwords, ReportCollector, REPORT_PATH
+from chester.util import get_stopwords
 
 
 def remove_punctuation(text: str) -> str:
     """Remove all punctuation from the given text."""
-    return str(text).translate(str(text).maketrans("", "", string.punctuation))
+    return text.translate(text.maketrans("", "", string.punctuation))
 
 
 def remove_numbers(text: str) -> str:
     """Remove all numbers from the given text."""
     return ''.join(c for c in text if not c.isdigit())
 
 
 def remove_whitespace(text: str) -> str:
     """Remove excess whitespace from the given text."""
-    return ' '.join(str(text).split())
+    return ' '.join(text.split())
 
 
 def remove_empty_lines(text: str):
     """Remove excess empty lines from the given text."""
-    lines = str(text).splitlines()
+    lines = text.splitlines()
     cleaned_text = '\n'.join([line for line in lines if line.strip()])
     return cleaned_text
 
 
 def lowercase(text: str) -> str:
     """Convert the given text to lowercase."""
     return text.lower()
@@ -115,15 +115,14 @@
     remove_stopwords_flag: a flag indicating whether to remove common words that do not contribute to the meaning of the text.
     stopwords: a list of words to remove from the text. Required if remove_stopwords_flag is True.
     remove_accented_characters_flag: a flag indicating whether to remove accented characters from the text.
     remove_special_characters_flag: a flag indicating whether to remove special characters from the text.
     remove_html_tags_flag: a flag indicating whether to remove HTML tags from the text.
     """
 
-    text = str(text)
     if remove_punctuation_flag:
         text = remove_punctuation(text)
     if remove_numbers_flag:
         text = remove_numbers(text)
     if remove_whitespace_flag:
         text = remove_whitespace(text)
     if remove_empty_line_flag:
@@ -170,15 +169,14 @@
         self.remove_stopwords_flag = remove_stopwords_flag
         self.stopwords = stopwords
         self.remove_accented_characters_flag = remove_accented_characters_flag
         self.remove_special_characters_flag = remove_special_characters_flag
         self.remove_html_tags_flag = remove_html_tags_flag
 
     def generate_report(self):
-        rc = ReportCollector(REPORT_PATH)
         report_str = ""
         if self.remove_punctuation_flag:
             report_str += "Removing punctuation, "
         if self.remove_numbers_flag:
             report_str += "Removing numbers, "
         if self.remove_whitespace_flag:
             report_str += "Removing whitespaces, "
@@ -195,17 +193,15 @@
             report_str += "Removing accented characters, "
         if self.remove_special_characters_flag:
             report_str += "Removing special characters, "
         if self.remove_html_tags_flag:
             report_str += "Removing html tags, "
         if report_str:
             report_str = report_str[:-2]
-            title_to_print = f"The following cleaning steps will be applied to clean column '{self.text_column}': {report_str}."
-            print(title_to_print)
-            rc.save_text(title_to_print)
+            print(f"The following cleaning steps will be applied to clean column '{self.text_column}': {report_str}.")
         else:
             print("No cleaning steps selected.")
 
 
 def clean_text_df(text_cleaner: TextCleaner) -> pd.DataFrame:
     df = text_cleaner.df
     text_col = text_cleaner.text_column
```

### Comparing `madcat-0.84/chester/data_loader/webtext_data.py` & `madcat-0.9/chester/data_loader/webtext_data.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/feature_analyzing/feature_correlation.py` & `madcat-0.9/chester/feature_analyzing/feature_correlation.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,28 +79,26 @@
     def correlation_matrix(self):
         print(correlation_matrix_message)
         corr = self.df.corr()
         plt.figure(figsize=(10, 8))
         plt.title("Feature correlation matrix")
         sns.heatmap(corr, annot=True)
         plt.show()
-        plt.close()
         return corr
 
     def tsne_plot(self, n_components=2, perplexity=30.0, n_iter=1000):
         print(tsne_plot_message)
         from sklearn.manifold import TSNE
         X = self.df.drop(columns=self.target_column)
         y = self.df[self.target_column]
         tsne = TSNE(n_components=n_components, perplexity=perplexity, n_iter=n_iter)
         X_tsne = tsne.fit_transform(X)
         plt.scatter(X_tsne[:, 0], X_tsne[:, 1], c=y)
         plt.title("t-SNE Plot of Features and Target Label")
         plt.show()
-        plt.close()
 
     def top_n_pairplot(self, N=4, trimming_left=0.05, trimming_right=0.05):
         if trimming_left > 0:
             print(f"left trimming {100 * trimming_left}% ")
         if trimming_right > 0:
             print(f"right trimming {100 * trimming_right}% ")
         import seaborn as sns
@@ -108,15 +106,14 @@
         top_n_features = corr.nlargest(N, self.target_column).index
         top_n_features = top_n_features.drop(self.target_column)
         X = self.df[top_n_features]
         X = X.dropna()
         X = X[(X > X.quantile(trimming_left)) & (X < X.quantile(1 - trimming_right))]
         sns.pairplot(X)
         plt.show()
-        plt.close()
 
     def chi_square_test(self, feature):
         from scipy.stats import chi2_contingency
         X = self.df[[feature, self.target_column]]
         X = X.dropna()
         crosstab = pd.crosstab(X[feature], X[self.target_column])
         chi2, p, dof, expected = chi2_contingency(crosstab)
@@ -149,27 +146,22 @@
             pass
         import matplotlib.pyplot as plt
         plt.hist(list(pvalues.values()), bins=20)
         plt.xlabel("p-values")
         plt.ylabel("Frequency")
         plt.title("Histogram of p-values")
         plt.show()
-        plt.close()
 
     def run(self):
-        import subprocess
         if self.top_n_features:
             self.df = self.df[self.select_top_variance_features(self.top_n_features)]
         if self.correlation_matrix_bool:
             self.correlation_matrix()
         if self.tsne_plot_bool:
-            try:
-                subprocess.run(["python", "tsne_plot.py"], timeout=120)
-            except subprocess.TimeoutExpired:
-                print("t-SNE plot did not complete within 2 minutes.")
+            self.tsne_plot()
         if self.top_n_pairplot_bool:
             self.top_n_pairplot()
         if self.chi_square_test_all_features_bool:
             self.plot_pvalues()
 
     def select_top_variance_features(self, n=200):
         variances = self.df.var()
```

### Comparing `madcat-0.84/chester/feature_stats/categorical_stats.py` & `madcat-0.9/chester/feature_stats/categorical_stats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import math
 
 import pandas as pd
+import seaborn as sns
 from matplotlib import pyplot as plt
 
 from chester.zero_break.problem_specification import DataInfo
 
 
 class CategoricalStats:
     def __init__(self, data_info: DataInfo, max_print=None):
         self.data_info = data_info
         self.max_print = max_print
-        self.cols = list(set(self.data_info.feature_types_val["categorical"]))
+        self.cols = self.data_info.feature_types_val["categorical"]
         self.data = self.data_info.data[self.cols]
-        if self.data.columns.duplicated().any():
-            self.data = self.data.loc[:, ~ self.data.columns.duplicated()]
-        self.data = self.data.sample(min(10000, len(self.data)))
         self.cols_sorted = self.sort_by_cardinality()
 
     def any_categorical(self):
         return True if len(self.cols) > 0 else False
 
     def sort_by_cardinality(self):
         if not self.any_categorical():
@@ -30,65 +28,55 @@
         sorted_cardinalities = sorted(cardinalities, key=lambda x: x[1], reverse=True)
         return [x[0] for x in sorted_cardinalities]
 
     def sample_top_features(self, n):
         top_features = self.cols_sorted[:3 * n]
         return top_features
 
-    def plot_value_counts(self, n=25, plot=True):
+    def plot_value_counts(self, n=25, norm=True, plot=True):
         if not self.any_categorical():
             return None
         if not plot:
             return None
         top_n = self.cols_sorted[:min(len(self.cols_sorted), n)]
         num_plots = len(top_n)
         if num_plots == 1:
             col = top_n[0]
-            fig, ax1 = plt.subplots(1, 1, figsize=(10, 5))
+            fig, ax = plt.subplots(1, 1, figsize=(20, 5))
             cat_col = self.data[col].apply(lambda x: "cat " + str(x))
-            count_data = cat_col.value_counts()
-            percent_data = count_data / count_data.sum() * 100
-            ax1.bar(count_data.index[:5], count_data.values[:5], color='gray')
-            ax2 = ax1.twinx()
-            ax2.plot(percent_data.index[:5], percent_data.values[:5], color='red', marker='o')
-            ax1.set_ylabel('Counts', color='gray')
-            ax2.set_ylabel('Percentages', color='red')
-            ax1.set_xlabel(None)
-            ax1.set_title(f"{col}")
+            data = cat_col.value_counts(normalize=norm)
+            sns.barplot(x=data.index[:5], y=data.values[:5], ax=ax)
+            plot_title = f"{col}"
+            ax.set_title(plot_title)
+            ax.set_xlabel(None)
+            ax.set_ylim(0, 1)
             return None
         else:
-            dim = max(math.floor(math.sqrt(len(top_n))), 2)
-            fig, ax = plt.subplots(dim, dim, figsize=(18, 3 + 3 * dim))
+            dim = math.ceil(math.sqrt(len(top_n)))
+            num_rows = math.ceil(num_plots / dim)
+            fig, ax = plt.subplots(num_rows, dim)
             fig.tight_layout()
-            fig.suptitle("Top 5 Value Counts and Percentages for Each Feature")
+            if norm:
+                fig.suptitle("Top 5 Value % for Each Feature")
+            else:
+                fig.suptitle("Top 5 Value Counts for Each Feature")
             for i, col in enumerate(top_n):
-                if i >= dim * dim:
-                    break
-                count_data = pd.DataFrame(self.data[col].value_counts().head(5)).reset_index(drop=False)
-                total_count = self.data[col].count()
-                percent_data = count_data.copy()
-                percent_data[col] = percent_data[col] / total_count * 100
-                percent_data.rename(columns={col: 'percentage', 'index': col}, inplace=True)
-
+                data = pd.DataFrame(self.data[col].value_counts(normalize=norm)[0:5]).reset_index(drop=False)
                 plot_title = f"{col}"
                 ax_i = ax[i // dim, i % dim]
-                ax1_i = ax_i
-                ax1_i.bar(count_data.iloc[:, 0], count_data.iloc[:, 1].to_list(), color='gray')
-                ax2_i = ax1_i.twinx()
-                ax2_i.plot(percent_data.iloc[:, 0], percent_data.iloc[:, 1].to_list(), marker='o', color='red')
-                ax1_i.set_ylabel('Counts', color='gray')
-                ax2_i.set_ylabel('Percentages', color='red')
-                ax1_i.set_xlabel(None)
-                ax1_i.set_title(plot_title)
+                sns.barplot(x=data.iloc[:, 0], y=data.iloc[:, 1].to_list(), ax=ax_i)
+                ax_i.set_title(plot_title)
+                ax_i.set_xlabel(None)
+                if norm:
+                    ax_i.set_ylim(0, 1)
+            plt.tight_layout()
             plt.show()
-            plt.close()
+            return None
 
     def calculate_stats(self, is_print=True):
-        from chester.util import ReportCollector, REPORT_PATH
-        rc = ReportCollector(REPORT_PATH)
         if not self.any_categorical():
             return None
         result_dicts = []
         for col in self.cols:
             data = self.data[col]
             unique_values = data.nunique()
             missing_values = data.isnull().sum()
@@ -104,35 +92,32 @@
             if col_len < values_to_sample:
                 values_to_sample = col_len
             sample_values = [str(value) for value in data_unique_values.sample(min(col_len, values_to_sample)).values]
             result_dicts[-1]['Sample'] = ', '.join(sample_values)
 
             # add more columns
             # 1. % from all that covers the top 5 values
-            top_5 = 100 * value_counts.head(5)["count"].sum() / value_counts["count"].sum()
+            top_5 = 100 * value_counts.iloc[:5]["count"].sum() / value_counts["count"].sum()
             result_dicts[-1][f'Top 5 values coverage'] = f"{top_5:.0f}%"
 
         results_df = pd.DataFrame(result_dicts)
 
         if is_print:
             if self.max_print is not None:
-                formatted_df = format_df(df=results_df,
-                                         max_value_width=self.max_print,
-                                         )
-                print(formatted_df)
+                print(format_df(df=results_df,
+                                max_value_width=self.max_print,
+                                ))
             else:
-                formatted_df = format_df(results_df)
-                print(formatted_df)
-            len_df = len(formatted_df)
-            rc.save_object(obj=formatted_df.sample(min(len_df, 10)), text="Feature stats:")
+                print(format_df(results_df))
         return results_df
 
     def run(self, plot=True):
         self.calculate_stats()
-        self.plot_value_counts(plot=plot)
+        self.plot_value_counts(norm=True, plot=plot)
+        self.plot_value_counts(norm=False, plot=plot)
         return None
 
 
 def format_df(df, max_value_width=30):
     pd.options.display.max_columns = None
 
     def trim_value(val):
```

### Comparing `madcat-0.84/chester/feature_stats/numeric_stats.py` & `madcat-0.9/chester/feature_stats/numeric_stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,23 +47,19 @@
         plt.title(plot_title)
         print("Matrix correlation for numerical features")
         print("""\n
         💡 Rule of thumb:
         👍 Strong positive correlation: >= 0.7
         🤔 Moderate positive correlation: between 0.5 and 0.7
         🤨 Weak positive correlation: between 0.3 and 0.5
-        🤷‍️ No/Negligible correlation: < 0.3
+        🤷‍♀️ No/Negligible correlation: < 0.3
         """)
         plt.show()
-        plt.close()
 
     def calculate_stats(self, is_print=True):
-        from chester.util import ReportCollector, REPORT_PATH
-        rc = ReportCollector(REPORT_PATH)
-
         if not self.any_numeric():
             return None
         result_dicts = []
         for col in self.cols:
             data = self.data[col]
             data_drop_dups = data.drop_duplicates()
             unique_values = data.nunique()
@@ -89,24 +85,20 @@
                                  'max': max_vals,
                                  'min': min_vals, 'avg': avg_vals, 'std': std_vals, 'CI': ci_vals,
                                  'median': median_vals,
                                  'top_vals': top_vals, 'bottom_vals': bottom_vals})
         results_df = pd.DataFrame(result_dicts)
         if is_print:
             if self.max_print is not None:
-                formatted_df = format_df(df=results_df,
-                                         max_value_width=self.max_print,
-                                         ci_max_value_width=self.max_print,
-                                         col_max_value_width=self.max_print)
-                print(formatted_df)
+                print(format_df(df=results_df,
+                                max_value_width=self.max_print,
+                                ci_max_value_width=self.max_print,
+                                col_max_value_width=self.max_print))
             else:
-                formatted_df = format_df(results_df)
-                print(formatted_df)
-            len_df = len(formatted_df)
-            rc.save_object(obj=formatted_df.sample(min(len_df, 10)), text="Feature stats:")
+                print(format_df(results_df))
         return results_df
 
     def run(self, plot=True):
         self.calculate_stats()
         self.plot_correlation(plot=plot)
         return None
```

### Comparing `madcat-0.84/chester/features_engineering/bag_of_words.py` & `madcat-0.9/chester/features_engineering/bag_of_words.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/features_engineering/corex.py` & `madcat-0.9/chester/features_engineering/corex.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 import numpy as np
 import pandas as pd
 import scipy.sparse as ss
 from corextopic import corextopic as ct
 from sklearn.feature_extraction.text import CountVectorizer
 
 
-def get_corex_embedding(training_data, test_data=None, text_column='text', ngram_range=(1, 2),
-                        n_topics=50, anchor_words=None, anchor_strength=1.6,
+def get_corex_embedding(training_data, test_data=None, text_column='text', ngram_range=(1, 1),
+                        n_topics=50,
                         max_features=10000):
     # Preprocess data
     vectorizer = CountVectorizer(stop_words='english', max_features=max_features, binary=True, ngram_range=ngram_range)
     doc_word = vectorizer.fit_transform(training_data[text_column])
-
     doc_word = ss.csr_matrix(doc_word)
     feature_names = list(vectorizer.vocabulary_.keys())
     words = list(np.asarray(feature_names))
 
     # Train model
     topic_model = ct.Corex(n_hidden=n_topics, words=words, max_iter=200, verbose=False, seed=1)
-    if anchor_words is None:
-        topic_model.fit(doc_word, words=words)
-    else:
-        print("Anchored Corex")
-        topic_model.fit(doc_word, words=words, anchor_strength=anchor_strength, anchors=anchor_words)
+    topic_model.fit(doc_word, words=words)
 
     # Get the topic probabilities for the training data
     topic_probs = topic_model.transform(doc_word, details=True)[0]
     # Normalize the topic probabilities
     topic_probs = topic_probs / np.sum(topic_probs, axis=1, keepdims=True)
     # Create a DataFrame of topic probability features
     topic_prob_df = pd.DataFrame(topic_probs, columns=[f"corex_topic_{i + 1}" for i in range(n_topics)])
```

### Comparing `madcat-0.84/chester/features_engineering/fe_nlp.py` & `madcat-0.9/chester/features_engineering/fe_nlp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
 from chester.features_engineering.bag_of_words import get_bow_embedding
 from chester.features_engineering.corex import get_corex_embedding
 from chester.features_engineering.tfidf import get_tfidf_embedding
-from chester.util import ReportCollector, REPORT_PATH
 
 
 def get_embeddings(training_data: pd.DataFrame,
                    test_data: pd.DataFrame = None,
                    split_data: bool = True, split_prop: float = 0.3,
                    split_random_state=42,
                    text_column="clean_text", target_column='target',
-                   corex=True, corex_dim=50, anchor_words=None, anchor_strength=1.6,
-                   tfidf=True, tfidf_dim=100, bow=True, bow_dim=100,
-                   ngram_range=(1, 2)):
-    rc = ReportCollector(REPORT_PATH)
-    rc.save_text("Extracting embedding")
+                   corex=True, corex_dim=50, tfidf=True,
+                   tfidf_dim=100, bow=True, bow_dim=100,
+                   ngram_range=(1, 1)):
     if split_data:
         if not test_data:
             training_data, test_data = train_test_split(training_data, test_size=split_prop,
                                                         random_state=split_random_state)
 
     order_list = ["First", "Next", "Then", "Additionally", "Furthermore", "Then", "Additionally", "Furthermore", "Then",
                   "Additionally"]
@@ -32,62 +29,53 @@
     corex_test_embedding = pd.DataFrame()
     tfidf_test_embedding = pd.DataFrame()
     bow_test_embedding = pd.DataFrame()
     ner_bow_test_embedding = pd.DataFrame()
     i = 0
     # Extract Corex topic model embeddings if requested
     if corex:
-        title_to_print = f"{order_list[i]}, Extracting Corex topic model embeddings with dimension {corex_dim}"
-        print(title_to_print)
-        rc.save_text(title_to_print)
-        corex_embedding, corex_test_embedding = \
-            get_corex_embedding(training_data=training_data, test_data=test_data,
-                                ngram_range=ngram_range, n_topics=corex_dim, text_column=text_column,
-                                anchor_words=anchor_words, anchor_strength=anchor_strength)
+        print(f"{order_list[i]}, Extracting Corex topic model embeddings with dimension {corex_dim}")
+        corex_embedding, corex_test_embedding = get_corex_embedding(training_data=training_data, test_data=test_data,
+                                                                    ngram_range=ngram_range,
+                                                                    n_topics=corex_dim, text_column=text_column)
         i += 1
 
     # Extract TF-IDF embeddings if requested
     if tfidf:
-        title_to_print = f"{order_list[i]}, Extracting TF-IDF embeddings with dimension {tfidf_dim}"
-        print(title_to_print)
-        rc.save_text(title_to_print)
+        print(f"{order_list[i]}, Extracting TF-IDF embeddings with dimension {tfidf_dim}")
         tfidf_embedding, tfidf_test_embedding, _ = get_tfidf_embedding(training_data, test_df=test_data,
                                                                        ngram_range=ngram_range,
                                                                        embedding_size=tfidf_dim,
                                                                        text_column=text_column)
         i += 1
 
     # Extract bag-of-words embeddings if requested
     if bow:
-        title_to_print = f"{order_list[i]}, Extracting bag-of-words embeddings with dimension {bow_dim}"
-        print(title_to_print)
-        rc.save_text(title_to_print)
+        print(f"{order_list[i]}, Extracting bag-of-words embeddings with dimension {bow_dim}")
         bow_embedding, bow_test_embedding, _ = get_bow_embedding(training_data, test_data=test_data,
                                                                  ngram_range=ngram_range,
                                                                  embedding_size=bow_dim,
                                                                  text_column=text_column)
         i += 1
 
     # Concatenate the embeddings and return them
     embeddings = pd.concat([corex_embedding, tfidf_embedding, ner_bow_embedding, bow_embedding], axis=1)
     test_embeddings = pd.concat(
         [corex_test_embedding, tfidf_test_embedding, ner_bow_test_embedding, bow_test_embedding], axis=1)
 
-    title_to_print = f"Lastly, All embeddings have been concatenated"
-    print(title_to_print)
-    rc.save_text(title_to_print)
-    # adding the label to train and test embedding
+    # # adding the label to train and test embedding
     try:
         training_data.reset_index(drop=True, inplace=True)
         embeddings.reset_index(drop=True, inplace=True)
         embeddings = pd.concat([embeddings, training_data[target_column]], axis=1)
 
         test_data.reset_index(drop=True, inplace=True)
         test_embeddings.reset_index(drop=True, inplace=True)
         test_embeddings = pd.concat([test_embeddings, test_data[target_column]], axis=1)
+        print(f"Lastly, All embeddings have been concatenated")
     except:
         pass
     return embeddings, test_embeddings
 
 
 class TextFeatureExtraction:
     def __init__(self, training_data: pd.DataFrame = None,
```

### Comparing `madcat-0.84/chester/features_engineering/feature_handler.py` & `madcat-0.9/chester/features_engineering/feature_handler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 import pandas as pd
 
 from chester.features_engineering.fe_nlp import get_embeddings
-from chester.features_engineering.time_series.ts_feature_extraction import TimeSeriesFeatureExtraction
-from chester.run.user_classes import TextFeatureExtraction, TimeSeriesHandler
-from chester.zero_break.problem_specification import DataInfo
+from chester.run.user_classes import TextFeatureSpec
 
 
 class FeatureHandler:
     def __init__(self, column, col_name,
                  feature_type=None,
-                 time_series_handler: TimeSeriesHandler = None,
-                 text_feature_extraction: TextFeatureExtraction = None,
-                 data_info: DataInfo = None):
+                 text_feature_extraction: TextFeatureSpec = None):
         self.column = column
         self.feature_type = feature_type
-        self.data_info = data_info
-        self.time_series_handler = time_series_handler
         self.col_name = col_name
         self.text_feature_extraction = text_feature_extraction
 
     def handle_numerical(self):
         self.column.name = "num_" + self.column.name
         return self.column, ["num_" + self.col_name]
 
@@ -48,64 +42,51 @@
         elif self.n_unique_words < 10000 and self.n_rows < 10000000:
             size = 240
         else:
             size = 300
         return size
 
     def handle_text(self):
+        embedding_size = self.decide_embedding_size()
+        print(f"Feature: {self.col_name} calculating {embedding_size} dim embedding")
+        embedding_size_method = int(embedding_size / 3)
         data = pd.DataFrame({self.col_name: self.column})
+
         if self.text_feature_extraction is not None:
             feat_ext = self.text_feature_extraction
-            print(
-                f"Feature: {self.col_name} calculating"
-                f" {feat_ext.corex_dim + feat_ext.bow_dim + feat_ext.tfidf_dim} dim embedding")
             embedding, _ = get_embeddings(
                 training_data=data,
                 test_data=None,
                 split_data=False,
                 text_column=self.col_name,
                 corex_dim=feat_ext.corex_dim, corex=feat_ext.corex,
-                anchor_words=feat_ext.anchor_words, anchor_strength=feat_ext.anchor_strength,
                 bow_dim=feat_ext.bow_dim, bow=feat_ext.bow,
                 tfidf_dim=feat_ext.tfidf_dim, tfidf=feat_ext.tfidf,
                 ngram_range=feat_ext.ngram_range
             )
 
         else:
-            embedding_size = self.decide_embedding_size()
-            print(f"Feature: {self.col_name} calculating {embedding_size} dim embedding")
-            embedding_size_method = int(embedding_size / 3)
             embedding, _ = get_embeddings(training_data=data, split_data=False, text_column=self.col_name,
                                           corex_dim=embedding_size_method, bow_dim=embedding_size_method,
                                           tfidf_dim=embedding_size_method)
 
         new_col_name_list = [self.col_name + "_" + col for col in embedding.columns]
         new_col_name_dict = dict(zip(embedding.columns, new_col_name_list))
         embedding.rename(columns=new_col_name_dict, inplace=True)
         return embedding, embedding.columns
 
-    def handle_time_series(self):
-        ts_fe = TimeSeriesFeatureExtraction(
-            time_series_handler=self.time_series_handler,
-            data_info=self.data_info,
-            col_name=self.col_name,
-            column=self.column
-        )
-        ts_fe.run()
-        self.data_info = ts_fe.data_info
-
-    def run(self):
-        if self.feature_type == 'time':
-            return self.handle_time_series()
+    def handle_feature(self):
         if self.feature_type == 'numeric':
             return self.handle_numerical()
         elif self.feature_type == 'categorical':
             return self.handle_categorical()
         elif self.feature_type == 'boolean':
             return self.handle_boolean()
         elif self.feature_type == 'text':
             return self.handle_text()
+        elif self.feature_type == 'time':
+            return None, None
         else:
             if not (self.col_name == self.col_name):
                 print(
                     f"No appropriate feature handler found for feature {self.col_name}. This feature will be ignored.")
                 return None, None
```

### Comparing `madcat-0.84/chester/features_engineering/features_handler.py` & `madcat-0.9/chester/features_engineering/features_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import pandas as pd
 
 from chester.features_engineering.feature_handler import FeatureHandler
-from chester.run.user_classes import TextFeatureExtraction
+from chester.run.user_classes import TextFeatureSpec
 from chester.zero_break.problem_specification import DataInfo
 
 
 class FeaturesHandler:
-    def __init__(self,
-                 data_info: DataInfo,
-                 text_feature_extraction: TextFeatureExtraction = None):
-        self.data_info = data_info
+    def __init__(self, data_info: DataInfo, text_feature_extraction: TextFeatureSpec = None):
         self.data = data_info.data
         self.target = data_info.target
         self.text_feature_extraction = text_feature_extraction
         self.problem_type_val = data_info.problem_type_val
         self.feature_types_val = data_info.feature_types_val
         self.loss_detector_val = data_info.loss_detector_val
         self.metrics_detector_val = data_info.metrics_detector_val
@@ -31,29 +28,27 @@
                     feature_type = key
                     break
                 # Prepare an instance of FeatureHandler
             feature_handler = FeatureHandler(
                 column=data[col],
                 feature_type=feature_type,
                 col_name=col,
-                text_feature_extraction=self.text_feature_extraction,
-                data_info=self.data_info
-            )
+                text_feature_extraction=self.text_feature_extraction)
             feature_handlers.append(feature_handler)
         return feature_handlers
 
     def transform(self):
         feature_types = {'numeric': [], 'categorical': []}
         feature_handlers = self._get_features_handler(data=self.data)
-        print(f"Handling {len(feature_handlers)} potential raw features")
+        print(f"Handling {len(feature_handlers)} raw features")
         feat_values = []
         feat_names = []
         for feature_handler in feature_handlers:
             try:
-                values, names = feature_handler.run()
+                values, names = feature_handler.handle_feature()
                 feat_values.append(values)
                 if feature_handler.feature_type is None:
                     pass
                 if feature_handler.feature_type == 'numeric':
                     feature_types['numeric'].extend(names)
                     feat_names.append(names)
                 elif feature_handler.feature_type == 'boolean':
```

### Comparing `madcat-0.84/chester/features_engineering/tfidf.py` & `madcat-0.9/chester/features_engineering/tfidf.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_analyzer/model_analysis.py` & `madcat-0.9/chester/model_analyzer/model_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,28 +26,27 @@
         if len(coef) < 10:
             plt.bar(np.arange(len(coef)), coef)
             plt.xticks(np.arange(len(coef)), feature_names, rotation=90)
             plt.title("Coefficients for Logistic Regression Model")
             plt.xlabel("Features")
             plt.ylabel("Values")
             plt.show()
-            plt.close()
+
         else:
             sns.violinplot(coef, inner="stick")
             plt.title("Coefficients distribution for logistic regression model")
             plt.xlabel("Coefficients")
             print(AnalyzeMessages().coefficients_message())
         plt.show()
-        plt.close()
 
     def analyze(self, X_train: pd.DataFrame, y_train: pd.Series,
                 X_test: pd.DataFrame, y_test: pd.Series,
                 model, plot_shap_values: bool = True, coefficients: bool = True,
                 confusion_matrix: bool = True,
-                roc_curve: bool = True, learning_curve: bool = True,
+                roc_curve: bool = True, learning_curve: bool = False,
                 feature_importance: bool = True) -> None:
         unique_classes = len(np.unique(y_train))
         if feature_importance:
             try:
                 self.plot_feature_importance(X_train)
             except:
                 try:
@@ -84,15 +83,14 @@
         y_pred = self.model.predict(X_test)
         cm = confusion_matrix(y_test, y_pred)
         sns.heatmap(cm, annot=True, cmap='Blues', fmt='g')
         plt.title('Confusion Matrix')
         plt.xlabel('Predicted')
         plt.ylabel('Actual')
         plt.show()
-        plt.close()
 
     def roc_curve(self, X_test: pd.DataFrame, y_test: pd.Series) -> None:
         from sklearn.metrics import roc_curve, auc
         try:
             y_pred = self.model.predict_proba(X_test)
             fpr, tpr, thresholds = roc_curve(y_test, y_pred[:, 1])
             roc_auc = auc(fpr, tpr)
@@ -103,17 +101,16 @@
             plt.ylim([0.0, 1.05])
             plt.xlabel('False Positive Rate')
             plt.ylabel('True Positive Rate')
             plt.title('Receiver operating characteristic')
             plt.legend(loc="lower right")
             print(AnalyzeMessages().roc_curve_message())
             plt.show()
-            plt.close()
         except:
-            return None
+            pass
 
     def learning_curve(self, X: pd.DataFrame, y: pd.Series) -> None:
         try:
             from sklearn.model_selection import learning_curve
             train_sizes, train_scores, test_scores = learning_curve(self.model, X, y, cv=5, scoring='accuracy')
             train_scores_mean = np.mean(train_scores, axis=1)
             train_scores_std = np.std(train_scores, axis=1)
@@ -128,42 +125,38 @@
             plt.grid()
             plt.xlabel("Training examples")
             plt.ylabel("Accuracy Score")
             plt.title("Learning Curve")
             plt.legend(loc="best")
             print(AnalyzeMessages().learning_curve_message())
             plt.show()
-            plt.close()
         except:
-            plt.close()
-            return None
+            pass
 
     def plot_simple_feature_importance(self, X_train: pd.DataFrame):
         feature_importance = self.model.feature_importances_
         feature_importance = 100.0 * (feature_importance / feature_importance.max())
         feature_names = X_train.columns
         important_idx = np.argsort(feature_importance)
         data = {'feature_names': feature_names[important_idx], 'feature_importance': feature_importance[important_idx]}
         df = pd.DataFrame(data)
         sns.barplot(y='feature_names', x='feature_importance', data=df)
         plt.xlabel("Feature importance")
         plt.show()
-        plt.close()
 
     def plot_feature_importance(self, X_train: pd.DataFrame):
         feature_importance = self.model.feature_importances_
         feature_importance = 100.0 * (feature_importance / feature_importance.max())
         feature_names = X_train.columns
         important_idx = np.argsort(feature_importance)
         data = {'feature_names': feature_names[important_idx], 'feature_importance': feature_importance[important_idx]}
         df = pd.DataFrame(data)
         print(AnalyzeMessages().feature_importance_message())
         fig = px.bar(df, x='feature_importance', y='feature_names', orientation='h', text='feature_importance')
         fig.show()
-        plt.close()
 
 
 class AnalyzeMessages:
     def shap_values_message(self):
         return "SHAP values can be used to understand the importance of each feature in the model's" \
                " predictions.\n The plot shows the average absolute SHAP value of each feature for all " \
                "the samples in the test set.\n Features with higher absolute SHAP values have a greater " \
@@ -190,15 +183,17 @@
         return "The ROC curve shows the trade-off between true positive rate (sensitivity) " \
                "and false positive rate (1-specificity) for different threshold settings.\n T" \
                "he AUC (Area under the curve) value gives an overall measure of the model's performance.\n"
 
     def learning_curve_message(self):
         return "The learning curve displays model performance as training samples increase.\n" \
                "High training and low validation suggest overfitting,\n" \
-               "low training and high validation suggest underfitting.\n"
+               "low training and high validation suggest underfitting.\n" \
+               "To improve performance, consider adding more data or using regularization techniques\n" \
+               "if the evaluation score plateaus.\n"
 
     def feature_importance_message(self):
         return "The feature importance plot shows the relative importance of each feature in the model's predictions.\n" \
                " Features with higher importance have a greater impact on the model's predictions and are more useful\n" \
                " for making accurate predictions.\n"
```

### Comparing `madcat-0.84/chester/model_monitor/calculate_scores_utils.py` & `madcat-0.9/chester/model_monitor/calculate_scores_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_monitor/error_prediction.py` & `madcat-0.9/chester/model_monitor/error_prediction.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 import pandas as pd
 import seaborn as sns
 from catboost import CatBoostRegressor
 from matplotlib import pyplot as plt
 from sklearn.compose import ColumnTransformer
 from sklearn.impute import SimpleImputer
 from sklearn.preprocessing import OneHotEncoder
-from sklearn.tree import DecisionTreeRegressor, export_text
+from sklearn.tree import DecisionTreeRegressor
 
-from chester.feature_stats.utils import create_pretty_table
 from chester.model_training.data_preparation import CVData
 from chester.zero_break.problem_specification import DataInfo
 
 
 class ModelWeaknesses:
     def __init__(self, cv_data: CVData, data_info: DataInfo, model):
         self.cv_data = cv_data
@@ -24,16 +23,14 @@
         self.y_test = self.cv_data.test_data[self.cv_data.target_column]
         # retrain the model
         self.model.retrain(self.X_train, self.y_train)
         # predicting
         self.predict_test = self.model.predict(self.X_test)
         self.predict_test = self.handle_predictions()
         self.error = self.calculate_error()
-        from chester.util import ReportCollector, REPORT_PATH
-        self.rc = ReportCollector(REPORT_PATH)
 
     def handle_predictions(self):
         y = self.predict_test
         if isinstance(y, pd.Series):
             return y
         elif y.ndim == 2 and y.shape[1] == 1:
             return pd.Series(y.flatten()).reset_index(drop=True)
@@ -79,54 +76,43 @@
         X_test_transformed = transformer.fit_transform(self.X_test)
 
         # Train the DecisionTreeRegressor model
         model = DecisionTreeRegressor(min_samples_leaf=min_samples_leaf, max_depth=max_depth)
         model.fit(X_test_transformed, self.error)
 
         # Get the feature names of the numeric features
+        # Get the feature names of the numeric features
         numeric_feature_names = self.data_info.feature_types_val["numeric"]
         # Get the feature names of the categorical features
         categorical_transformer.fit(self.X_test[self.data_info.feature_types_val["categorical"]])
         categories = categorical_transformer.categories_
         categorical_feature_names = []
         for i, col in enumerate(self.data_info.feature_types_val["categorical"]):
             for j in range(len(categories[i])):
                 categorical_feature_names.append(f"{col}_{categories[i][j]}")
         # Concatenate the feature names of the categorical and numeric features
         feature_names = numeric_feature_names + categorical_feature_names
 
-        plt.figure(figsize=(13, 13))
+        plt.figure()
         tree.plot_tree(model,
                        feature_names=feature_names,
                        class_names=['error'],
                        rounded=True,
                        filled=True,
                        )
-        # Get the tree structure as text
-        self.rc.save_object(obj=export_text(model, feature_names=feature_names),
-                            text="Print of tree to look for potential segments with high error (use with caution)")
         plt.suptitle("Decision Tree Trained on Model Error")
+        return None
 
     def plot_catboost_error_regressor(self, iterations=100, depth=3, learning_rate=0.1):
         model = CatBoostRegressor(iterations=iterations, depth=depth, learning_rate=learning_rate)
         model.fit(self.X_test, self.error, verbose=False)
         plt.figure(figsize=(15, 15))
-        feature_importances = np.round(model.feature_importances_, decimals=0)
-        feature_imp = pd.DataFrame({'Feature': self.X_test.columns, 'Importance': feature_importances})
-        feature_imp = feature_imp.sort_values(by='Importance', ascending=False)
-        self.rc.save_object(create_pretty_table(feature_imp[0:50]), text="Most important features by catboost:")
-        feature_imp = feature_imp[0:30]
+        feature_imp = pd.DataFrame({'Feature': self.X_test.columns, 'Importance': model.feature_importances_})
+        feature_imp = feature_imp.sort_values(by='Importance', ascending=False)[0:30]
         sns.barplot(x=feature_imp['Importance'], y=feature_imp['Feature'])
         plt.title('CatBoost Feature Importance to Detect Segments with High Error')
         plt.show()
-        plt.close()
 
     def run(self):
         print("Training model to predict the error")
-        if np.unique(self.error).size == 1:
-            print("🎉 No weaknesses found! All errors on the test set are 0.")
-            return None
         self.plot_catboost_error_regressor()
         self.plot_decision_tree_error_regressor()
-
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `madcat-0.84/chester/model_monitor/model_boostrap.py` & `madcat-0.9/chester/model_monitor/model_boostrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
-from chester.feature_stats.utils import create_pretty_table
 from chester.model_monitor import calculate_scores_utils
 from chester.model_training.data_preparation import CVData
 from chester.model_training.models.chester_models.catboost.catboost_utils import calculate_catboost_metrics_scores
 from chester.zero_break.problem_specification import DataInfo
 
-boostrap_message = "The following plots display the bootstrap distribution of the metrics, " \
-                   "\nUsing a violin plot and histogram: " \
-                   "\n\tℹ️ The violin plot shows the median, " \
+boostrap_message = "The following plots display the distribution of the metrics, " \
+                   "\nusing a violin plot and histogram. " \
+                   "\n\tThe violin plot shows the median, " \
                    "quartiles, and other important summary statistics of the data, " \
-                   "\n\tℹ️ While the histogram provides a visual representation of the " \
-                   "frequency of values in the data. " \
-                   "\nThese plots give you a sense of how the metrics are distributed " \
-                   "\nand can be used to identify any patterns or outliers in the data."
+                   "\n\twhile the histogram provides a visual representation of the frequency of values in the data. " \
+                   "\nThese plots give you a sense of how the metrics are distributed\n " \
+                   "and can be used to identify any " \
+                   "patterns or outliers in the data."
 
 
 class ModelBootstrap:
     def __init__(self, cv_data: CVData, data_info: DataInfo, model):
         self.cv_data = cv_data
         self.data_info = data_info
         self.model = model
@@ -27,16 +26,14 @@
         self.y_train = self.cv_data.train_data[self.cv_data.target_column]
         self.X_test = self.cv_data.test_data.drop(columns=[self.cv_data.target_column])
         self.y_test = self.cv_data.test_data[self.cv_data.target_column]
         # retrain the model
         self.model.retrain(self.X_train, self.y_train)
         self.predict_test = self.model.predict(self.X_test)
         self.metrics = self.get_metrics_functions()
-        from chester.util import ReportCollector, REPORT_PATH
-        self.rc = ReportCollector(REPORT_PATH)
 
     def get_metrics_functions(self):
         metric_functions = []
         metrics = self.data_info.metrics_detector_val
         for metric in metrics:
             metric_function = self.get_metric_function(metric)
             if metric_function is not None:
@@ -90,15 +87,13 @@
                 )
         return bootstrap_metrics
 
     def plot(self):
         print(boostrap_message)
         import seaborn as sns
         metrics = pd.DataFrame(self.bootstrap_metrics())
-        self.rc.save_object(create_pretty_table(metrics.sample(20)), "\nBoostrap metrics, sample 20 results:")
         for metric_name in metrics.columns:
             fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(10, 5))
             sns.violinplot(x=metrics[metric_name], ax=ax1)
             ax1.set_title(metric_name)
             sns.histplot(x=metrics[metric_name], ax=ax2)
             plt.show()
-            plt.close()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `madcat-0.84/chester/model_training/data_preparation.py` & `madcat-0.9/chester/model_training/data_preparation.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/model_utils.py` & `madcat-0.9/chester/model_training/model_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,8 +34,7 @@
     print("Model performance:")
     print(model_analysis.AnalyzeMessages().performance_metrics_message())
     print(results_pivot)
 
     sns.boxplot(x='fold', y='value', hue='variable', data=results_melt, palette="Set3")
     print(analysis_message)
     plt.show()
-    plt.close()
```

### Comparing `madcat-0.84/chester/model_training/models/chester_models/base_model.py` & `madcat-0.9/chester/model_training/models/chester_models/base_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,14 @@
     def __init__(self, data_info: DataInfo, cv_data: CVData, num_models_to_compare=10, best_practice_prop=0.33):
         self.data_info = data_info
         self.cv_data = cv_data
         self.num_models_to_compare = num_models_to_compare
         self.best_practice_prop = best_practice_prop
         self.best_model = None
         self.best_metrics = {}
-        try:
-            self.feature_names = self.cv_data.train_data.columns
-        except:
-            pass
 
     def get_metric_function(self, metric):
         from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
         from sklearn.metrics import mean_squared_error, mean_absolute_error, mean_absolute_percentage_error
         from sklearn.metrics import roc_auc_score
 
         if metric == 'Accuracy':
```

### Comparing `madcat-0.84/chester/model_training/models/chester_models/base_model_utils.py` & `madcat-0.9/chester/model_training/models/chester_models/base_model_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/models/chester_models/baseline/baseline_model.py` & `madcat-0.9/chester/model_training/models/chester_models/baseline/baseline_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,10 +26,7 @@
 
     def predict(self, X):
         return self.transform(X)
 
     def fit_transform(self, X, y):
         self.fit(y)
         return self.transform(X)
-
-    def get_params(self):
-        return {"model": "Baseline"}
```

### Comparing `madcat-0.84/chester/model_training/models/chester_models/baseline/baseline_utils.py` & `madcat-0.9/chester/model_training/models/chester_models/baseline/baseline_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/models/chester_models/best_baseline_model.py` & `madcat-0.9/chester/model_training/models/chester_models/best_baseline_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,9 +38,7 @@
                     results.append((base_res, model))
                 best = compare_models(results)
                 return best
 
     def calc_model_score(self, model):
         # calculate the score of a given baseline model
         pass
-
-
```

### Comparing `madcat-0.84/chester/model_training/models/chester_models/best_catboost.py` & `madcat-0.9/chester/model_training/models/chester_models/best_catboost.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/models/chester_models/best_linear_regression.py` & `madcat-0.9/chester/model_training/models/chester_models/best_linear_regression.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/models/chester_models/best_logistic_regression.py` & `madcat-0.9/chester/model_training/models/chester_models/best_logistic_regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from chester.model_training.models.chester_models.base_model import BaseModel
 from chester.model_training.models.chester_models.logistic_regression.logistic_regression_utils import \
     generate_logistic_regression_configs, logistic_regression_with_outputs, compare_models
 from chester.zero_break.problem_specification import DataInfo
 
 
 class LogisticRegressionModel(BaseModel):
-    def __init__(self, data_info: DataInfo, cv_data: CVData, num_models_to_compare=9, best_practice_prob=0.33):
+    def __init__(self, data_info: DataInfo, cv_data: CVData, num_models_to_compare=9, best_practice_prop=0.33):
         super().__init__(data_info, cv_data, num_models_to_compare)
         self.hp_list = generate_logistic_regression_configs(k=self.num_models_to_compare,
-                                                            best_practice_prob=best_practice_prob)
-        print(f"Running {self.num_models_to_compare} Logistic Regression models")
+                                                            best_practice_prob=best_practice_prop)
+        print(f"Running {self.num_models_to_compare} elastic net models")
 
     def get_best_model(self):
         models = self.data_info.model_selection_val
         metrics = self.get_metrics_functions()
         if models is None:
             return None
         else:
```

### Comparing `madcat-0.84/chester/model_training/models/chester_models/best_model.py` & `madcat-0.9/chester/model_training/models/chester_models/best_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                                                 ).get_best_model()
                 models.append((base_res, model))
             elif 'logistic' in model_type:
                 base_res, model = best_logistic_regression.LogisticRegressionModel(
                     data_info=self.data_info,
                     cv_data=self.cv_data,
                     num_models_to_compare=self.num_models_to_compare,
-                    best_practice_prob=self.best_practice_prop
+                    best_practice_prop=self.best_practice_prop
                 ).get_best_model()
                 models.append((base_res, model))
             elif 'catboost' in model_type:
                 base_res, model = best_catboost.CatboostModel(
                     data_info=self.data_info,
                     cv_data=self.cv_data,
                     num_models_to_compare=self.num_models_to_compare
```

### Comparing `madcat-0.84/chester/model_training/models/chester_models/catboost/catboost_model.py` & `madcat-0.9/chester/model_training/models/chester_models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/models/chester_models/catboost/catboost_utils.py` & `madcat-0.9/chester/model_training/models/chester_models/catboost/catboost_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import List
 
 import numpy as np
-from prettytable import PrettyTable
 from sklearn.exceptions import UndefinedMetricWarning
 
-from chester.feature_stats.utils import create_pretty_table
 from chester.model_training.data_preparation import CVData
 from chester.model_training.data_preparation import Parameter
 from chester.model_training.models.chester_models.base_model_utils import is_metric_higher_is_better
 from chester.model_training.models.chester_models.catboost.catboost_model import CatboostModel
 from chester.model_training.models.chester_models.hp_generator import HPGenerator
 from chester.zero_break.problem_specification import DataInfo
 
@@ -44,14 +42,16 @@
                           ):
     results = []
     problem_type = data_info.problem_type_val
     for i, (X_train, y_train, X_test, y_test) in enumerate(cv_data.format_splits()):
         model = train_catboost(X_train, y_train, parameters=parameters, data_info=data_info)
         prediction = predict_catboost(model, X_test)
         prediction_train = predict_catboost(model, X_train)
+        # print("prediction_train", prediction_train)
+        # print(metrics)
         scores = calculate_catboost_metrics_scores(y_test, prediction, metrics, problem_type)
         results.append({'type': 'test', 'fold': i, **scores})
         scores = calculate_catboost_metrics_scores(y_train, prediction_train, metrics, problem_type)
         results.append({'type': 'train', 'fold': i, **scores})
     return results, model
 
 
@@ -109,63 +109,48 @@
 
 import pandas as pd
 import matplotlib.pyplot as plt
 
 
 def visualize_performance(df, with_baseline=True):
     addition = 'excluding baseline model' if not with_baseline else ''
-
     # Create pivot table to summarize mean performance metric by type and model
     metric_columns = [col for col in df.columns if col not in ["type", "model"]]
-    metric_columns = [metric for metric in metric_columns if metric is not None]
     pivot = df.pivot(index="model", columns="type", values=metric_columns)
-
     if not with_baseline:
         pivot = df[df['model'] != 'BaselineModel'].pivot(index="model", columns="type", values=metric_columns)
-
     # Plot bar chart to compare mean performance metric by model
-    # fig, axes = plt.subplots(nrows=len(metric_columns), ncols=1, figsize=(12, 10), sharex=True)
-    fig, axes = plt.subplots(nrows=len(metric_columns), ncols=1, figsize=(12, 10), sharex=True)
+    fig, axes = plt.subplots(nrows=len(metric_columns), ncols=1, figsize=(8, 8), sharex=True)
 
     for i, metric in enumerate(metric_columns):
         pivot[metric].plot.bar(ax=axes[i], rot=0)
-        axes[i].set_ylabel(None)
+        axes[i].set_ylabel(metric)
         axes[i].set_title("Comparison of {} by Model {}".format(metric, addition))
 
-    plt.xlabel(None)
-    plt.ylabel(None)
+    plt.xlabel("Model")
     plt.tight_layout()
     plt.show()
-    plt.close()
 
     return pivot
 
 
 def compare_best_models(results, plot_results=True):
-    from chester.util import ReportCollector, REPORT_PATH
-    rc = ReportCollector(REPORT_PATH)
-
     all_results = []
     all_results_with_models = []
     for res in results:
         result, model = res
         result_organized = pd.DataFrame(result)
         result_organized['model'] = get_model_name(model)
         all_results.append(result_organized)
         all_results_with_models.append((result_organized, model))
-
-    metrics_results = calculate_average(pd.concat(all_results))
     if plot_results:
         print("Model results - comparing the best out of each type")
-        visualize_performance(metrics_results, with_baseline=True)
+        visualize_performance(calculate_average(pd.concat(all_results)), with_baseline=True)
         print("Model results - comparing the best out of each type, excluding baseline model")
-        visualize_performance(metrics_results, with_baseline=False)
-
-    rc.save_object(create_pretty_table(metrics_results),
-                   text="Model results compared - showing the best out of each type after CV & HP tuning: ")
+        visualize_performance(calculate_average(pd.concat(all_results)), with_baseline=False)
 
     metric_name = [col for col in all_results[0].columns if col not in ['type', 'fold', 'model']][0]
     sort_ascending = is_metric_higher_is_better(metric_name)
     best_result = None
     best_model = None
     best_value = None
     for (result, model) in all_results_with_models:
```

### Comparing `madcat-0.84/chester/model_training/models/chester_models/hp_generator.py` & `madcat-0.9/chester/model_training/models/chester_models/hp_generator.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/models/chester_models/linear_regression/linear_regression.py` & `madcat-0.9/chester/model_training/models/chester_models/linear_regression/linear_regression.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,41 +10,40 @@
 
 class LinearRegressionModel:
     def __init__(self, parameters: list, data_info: DataInfo):
         self.parameters = parameters
         self.data_info = data_info
         self.model_type = self.data_info.problem_type_val
         if "regression" in self.model_type.lower():
-            self.model = ElasticNet()
+            self.en_model = ElasticNet()
         self.categorical_features = self.data_info.feature_types_val["categorical"]
         self.numeric_features = self.data_info.feature_types_val["numeric"]
         self.transformer = None
         self.pipeline = None
 
     def fit(self, X, y):
         import warnings
         warnings.filterwarnings("ignore", category=ConvergenceWarning)
         # Prepare the numerical features for processing
         numerical_transformer = SimpleImputer(strategy='median')
         # Prepare the categorical features for processing
         categorical_transformer = OneHotEncoder(handle_unknown='ignore')
         # Use the ColumnTransformer to apply the transformations to the corresponding features
-
         self.transformer = ColumnTransformer(
             transformers=[
                 ('c', categorical_transformer, self.categorical_features),
                 ('n', numerical_transformer, self.numeric_features)
             ])
         # Prepare the pipeline
         self.pipeline = Pipeline(steps=[('preprocessor', self.transformer),
-                                        ('regressor', self.model)
+                                        ('regressor', self.en_model)
                                         ])
         # Fit the pipeline with the training data
         hyperparams = {param.name: param.value for param in self.parameters}
-        self.model.set_params(**hyperparams)
+        self.en_model.set_params(**hyperparams)
         self.pipeline.fit(X, y)
 
     def retrain(self, X, y):
         # Fit the pipeline with the updated data
         self.pipeline.fit(X, y)
 
     def predict(self, X):
```

### Comparing `madcat-0.84/chester/model_training/models/chester_models/linear_regression/linear_regression_utils.py` & `madcat-0.9/chester/model_training/models/chester_models/linear_regression/linear_regression_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/models/chester_models/logistic_regression/logistic_regression_model.py` & `madcat-0.9/chester/model_training/models/chester_models/logistic_regression/logistic_regression_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 from scipy.optimize._linesearch import LineSearchWarning
 from sklearn.compose import ColumnTransformer
 from sklearn.exceptions import ConvergenceWarning
 from sklearn.impute import SimpleImputer
 from sklearn.linear_model import LogisticRegression
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import OneHotEncoder
@@ -15,15 +14,14 @@
         self.parameters = parameters
         self.model = LogisticRegression()
         self.data_info = data_info
         self.categorical_features = self.data_info.feature_types_val["categorical"]
         self.numeric_features = self.data_info.feature_types_val["numeric"]
         self.transformer = None
         self.pipeline = None
-        self.feature_names = None
 
     def fit(self, X, y):
         import warnings
         warnings.filterwarnings("ignore", category=ConvergenceWarning)
         warnings.filterwarnings("ignore", category=LineSearchWarning)
         warnings.filterwarnings("ignore", category=UserWarning)
 
@@ -58,10 +56,7 @@
 
     def fit_transform(self, X, y):
         self.fit(X, y)
         return self.transform(X)
 
     def get_params(self):
         return self.parameters
-
-    def coef_(self):
-        return self.model.coef_
```

### Comparing `madcat-0.84/chester/model_training/models/chester_models/logistic_regression/logistic_regression_utils.py` & `madcat-0.9/chester/model_training/models/chester_models/logistic_regression/logistic_regression_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/models/cv_training.py` & `madcat-0.9/chester/model_training/models/cv_training.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/models/lstm.py` & `madcat-0.9/chester/model_training/models/lstm.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/model_training/models/scoring.py` & `madcat-0.9/chester/model_training/models/scoring.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/post_model_analysis/post_model_analysis_class.py` & `madcat-0.9/chester/post_model_analysis/post_model_analysis_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from wordcloud import WordCloud
 
-from chester.feature_stats.utils import create_pretty_table
 from chester.model_analyzer.model_analysis import AnalyzeMessages
 from chester.model_training.data_preparation import CVData
 from chester.post_model_analysis.post_regression import VisualizeRegressionResults
 from chester.zero_break.problem_specification import DataInfo
 
 
 class PostModelAnalysis:
@@ -19,39 +18,28 @@
         self.X_train = self.cv_data.train_data.drop(columns=[self.cv_data.target_column])
         self.y_train = self.cv_data.train_data[self.cv_data.target_column]
         self.X_test = self.cv_data.test_data.drop(columns=[self.cv_data.target_column])
         self.y_test = self.cv_data.test_data[self.cv_data.target_column]
         # retrain the model
         self.model.retrain(self.X_train, self.y_train)
         self.predict_test = self.model.predict(self.X_test)
-        from chester.util import ReportCollector, REPORT_PATH
-        self.rc = ReportCollector(REPORT_PATH)
 
     def plot_feature_importance(self, X_train: pd.DataFrame, top_feat=30):
         feature_importance = self.model.model.feature_importances_
         feature_importance = 100.0 * (feature_importance / feature_importance.max())
         feature_names = X_train.columns
         important_idx = np.argsort(feature_importance)
         data = {'feature_names': feature_names[important_idx],
                 'feature_importance': feature_importance[important_idx]}
         df = pd.DataFrame(data)
         print(AnalyzeMessages().feature_importance_message())
         df.sort_values(by='feature_importance', ascending=False, inplace=True)
+        sns.barplot(x='feature_importance', y='feature_names', data=df[0:top_feat])
         plt.figure(figsize=(15, 13))
         plt.title(f'Feature Importance (top {top_feat} features)')
-
-        feature_importance = {}
-        # Iterate over the rows of the DataFrame and add each feature and its importance to the dictionary
-        for i, row in df[0:100].iterrows():
-            feature = row['feature_names']
-            importance = int(round(row['feature_importance']))
-            feature_importance[feature] = importance
-        self.rc.save_object(feature_importance,
-                            text="Top 100 Feature importance (in %, 100 = the most important one):")
-        sns.barplot(x='feature_importance', y='feature_names', data=df[0:top_feat])
         self.plot_wordcloud_importance(df=df)
         plt.show()
 
     @staticmethod
     def plot_wordcloud_importance(df, title="Feature Importance Cloud"):
         """
         Plot word cloud of features weighted by their importance.
@@ -62,20 +50,19 @@
         df = df.sort_values(by='feature_importance', ascending=False)
         features_importance = list(zip(df['feature_names'], df['feature_importance']))
 
         wordcloud = WordCloud(
             random_state=21,
             normalize_plurals=True,
             max_words=100).generate_from_frequencies(dict(features_importance))
-        plt.figure(figsize=(12, 8))
-        plt.title(title, fontsize=15)
+        plt.figure(figsize=(10, 10))
         plt.imshow(wordcloud)
         plt.axis("off")
+        plt.title(title, fontsize=15)
         plt.show()
-        plt.close()
 
     def shap_values(self, X_train: pd.DataFrame, shap):
         explainer = shap.Explainer(self.model, X_train, check_additivity=False)
         shap_values = explainer(X_train, check_additivity=False)
         plt.title("SHAP values for train set")
         print(AnalyzeMessages().shap_values_message())
         shap.summary_plot(shap_values, X_train)
@@ -118,31 +105,28 @@
         if roc_curve:
             try:
                 self.roc_curve(self.X_test, self.y_test)
             except:
                 try:
                     self.roc_curve_multiclass(self.X_test, self.y_test)
                 except:
-                    return None
+                    pass
 
     def confusion_matrix(self, X_test: pd.DataFrame, y_test: pd.Series) -> None:
         from sklearn.metrics import confusion_matrix
         import seaborn as sns
         print(AnalyzeMessages().confusion_matrix_message())
 
         y_pred = self.model.predict(X_test)
         cm = confusion_matrix(y_test, y_pred)
-        self.rc.save_object(cm, text="confusion matrix on the test set")
-
         sns.heatmap(cm, annot=True, cmap='Blues', fmt='g')
         plt.title('Confusion Matrix')
         plt.xlabel('Predicted')
         plt.ylabel('Actual')
         plt.show()
-        plt.close()
 
     def roc_curve(self, X_test: pd.DataFrame, y_test: pd.Series) -> None:
         from sklearn.metrics import roc_curve, auc
         try:
             y_pred = self.model.predict(X_test)
             fpr, tpr, thresholds = roc_curve(y_test, y_pred)
             roc_auc = auc(fpr, tpr)
@@ -153,18 +137,16 @@
             plt.ylim([0.0, 1.05])
             plt.xlabel('False Positive Rate')
             plt.ylabel('True Positive Rate')
             plt.title('Receiver operating characteristic')
             plt.legend(loc="lower right")
             print(AnalyzeMessages().roc_curve_message())
             plt.show()
-            plt.close()
         except:
-            plt.close()
-            return None
+            pass
 
     def roc_curve_multiclass(self, X_test: pd.DataFrame, y_test: pd.Series) -> None:
         from sklearn.metrics import roc_auc_score, roc_curve
         from sklearn.preprocessing import label_binarize
         from scipy import interp
 
         y_test_bin = label_binarize(y_test, classes=np.unique(y_test))
@@ -201,92 +183,56 @@
         plt.ylim([0.0, 1.05])
         plt.xlabel('False Positive Rate')
         plt.ylabel('True Positive Rate')
         plt.title('Receiver operating characteristic')
         plt.legend(loc="lower right")
         print(AnalyzeMessages().roc_curve_message())
         plt.show()
-        plt.close()
 
     def learning_curve(self, X: pd.DataFrame, y: pd.Series) -> None:
         import os
         import sys
 
         original_stderr = sys.stderr
         sys.stderr = open(os.devnull, 'w')
         try:
             from sklearn.model_selection import learning_curve
-            metric_name = self.data_info.metrics_detector_val[0].lower()
-            metric_name = 'roc_auc' if metric_name == 'roc' else metric_name
-            metric_name = 'neg_mean_squared_error' if metric_name == 'mse' else metric_name
-            train_sizes, train_scores, test_scores = learning_curve(self.model.model, X, y, cv=5, scoring=metric_name)
+            train_sizes, train_scores, test_scores = learning_curve(self.model.model, X, y, cv=5, scoring='accuracy')
             train_scores_mean = np.mean(train_scores, axis=1)
             train_scores_std = np.std(train_scores, axis=1)
             test_scores_mean = np.mean(test_scores, axis=1)
             test_scores_std = np.std(test_scores, axis=1)
-
-            # create the pandas DataFrame
-            learning_curve_df = pd.DataFrame({
-                'train_sizes': train_sizes,
-                'train_scores_mean': train_scores_mean,
-                'train_scores_std': train_scores_std,
-                'test_scores_mean': test_scores_mean,
-                'test_scores_std': test_scores_std
-            })
-            self.rc.save_object(obj=create_pretty_table(learning_curve_df),
-                                text="Learning curve by training examples")
-
-            if len(test_scores_std) == 0:
-                plt.close()
-                return None
             plt.plot(train_sizes, train_scores_mean, 'o-', color="r", label="Training score")
             plt.plot(train_sizes, test_scores_mean, 'o-', color="g", label="Cross-validation score")
-            plt.fill_between(train_sizes, train_scores_mean - train_scores_std, train_scores_mean + train_scores_std,
-                             alpha=0.1, color="r")
+            plt.fill_between(train_sizes, train_scores_mean - train_scores_std,
+                             train_scores_mean + train_scores_std, alpha=0.1, color="r")
             plt.fill_between(train_sizes, test_scores_mean - test_scores_std,
                              test_scores_mean + test_scores_std, alpha=0.1, color="g")
             plt.grid()
             plt.xlabel("Training examples")
             plt.ylabel("Accuracy Score")
             plt.title("Learning Curve")
             plt.legend(loc="best")
             print(AnalyzeMessages().learning_curve_message())
             plt.show()
-            plt.close()
         except:
-            plt.close()
-            return None
+            pass
         finally:
-            plt.close()
             sys.stderr = original_stderr
 
     def coefficients(self) -> None:
         try:
-            coef = self.model.coef_[0]
-            abs_coef = np.abs(self.model.coef_[0])
-            top_100_coef_idx = np.argsort(abs_coef)[::-1][:100]
-            top_100_coef_values = [self.model.coef_[0][i] for i in top_100_coef_idx]
-            self.rc.save_object(top_100_coef_values, text="First 100 model coefficients: ")
-            feature_names = self.model.feature_names
+            coef = self.model.model.coef_[0]
+            print(coef)
             if len(coef) < 10:
                 plt.bar(np.arange(len(coef)), coef)
-                plt.xticks(np.arange(len(coef)), feature_names, rotation=90)
                 plt.title("Coefficients for logistic regression model")
                 plt.xlabel("Features")
                 plt.ylabel("Values")
             else:
                 sns.violinplot(coef, inner="stick")
                 plt.title("Coefficients distribution for logistic regression model")
                 plt.xlabel("Coefficients")
                 print(AnalyzeMessages().coefficients_message())
             plt.show()
-            plt.close()
-
-            coef_dict = {}
-            for i in range(len(feature_names)):
-                coef_dict[feature_names[i]] = abs(coef[i])
-            sorted_coef_dict = dict(sorted(coef_dict.items(), key=lambda x: x[1], reverse=True)[:100])
-            self.rc.save_object(obj=sorted_coef_dict,
-                                text="Top 100 feature with highest abs(coef): ")
         except:
-            plt.close()
-            return None
+            pass
```

### Comparing `madcat-0.84/chester/post_model_analysis/post_regression.py` & `madcat-0.9/chester/post_model_analysis/post_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,7 @@
     def all_plots(self):
         fig, axs = plt.subplots(2, 2, figsize=(15, 15))
         self.scatter_plot(axs[0, 0])
         self.residual_plot(axs[0, 1])
         self.histogram_plot(axs[1, 0])
         self.qq_plot(axs[1, 1])
         plt.show()
-        plt.close()
```

### Comparing `madcat-0.84/chester/pre_model_analysis/categorical.py` & `madcat-0.9/chester/pre_model_analysis/categorical.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,64 +12,57 @@
 
 from chester.zero_break.problem_specification import DataInfo
 
 
 class CategoricalPreModelAnalysis:
     def __init__(self, data_info: DataInfo):
         self.data_info = data_info
-        self.cols = list(set(self.data_info.feature_types_val["categorical"]))
-        # drop dups
-        if self.data_info.data.columns.duplicated().any():
-            drop_dup_data = self.data_info.data.loc[:, ~ self.data_info.data.columns.duplicated()]
-            self.data = drop_dup_data
-            self.data_info.data = drop_dup_data
+        self.cols = self.data_info.feature_types_val["categorical"]
         self.n_cols = len(self.cols)
         self.target = self.data_info.data[self.data_info.target]
         self.target_df = self.data_info.data[[self.data_info.target]]
         self.data = self.data_info.data[self.cols]
         # calc
         self.cols_sorted = self.sort_by_pvalue()
         self.cols_sorted_with_pvalue = None
 
     def tsne(self):
-        X = self.data.copy()
-        X = X.sample(n=5000)
-        target = self.target[X.index]
-
-        X_tsne_2d = TSNE(n_components=2).fit_transform(pd.get_dummies(X))
+        X_tsne_3d = TSNE(n_components=3).fit_transform(pd.get_dummies(self.data))
+        X_tsne_2d = X_tsne_3d[:, :2]
 
         fig = plt.figure(figsize=(16, 10))
         ax1 = plt
         # ax2 = fig.add_subplot(122, projection='3d')
         if self.data_info.problem_type_val in ["Regression"]:
-            ax1.hexbin(X_tsne_2d[:, 0], X_tsne_2d[:, 1], C=target, gridsize=50, cmap='viridis', edgecolors='black')
+            ax1.hexbin(X_tsne_2d[:, 0], X_tsne_2d[:, 1], C=self.target, gridsize=50, cmap='viridis', edgecolors='black')
             # ax2.scatter(X_tsne_3d[:, 0], X_tsne_3d[:, 1], X_tsne_3d[:, 2], c=self.target, cmap='viridis')
             ax1.title("Visualizing Categorical Features and Target with t-SNE (2D)")
             # ax2.set_title("Visualizing Categorical Features and Target with t-SNE (3D)")
         elif self.data_info.problem_type_val in ["Binary regression", "Binary classification"]:
-            target_classes = target.unique()
+            target_classes = self.target.unique()
             color_map = {target_class: color for target_class, color in zip(target_classes, ['red', 'blue'])}
-            colors = target.apply(lambda x: color_map[x])
+            colors = self.target.apply(lambda x: color_map[x])
             ax1.scatter(X_tsne_2d[:, 0], X_tsne_2d[:, 1], c=colors)
             # ax2.scatter(X_tsne_3d[:, 0], X_tsne_3d[:, 1], X_tsne_3d[:, 2], c=colors)
             legend_handles = [Patch(color=color_map[target_class], label=target_class) for target_class in
                               target_classes]
             ax1.title("Visualizing Categorical Features and Target with t-SNE (2D)")
             # ax2.set_title("Visualizing Categorical Features and Target with t-SNE (3D)")
             ax1.legend(handles=legend_handles)
         else:  # Multi-class classification
-            target_classes = target.unique()
+            target_classes = self.target.unique()
             color_map = {target_class: color for target_class, color in
                          zip(target_classes, plt.cm.rainbow(np.linspace(0, 1, len(target_classes))))}
             ax1.legend(
                 handles=[Patch(color=color_map[target_class], label=target_class) for target_class in target_classes])
             # ax2.legend(
             #     handles=[Patch(color=color_map[target_class], label=target_class) for target_class in target_classes])
-        plt.show()
-        plt.close()
+
+    def any_categorical(self):
+        return True if len(self.cols) > 0 else False
 
     def sort_by_pvalue(self):
         from sklearn.cluster import KMeans
         from scipy.stats import chi2_contingency
         import warnings
         warnings.simplefilter("ignore")
 
@@ -93,149 +86,118 @@
             feature_pvalue_list.append((col, pvalue))
 
         sorted_list = sorted(feature_pvalue_list, key=lambda x: x[1], reverse=False)
         self.cols_sorted_with_pvalue = sorted_list
         return [x[0] for x in sorted_list]
 
     def analyze_pvalue(self, is_plot=True, top_features=10):
-        from chester.util import ReportCollector, REPORT_PATH
-        rc = ReportCollector(REPORT_PATH)
         self.sort_by_pvalue()
-        rc.save_object(self.cols_sorted_with_pvalue[0:50],
-                       text="top 50 with lowest partial pvalue for categorical feat based on chi square:")
         if len(self.cols) == 0:
             return None
+        self.plot_wordcloud_pvalues(self.cols_sorted_with_pvalue)
         if is_plot:
-            self.plot_wordcloud_pvalues(self.cols_sorted_with_pvalue)
             if self.n_cols > 50:
+                print("plotting!")
                 self.plot_histogram_pvalues(self.cols_sorted_with_pvalue)
         print("Pvalues for top categorical features:")
         print(pd.DataFrame(self.cols_sorted_with_pvalue[0:top_features], columns=["feature", "pvalue"]))
 
     def partial_plot(self, classification_row_percent=True):
         import warnings
         warnings.simplefilter("ignore")
         top_features = 25
+
         if self.n_cols <= 25:
             sample_features = self.n_cols
             top_features = self.n_cols
         else:
-            sample_features = min(50, int(self.n_cols / 2))
-        top_features = min(top_features, sample_features)
-        top_feature_names = random.sample(self.cols_sorted[0:sample_features], top_features)
-        feature_index = {feature: index for index, feature in enumerate(self.cols_sorted)}
+            sample_features = min(2 * 25, int(self.n_cols / 2))
+        top_feature_names = random.sample(self.cols_sorted[0:top_features], sample_features)
+        feature_index = {feature: index for index, feature in enumerate(self.cols_sorted[0:top_features])}
         top_feature_names.sort(key=lambda x: feature_index[x])
         if self.data_info.problem_type_val in ["Binary regression", "Binary classification"]:
-            if top_features == 1:
-                fig, ax = plt.subplots(figsize=(14, 10))
-                if classification_row_percent:
-                    plt.suptitle("Partial Plot to Identify Patterns between Sampled Categorical Features and Target\n"
-                                 "Showing % from Feature (row)",
-                                 fontsize=14, fontweight='bold')
-                else:
-                    plt.suptitle("Partial Plot to Identify Patterns between Sampled Categorical Features and Target\n"
-                                 "Showing % from Target (column)",
-                                 fontsize=14, fontweight='bold')
+            max_plots = 9
+            top_n = self.data[:top_features].columns
+            dim = math.ceil(math.sqrt(len(top_n)))
+            num_rows = math.ceil(max_plots / dim)
+            fig, ax = plt.subplots(dim, dim)
+            fig.tight_layout()
+            if classification_row_percent:
+                plt.suptitle("Partial Plot to Identify Patterns between Sampled Categorical Features and Target\n"
+                             "Showing % from Feature (row)",
+                             fontsize=14, fontweight='bold')
+            else:
+                plt.suptitle("Partial Plot to Identify Patterns between Sampled Categorical Features and Target\n"
+                             "Showing % from Target (column)",
+                             fontsize=14, fontweight='bold')
+            plt.figure(figsize=(15, 15))
+            for i, col in enumerate(top_feature_names):
+                if i >= num_rows * num_rows:
+                    return None
+                ax_i = ax[i // dim, i % dim]
                 if classification_row_percent:
-                    crosstab = pd.crosstab(self.data[top_feature_names[0]], self.target, normalize='index') * 100
+                    crosstab = pd.crosstab(self.data[col], self.target, normalize='index') * 100
                     crosstab = crosstab[(crosstab.T != 0).any()]
                     crosstab = crosstab.loc[:, (crosstab != 0).any(axis=0)]
                     crosstab = crosstab.loc[crosstab.sum(axis=1).sort_values(ascending=False).index[:5]]
                 else:
-                    crosstab = pd.crosstab(self.data[top_feature_names[0]], self.target, normalize='columns') * 100
+                    crosstab = pd.crosstab(self.data[col], self.target, normalize='columns') * 100
                     crosstab = crosstab[(crosstab.T != 0).any()]
                     crosstab = crosstab.loc[:, (crosstab != 0).any(axis=0)]
                     crosstab = crosstab.loc[crosstab.sum(axis=1).sort_values(ascending=False).index[:5]]
-                sns.heatmap(crosstab, annot=False, cmap="YlGnBu", fmt='g', ax=ax)
-                ax.set_ylabel(None)
-                ax.set_xlabel(None)
-                ax.set_title(top_feature_names[0], fontsize=12, fontweight='bold')
-                plt.show()
-                plt.close()
-
-            else:
-                max_plots = min(9, top_features)
-                dim = min(math.ceil(math.sqrt(max_plots)), 2)
-                fig, ax = plt.subplots(dim, dim, figsize=(14, 4 + 4 * dim))
-                fig.tight_layout()
-                if classification_row_percent:
-                    plt.suptitle("Partial Plot to Identify Patterns between Sampled Categorical Features and Target\n"
-                                 "Showing % from Feature (row)",
-                                 fontsize=14, fontweight='bold')
-                else:
-                    plt.suptitle("Partial Plot to Identify Patterns between Sampled Categorical Features and Target\n"
-                                 "Showing % from Target (column)",
-                                 fontsize=14, fontweight='bold')
-                for i, col in enumerate(top_feature_names):
-                    if i >= dim * dim:
-                        break
-                    ax_i = ax[i // dim, i % dim]
-                    if classification_row_percent:
-                        crosstab = pd.crosstab(self.data[col], self.target, normalize='index') * 100
-                        crosstab = crosstab[(crosstab.T != 0).any()]
-                        crosstab = crosstab.loc[:, (crosstab != 0).any(axis=0)]
-                        crosstab = crosstab.loc[crosstab.sum(axis=1).sort_values(ascending=False).index[:5]]
-                    else:
-                        crosstab = pd.crosstab(self.data[col], self.target, normalize='columns') * 100
-                        crosstab = crosstab[(crosstab.T != 0).any()]
-                        crosstab = crosstab.loc[:, (crosstab != 0).any(axis=0)]
-                        crosstab = crosstab.loc[crosstab.sum(axis=1).sort_values(ascending=False).index[:5]]
-                    sns.heatmap(crosstab, annot=False, cmap="YlGnBu", fmt='g', ax=ax_i)
-                    ax_i.set_ylabel(None)
-                    ax_i.set_xlabel(None)
-                    ax_i.set_title(col, fontsize=12, fontweight='bold')
-                plt.tight_layout()
-                plt.show()
-                plt.close()
+                sns.heatmap(crosstab, annot=False, cmap="YlGnBu", fmt='g', ax=ax_i)
+                ax_i.set_ylabel(None)
+                ax_i.set_xlabel(None)
+                ax_i.set_title(col, fontsize=12, fontweight='bold')
+            plt.tight_layout()
+            plt.show()
         if self.data_info.problem_type_val in ["Regression"]:
-            max_plots = 9
-            top_n = self.data[:top_features].columns
-            dim = max(math.floor(math.sqrt(min(max_plots, len(top_n)))), 2)
-            fig, ax = plt.subplots(dim, dim, figsize=(20, 4 + 4 * dim))
+            from sklearn.cluster import KMeans
             target = self.target
-            plt.suptitle(
-                "Partial Plot to Identify Patterns between Categorical Sampled Features and Target (grouped by kmeans)",
-                fontsize=16,
-                fontweight='bold')
-            grid_size = math.ceil(math.sqrt(top_features))
+            kmeans = KMeans(n_clusters=10)
+            kmeans.fit(self.target_df)
+            target_labels = kmeans.labels_
+            plt.figure(figsize=(15, 15))
+            plt.suptitle("Partial Plot to Identify Patterns between Categorical Sampled Features and Target",
+                         fontsize=16,
+                         fontweight='bold')
+            grid_size = 4
             num_features = min(grid_size * grid_size, top_features)
+            num_rows = int(np.ceil(num_features / grid_size))
             for i, col in enumerate(top_feature_names[:num_features]):
-                if i >= dim * dim:
-                    break
-                plt.subplot(dim, dim, i + 1)
-                column = self.data[col].apply(lambda x: "'" + str(x))
-                new_df = pd.concat([column, target], axis=1)
-                top_values = list(column.value_counts().nlargest(5).index)
-                data_filtered = new_df[column.isin(top_values)]
-                sns.boxplot(x=col, y=target, data=data_filtered)
-                plt.ylabel("Target")
+                plt.subplot(num_rows, grid_size, i + 1)
+                column = self.data[col]
+                if column.dtype == "object":
+                    column = column.astype("category").cat.codes
+                    column = column[column < 5]
+                crosstab = pd.crosstab(target_labels, column, normalize='index')
+                sns.heatmap(crosstab, annot=False, cmap='Greens', cbar=True)
+                plt.ylabel("Clusters")
                 plt.xlabel("{} Value".format(col))
                 plt.subplots_adjust(hspace=0.5, wspace=0.5)
-            plt.show()
-            plt.close()
         elif self.data_info.problem_type_val in ["Multiclass classification"]:
-            max_plots = 16
-            top_n = self.data[:max_plots].columns
-            dim = max(math.floor(math.sqrt(len(top_n))), 2)
-            fig, ax = plt.subplots(dim, dim, figsize=(19, 4 * dim))
-            fig.tight_layout()
+            plt.figure(figsize=(16, 16))
             plt.suptitle(
                 "Heatmap to Show Correlation between Sampled Categorical Features (top 5 categories) and Target",
-                fontsize=15,
+                fontsize=16,
                 fontweight='bold')
+            top_features = 16
+            top_feature_names = self.data[:top_features].columns
+            rows = 4
+            cols = 4
             for i, col in enumerate(top_feature_names):
-                if i >= dim * dim:
-                    break
-                plt.subplot(dim, dim, i + 1)
+                if i > 15:
+                    return None
+                plt.subplot(rows, cols, i + 1)
                 crosstab = pd.crosstab(self.data[col], self.target, normalize='index') * 100
                 crosstab = crosstab[(crosstab.T != 0).any()]
                 crosstab = crosstab.loc[:, (crosstab != 0).any(axis=0)]
                 crosstab = crosstab.loc[crosstab.sum(axis=1).sort_values(ascending=False).index[:5]]
                 sns.heatmap(crosstab, annot=False, cmap="YlGnBu", fmt='g')
-                plt.title(col, fontsize=10, fontweight='bold')
+                plt.title(col, fontsize=12, fontweight='bold')
             plt.show()
             plt.close()
 
     @staticmethod
     def plot_histogram_pvalues(features_pvalues):
         """
         Plot histogram of p-values for features.
@@ -263,19 +225,17 @@
         """
         Plot word cloud of features weighted by their p-value.
         :param features_pvalues: List of tuples (column name, pvalue).
         :param title: Title of the plot.
         :return: None.
         """
         features_pvalues = [(feature, 1 - pvalue) for feature, pvalue in features_pvalues]
-
-        n_features = len(features_pvalues)
-        width = min(int(900 * n_features / 4), 900)
-        height = min(int(500 * n_features / 4), 500)
-        wordcloud = WordCloud(width=width, height=height).generate_from_frequencies(dict(features_pvalues))
+        wordcloud = WordCloud(
+            random_state=21,
+            normalize_plurals=True).generate_from_frequencies(dict(features_pvalues))
         plt.imshow(wordcloud)
         plt.axis("off")
         plt.title(title, fontsize=15)
         plt.show()
         plt.close()
 
     def run(self, is_plot=True):
@@ -283,24 +243,20 @@
             self.analyze_pvalue(is_plot=is_plot)
             if is_plot:
                 if 'classification' or 'binary regression' in self.data_info.problem_type_val.lower():
                     self.partial_plot(classification_row_percent=False)
                     self.partial_plot(classification_row_percent=True)
                 else:
                     self.partial_plot()
-                try:
-                    self.tsne()
-                except:
-                    pass
+                self.tsne()
         elif self.n_cols == 1:
             self.analyze_pvalue(is_plot=is_plot)
             if is_plot:
                 self.partial_plot()
         plt.show()
-        plt.close()
 
 
 def format_df(df, max_value_width=10, ci_max_value_width=15, ci_col="CI"):
     pd.options.display.max_columns = None
 
     def trim_value(val):
         if len(str(val)) > max_value_width:
```

### Comparing `madcat-0.84/chester/pre_model_analysis/numerics.py` & `madcat-0.9/chester/pre_model_analysis/numerics.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,270 +19,228 @@
 
 from chester.zero_break.problem_specification import DataInfo
 
 
 class NumericPreModelAnalysis:
     def __init__(self, data_info: DataInfo):
         self.data_info = data_info
-        self.cols = list(set(self.data_info.feature_types_val["numeric"]))
+        self.cols = self.data_info.feature_types_val["numeric"]
         self.n_cols = len(self.cols)
         self.target = self.data_info.data[self.data_info.target]
         self.target_df = self.data_info.data[[self.data_info.target]]
         self.data = self.data_info.data[self.cols]
         # calc
         self.cols_sorted = self.sort_by_pvalue()
         self.cols_sorted_with_pvalue = None
 
     def tsne(self):
+
         if self.n_cols in (1, 2):
             return None
-        all_cols = list(self.data.columns)
-        ts_cols = list(set([name for name in all_cols if
-                            name.startswith("num_ts_mm") or name.startswith("num_ts_freq_") or
-                            (name.startswith("num_ts_") and (name.endswith("_sin") or name.endswith("_cos")))]))
-
-        not_ts_cols = [col for col in all_cols if col not in ts_cols]
-        if len(ts_cols) > 5:
-            numeric_cols = not_ts_cols + self.sample_list(ts_cols)
-        else:
-            numeric_cols = not_ts_cols
-        X = self.data[numeric_cols].copy()
-        X = X.sample(n=min(5000, len(X)))
-        target = self.target[X.index]
-
+        X = self.data.copy()
         numerical_transformer = SimpleImputer(strategy='median')
         transformer = ColumnTransformer(
             transformers=[
-                ('n', numerical_transformer, numeric_cols)
+                ('n', numerical_transformer, self.cols)
             ])
         pipeline = Pipeline(steps=[('preprocessor', transformer)])
         X = pipeline.fit_transform(X)
         scaler = StandardScaler()
         X = scaler.fit_transform(X)
-        try:
-            X_tsne_2d = TSNE(n_components=2).fit_transform(X)
-        except:
-            X_tsne_2d = TSNE(n_components=2, perplexity=10).fit_transform(X)
+
+        X_tsne_3d = TSNE(n_components=3).fit_transform(X)
+        X_tsne_2d = X_tsne_3d[:, :2]
         fig = plt.figure(figsize=(12, 12))
         # ax1 = fig.add_subplot(121)
         ax1 = plt
         # ax2 = fig.gca(122, projection='3d')
 
         if self.data_info.problem_type_val in ["Regression"]:
-            ax1.scatter(X_tsne_2d[:, 0], X_tsne_2d[:, 1], c=target, cmap='viridis')
+            ax1.scatter(X_tsne_2d[:, 0], X_tsne_2d[:, 1], c=self.target, cmap='viridis')
+            # ax2.scatter(X_tsne_3d[:, 0], X_tsne_3d[:, 1], X_tsne_3d[:, 2], c=self.target, cmap='viridis')
             ax1.title("Visualizing Numerical Features and Target with t-SNE (2D)")
             # ax2.set_title("Visualizing Numerical Features and Target with t-SNE (3D)")
         elif self.data_info.problem_type_val in ["Binary regression", "Binary classification"]:
-            target_classes = target.unique()
+            target_classes = self.target.unique()
             color_map = {target_class: color for target_class, color in zip(target_classes, ['red', 'blue'])}
-            colors = target.apply(lambda x: color_map[x])
+            colors = self.target.apply(lambda x: color_map[x])
             ax1.scatter(X_tsne_2d[:, 0], X_tsne_2d[:, 1], c=colors)
+            # ax2.scatter(X_tsne_3d[:, 0], X_tsne_3d[:, 1], X_tsne_3d[:, 2], c=colors)
             legend_handles = [Patch(color=color_map[target_class], label=target_class) for target_class in
                               target_classes]
             ax1.title("Visualizing Numerical Features and Target with t-SNE (2D)")
+            # ax2.set_title("Visualizing Numerical Features and Target with t-SNE (3D)")
             ax1.legend(handles=legend_handles)
         else:  # Multi-class classification
-            target = target.astype(str)
-            target_classes = target.unique()
+            target_classes = self.target.unique()
             color_map = {target_class: color for target_class, color in
                          zip(target_classes, plt.cm.rainbow(np.linspace(0, 1, len(target_classes))))}
-            try:
-                colors = target.apply(lambda x: color_map[x])
-            except:
-                colors = target.apply(lambda x: color_map[str(x)])
+            colors = self.target.apply(lambda x: color_map[x])
             plt.scatter(X_tsne_2d[:, 0], X_tsne_2d[:, 1], c=colors)
+            # ax2.scatter(X_tsne_3d[:, 0], X_tsne_3d[:, 1], X_tsne_3d[:, 2], c=colors)
             legend_handles = [Patch(color=color_map[target_class], label=target_class) for target_class in
                               target_classes]
             ax1.title("Visualizing Numerical Features and Target with t-SNE (2D)")
+            # ax2.set_title("Visualizing Numerical Features and Target with t-SNE (3D)")
             ax1.legend(handles=legend_handles)
-        plt.show()
-        plt.close()
-
-    @staticmethod
-    def sample_list(l):
-        if not l:
-            return []
-
-        n = len(l)
-        min_sample_size = max(5, int(0.2 * n))
-        max_sample_size = min(15, n)
-
-        sample_size = random.randint(min_sample_size, max_sample_size)
-        sample = random.sample(l, sample_size)
-
-        return sample
 
     @staticmethod
     def median_imputation(df):
         import warnings
         warnings.filterwarnings("ignore", category=SettingWithCopyWarning)
 
         median = df.median()
         df.fillna(median, inplace=True)
         return df
 
     def any_numeric(self):
         return True if len(self.cols) > 0 else False
 
     def sort_by_pvalue(self):
-        try:
-            import warnings
-            warnings.simplefilter("ignore")
-
-            problem_type = self.data_info.problem_type_val
-
-            if problem_type in ["Regression"]:
-                num_groups = max(2, min(floor(self.data_info.rows / 20), 10))
-                kmeans = KMeans(n_clusters=num_groups, n_init=10)
-                kmeans.fit(self.target_df)
-                target_labels = kmeans.labels_
-
-            feature_pvalue_list = []
-            for col in self.cols:
-                data_col = self.data[[col]]
-                num_groups = min(floor(self.data_info.rows / 20), 10)
-                kmeans = KMeans(n_clusters=num_groups, n_init=10)
-                if self.data[col].isna().any():
-                    data_col = self.median_imputation(data_col)
-                kmeans.fit(data_col)
-                labels = kmeans.labels_
-                if problem_type == "Regression":
-                    contingency_table = pd.crosstab(index=labels, columns=target_labels)
-                    chi2, pvalue, _, _ = chi2_contingency(contingency_table)
-                else:
-                    contingency_table = pd.crosstab(index=labels, columns=self.target)
-                    chi2, pvalue, _, _ = chi2_contingency(contingency_table)
-                feature_pvalue_list.append((col, pvalue))
-
-            sorted_list = sorted(feature_pvalue_list, key=lambda x: x[1], reverse=False)
-            self.cols_sorted_with_pvalue = sorted_list
-            return [x[0] for x in sorted_list]
-        except:
-            return self.cols
+        import warnings
+        warnings.simplefilter("ignore")
+
+        problem_type = self.data_info.problem_type_val
+
+        if problem_type in ["Regression"]:
+            num_groups = min(floor(self.data_info.rows / 20), 10)
+            kmeans = KMeans(n_clusters=num_groups, n_init=10)
+            kmeans.fit(self.target_df)
+            target_labels = kmeans.labels_
+
+        feature_pvalue_list = []
+        for col in self.cols:
+            data_col = self.data[[col]]
+            num_groups = min(floor(self.data_info.rows / 20), 10)
+            kmeans = KMeans(n_clusters=num_groups, n_init=10)
+            if self.data[col].isna().any():
+                data_col = self.median_imputation(data_col)
+            kmeans.fit(data_col)
+            labels = kmeans.labels_
+            if problem_type == "Regression":
+                contingency_table = pd.crosstab(index=labels, columns=target_labels)
+                chi2, pvalue, _, _ = chi2_contingency(contingency_table)
+            else:
+                contingency_table = pd.crosstab(index=labels, columns=self.target)
+                chi2, pvalue, _, _ = chi2_contingency(contingency_table)
+            feature_pvalue_list.append((col, pvalue))
+
+        sorted_list = sorted(feature_pvalue_list, key=lambda x: x[1], reverse=False)
+        self.cols_sorted_with_pvalue = sorted_list
+        return [x[0] for x in sorted_list]
 
     def analyze_pvalue(self, is_plot=True, top_features=10):
-        from chester.util import ReportCollector, REPORT_PATH
-        rc = ReportCollector(REPORT_PATH)
         self.sort_by_pvalue()
-        rc.save_object(self.cols_sorted_with_pvalue[0:50],
-                       text="top 50 with lowest partial pvalue for numerical feat, based on chi square:")
         self.plot_wordcloud_pvalues(self.cols_sorted_with_pvalue)
         if is_plot:
             if self.n_cols > 50:
                 print("Numerical Pvalues plot:")
                 self.plot_histogram_pvalues(self.cols_sorted_with_pvalue)
-        print("Pvalues for Top Numerical Features for Chi Square test:")
+        print("Pvalues for top numerical features for chi square test:")
         print(pd.DataFrame(self.cols_sorted_with_pvalue[0:top_features], columns=["feature", "pvalue"]))
+        return None
 
     @staticmethod
     def plot_histogram_pvalues(features_pvalues):
         """
         Plot histogram of p-values for features.
         :param features_pvalues: List of tuples (column name, pvalue).
         :return: None.
         """
         pvalues = [pvalue for _, pvalue in features_pvalues]
         fig, ax = plt.subplots()
-        plt.figure(figsize=(13, 10))
+        plt.figure(figsize=(15, 15))
         ax.hist(pvalues, bins=50, edgecolor='k', color='#2ecc71')
         ax.set_title("Histogram of P-values for Numerical Features", fontsize=18)
         ax.set_xlabel("P-value", fontsize=17)
         ax.set_ylabel("Frequency", fontsize=17)
         ax.spines['right'].set_visible(False)
         ax.spines['top'].set_visible(False)
         ax.spines['left'].set_linewidth(0.5)
         ax.spines['bottom'].set_linewidth(0.5)
         ax.tick_params(axis='both', which='both', labelsize=12)
         plt.show()
-        plt.close()
+        return None
 
     @staticmethod
     def plot_wordcloud_pvalues(features_pvalues,
-                               title="Numeric Features Pvalues Word Cloud Based on Partial Plot"):
+                               title="Numeric Features Pvalues Based on Partial Plot"):
         """
         Plot word cloud of features weighted by their p-value.
         :param features_pvalues: List of tuples (column name, pvalue).
         :param title: Title of the plot.
         :return: None.
         """
-        features_pvalues = [(feature, 1 - pvalue + 0.00001) for feature, pvalue in features_pvalues]
-        wordcloud = WordCloud(width=900, height=500). \
-            generate_from_frequencies(dict(features_pvalues))
-        plt.title(title, fontsize=15)
+        features_pvalues = [(feature, 1 - pvalue) for feature, pvalue in features_pvalues]
+        wordcloud = WordCloud(
+            random_state=21,
+            normalize_plurals=True).generate_from_frequencies(dict(features_pvalues))
         plt.imshow(wordcloud)
+        plt.figure(figsize=(12, 12))
+        plt.title(title, fontsize=15)
         plt.show()
-        plt.close()
+        return None
 
     def partial_plot(self, classification_row_percent=True):
         import warnings
         warnings.simplefilter("ignore")
-        top_features = min(self.n_cols, 25)
+        top_features = 25
         if self.n_cols <= 25:
             sample_features = self.n_cols
+            top_features = self.n_cols
         else:
             sample_features = min(2 * 25, int(self.n_cols / 2))
-        A = max(top_features, sample_features)
-        B = min(top_features, sample_features)
-        top_feature_names = random.sample(self.cols_sorted[0:A], B)
+        top_feature_names = random.sample(self.cols_sorted[0:sample_features], top_features)
         feature_index = {feature: index for index, feature in enumerate(self.cols_sorted)}
         top_feature_names.sort(key=lambda x: feature_index[x])
 
-        dim = math.ceil(math.sqrt(top_features))
-        num_rows = math.ceil(top_features / dim)
+        num_plots = len(top_feature_names)
+        dim = math.ceil(math.sqrt(num_plots))
+        num_rows = math.ceil(num_plots / dim)
+        fig, ax = plt.subplots(num_rows, dim)
+        plt.figure(figsize=(15, 15))
         if self.data_info.problem_type_val in ["Binary regression"]:
-            try:
-                fig, ax = plt.subplots(num_rows, dim)
-                plt.figure(figsize=(18, 15))
-                plt.suptitle("Partial Plot to Identify Patterns between Sampled Numeric Features and Target",
-                             fontsize=16, fontweight='bold')
-                for i in range(len(top_feature_names)):
-                    col = top_feature_names[i]
-                    column = self.data[col]
-                    target = self.target
-                    ax_i = ax[i // dim, i % dim]
-                    sns.regplot(x=column, y=target, logistic=True, n_boot=250, y_jitter=.03, ax=ax_i)
-                    ax_i.set_xlabel("")
-                    ax_i.set_ylabel("")
-                    ax_i.set_title(col, fontweight='bold', transform=ax_i.transAxes, y=0.5)
-                plt.show()
-                plt.close()
-            except:
-                pass
-        elif self.data_info.problem_type_val in ["Regression"]:
-            plt.figure(figsize=(18, 15))
+            plt.suptitle("Partial Plot to Identify Patterns between Sampled Numeric Features and Target",
+                         fontsize=16, fontweight='bold')
+            for i in range(len(top_feature_names)):
+                col = top_feature_names[i]
+                column = self.data[col]
+                target = self.target
+                ax_i = ax[i // dim, i % dim]
+                sns.regplot(x=column, y=target, logistic=True, n_boot=250, y_jitter=.03, ax=ax_i)
+                ax_i.set_xlabel("")
+                ax_i.set_ylabel("")
+                ax_i.set_title(col, fontweight='bold', transform=ax_i.transAxes, y=0.5)
+            plt.show()
+        if self.data_info.problem_type_val in ["Regression"]:
             plt.suptitle("Partial Plot to Identify Patterns between Sampled Numeric Features and Target", fontsize=16,
                          fontweight='bold')
-            for i, col in enumerate(top_feature_names[:top_features]):
-                plt.subplot(num_rows, dim, i + 1)
+            grid_size = 4
+            num_features = min(grid_size * grid_size, top_features)
+            num_rows = int(np.ceil(num_features / grid_size))
+            for i, col in enumerate(top_feature_names[:num_features]):
+                plt.subplot(num_rows, grid_size, i + 1)
                 column = self.data[col]
                 target = self.target
                 plt.scatter(column, target)
                 plt.xlabel(col)
                 plt.ylabel(self.data_info.target)
             plt.show()
-            plt.close()
         elif self.data_info.problem_type_val in ["Multiclass classification", "Binary classification"]:
-            dim = min(dim, 3)
-            fig, axs = plt.subplots(nrows=dim, ncols=dim, figsize=(18, 15))
             if classification_row_percent:
                 plt.suptitle("Partial Plot to Identify Patterns between Sampled Numeric Features and Target\n"
                              "Showing % from cluster (row)",
                              fontsize=14, fontweight='bold')
             else:
                 plt.suptitle("Partial Plot to Identify Patterns between Sampled Numeric Features and Target\n"
                              "Showing % from Target (column)",
                              fontsize=14, fontweight='bold')
-            for i in range(min(len(top_feature_names), dim * dim)):
-                if i < dim * dim:
-                    row = i // dim
-                    col = i % dim
-                    try:
-                        ax = axs[row, col]
-                    except:
-                        ax = axs
+            for i in range(len(top_feature_names)):
+                if i < 9:
+                    plt.subplot(3, 3, i + 1)
                     col = top_feature_names[i]
                     data_col = self.data[[col]]
                     num_groups = min(floor(self.data_info.rows / 20), 10)
                     kmeans = KMeans(n_clusters=num_groups, n_init=10)
                     if self.data[col].isna().any():
                         data_col = self.median_imputation(data_col)
                     kmeans.fit(data_col)
@@ -291,20 +249,19 @@
                     target_filtered = self.target[self.target.isin(top_5_target_values)]
                     labels_filtered = labels[self.target.isin(top_5_target_values)]
                     contingency_table = pd.crosstab(index=labels_filtered, columns=target_filtered)
                     if classification_row_percent:
                         contingency_table_pct = contingency_table.div(contingency_table.sum(1), axis=0)
                     else:
                         contingency_table_pct = contingency_table.div(contingency_table.sum(0), axis=1)
-                    sns.heatmap(contingency_table_pct, annot=False, cmap='Blues', ax=ax)
-                    ax.set_ylabel(col, fontsize=12, fontweight='bold')
-                    ax.set_xlabel(None)
-
+                    sns.heatmap(contingency_table_pct, annot=False, cmap='Blues')
+                    plt.ylabel(col, fontsize=12, fontweight='bold')
+                    plt.xlabel(None)
             plt.show()
-            plt.close()
+            return None
 
     def run(self, plot=True):
         if self.n_cols > 1:
             self.analyze_pvalue(is_plot=plot)
             if ('classification' in self.data_info.problem_type_val.lower()) and plot:
                 self.partial_plot(classification_row_percent=True)
                 self.partial_plot(classification_row_percent=False)
@@ -315,15 +272,15 @@
             self.analyze_pvalue()
             if ('classification' in self.data_info.problem_type_val.lower()) and plot:
                 self.partial_plot(classification_row_percent=True)
                 self.partial_plot(classification_row_percent=False)
             else:
                 if plot:
                     self.partial_plot()
-        plt.close()
+        return None
 
 
 def format_df(df, max_value_width=10, ci_max_value_width=15, ci_col="CI"):
     pd.options.display.max_columns = None
 
     def trim_value(val):
         if len(str(val)) > max_value_width:
```

### Comparing `madcat-0.84/chester/preprocessing/preprocessing_func.py` & `madcat-0.9/chester/preprocessing/preprocessing_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import nltk
 import pandas as pd
 from nltk.corpus import wordnet
 from nltk.stem import PorterStemmer, SnowballStemmer, LancasterStemmer
 from nltk.stem import WordNetLemmatizer
 
-from chester.util import ReportCollector, REPORT_PATH
-
 
 def get_stemmer(name=None):
     if name == "porter":
         return PorterStemmer()
     elif name == "snowball":
         return SnowballStemmer("english")
     elif name == "lancaster":
@@ -134,18 +132,16 @@
                 report_str += f"Using {self.lemmatizer} lemmatizer, "
             else:
                 report_str += "Lemmatizing text, "
         if self.tokenize_flag:
             report_str += "Tokenizing text, "
         if report_str:
             report_str = report_str[:-2]
-            title_to_print = f"The following preprocessing steps will be applied to the column '{self.text_column}': {report_str}."
-            print(title_to_print)
-            rc = ReportCollector(REPORT_PATH)
-            rc.save_text(title_to_print)
+            print(
+                f"The following preprocessing steps will be applied to the column '{self.text_column}': {report_str}.")
         else:
             print("No preprocessing steps selected.")
 
 
 def preprocess_text_df(text_preprocessor: TextPreprocessor):
     df = text_preprocessor.df
     text_column = text_preprocessor.text_column
```

### Comparing `madcat-0.84/chester/preprocessing/preprocessor_handler.py` & `madcat-0.9/chester/preprocessing/preprocessor_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from chester.preprocessing import preprocessing_func as pp
-from chester.util import ReportCollector, REPORT_PATH
 from chester.zero_break.problem_specification import DataInfo
 
 
 class PreprocessHandler:
     def __init__(self, data_info: DataInfo, text_pre_process: pp.TextPreprocessor = None):
         self.data_info = data_info
         self.text_pre_process = text_pre_process
@@ -22,13 +21,10 @@
         for col in text_columns:
             if self.text_pre_process is not None:
                 curr_text_pre_processor = self.text_pre_process
                 curr_text_pre_processor.text_column = col
                 text_reprocess = curr_text_pre_processor
             else:
                 text_reprocess = pp.TextPreprocessor(self.data_info.data, text_column=col)
-            title_to_print = f"{col} column preprocessing"
-            print(title_to_print)
-            rc = ReportCollector(REPORT_PATH)
-            rc.save_text(title_to_print)
+            print(f"{col} text preprocessing")
             text_reprocess.generate_report()
             self.data_info.data = pp.preprocess_text_df(text_reprocess)
```

### Comparing `madcat-0.84/chester/run/chapter_titles.py` & `madcat-0.9/chester/run/chapter_titles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import random
 
-META_LEARN_EMOJIS = ["🤖", "📊", "🔬", "🚀", "🔍", "📉", "📈"]
-FEATURE_STATS_EMOJIS = ["📈", "📉", "📊", "🔍", "💡", "📚", "🔧"]
-FEATURE_ENGINEERING_EMOJIS = ["🔧", "🔬", "🔍", "🧰", "💡", "📚", "📊"]
-MODEL_PRE_ANALYSIS_EMOJIS = ["📊", "📈", "🔬", "🧰", "💡", "📚", "🔧"]
-MODEL_RUN_EMOJIS = ["🤖", "🔥", "🧠", "🚀", "💻", "💡", "🔬"]
-POST_MODEL_ANALYSIS_EMOJIS = ["📊", "📉", "🔬", "📚", "💡", "📈", "📉"]
-MODEL_WEAKNESSES_EMOJIS = ["🔬", "📉", "💥", "❌", "🔍", "📈", "💡"]
-CLEAN_TEXT_EMOJIS = ["🧼", "🧹", "💧", "🧹", "📚", "💡", "🔍"]
+META_LEARN_EMOJIS = ["🤖", "📊", "🔬", "🚀"]
+FEATURE_STATS_EMOJIS = ["📈", "📉", "📊", "🔍"]
+FEATURE_ENGINEERING_EMOJIS = ["🔧", "🔬", "🔍", "🧰"]
+MODEL_PRE_ANALYSIS_EMOJIS = ["📊", "📈", "🔬", "🧰"]
+MODEL_RUN_EMOJIS = ["🤖", "🔥", "🧠", "🚀"]
+POST_MODEL_ANALYSIS_EMOJIS = ["📊", "📉", "🔬", "📚"]
+MODEL_WEAKNESSES_EMOJIS = ["🔬", "📉", "💥", "❌"]
 
 
 def chapter_title(chapter_name: str, prefix=" Chapter: "):
     stars = '*' * (len(chapter_name + prefix) + 12)
     if chapter_name == 'meta learn':
         emoji = random.choice(META_LEARN_EMOJIS)
     elif chapter_name == 'feature statistics':
@@ -24,13 +23,11 @@
         emoji = random.choice(MODEL_RUN_EMOJIS)
     elif chapter_name == 'post model analysis':
         emoji = random.choice(POST_MODEL_ANALYSIS_EMOJIS)
     elif chapter_name == 'model weaknesses':
         emoji = random.choice(MODEL_WEAKNESSES_EMOJIS)
     elif chapter_name == 'model weaknesses':
         emoji = random.choice(MODEL_WEAKNESSES_EMOJIS)
-    elif chapter_name == 'text cleaning':
-        emoji = random.choice(CLEAN_TEXT_EMOJIS)
     else:
         emoji = '🍵'
     message = f'{stars}\n***{prefix} {chapter_name} {emoji} ***\n{stars}'
     return message
```

### Comparing `madcat-0.84/chester/run/feature_attention_utils.py` & `madcat-0.9/chester/run/feature_attention_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-0.84/chester/run/full_run.py` & `madcat-0.9/chester/run/full_run.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,44 @@
-from itertools import chain
-
-from chester.feature_stats.numeric_stats import NumericStats
-from matplotlib import pyplot as plt
+import warnings
 
 from chester.cleaning.cleaner_handler import CleanerHandler
 from chester.feature_stats.categorical_stats import CategoricalStats
+from chester.feature_stats.numeric_stats import NumericStats
 from chester.feature_stats.text_stats import TextStats
-from chester.feature_stats.time_series_stats import TimeSeriesFeatureStatistics
 from chester.features_engineering.features_handler import FeaturesHandler
-from chester.features_engineering.time_series.ts_features_extraction import TimeSeriesFeaturesExtraction
 from chester.model_monitor.error_prediction import ModelWeaknesses
 from chester.model_monitor.model_boostrap import ModelBootstrap
 from chester.model_training.models.chester_models.best_model import BestModel
 from chester.post_model_analysis.post_model_analysis_class import PostModelAnalysis
 from chester.pre_model_analysis.categorical import CategoricalPreModelAnalysis
 from chester.pre_model_analysis.numerics import NumericPreModelAnalysis
 from chester.pre_model_analysis.target import TargetPreModelAnalysis
-from chester.pre_model_analysis.time_series import TimeSeriesPreModelAnalysis
 from chester.preprocessing.preprocessor_handler import PreprocessHandler
 from chester.run.chapter_titles import chapter_title
-from chester.run.user_classes import Data, TextHandler, FeatureStats, ModelRun, TextFeatureExtraction, FeatureTypes, \
-    TimeSeriesHandler, TextSummary, break_text_into_rows
-from chester.text_stats_analysis.text_summary import get_summary
-from chester.util import REPORT_PATH, ReportCollector
+from chester.run.user_classes import Data, TextHandler, FeatureStats, ModelRun, TextFeatureSpec, FeatureTypes
 from chester.zero_break.problem_specification import DataInfo
 
+warnings.filterwarnings("ignore", category=UserWarning, module="lightgbm")
 import logging
 
 logging.basicConfig(level=logging.WARNING)
 
 from chester.model_training.data_preparation import CVData
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder
 
 
-def run(
+def run_madcat(
         data_spec: Data,
         feature_types: dict = None,
         text_handler: TextHandler = None, is_text_handler=True,
-        text_summary: TextSummary = None,
-        time_series_handler: TimeSeriesHandler = None, is_time_series_handler=True,
         feature_stats: FeatureStats = None, is_feature_stats=True,
-        text_feature_extraction: TextFeatureExtraction = None, is_feature_extract=True,
+        text_feature_extraction: TextFeatureSpec = None,
         is_pre_model=True,
-        is_model_training=True, model_run: ModelRun = None,
+        model_run: ModelRun = None,
         is_post_model=True,
         is_model_weaknesses=True,
         plot=True,
         max_stats_col_width=30,
 ):
     """
         Perform end-to-end machine learning modeling on the provided data.
@@ -80,47 +71,31 @@
     if is_model_weaknesses:
         story += "The weaknesses of the model will be analyzed to understand how to improve it.\n"
     if plot:
         story += "The results will be plotted for visualization.\n"
     story += "The maximum column width for stats display is set to {}.\n".format(max_stats_col_width)
     print(story)
 
-    # reset the file
-    rc = ReportCollector(REPORT_PATH)
-    with open(REPORT_PATH, 'w') as f:
-        pass
-    chester_collector = {}
+    run_metadata_collector = {}
 
     # meta learn
     df = data_spec.df.sample(frac=1).reset_index(drop=True)
-    data_info = DataInfo(data=df.sample(min(10000, len(df))), target=data_spec.target_column)
+    data_info = DataInfo(data=df, target='target')
     data_info.calculate()
-    data_info.data = df
 
     if feature_types is not None:
         data_info = FeatureTypes(feature_types).update_data_info(data_info=data_info)
     target_column = data_info.target
 
     print(chapter_title("meta learn"))
     print(data_info)
-    chester_collector["data info"] = data_info
-
-    rc.save_text(text="Full report to analyze my data:\n")
-    rc.save_object(obj=data_info, text="Data information:")
+    run_metadata_collector["data info"] = data_info
     ####################################################
     # Text handling
-    # Summary, if asked
-    text_cols = data_info.feature_types_val["text"]
-    if text_summary is None:
-        text_summary = TextSummary(is_summary=True)
-    if len(text_cols) > 0 and text_summary is not None:
-        if text_summary.is_summary:
-            chester_collector["raw text summary"] = get_summary(df=df, text_columns=text_cols,
-                                                                text_summary=text_summary)
-
+    # TODO: print message
     # cleaning
     if is_text_handler:
         text_cleaner = None
         text_pre_process = None
         if text_handler is not None:
             text_cleaner = text_handler.text_cleaner
             text_pre_process = text_handler.text_pre_process
@@ -142,64 +117,34 @@
         pp.transform()
         data_info_original = data_info  # in case you need it
         data_info = pp.data_info
 
         # data_info_text_cleaning for later text analysis
         if len(text_cols) > 0:
             clean_text_df = pd.concat([df, clean_text_df], axis=1)
-        chester_collector["data info"] = data_info
+        run_metadata_collector["data info"] = data_info
     ####################################################
 
-    ####################################################
-    # Time series handling
-    # is_time_series_handler
-    ####################################################
     # Feat extract
-    if is_feature_extract:
-        print(chapter_title('feature engineering'))
-        rc.save_text(text="features engineering process for the data:")
-        # Handle TS
-        orig_di = data_info
-        if is_time_series_handler:
-            if time_series_handler is None:
-                time_series_handler = TimeSeriesHandler()
-            time_cols = data_info.feature_types_val["time"]
-            if len(time_cols) > 0:
-                ts_fe = TimeSeriesFeaturesExtraction(data_info=data_info, time_series_handler=time_series_handler)
-                ts_fe.run()
-                ts_fe.data_info.data = ts_fe.data_info.data. \
-                                           loc[:, ~ts_fe.data_info.data.columns.duplicated()]  # drop col dups
-                data_info = ts_fe.data_info
-                time_series_handler = ts_fe.time_series_handler
-                # orig_di = data_info
-
-        # Continue the rest
+    print(chapter_title('feature engineering'))
+    if text_feature_extraction is not None:
+        feat_hand = FeaturesHandler(data_info=data_info, text_feature_extraction=text_feature_extraction)
+    else:
         feat_hand = FeaturesHandler(data_info=data_info)
-        if text_feature_extraction is not None:
-            feat_hand.text_feature_extraction = text_feature_extraction
-        feature_types, final_df = feat_hand.transform()
-        if target_column is not None:
-            final_df[target_column] = data_info.data[data_info.target]
-        final_df = final_df.loc[:, ~final_df.columns.duplicated()]
-        data_info.data = data_info.data.loc[:, ~data_info.data.columns.duplicated()]
+    feature_types, final_df = feat_hand.transform()
+    final_df[target_column] = data_info.data[data_info.target]
 
-        chester_collector["data info"] = data_info
-        chester_collector["features data"] = final_df
+    run_metadata_collector["data info"] = data_info
+    run_metadata_collector["features data"] = final_df
     ####################################################
+
     # Feat Stats
     data_info_num_stats = None
     if is_feature_stats:
-        rc.save_text(
-            text="features statistics for the data. Analyzed by groups (text, numeric, categorical) if exists:")
         print(chapter_title('feature statistics'))
-        if feature_stats is None:
-            feature_stats = FeatureStats()
-        sample_obs = feature_stats.sample_obs
-        # sample data for stats
-        final_df = final_df.loc[:, ~final_df.columns.duplicated()].sample(min(sample_obs, len(final_df)))
         data_info_num_stats = DataInfo(data=final_df, target=target_column)
         data_info_num_stats.calculate()
 
         num_cols = data_info_num_stats.feature_types_val["numeric"]
         cat_cols = data_info.feature_types_val["categorical"]
         text_cols = data_info.feature_types_val["text"]
 
@@ -212,133 +157,88 @@
                 if feature_stats.plot is not None:
                     plot_stats = feature_stats.plot
             else:
                 plot_stats = True
 
         max_stats_col_width = max_stats_col_width or 30
         if len(num_cols) > 0:
-            title = "\nNumerical Feature statistics:"
-            print(title)
-            rc.save_text(title)
+            print("Numerical Feature statistics")
             NumericStats(data_info_num_stats, max_print=max_stats_col_width).run(plot=plot_stats)
-        title = "\nCategorical Feature statistics:"
-        print(title)
-        rc.save_text(title)
-
+        print("Categorical Feature statistics")
         CategoricalStats(data_info, max_print=max_stats_col_width).run(plot=plot_stats)
         if len(text_cols) > 0:
-            print("Text Feature Statistics")
-            orig_df = data_info.data
+            print("Text Feature statistics")
             data_info.data = clean_text_df
-            if text_feature_extraction is None:
-                text_feature_extraction = TextFeatureExtraction()
-            TextStats(data_info, text_spec=text_feature_extraction, chester_collector=chester_collector).run()
-            data_info.data = orig_df
-            if "raw text summary" in chester_collector is not None:
-                print(f"Text Columns Summary:")
-                try:
-                    for col in text_cols:
-                        print("\t", chester_collector["raw text summary"][col])
-                except:
-                    print("\t", chester_collector["raw text summary"])
-
-        all_features = list(set(chain.from_iterable(list(data_info.feature_types_val.values()))))
-        ts_cols = [feat for feat in all_features if feat.startswith("ts_")]
-        if len(ts_cols) > 0:
-            print("Time Series Feature Statistics")
-            TimeSeriesFeatureStatistics(data_info=data_info, ts_cols=ts_cols,
-                                        time_series_handler=time_series_handler).run(plot=True)
+            TextStats(data_info).run()
     ####################################################
-    # No target => no model! The story ends here
+
+    # No target => no model!
     if data_info.problem_type_val == "No target variable":
-        return chester_collector
+        return run_metadata_collector
 
     # Pre model
     if is_pre_model:
-        final_df = final_df.loc[:, ~final_df.columns.duplicated()]
-        rc.save_text("** model pre analysis report:")
         print(chapter_title('model pre analysis'))
         # label stats
-        print("Label pre model analysis:")
-        TargetPreModelAnalysis(data_info=data_info, time_series_handler=time_series_handler).run(plot)
-        TimeSeriesPreModelAnalysis(data_info=data_info, time_series_handler=time_series_handler).run()
+        TargetPreModelAnalysis(data_info).run(plot)
         # num, cat pre model
         if data_info_num_stats is None:
             data_info_num_stats = DataInfo(data=final_df, target=target_column)
             data_info_num_stats.calculate()
         NumericPreModelAnalysis(data_info_num_stats).run(plot)
-        plt.close()
-        # cat if found any
-        cat_not_ts = data_info.feature_types_val["categorical"]
-        if len(cat_not_ts) > 0:
-            print("Categorical pre model analysis:")
-            CategoricalPreModelAnalysis(data_info).run(plot)
+        data_info.data = df
+        CategoricalPreModelAnalysis(data_info).run(plot)
     ####################################################
     # model
-    if not is_model_training:
-        return chester_collector
-    if is_model_training:
-        print(chapter_title("model training"))
-        rc.save_text("Training models and choosing the best one")
-        # drop col dups
-        data_info.feature_types_val["numeric"] = list(set(data_info.feature_types_val["numeric"]))
-        data_info.feature_types_val["categorical"] = list(set(data_info.feature_types_val["categorical"]))
-        # encode if needed
-        if data_info.problem_type_val in ["Binary classification", "Multiclass classification"]:
-            label_encoder = LabelEncoder()
-            final_df[target_column] = label_encoder.fit_transform(final_df[target_column])
-
-        # cv data
-        cv_data = CVData(train_data=final_df, test_data=None, target_column='target', split_data=True)
-        data_info.feature_types_val = feature_types
-        # run the model
-        if model_run is not None:
-            model = BestModel(data_info=data_info,
-                              cv_data=cv_data,
-                              num_models_to_compare=model_run.n_models,
-                              best_practice_prob=model_run.best_practice_prob)
-        else:
-            model = BestModel(data_info=data_info, cv_data=cv_data)
-        model_results = model.get_best_model()  # returns result of the best baseline model
-        # print model metadata
-        params = model_results[1].get_params()
-        try:
-            print(f"Best model: {type(model_results[1].model)}, with parameters:")
-            for p in params:
-                print(p.name, ":", p.value)
-        except:
-            pass
-
-        chester_collector["data info"] = data_info
-        chester_collector["features data"] = final_df
-        chester_collector["model"] = model_results[1]
-        chester_collector["parameters"] = params
-        chester_collector["model_results"] = model_results[0]
+    print(chapter_title("model training"))
+    # encode if needed
+    if data_info.problem_type_val in ["Binary classification", "Multiclass classification"]:
+        # print("Encoding target")
+        label_encoder = LabelEncoder()
+        final_df[target_column] = label_encoder.fit_transform(final_df[target_column])
+
+    # cv data
+    cv_data = CVData(train_data=final_df, test_data=None, target_column='target', split_data=True)
+    data_info.feature_types_val = feature_types
+    # run the model
+    if model_run is not None:
+        model = BestModel(data_info=data_info,
+                          cv_data=cv_data,
+                          num_models_to_compare=model_run.n_models,
+                          best_practice_prob=model_run.best_practice_prob)
+    else:
+        model = BestModel(data_info=data_info, cv_data=cv_data)
+    model_results = model.get_best_model()  # returns result of the best baseline model
+    # print model metadata
+    params = model_results[1].get_params()
+    print(f"Best model: {type(model_results[1].model)}, with parameters:")
+    for p in params:
+        print(p.name, ":", p.value)
+
+    run_metadata_collector["data info"] = data_info
+    run_metadata_collector["features data"] = final_df
+    run_metadata_collector["model"] = model
+    run_metadata_collector["parameters"] = model_results[1]
+    run_metadata_collector["model_results"] = model_results[0]
     ####################################################
 
     # post model
-    is_baseline = type(model_results[1]).__name__ == "BaselineModel"
-    if is_baseline:
-        print("Best model is a simple baseline")
-        return chester_collector
-    if is_post_model and is_model_training:
-        rc.save_text("\nPost model analysis - analyzing results of the chosen model: ")
+    if is_post_model:
         print(chapter_title('post model analysis'))
         post_model_analysis = PostModelAnalysis(cv_data, data_info, model=model_results[1])
-        chester_collector["post_model_analysis"] = post_model_analysis
+        run_metadata_collector["post_model_analysis"] = post_model_analysis
         post_model_analysis.analyze()
 
         model_bootstrap = ModelBootstrap(cv_data, data_info, model=model_results[1])
-        chester_collector["model_bootstrap"] = model_bootstrap
+        run_metadata_collector["model_bootstrap"] = model_bootstrap
         model_bootstrap.plot()
     ####################################################
 
     #  model weaknesses
-    if is_model_weaknesses and is_model_training:
-        rc.save_text("Trying to find weaknesses in the model by training models on the error:")
+    if is_model_weaknesses:
         print(chapter_title('model weaknesses'))
         model_weaknesses = ModelWeaknesses(cv_data, data_info, model=model_results[1])
-        chester_collector["model_weaknesses"] = model_weaknesses
+        run_metadata_collector["model_weaknesses"] = model_weaknesses
         model_weaknesses.run()
     ####################################################
 
-    return chester_collector
+    return run_metadata_collector
```

### Comparing `madcat-0.84/chester/text_stats_analysis/common_words.py` & `madcat-0.9/chester/text_stats_analysis/common_words.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from collections import Counter
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 
-from chester.util import ReportCollector, REPORT_PATH
-
 
 def most_common_words(data, common_words=10, text_column='text'):
-    rc = ReportCollector(REPORT_PATH)
     # create a Counter object to store the word counts
     word_counts = Counter()
 
     # iterate over each row in the data
     for index, row in data.iterrows():
         # split the text into a list of words
         words = row[text_column].split()
@@ -21,18 +18,16 @@
 
     # sort the Counter by value (count) in descending order
     sorted_word_counts = sorted(word_counts.items(), key=lambda x: x[1], reverse=True)
 
     # create a barplot using seaborn
     plt.figure(figsize=(11, 11))
     plt.rcParams.update({'font.size': 25})
-    rc.save_text(str(sorted_word_counts[:100]))  # save top 100 common words
     sns.barplot(x=[t[0] for t in sorted_word_counts[:common_words]],
                 y=[t[1] for t in sorted_word_counts[:common_words]])
     plt.xlabel('Word')
     plt.ylabel('Count')
     plt.title('Most Common Words')
     plt.show()
-    plt.close()
 
     # return the sorted list of tuples (word, count)
     return sorted_word_counts[:common_words]
```

### Comparing `madcat-0.84/chester/text_stats_analysis/corex_topics.py` & `madcat-0.9/chester/text_stats_analysis/corex_topics.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,92 +4,69 @@
 import numpy as np
 import pandas as pd
 import scipy.sparse as ss
 from corextopic import corextopic as ct
 from sklearn.feature_extraction.text import CountVectorizer
 from wordcloud import WordCloud
 
-from chester.util import ReportCollector, REPORT_PATH
 
-
-def plot_corex_wordcloud(df, top_words=20, n_topics=10, plot=True, text_column='text',
-                         corex_anchor_strength=1.6,
-                         corex_anchor_words=None):
-    top_words_list = get_top_words(df, top_words, n_topics, text_column=text_column,
-                                   corex_anchor_strength=corex_anchor_strength,
-                                   corex_anchor_words=corex_anchor_words)
+def plot_corex_wordcloud(df, top_words=20, n_topics=10, plot=True, text_column='text'):
+    top_words_list = get_top_words(df, top_words, n_topics, text_column=text_column)
     top_words_list = pd.DataFrame(top_words_list, columns=["topic_index", "term", "weight"])
     if plot:
         # Plot the word clouds
         N = math.floor(math.sqrt(n_topics))
         fig, axs = plt.subplots(N, N, figsize=(N * 4, N * 4), dpi=100)
         fig.suptitle("Word Clouds for Top Word for Corex Topics", fontsize=16)
 
         for i in range(n_topics - 1):
             topic_words = top_words_list[top_words_list["topic_index"] == i]
             topic_words = dict(zip(topic_words["term"], topic_words["weight"]))
-            if len(topic_words) == 0:
-                break
             wordcloud = WordCloud(width=800, height=800, background_color='black',
                                   stopwords=None, min_font_size=10).generate_from_frequencies(topic_words)
 
             subplot_index = i + 1
             try:
                 ax = plt.subplot(N, N, subplot_index)
                 plt.imshow(wordcloud)
                 plt.axis("off")
                 plt.title("Topic {}".format(i), fontsize=14)
             except:
-                plt.close()
                 pass
         plt.tight_layout()
         plt.show()
-        plt.close()
 
 
 def get_top_words(df: pd.DataFrame,
                   top_words,
                   n_topics,
                   max_features=1000,
                   text_column: str = 'text',
-                  ngram_range=(1, 3),
-                  corex_anchor_strength=1.6,
-                  corex_anchor_words=None
-                  ):
-    rc = ReportCollector(REPORT_PATH)
+                  ngram_range=(1, 3)):
     # Preprocess data
     vectorizer = CountVectorizer(stop_words='english',
                                  max_features=max_features,
                                  binary=True,
                                  ngram_range=ngram_range)
     doc_word = vectorizer.fit_transform(df[text_column])
     doc_word = ss.csr_matrix(doc_word)
     feature_names = list(vectorizer.vocabulary_.keys())
     words = list(np.asarray(feature_names))
 
     # Train model
-    topic_model = ct.Corex(n_hidden=n_topics, words=words, max_iter=200, verbose=False, seed=12345)
-    if corex_anchor_words is None:
-        topic_model.fit(doc_word, words=words)
-    else:
-        print("Anchored Corex")
-        topic_model.fit(doc_word, words=words, anchor_strength=corex_anchor_strength, anchors=corex_anchor_words)
+    topic_model = ct.Corex(n_hidden=n_topics, words=words, max_iter=200, verbose=False, seed=1)
+    topic_model.fit(doc_word, words=words)
 
     # Get top words and weights for each topic
     topics = topic_model.get_topics()
     if topics is None:
         return []
 
     top_words_list = []
-    rc.save_text("\nCorex topic analysis:")
     for i, topic in enumerate(topics):
-        if len(topic) == 0:
-            break
         topic_words, weights, _ = zip(*topic)
         num_words = min(top_words, len(topic_words))  # Use smaller of n and num words in topic
         top_words_list += [(i, topic_words[j], weights[j]) for j in range(num_words)]
-        title = '\tTopic {}: '.format(i + 1) + ', '.join(topic_words)
-        print(title)
-        rc.save_text(text=title)
+        print('\tTopic {}: '.format(i + 1) + ', '.join(topic_words))
     print("\n")
 
     return top_words_list
```

### Comparing `madcat-0.84/chester/text_stats_analysis/data_quality.py` & `madcat-0.9/chester/text_stats_analysis/data_quality.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import matplotlib.pyplot as plt
 import nltk
 import pandas as pd
 import seaborn as sns
 
-from chester.run.user_classes import TextSummary
-from chester.util import ReportCollector, REPORT_PATH
-
 
 def calculate_text_metrics(text):
     metrics = {'text_length': len(text), 'num_sentences': len(nltk.sent_tokenize(text))}
     if not text:
         return metrics
     if any(c.isalpha() for c in text):
         metrics['num_characters'] = len([c for c in text if c.isalpha()])
@@ -34,39 +31,36 @@
     words = df[text_column].str.split(expand=True).stack().unique()
     num_unique_words = len(words)
     df = pd.json_normalize(df[f'{text_column}_metrics'])
     return df, num_unique_words
 
 
 def create_report(df, num_unique_words):
-    rc = ReportCollector(REPORT_PATH)
     report = ""
     report += f"Number of rows with missing data: {df['num_missing'].sum()}\n"
     report += f"Number of unique words: {num_unique_words}\n"
     report += f"Average type-token ratio: {df['ttr'].mean():.2f}\n"
     report += f"Median type-token ratio: {df['ttr'].median():.2f}\n"
     report += f"Average number of words per text: {df['num_words'].mean():.2f}\n"
     report += f"Median number of words per text: {df['num_words'].median():.2f}\n"
     report += f"Average number of sentences per text: {df['num_sentences'].mean():.2f}\n"
     report += f"Median number of sentences per text: {df['num_sentences'].median():.2f}\n"
     report += f"Average length of text: {df['text_length'].mean():.2f}\n"
     report += f"Median length of text: {df['text_length'].median():.2f}\n"
-    rc.save_text(text=report)
     return report
 
 
 def plot_text_length_and_num_words(df):
     sns.set(style="darkgrid")
-    fig, ax = plt.subplots(2, 1, figsize=(14, 14))
+    fig, ax = plt.subplots(1, 2, figsize=(15, 15))
     plt.rcParams.update({'font.size': 20})
     sns.histplot(data=df, x='text_length', ax=ax[0])
     sns.histplot(data=df, x='num_words', ax=ax[1])
     fig.suptitle('Text Statistics')
     plt.show()
-    plt.close()
 
 
 def analyze_text_stats(df, text_column='text'):
     df, num_unique_words = calculate_text_column_metrics(df, text_column)
     plot_text_length_and_num_words(df)
     report = create_report(df, num_unique_words)
     df_report = pd.DataFrame(
@@ -74,33 +68,25 @@
         columns=["Metric", "Value"])
     df_report["Value"] = df_report["Value"].apply(lambda x: f"{int(x)}" if x.is_integer() else f"{x:.2f}")
     return df_report
 
 
 class TextAnalyzer:
     def __init__(self, df: pd.DataFrame = None, text_column: str = 'text', create_wordcloud: bool = True,
-                 corex_topics: bool = True,
-                 key_sentences: bool = True,
+                 corex_topics: bool = True, key_sentences: bool = True,
                  common_words: bool = True, sentiment: bool = True,
                  ner_extraction: bool = True, kewords_extraction: bool = True,
-                 data_quality: bool = True, corex_topics_num: int = 10, corex_anchor_words=None,
-                 corex_anchor_strength=1.6,
-                 top_words: int = 10, n_sentences: int = 5,
-                 text_summary: TextSummary = None,
-                 chester_collector=None):
+                 data_quality: bool = True, corex_topics_num: int = 10,
+                 top_words: int = 10, n_sentences: int = 5):
         self.df = df
         self.create_wordcloud = create_wordcloud
         self.corex_topics = corex_topics
         self.key_sentences = key_sentences
         self.common_words = common_words
         self.sentiment = sentiment
         self.data_quality = data_quality
         self.ner_extraction = ner_extraction
         self.kewords_extraction = kewords_extraction
         self.corex_topics_num = corex_topics_num
-        self.corex_anchor_words = corex_anchor_words
-        self.corex_anchor_strength = corex_anchor_strength
         self.top_words = top_words
         self.n_sentences = n_sentences
         self.text_column = text_column
-        self.text_summary = text_summary
-        self.chester_collector = chester_collector or {}
```

### Comparing `madcat-0.84/chester/text_stats_analysis/key_sentences.py` & `madcat-0.9/chester/text_stats_analysis/key_sentences.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 import numpy as np
 import pandas as pd
 from nltk.tokenize import sent_tokenize
 from sklearn.decomposition import TruncatedSVD
 from sklearn.feature_extraction.text import TfidfVectorizer
 
-from chester.util import ReportCollector, REPORT_PATH
-
 
 def extract_key_sentences_lsa(text, k=10):
     """
     Extract k most important sentences from text using LSA algorithm.
     :param text: the text to extract key sentences from
     :param k: the number of sentences to extract (default: 10)
     :return: list of k most important sentences
@@ -29,16 +27,15 @@
 
     # use cosine similarity to identify the most important sentences
     similarity = np.asarray(np.asmatrix(X) * np.asmatrix(X).T)
     sentence_scores = similarity.diagonal()
 
     # sort the sentences by importance
     sentence_scores_sorted = sentence_scores.argsort()[::-1]
-    return_list = [sentences[i] for i in sentence_scores_sorted]
-    return return_list
+    return [sentences[i] for i in sentence_scores_sorted]
 
 
 def key_sentences(df, text_column='text', common_sentences=10):
     # Concatenate all text in the specified column into one string
     all_text = ". ".join(df[text_column])
 
     # Tokenize the string into sentences
@@ -58,30 +55,27 @@
     Extract k most important sentences from a pandas dataframe containing text data.
     :param df: the dataframe to extract key sentences from
     :param text_column: the name of the column containing the text data (default: 'clean_text')
     :param algorithm: the algorithm to use for sentence extraction (default: 'summarization')
     :param n_sentences: the number of sentences to extract (default: 10)
     :return: list of k most important sentences
     """
-    rc = ReportCollector(REPORT_PATH)
-
     full_text = '. '.join(df[text_column])
+
     if algorithm == 'LSA':
         sentences = list(set(extract_key_sentences_lsa(full_text, n_sentences)))[0:n_sentences]
     elif algorithm == 'common_sentences':
         tokenized_sentences = [sentence.split() for sentence in sent_tokenize(full_text)]
         sentence_counter = Counter([tuple(sentence) for sentence in tokenized_sentences])
         common_sentences = [" ".join(sentence) for sentence, count in sentence_counter.most_common(n_sentences)]
         sentences = common_sentences
     else:
         raise ValueError(f'Invalid algorithm: {algorithm}')
 
-    title = f'\tKey sentences out of based on {algorithm} algorithm: {sentences} \n'
-    rc.save_text(title)
-    return title
+    return f'\tKey sentences out of based on {algorithm} algorithm: {sentences} \n'
 
 
 def extract_first_k_words(text, k):
     """
     Extract the first k words from text.
     :param text: the text to extract words from
     :param k: the number of words to extract
```

### Comparing `madcat-0.84/chester/text_stats_analysis/keywords_extraction.py` & `madcat-0.9/chester/text_stats_analysis/keywords_extraction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from __future__ import division
 
 import operator
 import string
 
 import nltk
 
-from chester.util import ReportCollector, REPORT_PATH
-
 
 def isPunct(word):
     return len(word) == 1 and word in string.punctuation
 
 
 def isNumeric(word):
     try:
         float(word) if '.' in word else int(word)
         return True
-    except:
+    except ValueError:
         return False
 
 
 class RakeKeywordExtractor:
 
     def __init__(self):
         self.stopwords = set(nltk.corpus.stopwords.words())
@@ -64,26 +62,22 @@
             phrase_score = 0
             for word in phrase:
                 phrase_score += word_scores[word]
             phrase_scores[" ".join(phrase)] = phrase_score
         return phrase_scores
 
     def extract(self, text, max_words=7, top_words=10):
-        rc = ReportCollector(REPORT_PATH)
-
         sentences = nltk.sent_tokenize(text)
         phrase_list = self._generate_candidate_keywords(sentences)
         word_scores = self._calculate_word_scores(phrase_list)
         phrase_scores = self._calculate_phrase_scores(
             phrase_list, word_scores)
         sorted_phrase_scores = sorted(phrase_scores.items(), key=operator.itemgetter(1), reverse=True)
         n_phrases = len(sorted_phrase_scores)
-        return_list = truncate_and_limit_keywords(sorted_phrase_scores, max_words, top_words)
-        rc.save_object(obj=return_list, text="popular terms extraction:")
-        return return_list
+        return truncate_and_limit_keywords(sorted_phrase_scores, max_words, top_words)
 
 
 def truncate_and_limit_keywords(keywords_list, max_words, top_words):
     truncated_keywords = []
     for keyword in keywords_list[:top_words]:
         text = trim_repeated_words(keyword[0], 1)
         score = keyword[1]
```

### Comparing `madcat-0.84/chester/text_stats_analysis/sentiment.py` & `madcat-0.9/chester/text_stats_analysis/sentiment.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 
 import matplotlib.pyplot as plt
 import pandas as pd
 import seaborn as sns
 from prettytable import PrettyTable
 from textblob import TextBlob
 
-from chester.util import ReportCollector, REPORT_PATH
-
 
 def report_sentiment_stats(sentiment_df: pd.DataFrame) -> Dict[str, Union[int, float]]:
-    rc = ReportCollector(REPORT_PATH)
     # count number of positive, negative and neutral sentiments
     pos_count = len(sentiment_df[sentiment_df['sentiment'] > 0])
     neg_count = len(sentiment_df[sentiment_df['sentiment'] < 0])
     neutral_count = len(sentiment_df[sentiment_df['sentiment'] == 0])
     # calculate percentage of positive, negative and neutral sentiments
     total_count = pos_count + neg_count + neutral_count
     pos_percent = pos_count / total_count * 100
@@ -24,26 +21,24 @@
     # create a table
     table = PrettyTable()
     table.field_names = ["Sentiment", "Count", "Percentage"]
     table.add_row(["Positive", pos_count, f"{pos_percent:.1f}%"])
     table.add_row(["Negative", neg_count, f"{neg_percent:.1f}%"])
     table.add_row(["Neutral", neutral_count, f"{neutral_percent:.1f}%"])
 
-    rc.save_object(obj=table.get_string(title="Sentiment Statistics"), text="Sentiment Statistics")
     return table.get_string(title="Sentiment Statistics")
 
 
 def analyze_sentiment(df, text_column='text'):
     # Add a new column to the DataFrame with the sentiment of each text
     df['sentiment'] = df[text_column].apply(lambda x: TextBlob(x).sentiment.polarity)
 
     return df
 
 
 def plot_sentiment_scores(sentiment_df):
-    # Create a histogram of the sentiment scores
+    # Create a histogram of the sentiment scores using Seaborn
     ax = sns.histplot(data=sentiment_df, x='sentiment', kde=False)
-    sns.set(rc={'figure.figsize': (12, 12)})
-    plt.rcParams.update({'font.size': 14})
     ax.set(xlabel='Sentiment Score', ylabel='Count', title='Sentiment Scores')
+    plt.figure(figsize=(12, 12))
+    plt.rcParams.update({'font.size': 14})
     plt.show()
-    plt.close()
```

### Comparing `madcat-0.84/chester/text_stats_analysis/smart_text_analyzer.py` & `madcat-0.9/chester/text_stats_analysis/smart_text_analyzer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import pandas as pd
 
-from chester.run.user_classes import TextSummary
 from chester.text_stats_analysis import common_words as cw, corex_topics as corex, keywords_extraction as kw_extract
 from chester.text_stats_analysis.data_quality import analyze_text_stats, TextAnalyzer
 from chester.text_stats_analysis.key_sentences import extract_key_sentences
 from chester.text_stats_analysis.sentiment import analyze_sentiment, report_sentiment_stats, plot_sentiment_scores
 from chester.text_stats_analysis.word_cloud import create_word_cloud
-from chester.util import ReportCollector, REPORT_PATH
 
 data_quality_message = "Before analyzing text, ensure data is clean and of good quality.\n" \
                        "Report provides key stats on data quality, incl. missing data,\n" \
                        "unique words, type-token ratio, words/sentences per text, and text length:"
 
 common_words_message = "Count word frequency for basic text analysis.\n" \
                        "Report shows most common words, giving insight into text topic and content:"
@@ -76,60 +74,49 @@
 
 
 def analyze_text(df: pd.DataFrame,
                  create_wordcloud: bool = True,
                  corex_topics: bool = True,
                  key_sentences: bool = True,
                  common_words: bool = True,
+                 sentiment: bool = True,
                  data_quality: bool = True,
                  kewords_extraction: bool = True,
                  corex_topics_num: int = 10,
-                 corex_anchor_strength=1.6,
-                 corex_anchor_words=None,
                  top_words: int = 10,
                  n_sentences: int = 10,
-                 text_column: str = 'text',
-                 text_summary: TextSummary = None,
-                 chester_collector=None):
+                 text_column: str = 'text'):
     """
     Analyze text using various text analysis techniques.
     :param df: pandas data with clean text column
     :param create_wordcloud: flag indicating whether to create a word cloud (default: True)
     :param corex_topics: flag indicating whether to extract corex topics (default: True)
     :param key_sentences: flag indicating whether to extract key sentences (default: True)
     :param common_words: flag indicating whether to extract common words (default: True)
     :param sentiment: flag indicating whether to perform sentiment analysis (default: True)
     :param data_quality: flag indicating whether to check data quality (default: True)
     :param kewords_extraction: flag indicating whether to create potential keywords
     :param corex_topics_num: number of corex topics to extract (default: 10)
     :param top_words: top words
     :param n_sentences: number of sentences to return
-    :param text_column: the text column
-    :param corex_anchor_words: corex anchore words (for semi supervised version)
-    :param corex_anchor_strength: anchore strength
-    :param text_summary: text sentiment, summary and other requirements
-    :param chester_collector: collector to track stats
     """
 
-    rc = ReportCollector(REPORT_PATH)
     is_clean_col_exists = True if f"clean_{text_column}" in df.columns else False
     if is_clean_col_exists:
         modified_df = df.drop(columns=[text_column], axis=1). \
             rename(columns={f'clean_{text_column}': text_column})
 
     print_analyze_message()
     if data_quality:
         print(data_quality_message)
-        rc.save_text("Data quality stats:")
         if is_clean_col_exists:
             print(analyze_text_stats(modified_df, text_column), "\n")
         else:
             print(analyze_text_stats(df, text_column), "\n")
     if common_words:
-        rc.save_text(common_words_message)
         print(common_words_message)
 
         if is_clean_col_exists:
             print("\t", cw.most_common_words(modified_df, common_words=top_words, text_column=text_column))
         else:
             print("\t", cw.most_common_words(df, common_words=top_words, text_column=text_column))
 
@@ -138,39 +125,34 @@
         print(word_cloud_message)
 
         if is_clean_col_exists:
             create_word_cloud(modified_df, text_column=text_column)
         else:
             create_word_cloud(df, text_column=text_column)
 
-    sentiment = text_summary.is_sentiment or True
     if sentiment:
         print(sentiment_analysis_message)
         df = df.copy()
         modified_df = modified_df.copy()
         if is_clean_col_exists:
             df = analyze_sentiment(modified_df, text_column=text_column)
         else:
             df = analyze_sentiment(df, text_column=text_column)
-        chester_collector["sentiment df"] = df
         print(report_sentiment_stats(df), "\n")
         print()
         plot_sentiment_scores(df)
 
     if corex_topics:
         print(corex_topic_message)
+
         if is_clean_col_exists:
             corex.plot_corex_wordcloud(modified_df, n_topics=corex_topics_num, top_words=top_words,
-                                       text_column=text_column, corex_anchor_words=corex_anchor_words,
-                                       corex_anchor_strength=corex_anchor_strength)
+                                       text_column=text_column)
         else:
-            corex.plot_corex_wordcloud(df, n_topics=corex_topics_num, top_words=top_words, text_column=text_column,
-                                       corex_anchor_words=corex_anchor_words,
-                                       corex_anchor_strength=corex_anchor_strength
-                                       )
+            corex.plot_corex_wordcloud(df, n_topics=corex_topics_num, top_words=top_words, text_column=text_column)
 
     if key_sentences:
         print(key_sentences_message)
 
         if is_clean_col_exists:
             print(extract_key_sentences(modified_df, n_sentences=n_sentences, text_column=text_column))
         else:
@@ -183,26 +165,20 @@
             full_text = '. '.join(modified_df[text_column])
         else:
             full_text = '. '.join(df[text_column])
 
         kws_rake = kw_extract.RakeKeywordExtractor()
         print("\t", kws_rake.extract(text=full_text))
 
-    return chester_collector
-
 
 def analyze_text_df(text_analyzer: TextAnalyzer):
     df = text_analyzer.df
-    text_analyzer.chester_collector = analyze_text(df=df, text_column=text_analyzer.text_column,
-                                                   create_wordcloud=text_analyzer.create_wordcloud,
-                                                   corex_topics=text_analyzer.corex_topics,
-                                                   key_sentences=text_analyzer.key_sentences,
-                                                   common_words=text_analyzer.common_words,
-                                                   data_quality=text_analyzer.data_quality,
-                                                   corex_topics_num=text_analyzer.corex_topics_num,
-                                                   top_words=text_analyzer.top_words,
-                                                   n_sentences=text_analyzer.n_sentences,
-                                                   corex_anchor_strength=text_analyzer.corex_anchor_strength,
-                                                   corex_anchor_words=text_analyzer.corex_anchor_words,
-                                                   text_summary=text_analyzer.text_summary,
-                                                   chester_collector=text_analyzer.chester_collector,
-                                                   )
+    analyze_text(df=df, text_column=text_analyzer.text_column,
+                 create_wordcloud=text_analyzer.create_wordcloud,
+                 corex_topics=text_analyzer.corex_topics,
+                 key_sentences=text_analyzer.key_sentences,
+                 common_words=text_analyzer.common_words,
+                 sentiment=text_analyzer.sentiment,
+                 data_quality=text_analyzer.data_quality,
+                 corex_topics_num=text_analyzer.corex_topics_num,
+                 top_words=text_analyzer.top_words,
+                 n_sentences=text_analyzer.n_sentences)
```

### Comparing `madcat-0.84/chester/zero_break/problem_specification.py` & `madcat-0.9/chester/zero_break/problem_specification.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,19 @@
-import itertools
-import re
-from datetime import datetime
-
 import pandas as pd
-# need an extension for ts module
 from dateutil.parser import parse
 
 from chester.zero_break.text_detector import determine_if_text_or_categorical_column
 
 
+# need an extension for ts module
 def is_date(string):
-    if len(string) < 7:
-        return False
-    # Define regular expressions to match various date and datetime formats
-    date_formats = ["%Y-%m-%d", "%m/%d/%Y", "%d/%m/%Y"]
-    datetime_formats = ["%Y-%m-%d %H:%M:%S", "%Y-%m-%d %H:%M", "%m/%d/%Y %H:%M:%S", "%m/%d/%Y %H:%M"]
-    regexes = [
-        re.compile(r'\d{4}-\d{2}-\d{2}'),
-        re.compile(r'\d{2}/\d{2}/\d{4}'),
-        re.compile(r'\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}'),
-        re.compile(r'\d{4}-\d{2}-\d{2} \d{2}:\d{2}'),
-        re.compile(r'\d{2}/\d{2}/\d{4} \d{2}:\d{2}:\d{2}'),
-        re.compile(r'\d{2}/\d{2}/\d{4} \d{2}:\d{2}')
-    ]
-
-    # Check if the string matches any of the known formats or regexes
     try:
-        if string.isdigit() and len(string) >= 9:
-            return False
         parse(string)
         return True
     except ValueError:
-        for fmt in date_formats + datetime_formats:
-            try:
-                datetime.strptime(string, fmt)
-                return True
-            except ValueError:
-                pass
-        for regex in regexes:
-            if regex.match(string):
-                return True
         return False
 
 
 class DataInfo:
     def __init__(self, data: pd.DataFrame, target: str = None):
         self.data = data
         self.target = target
@@ -51,18 +21,14 @@
         self.problem_type_val = None
         self.feature_types_val = None
         self.loss_detector_val = None
         self.metrics_detector_val = None
         self.model_selection_val = None
         self.label_transformation_val = None
         self.rows = self.data.shape[0]
-        self.feature_types_val_flatten = None
-
-    def get_all_features(self):
-        return list(set(itertools.chain(*self.feature_types_val.values())))
 
     def calculate(self):
         self.problem_type_val = self.problem_type()
         self.feature_types_val = self.feature_types()
         self.loss_detector_val = self.loss_detector()
         self.metrics_detector_val = self.metrics_detector()
         self.model_selection_val = self.model_selection()
@@ -91,87 +57,68 @@
                 pass
             elif col == self.target:
                 pass
             elif pd.api.types.is_datetime64_dtype(self.data[col]):
                 time_cols.append(col)
             else:
                 non_missing_values = self.data[col][self.data[col].notna()].astype(str)
-                if non_missing_values.shape[0] == 0:
-                    pass
                 count = 0
                 for value in non_missing_values:
                     if is_date(value):
                         count += 1
-                try:
-                    if count / non_missing_values.shape[0] >= 0.9:
-                        time_cols.append(col)
-                except:
-                    pass
+                if count / non_missing_values.shape[0] >= 0.9:
+                    time_cols.append(col)
         return time_cols
 
     def _determine_numerical_cols(self):
         numerical_cols = []
         for col in self.data.columns:
-            if self.data[col].dtype in ['int64', 'float64', 'int32', 'float32']:
+            if self.data[col].dtype in ['int64', 'float64']:
                 numerical_cols.append(col)
         return numerical_cols
 
     def _determine_boolean_cols(self):
         boolean_cols = []
         for col in self.data.columns:
             if pd.api.types.is_bool_dtype(self.data[col]):
                 boolean_cols.append(col)
         return boolean_cols
 
-    def _determine_id_cols(self):
-        id_cols = []
-        for col in self.data.columns:
-            if col.startswith("ID_") or col.endswith("_id") \
-                    or col.endswith("_ID") or col.lower().endswith(" id") \
-                    or col.lower() == "id":
-                id_cols.append(col)
-        return id_cols
-
-    @staticmethod
-    def remove_common_elements(l1, l2):
-        return [x for x in l1 if x not in l2]
-
     def feature_types(self):
-        # get basic
         numerical_cols = self._determine_numerical_cols()
         boolean_cols = self._determine_boolean_cols()
         time_cols = self._determine_time_cols()
-        id_cols = self._determine_id_cols()
-
         text_cols = []
         categorical_cols = []
         for col in self.data.columns:
             if col not in numerical_cols and col not in boolean_cols:
                 is_text, is_categorical = determine_if_text_or_categorical_column(self.data[col])
                 if is_text:
                     text_cols.append(col)
                 elif is_categorical:
                     categorical_cols.append(col)
-        # remove target
         if self.target in numerical_cols:
             numerical_cols.remove(self.target)
         if self.target in boolean_cols:
             boolean_cols.remove(self.target)
         if self.target in text_cols:
             text_cols.remove(self.target)
         if self.target in categorical_cols:
             categorical_cols.remove(self.target)
 
-        # hirerchy
-        numerical_cols = list(self.remove_common_elements(numerical_cols, time_cols + id_cols))
-        time_cols = list(self.remove_common_elements(time_cols, id_cols))
-        text_cols = list(self.remove_common_elements(text_cols, time_cols + id_cols))
-        categorical_cols = list(self.remove_common_elements(categorical_cols, time_cols + id_cols))
+        for numeric_col in numerical_cols:
+            if numeric_col in time_cols:
+                time_cols.remove(numeric_col)
+        for time_col in time_cols:
+            if time_col in text_cols:
+                text_cols.remove(time_col)
+            elif time_col in categorical_cols:
+                categorical_cols.remove(time_col)
         return {'numeric': numerical_cols, 'boolean': boolean_cols, 'text': text_cols,
-                'categorical': categorical_cols, 'time': time_cols, 'id': id_cols}
+                'categorical': categorical_cols, 'time': time_cols}
 
     def loss_detector(self):
         problem_type = self.problem_type()
         if problem_type == "Regression":
             return "R squared"
         elif problem_type in ["Binary regression", "Binary classification", "Multiclass classification"]:
             return "Cross entropy"
@@ -179,19 +126,19 @@
             return None
 
     def metrics_detector(self):
         problem_type = self.problem_type()
         if problem_type == "No target variable":
             return None
         elif problem_type == "Binary regression":
-            return ["MSE", "ROC", "MAE", "MAPE"]
+            return ["MSE", "MAE", "MAPE", "ROC"]
         elif problem_type == "Binary classification":
             return ["Accuracy", "Precision", "Recall", "F1"]
         elif problem_type == "Regression":
-            return ["R2", "MSE", "MAE", "MAPE"]
+            return ["MSE", "MAE", "MAPE"]
         elif problem_type == "Multiclass classification":
             return ["Accuracy", "Precision", "Recall", "F1"]
 
     def model_selection(self):
         problem_type = self.problem_type()
         if problem_type == "No target variable":
             return None
@@ -218,10 +165,10 @@
             report += "Problem Type: " + self.problem_type_val + "\n"
         if self.target:
             report += "Target Variable: " + self.target + "\n"
         report += "Feature Types: " + str(self.feature_types_val) + "\n"
         if self.target:
             report += "Loss Function: " + self.loss_detector_val + "\n"
         report += "Evaluation Metrics: " + str(self.metrics_detector_val) + "\n"
-        report += "Optional Models: " + str(self.model_selection_val) + "\n"
+        report += "Model Selection: " + str(self.model_selection_val) + "\n"
         # report += "Label Transformation: " + str(self.label_transformation_val)
         return report
```

### Comparing `madcat-0.84/chester/zero_break/text_detector.py` & `madcat-0.9/chester/zero_break/text_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import pandas as pd
 
 
 def determine_if_text_or_categorical_column(column):
     # Check if column is a string or categorical data type
     if column.dtype == 'object' or column.dtype.name == 'category':
-        # less than 20 unique values -> not a text column
-        if len(column.unique()) < 20:
-            return False, True
         # Check if column contains more than 50% unique values
-        elif len(column.unique()) > 0.5 * len(column):
+        if len(column.unique()) > 0.5 * len(column):
             return True, False  # Text column
         else:
             return False, True  # Categorical column
     return False, False  # Not a text or categorical column
 
 
 def test_determine_if_text_column():
```

### Comparing `madcat-0.84/setup.py` & `madcat-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open('requirements.txt') as f:
     install_requires = f.read().strip().split('\n')
 
 setuptools.setup(
     name="madcat",
-    version="0.84",
+    version="0.9",
     author="Amit Osi",
     author_email="amitosi6666@gmail.com",
     description=open('README.md').read(),
     url="https://github.com/amito-ds/chester",
     packages=setuptools.find_packages(exclude=["tests*"]),
     include_package_data=True,
-    python_requires=">=3.8",
+    python_requires=">=3.7",
     # List of dependencies for this package
     install_requires=install_requires,
     setup_requires=["pytest-runner"]
-)
+)
```

