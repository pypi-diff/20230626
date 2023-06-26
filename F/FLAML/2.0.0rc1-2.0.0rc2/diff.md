# Comparing `tmp/FLAML-2.0.0rc1.tar.gz` & `tmp/FLAML-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAML-2.0.0rc1.tar", last modified: Fri Jun  9 23:38:39 2023, max compression
+gzip compressed data, was "FLAML-2.0.0rc2.tar", last modified: Mon Jun 26 17:08:09 2023, max compression
```

## Comparing `FLAML-2.0.0rc1.tar` & `FLAML-2.0.0rc2.tar`

### file list

```diff
@@ -1,133 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/FLAML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-06-09 23:38:39.000000 FLAML-2.0.0rc1/FLAML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-09 23:38:39.000000 FLAML-2.0.0rc1/FLAML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:38:39.000000 FLAML-2.0.0rc1/FLAML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-09 23:38:39.000000 FLAML-2.0.0rc1/FLAML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 23:38:39.000000 FLAML-2.0.0rc1/FLAML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/autogen/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/agent/assistant_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/agent/chat_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/agent/user_proxy_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/code_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/autogen/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/autogen/oai/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/oai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45993 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/oai/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/autogen/oai/openai_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129988 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    22656 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)   104594 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/automl/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.821034 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/data_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/training_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/automl/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/spark/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/spark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9829 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/automl/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/task/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    44194 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/task/generic_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13704 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/automl/training_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/all/
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/all/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/all/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/all/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/extra_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/extra_tree/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/extra_tree/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/extra_tree/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/lgbm/
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/lgbm/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/lgbm/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/lgbm/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/regret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/rf/
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/rf/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/rf/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/rf/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/suggest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.825034 FLAML-2.0.0rc1/flaml/default/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgboost/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgboost/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/default/xgboost/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/flaml/onlineml/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/onlineml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/onlineml/autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/onlineml/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/onlineml/trial_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/flaml/tune/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/flaml/tune/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/scheduler/online_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/scheduler/trial_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/flaml/tune/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50288 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/blendsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/cfo_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/flow2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/online_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/search_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/searcher/variant_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23100 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/flaml/tune/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/trial_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    40082 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/tune.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/tune/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/flaml/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 23:38:39.833034 FLAML-2.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:38:39.829034 FLAML-2.0.0rc1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/test/test_autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/test/test_conda_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/test/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 23:37:50.000000 FLAML-2.0.0rc1/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.751581 FLAML-2.0.0rc2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.731581 FLAML-2.0.0rc2/FLAML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-06-26 17:08:09.000000 FLAML-2.0.0rc2/FLAML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 17:08:09.000000 FLAML-2.0.0rc2/FLAML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:08:09.000000 FLAML-2.0.0rc2/FLAML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 17:08:09.000000 FLAML-2.0.0rc2/FLAML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 17:08:09.000000 FLAML-2.0.0rc2/FLAML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-06-26 17:08:09.751581 FLAML-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/autogen/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/agent/assistant_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/agent/math_user_proxy_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/agent/user_proxy_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18621 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/code_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/autogen/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/autogen/oai/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/oai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47084 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/oai/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/oai/openai_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130405 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78597 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.739581 FLAML-2.0.0rc2/flaml/automl/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.739581 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/data_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.739581 FLAML-2.0.0rc2/flaml/automl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/spark/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/spark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9829 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.739581 FLAML-2.0.0rc2/flaml/automl/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/task/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39625 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/task/generic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/task/time_series_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.739581 FLAML-2.0.0rc2/flaml/automl/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/tft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/ts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26508 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/ts_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/training_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/all/
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/all/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/all/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/all/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/extra_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/extra_tree/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/extra_tree/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/extra_tree/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/lgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/lgbm/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/lgbm/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/lgbm/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/regret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/rf/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/rf/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/rf/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/suggest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgboost/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgboost/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgboost/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.747581 FLAML-2.0.0rc2/flaml/onlineml/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/onlineml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/onlineml/autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/onlineml/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/onlineml/trial_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.747581 FLAML-2.0.0rc2/flaml/tune/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.747581 FLAML-2.0.0rc2/flaml/tune/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/scheduler/online_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/scheduler/trial_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.747581 FLAML-2.0.0rc2/flaml/tune/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50288 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/blendsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/cfo_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/flow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/online_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/search_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/variant_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23100 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.751581 FLAML-2.0.0rc2/flaml/tune/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/trial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40082 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:08:09.751581 FLAML-2.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.751581 FLAML-2.0.0rc2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/test/test_autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/test/test_conda_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/test/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/test/test_version.py
```

### Comparing `FLAML-2.0.0rc1/FLAML.egg-info/PKG-INFO` & `FLAML-2.0.0rc2/FLAML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,37 +23,40 @@
 Provides-Extra: hf
 Provides-Extra: nlp
 Provides-Extra: ts_forecast
 Provides-Extra: forecast
 Provides-Extra: benchmark
 Provides-Extra: openai
 Provides-Extra: autogen
+Provides-Extra: mathchat
 Provides-Extra: synapse
 Provides-Extra: autozero
 License-File: LICENSE
 License-File: NOTICE.md
 
 [![PyPI version](https://badge.fury.io/py/FLAML.svg)](https://badge.fury.io/py/FLAML)
 ![Conda version](https://img.shields.io/conda/vn/conda-forge/flaml)
 [![Build](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml/badge.svg)](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml)
-![Python Version](https://img.shields.io/badge/3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
+![Python Version](https://img.shields.io/badge/3.8%20%7C%203.9%20%7C%203.10-blue)
 [![Downloads](https://pepy.tech/badge/flaml)](https://pepy.tech/project/flaml)
 [![](https://img.shields.io/discord/1025786666260111483?logo=discord&style=flat)](https://discord.gg/Cppx2vSPVP)
 <!-- [![Join the chat at https://gitter.im/FLAMLer/community](https://badges.gitter.im/FLAMLer/community.svg)](https://gitter.im/FLAMLer/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) -->
 
 
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: FLAML is highlighted in OpenAI's [cookbook](https://github.com/openai/openai-cookbook#related-resources-from-around-the-web)
+:fire: FLAML is highlighted in OpenAI's [cookbook](https://github.com/openai/openai-cookbook#related-resources-from-around-the-web).
+
 :fire: [autogen](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) is released with support for ChatGPT and GPT-4, based on [Cost-Effective Hyperparameter Optimization for Large Language Model Generation Inference](https://arxiv.org/abs/2303.04673).
+
 :fire: FLAML supports AutoML and Hyperparameter Tuning features in [Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/get-started/microsoft-fabric-overview) private preview. Sign up for these features at: https://aka.ms/fabric/data-science/sign-up.
 
 
 ## What is FLAML
 FLAML is a lightweight Python library for efficient automation of machine
 learning and AI operations, including selection of
 models, hyperparameters, and other tunable choices of an application (e.g., inference hyperparameters for foundation models, configurations in MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations).
```

### Comparing `FLAML-2.0.0rc1/FLAML.egg-info/SOURCES.txt` & `FLAML-2.0.0rc2/FLAML.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 flaml/version.py
 flaml/autogen/__init__.py
 flaml/autogen/code_utils.py
 flaml/autogen/math_utils.py
 flaml/autogen/agent/__init__.py
 flaml/autogen/agent/agent.py
 flaml/autogen/agent/assistant_agent.py
-flaml/autogen/agent/chat_agent.py
+flaml/autogen/agent/math_user_proxy_agent.py
 flaml/autogen/agent/user_proxy_agent.py
 flaml/autogen/extensions/__init__.py
 flaml/autogen/oai/__init__.py
 flaml/autogen/oai/completion.py
 flaml/autogen/oai/openai_utils.py
 flaml/automl/__init__.py
 flaml/automl/automl.py
@@ -45,14 +45,21 @@
 flaml/automl/spark/configs.py
 flaml/automl/spark/metrics.py
 flaml/automl/spark/utils.py
 flaml/automl/task/__init__.py
 flaml/automl/task/factory.py
 flaml/automl/task/generic_task.py
 flaml/automl/task/task.py
+flaml/automl/task/time_series_task.py
+flaml/automl/time_series/__init__.py
+flaml/automl/time_series/feature.py
+flaml/automl/time_series/sklearn.py
+flaml/automl/time_series/tft.py
+flaml/automl/time_series/ts_data.py
+flaml/automl/time_series/ts_model.py
 flaml/default/__init__.py
 flaml/default/estimator.py
 flaml/default/greedy.py
 flaml/default/portfolio.py
 flaml/default/regret.py
 flaml/default/suggest.py
 flaml/default/all/binary.json
```

### Comparing `FLAML-2.0.0rc1/FLAML.egg-info/requires.txt` & `FLAML-2.0.0rc2/FLAML.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 NumPy>=1.17.0rc1
 
 [autogen]
-openai==0.27.4
+openai==0.27.8
 diskcache
 docker
 
 [automl]
 lightgbm>=2.3.1
 xgboost>=0.90
 scipy>=1.4.1
@@ -20,50 +20,61 @@
 [azureml]
 azureml-mlflow
 
 [benchmark]
 catboost>=0.26
 psutil==5.8.0
 xgboost==1.3.3
+pandas==1.1.4
 
 [blendsearch]
 optuna==2.8.0
 
 [catboost]
 catboost>=0.26
 
 [forecast]
 holidays<0.14
 prophet>=1.0.1
 statsmodels>=0.12.2
 hcrystalball==0.1.10
 pytorch-forecasting>=0.9.0
+pytorch-lightning==1.9.0
+tensorboardX==2.6
 
 [hf]
 transformers[torch]==4.26
 datasets
 nltk
 rouge_score
 seqeval
 
+[mathchat]
+openai==0.27.8
+diskcache
+docker
+sympy
+pydantic
+wolframalpha
+
 [nlp]
 transformers[torch]==4.26
 datasets
 nltk
 rouge_score
 seqeval
 
 [nni]
 nni
 
 [notebook]
 jupyter
 
 [openai]
-openai==0.27.4
+openai==0.27.8
 diskcache
 
 [ray]
 ray[tune]~=1.13
 
 [spark]
 pyspark>=3.2.0
@@ -103,16 +114,20 @@
 mlflow
 pyspark>=3.2.0
 joblibspark>=0.5.0
 nbconvert
 nbformat
 ipykernel
 pytorch-lightning<1.9.1
+tensorboardX==2.6
 requests<2.29.0
 packaging
+pydantic
+sympy
+wolframalpha
 
 [ts_forecast]
 holidays<0.14
 prophet>=1.0.1
 statsmodels>=0.12.2
 hcrystalball==0.1.10
```

### Comparing `FLAML-2.0.0rc1/LICENSE` & `FLAML-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/NOTICE.md` & `FLAML-2.0.0rc2/NOTICE.md`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/PKG-INFO` & `FLAML-2.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,37 +23,40 @@
 Provides-Extra: hf
 Provides-Extra: nlp
 Provides-Extra: ts_forecast
 Provides-Extra: forecast
 Provides-Extra: benchmark
 Provides-Extra: openai
 Provides-Extra: autogen
+Provides-Extra: mathchat
 Provides-Extra: synapse
 Provides-Extra: autozero
 License-File: LICENSE
 License-File: NOTICE.md
 
 [![PyPI version](https://badge.fury.io/py/FLAML.svg)](https://badge.fury.io/py/FLAML)
 ![Conda version](https://img.shields.io/conda/vn/conda-forge/flaml)
 [![Build](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml/badge.svg)](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml)
-![Python Version](https://img.shields.io/badge/3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
+![Python Version](https://img.shields.io/badge/3.8%20%7C%203.9%20%7C%203.10-blue)
 [![Downloads](https://pepy.tech/badge/flaml)](https://pepy.tech/project/flaml)
 [![](https://img.shields.io/discord/1025786666260111483?logo=discord&style=flat)](https://discord.gg/Cppx2vSPVP)
 <!-- [![Join the chat at https://gitter.im/FLAMLer/community](https://badges.gitter.im/FLAMLer/community.svg)](https://gitter.im/FLAMLer/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) -->
 
 
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: FLAML is highlighted in OpenAI's [cookbook](https://github.com/openai/openai-cookbook#related-resources-from-around-the-web)
+:fire: FLAML is highlighted in OpenAI's [cookbook](https://github.com/openai/openai-cookbook#related-resources-from-around-the-web).
+
 :fire: [autogen](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) is released with support for ChatGPT and GPT-4, based on [Cost-Effective Hyperparameter Optimization for Large Language Model Generation Inference](https://arxiv.org/abs/2303.04673).
+
 :fire: FLAML supports AutoML and Hyperparameter Tuning features in [Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/get-started/microsoft-fabric-overview) private preview. Sign up for these features at: https://aka.ms/fabric/data-science/sign-up.
 
 
 ## What is FLAML
 FLAML is a lightweight Python library for efficient automation of machine
 learning and AI operations, including selection of
 models, hyperparameters, and other tunable choices of an application (e.g., inference hyperparameters for foundation models, configurations in MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations).
```

### Comparing `FLAML-2.0.0rc1/README.md` & `FLAML-2.0.0rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [![PyPI version](https://badge.fury.io/py/FLAML.svg)](https://badge.fury.io/py/FLAML)
 ![Conda version](https://img.shields.io/conda/vn/conda-forge/flaml)
 [![Build](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml/badge.svg)](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml)
-![Python Version](https://img.shields.io/badge/3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
+![Python Version](https://img.shields.io/badge/3.8%20%7C%203.9%20%7C%203.10-blue)
 [![Downloads](https://pepy.tech/badge/flaml)](https://pepy.tech/project/flaml)
 [![](https://img.shields.io/discord/1025786666260111483?logo=discord&style=flat)](https://discord.gg/Cppx2vSPVP)
 <!-- [![Join the chat at https://gitter.im/FLAMLer/community](https://badges.gitter.im/FLAMLer/community.svg)](https://gitter.im/FLAMLer/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) -->
 
 
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: FLAML is highlighted in OpenAI's [cookbook](https://github.com/openai/openai-cookbook#related-resources-from-around-the-web)
+:fire: FLAML is highlighted in OpenAI's [cookbook](https://github.com/openai/openai-cookbook#related-resources-from-around-the-web).
+
 :fire: [autogen](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) is released with support for ChatGPT and GPT-4, based on [Cost-Effective Hyperparameter Optimization for Large Language Model Generation Inference](https://arxiv.org/abs/2303.04673).
+
 :fire: FLAML supports AutoML and Hyperparameter Tuning features in [Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/get-started/microsoft-fabric-overview) private preview. Sign up for these features at: https://aka.ms/fabric/data-science/sign-up.
 
 
 ## What is FLAML
 FLAML is a lightweight Python library for efficient automation of machine
 learning and AI operations, including selection of
 models, hyperparameters, and other tunable choices of an application (e.g., inference hyperparameters for foundation models, configurations in MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations).
```

### Comparing `FLAML-2.0.0rc1/flaml/autogen/agent/agent.py` & `FLAML-2.0.0rc2/flaml/autogen/agent/agent.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/autogen/agent/assistant_agent.py` & `FLAML-2.0.0rc2/flaml/autogen/agent/assistant_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,13 +35,14 @@
 
     def receive(self, message, sender):
         if sender.name not in self._sender_dict:
             self._sender_dict[sender.name] = sender
             self._conversations[sender.name] = [{"content": self._system_message, "role": "system"}]
         super().receive(message, sender)
         responses = oai.ChatCompletion.create(messages=self._conversations[sender.name], **self._config)
+        # TODO: handle function_call
         response = oai.ChatCompletion.extract_text(responses)[0]
         self._send(response, sender)
 
     def reset(self):
         self._sender_dict.clear()
         self._conversations.clear()
```

### Comparing `FLAML-2.0.0rc1/flaml/autogen/agent/user_proxy_agent.py` & `FLAML-2.0.0rc2/flaml/autogen/agent/user_proxy_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 Possible values are "ALWAYS", "TERMINATE", "NEVER".
                 (1) When "ALWAYS", the agent prompts for human input every time a message is received.
                     Under this mode, the conversation stops when the human input is "exit",
                     or when is_termination_msg is True and there is no human input.
                 (2) When "TERMINATE", the agent only prompts for human input only when a termination message is received or
                     the number of auto reply reaches the max_consecutive_auto_reply.
                 (3) When "NEVER", the agent will never prompt for human input. Under this mode, the conversation stops
-                    when the number of auto reply reaches the max_consecutive_auto_reply or or when is_termination_msg is True.
+                    when the number of auto reply reaches the max_consecutive_auto_reply or when is_termination_msg is True.
             max_consecutive_auto_reply (int): the maximum number of consecutive auto replies.
                 default to None (no limit provided, class attribute MAX_CONSECUTIVE_AUTO_REPLY will be used as the limit in this case).
                 The limit only plays a role when human_input_mode is not "ALWAYS".
             is_termination_msg (function): a function that takes a message and returns a boolean value.
                 This function is used to determine if a received message is a termination message.
             use_docker (bool): whether to use docker to execute the code.
             **config (dict): other configurations.
```

### Comparing `FLAML-2.0.0rc1/flaml/autogen/code_utils.py` & `FLAML-2.0.0rc2/flaml/autogen/code_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from hashlib import md5
 from flaml.autogen import oai, DEFAULT_MODEL, FAST_MODEL
 
 # Regular expression for finding a code block
 CODE_BLOCK_PATTERN = r"```(\w*)\n(.*?)\n```"
 WORKING_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), "extensions")
 UNKNOWN = "unknown"
+TIMEOUT_MSG = bytes("Timeout", "utf-8")
 
 
 def infer_lang(code):
     """infer the language for the code.
     TODO: make it robust.
     """
     if code.startswith("python ") or code.startswith("pip"):
@@ -176,15 +177,14 @@
         # create a file with a automatically generated name
         filename = f"tmp_code_{code_hash}.{'py' if lang.startswith('python') else lang}"
     if work_dir is None:
         work_dir = WORKING_DIR
     filepath = os.path.join(work_dir, filename)
     file_dir = os.path.dirname(filepath)
     os.makedirs(file_dir, exist_ok=True)
-
     if code is not None:
         with open(filepath, "w") as fout:
             fout.write(code)
     # check if already running in a docker container
     in_docker_container = os.path.exists("/.dockerenv")
     if not use_docker or in_docker_container:
         # already running in a docker container
@@ -198,15 +198,15 @@
                 cwd=work_dir,
                 capture_output=True,
             )
             signal.alarm(0)
         except TimeoutError:
             if original_filename is None:
                 os.remove(filepath)
-            return 1, "Timeout", None
+            return 1, TIMEOUT_MSG, None
         if original_filename is None:
             os.remove(filepath)
         return result.returncode, result.stderr if result.returncode else result.stdout, None
 
     import docker
 
     # create a docker client
@@ -256,15 +256,15 @@
         # Reload the container object
         container.reload()
     if container.status != "exited":
         container.stop()
         container.remove()
         if original_filename is None:
             os.remove(filepath)
-        return 1, "Timeout", image
+        return 1, TIMEOUT_MSG, image
     # try:
     #     container.wait(timeout=timeout)
     # except (ReadTimeout, ConnectionError):
     #     container.stop()
     #     container.remove()
     #     if original_filename is None:
     #         os.remove(filepath)
```

### Comparing `FLAML-2.0.0rc1/flaml/autogen/math_utils.py` & `FLAML-2.0.0rc2/flaml/autogen/math_utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/autogen/oai/completion.py` & `FLAML-2.0.0rc2/flaml/autogen/oai/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,38 +41,46 @@
 
     It also supports: ChatCompletion, Azure OpenAI API.
     """
 
     # set of models that support chat completion
     chat_models = {
         "gpt-3.5-turbo",
-        "gpt-3.5-turbo-0301",
+        "gpt-3.5-turbo-0301",  # deprecate in Sep
+        "gpt-3.5-turbo-0613",
+        "gpt-3.5-turbo-16k",
         "gpt-35-turbo",
         "gpt-4",
         "gpt-4-32k",
-        "gpt-4-32k-0314",
-        "gpt-4-0314",
+        "gpt-4-32k-0314",  # deprecate in Sep
+        "gpt-4-0314",  # deprecate in Sep
+        "gpt-4-0613",
+        "gpt-4-32k-0613",
     }
 
     # price per 1k tokens
     price1K = {
         "text-ada-001": 0.0004,
         "text-babbage-001": 0.0005,
         "text-curie-001": 0.002,
         "code-cushman-001": 0.024,
         "code-davinci-002": 0.1,
         "text-davinci-002": 0.02,
         "text-davinci-003": 0.02,
-        "gpt-3.5-turbo": 0.002,
-        "gpt-3.5-turbo-0301": 0.002,
+        "gpt-3.5-turbo": (0.0015, 0.002),
+        "gpt-3.5-turbo-0301": (0.0015, 0.002),  # deprecate in Sep
+        "gpt-3.5-turbo-0613": (0.0015, 0.002),
+        "gpt-3.5-turbo-16k": (0.003, 0.004),
         "gpt-35-turbo": 0.002,
         "gpt-4": (0.03, 0.06),
-        "gpt-4-0314": (0.03, 0.06),
         "gpt-4-32k": (0.06, 0.12),
-        "gpt-4-32k-0314": (0.06, 0.12),
+        "gpt-4-0314": (0.03, 0.06),  # deprecate in Sep
+        "gpt-4-32k-0314": (0.06, 0.12),  # deprecate in Sep
+        "gpt-4-0613": (0.03, 0.06),
+        "gpt-4-32k-0613": (0.06, 0.12),
     }
 
     default_search_space = {
         "model": tune.choice(
             [
                 "text-ada-001",
                 "text-babbage-001",
@@ -382,15 +390,15 @@
                     response = cls.create(data_i, raise_error=eval_only, **params)
                     if response == -1:  # rate limit/timeout error, treat as invalid
                         cls._update_invalid_n(prune, region_key, max_tokens, num_completions)
                         result[metric] = 0
                         result["cost"] = cost
                         return result
                     # evaluate the quality of the responses
-                    responses = cls.extract_text(response)
+                    responses = cls.extract_text_or_function_call(response)
                     usage = response["usage"]
                     n_input_tokens = usage["prompt_tokens"]
                     n_output_tokens = usage.get("completion_tokens", 0)
                     if not cls.avg_input_tokens and not input_tokens[i]:
                         # store the # input tokens
                         input_tokens[i] = n_input_tokens
                     query_cost = response["cost"]
@@ -894,15 +902,15 @@
         old_level = logger.getEffectiveLevel()
         logger.setLevel(logging_level)
         for i, data_i in enumerate(data):
             logger.info(f"evaluating data instance {i}")
             response = cls.create(data_i, use_cache, **config)
             cost += response["cost"]
             # evaluate the quality of the responses
-            responses = cls.extract_text(response)
+            responses = cls.extract_text_or_function_call(response)
             if eval_func is not None:
                 metrics = eval_func(responses, **data_i)
             elif hasattr(cls, "_eval_func"):
                 metrics = cls._eval_func(responses, **data_i)
             else:
                 logger.warning(
                     "Please either provide a valid eval_func or do the test after the tune function is called."
@@ -988,14 +996,32 @@
         """
         choices = response["choices"]
         if "text" in choices[0]:
             return [choice["text"] for choice in choices]
         return [choice["message"].get("content", "") for choice in choices]
 
     @classmethod
+    def extract_text_or_function_call(cls, response: dict) -> List[str]:
+        """Extract the text or function calls from a completion or chat response.
+
+        Args:
+            response (dict): The response from OpenAI API.
+
+        Returns:
+            A list of text or function calls in the responses.
+        """
+        choices = response["choices"]
+        if "text" in choices[0]:
+            return [choice["text"] for choice in choices]
+        return [
+            choice["message"] if "function_call" in choice["message"] else choice["message"].get("content", "")
+            for choice in choices
+        ]
+
+    @classmethod
     @property
     def logged_history(cls) -> Dict:
         """Return the book keeping dictionary."""
         return cls._history_dict
 
     @classmethod
     def start_logging(
```

### Comparing `FLAML-2.0.0rc1/flaml/autogen/oai/openai_utils.py` & `FLAML-2.0.0rc2/flaml/autogen/oai/openai_utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/automl.py` & `FLAML-2.0.0rc2/flaml/automl/automl.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,31 +9,30 @@
 from typing import Callable, List, Union, Optional
 from functools import partial
 import numpy as np
 import logging
 import json
 
 from flaml.automl.state import SearchState, AutoMLState
-from flaml.automl.ml import (
-    train_estimator,
-    get_estimator_class,
-)
+from flaml.automl.ml import train_estimator
+
+from flaml.automl.time_series import TimeSeriesDataset
 from flaml.config import (
     MIN_SAMPLE_TRAIN,
     MEM_THRES,
     RANDOM_SEED,
     SMALL_LARGE_THRES,
     CV_HOLDOUT_THRESHOLD,
     SPLIT_RATIO,
     N_SPLITS,
     SAMPLE_MULTIPLY_FACTOR,
 )
 
 # TODO check to see when we can remove these
-from flaml.automl.task.task import CLASSIFICATION, TS_FORECAST, Task
+from flaml.automl.task.task import CLASSIFICATION, Task
 from flaml.automl.task.factory import task_factory
 from flaml import tune
 from flaml.automl.logger import logger, logger_formatter
 from flaml.automl.training_log import training_log_reader, training_log_writer
 from flaml.default import suggest_learner
 from flaml.version import __version__ as flaml_version
 from flaml.automl.spark import psDataFrame, psSeries, DataFrame, Series
@@ -895,15 +894,17 @@
         if not isinstance(self._split_type, str):
             assert eval_method in [
                 "auto",
                 "cv",
             ], "eval_method must be 'auto' or 'cv' for custom data splitter."
             assert self._state.X_val is None, "custom splitter and custom validation data can't be used together."
             return "cv"
-        if self._state.X_val is not None:
+        if self._state.X_val is not None and (
+            not isinstance(self._state.X_val, TimeSeriesDataset) or len(self._state.X_val.test_data) > 0
+        ):
             assert eval_method in [
                 "auto",
                 "holdout",
             ], "eval_method must be 'auto' or 'holdout' for custom validation data."
             return "holdout"
         if eval_method != "auto":
             assert eval_method in [
@@ -1140,15 +1141,15 @@
             eval_method,
             self._split_type,
             split_ratio,
             n_splits,
             self._df,
             self._sample_weight_full,
         )
-        self.data_size_full = len(self._state.y_train_all)
+        self.data_size_full = self._state.data_size_full
 
     def fit(
         self,
         X_train=None,
         y_train=None,
         dataframe=None,
         label=None,
@@ -1192,14 +1193,15 @@
         auto_augment=None,
         min_sample_size=None,
         use_ray=None,
         use_spark=None,
         free_mem_ratio=0,
         metric_constraints=None,
         custom_hp=None,
+        time_col=None,
         cv_score_agg_func=None,
         skip_transform=None,
         mlflow_logging=None,
         fit_kwargs_by_estimator=None,
         **fit_kwargs,
     ):
         """Find a model for a given task.
@@ -1424,14 +1426,16 @@
                 },
                 "learning_rate": {
                     "domain": tune.choice([1e-4, 1e-5]),
                 }
             }
         }
         ```
+            time_col: for a time series task, name of the column containing the timestamps. If not
+                provided, defaults to the first column of X_train/X_val
 
             cv_score_agg_func: customized cross-validation scores aggregate function. Default to average metrics across folds. If specificed, this function needs to
                 have the following input arguments:
 
                 * val_loss_folds: list of floats, the loss scores of each fold;
                 * log_metrics_folds: list of dicts/floats, the metrics of each fold to log.
 
@@ -1518,14 +1522,15 @@
         """
 
         self._state._start_time_flag = self._start_time_flag = time.time()
         task = task or self._settings.get("task")
         if isinstance(task, str):
             task = task_factory(task, X_train, y_train)
         self._state.task = task
+        self._state.task.time_col = time_col
         self._estimator_type = "classifier" if task.is_classification() else "regressor"
         time_budget = time_budget or self._settings.get("time_budget")
         n_jobs = n_jobs or self._settings.get("n_jobs")
         gpu_per_trial = fit_kwargs.get("gpu_per_trial", 0)
         eval_method = eval_method or self._settings.get("eval_method")
         split_ratio = split_ratio or self._settings.get("split_ratio")
         n_splits = n_splits or self._settings.get("n_splits")
@@ -1820,15 +1825,15 @@
             or max_iter == 1
         )
         # add custom learner
         for estimator_name in estimator_list:
             if estimator_name not in self._state.learner_classes:
                 self.add_learner(
                     estimator_name,
-                    get_estimator_class(self._state.task, estimator_name),
+                    self._state.task.estimator_class_from_str(estimator_name),
                 )
         # set up learner search space
         if isinstance(starting_points, str) and starting_points.startswith("data"):
             from flaml.default import suggest_config
 
             location = starting_points[5:]
             starting_points = {}
@@ -1875,15 +1880,16 @@
                     estimator_name
                 ] = this_estimator_kwargs  # set self._state.fit_kwargs_by_estimator[estimator_name] to the update, so only self._state.fit_kwargs_by_estimator will be updated
             else:
                 self._state.fit_kwargs_by_estimator[estimator_name] = self._state.fit_kwargs
 
             self._search_states[estimator_name] = SearchState(
                 learner_class=estimator_class,
-                data_size=self._state.data_size,
+                # data_size=self._state.data_size,
+                data=self._state.X_train,
                 task=self._state.task,
                 starting_point=starting_points.get(estimator_name),
                 period=self._state.fit_kwargs.get(
                     "period"
                 ),  # NOTE: this is after kwargs is updated to fit_kwargs_by_estimator
                 custom_hp=custom_hp and custom_hp.get(estimator_name),
                 max_iter=max_iter / len(estimator_list) if self._learner_selector == "roundrobin" else max_iter,
@@ -2585,15 +2591,15 @@
                         " Please try increasing available RAM, decreasing n_jobs for ensemble, or disabling ensemble."
                     )
             elif self._state.retrain_final:
                 # reset time budget for retraining
                 if self._max_iter > 1:
                     self._state.time_budget = -1
                 if (
-                    self._state.task in TS_FORECAST
+                    self._state.task.is_ts_forecast()
                     or self._trained_estimator is None
                     or self._trained_estimator.model is None
                     or (
                         self._state.time_budget < 0
                         or self._state.time_budget - self._state.time_from_start
                         > self._selected.est_retrain_time(self.data_size_full)
                     )
```

### Comparing `FLAML-2.0.0rc1/flaml/automl/data.py` & `FLAML-2.0.0rc2/flaml/automl/data.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/ml.py` & `FLAML-2.0.0rc2/flaml/automl/ml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,22 @@
 # !
 #  * Copyright (c) FLAML authors. All rights reserved.
 #  * Licensed under the MIT License. See LICENSE file in the
 #  * project root for license information.
 import time
-import numpy as np
 from typing import Union, Callable, TypeVar, Optional, Tuple
-from flaml.automl.model import (
-    XGBoostSklearnEstimator,
-    XGBoost_TS,
-    XGBoostLimitDepthEstimator,
-    XGBoostLimitDepth_TS,
-    RandomForestEstimator,
-    RF_TS,
-    LGBMEstimator,
-    LGBM_TS,
-    LRL1Classifier,
-    LRL2Classifier,
-    CatBoostEstimator,
-    ExtraTreesEstimator,
-    ExtraTrees_TS,
-    KNeighborsEstimator,
-    Prophet,
-    ARIMA,
-    SARIMAX,
-    HoltWinters,
-    TransformersEstimator,
-    TemporalFusionTransformerEstimator,
-    TransformersEstimatorModelSelection,
-    SparkLGBMEstimator,
-)
+import logging
+
+import numpy as np
+
+
 from flaml.automl.data import group_counts
-from flaml.automl.task.task import TS_FORECAST, Task
-from flaml.automl.model import BaseEstimator
-from flaml.automl.spark import psDataFrame, psSeries, ERROR as SPARK_ERROR, Series
+from flaml.automl.task.task import Task
+from flaml.automl.model import BaseEstimator, TransformersEstimator
+from flaml.automl.spark import psDataFrame, psSeries, ERROR as SPARK_ERROR, Series, DataFrame
 
 try:
     from sklearn.metrics import (
         mean_squared_error,
         r2_score,
         roc_auc_score,
         accuracy_score,
@@ -49,14 +29,19 @@
     )
 except ImportError:
     pass
 
 if SPARK_ERROR is None:
     from flaml.automl.spark.metrics import spark_metric_loss_score
 
+from flaml.automl.time_series import TimeSeriesDataset
+
+logger = logging.getLogger(__name__)
+
+
 EstimatorSubclass = TypeVar("EstimatorSubclass", bound=BaseEstimator)
 
 sklearn_metric_name_set = {
     "r2",
     "rmse",
     "mae",
     "mse",
@@ -102,63 +87,14 @@
     "spearmanr": "max",
     "ter": "min",
     "wer": "min",
 }
 huggingface_submetric_to_metric = {"rouge1": "rouge", "rouge2": "rouge"}
 
 
-def get_estimator_class(task: str, estimator_name: str) -> EstimatorSubclass:
-    """Given a task and an estimator name, return the relevant flaml-wrapped estimator class
-
-    NOTE: See why the return type is declarad by using TypeVar here on the mypy doc
-    https://mypy.readthedocs.io/en/stable/kinds_of_types.html#the-type-of-class-objects
-    """
-    # when adding a new learner, need to add an elif branch
-    if "xgboost" == estimator_name:
-        estimator_class = XGBoost_TS if task in TS_FORECAST else XGBoostSklearnEstimator
-    elif "xgb_limitdepth" == estimator_name:
-        estimator_class = XGBoostLimitDepth_TS if task in TS_FORECAST else XGBoostLimitDepthEstimator
-    elif "rf" == estimator_name:
-        estimator_class = RF_TS if task in TS_FORECAST else RandomForestEstimator
-    elif "lgbm" == estimator_name:
-        estimator_class = LGBM_TS if task in TS_FORECAST else LGBMEstimator
-    elif "lgbm_spark" == estimator_name:
-        estimator_class = SparkLGBMEstimator
-    elif "lrl1" == estimator_name:
-        estimator_class = LRL1Classifier
-    elif "lrl2" == estimator_name:
-        estimator_class = LRL2Classifier
-    elif "catboost" == estimator_name:
-        estimator_class = CatBoostEstimator
-    elif "extra_tree" == estimator_name:
-        estimator_class = ExtraTrees_TS if task in TS_FORECAST else ExtraTreesEstimator
-    elif "kneighbor" == estimator_name:
-        estimator_class = KNeighborsEstimator
-    elif "prophet" in estimator_name:
-        estimator_class = Prophet
-    elif estimator_name == "arima":
-        estimator_class = ARIMA
-    elif estimator_name == "sarimax":
-        estimator_class = SARIMAX
-    elif estimator_name == "holt-winters":
-        estimator_class = HoltWinters
-    elif estimator_name == "transformer":
-        estimator_class = TransformersEstimator
-    elif estimator_name == "tft":
-        estimator_class = TemporalFusionTransformerEstimator
-    elif estimator_name == "transformer_ms":
-        estimator_class = TransformersEstimatorModelSelection
-    else:
-        raise ValueError(
-            estimator_name + " is not a built-in learner. "
-            "Please use AutoML.add_learner() to add a customized learner."
-        )
-    return estimator_class
-
-
 def metric_loss_score(
     metric_name: str,
     y_processed_predict,
     y_processed_true,
     labels=None,
     sample_weight=None,
     groups=None,
@@ -263,14 +199,15 @@
         labels: A list or an array of the unique labels.
         sample_weight: A 1d numpy array of the sample weight.
         groups: A 1d numpy array of the group labels.
 
     Returns:
         score: A float number of the loss, the lower the better.
     """
+
     metric_name = metric_name.lower()
 
     if "r2" == metric_name:
         score = 1.0 - r2_score(y_true, y_predict, sample_weight=sample_weight)
     elif metric_name == "rmse":
         score = np.sqrt(mean_squared_error(y_true, y_predict, sample_weight=sample_weight))
     elif metric_name == "mae":
@@ -352,168 +289,56 @@
         "roc_auc_ovo",
         "roc_auc_ovo_weighted",
         "roc_auc_ovr_weighted",
     ]:
         y_pred = estimator.predict_proba(X)
     else:
         y_pred = estimator.predict(X)
-    return y_pred
 
+    if isinstance(y_pred, Series) or isinstance(y_pred, DataFrame):
+        y_pred = y_pred.values
 
-def _eval_estimator(
-    config,
-    estimator,
-    X_train,
-    y_train,
-    X_val,
-    y_val,
-    weight_val,
-    groups_val,
-    eval_metric: Union[str, Callable],
-    task,
-    labels=None,
-    log_training_metric=False,
-    fit_kwargs: Optional[dict] = None,
-):
-    if fit_kwargs is None:
-        fit_kwargs = {}
-    if isinstance(eval_metric, str):
-        pred_start = time.time()
-        val_pred_y = get_y_pred(estimator, X_val, eval_metric, task)
-        pred_time = (time.time() - pred_start) / X_val.shape[0]
-
-        val_loss = metric_loss_score(
-            eval_metric,
-            y_processed_predict=val_pred_y,
-            y_processed_true=y_val,
-            labels=labels,
-            sample_weight=weight_val,
-            groups=groups_val,
-        )
-        metric_for_logging = {"pred_time": pred_time}
-        if log_training_metric:
-            train_pred_y = get_y_pred(estimator, X_train, eval_metric, task)
-            metric_for_logging["train_loss"] = metric_loss_score(
-                eval_metric,
-                train_pred_y,
-                y_train,
-                labels,
-                fit_kwargs.get("sample_weight"),
-                fit_kwargs.get("groups"),
-            )
-    else:  # customized metric function
-        val_loss, metric_for_logging = eval_metric(
-            X_val,
-            y_val,
-            estimator,
-            labels,
-            X_train,
-            y_train,
-            weight_val,
-            fit_kwargs.get("sample_weight"),
-            config,
-            groups_val,
-            fit_kwargs.get("groups"),
-        )
-        pred_time = metric_for_logging.get("pred_time", 0)
-        val_pred_y = None
-        # eval_metric may return val_pred_y but not necessarily. Setting None for now.
-    return val_loss, metric_for_logging, pred_time, val_pred_y
-
+    return y_pred
 
-def get_val_loss(
-    config,
-    estimator: EstimatorSubclass,
-    X_train,
-    y_train,
-    X_val,
-    y_val,
-    weight_val,
-    groups_val,
-    eval_metric: Union[str, Callable],
-    obj,
-    labels=None,
-    budget=None,
-    log_training_metric=False,
-    fit_kwargs: Optional[dict] = None,
-    free_mem_ratio=0,
-):
-    if fit_kwargs is None:
-        fit_kwargs = {}
-    start = time.time()
-    # if groups_val is not None:
-    #     fit_kwargs['groups_val'] = groups_val
-    #     fit_kwargs['X_val'] = X_val
-    #     fit_kwargs['y_val'] = y_val
-    estimator.fit(X_train, y_train, budget, free_mem_ratio, **fit_kwargs)
-    val_loss, metric_for_logging, pred_time, _ = _eval_estimator(
-        config,
-        estimator,
-        X_train,
-        y_train,
-        X_val,
-        y_val,
-        weight_val,
-        groups_val,
-        eval_metric,
-        obj,
-        labels,
-        log_training_metric,
-        fit_kwargs,
-    )
-    if hasattr(estimator, "intermediate_results"):
-        metric_for_logging["intermediate_results"] = estimator.intermediate_results
-    train_time = time.time() - start
-    return val_loss, metric_for_logging, train_time, pred_time
 
+def to_numpy(x):
+    if isinstance(x, Series or isinstance(x, DataFrame)):
+        x = x.values
+    else:
+        x = np.ndarray(x)
 
-def default_cv_score_agg_func(val_loss_folds, log_metrics_folds):
-    metric_to_minimize = sum(val_loss_folds) / len(val_loss_folds)
-    metrics_to_log = None
-    for single_fold in log_metrics_folds:
-        if metrics_to_log is None:
-            metrics_to_log = single_fold
-        elif isinstance(metrics_to_log, dict):
-            metrics_to_log = {k: metrics_to_log[k] + v for k, v in single_fold.items()}
-        else:
-            metrics_to_log += single_fold
-    if metrics_to_log:
-        n = len(val_loss_folds)
-        metrics_to_log = (
-            {k: v / n for k, v in metrics_to_log.items()} if isinstance(metrics_to_log, dict) else metrics_to_log / n
-        )
-    return metric_to_minimize, metrics_to_log
+    return x.reshape((-1, 1))
 
 
 def compute_estimator(
     X_train,
     y_train,
     X_val,
     y_val,
     weight_val,
     groups_val,
     budget,
     kf,
     config_dic: dict,
-    task: str,
+    task: Union[str, Task],
     estimator_name: str,
     eval_method: str,
     eval_metric: Union[str, Callable],
     best_val_loss=np.Inf,
     n_jobs: Optional[int] = 1,  # some estimators of EstimatorSubclass don't accept n_jobs. Should be None in that case.
     estimator_class: Optional[EstimatorSubclass] = None,
     cv_score_agg_func: Optional[callable] = None,
     log_training_metric: Optional[bool] = False,
     fit_kwargs: Optional[dict] = None,
     free_mem_ratio=0,
 ):
     if fit_kwargs is None:
         fit_kwargs = {}
 
-    estimator_class = estimator_class or get_estimator_class(task, estimator_name)
+    estimator_class = estimator_class or task.estimator_class_from_str(estimator_name)
     estimator = estimator_class(
         **config_dic,
         task=task,
         n_jobs=n_jobs,
     )
 
     if isinstance(estimator, TransformersEstimator):
@@ -572,28 +397,28 @@
     estimator_class: Optional[EstimatorSubclass] = None,
     budget=None,
     fit_kwargs: Optional[dict] = None,
     eval_metric=None,
     free_mem_ratio=0,
 ) -> Tuple[EstimatorSubclass, float]:
     start_time = time.time()
-    estimator_class = estimator_class or get_estimator_class(task, estimator_name)
+    estimator_class = estimator_class or task.estimator_class_from_str(estimator_name)
     estimator = estimator_class(
         **config_dic,
         task=task,
         n_jobs=n_jobs,
     )
     if fit_kwargs is None:
         fit_kwargs = {}
 
     if isinstance(estimator, TransformersEstimator):
         fit_kwargs["metric"] = eval_metric
 
     if X_train is not None:
-        train_time = estimator.fit(X_train, y_train, budget, free_mem_ratio, **fit_kwargs)
+        train_time = estimator.fit(X_train, y_train, budget=budget, free_mem_ratio=free_mem_ratio, **fit_kwargs)
     else:
         estimator = estimator.estimator_class(**estimator.params)
     train_time = time.time() - start_time
     return estimator, train_time
 
 
 def norm_confusion_matrix(y_true: Union[np.array, Series], y_pred: Union[np.array, Series]):
@@ -638,7 +463,144 @@
     classes = np.unique(y_true)
     y_true_binary = label_binarize(y_true, classes=classes)
 
     curve_x, curve_y = {}, {}
     for i in range(len(classes)):
         curve_x[i], curve_y[i], _ = curve_func(y_true_binary[:, i], y_pred_proba[:, i])
     return curve_x, curve_y
+
+
+def get_val_loss(
+    config,
+    estimator,
+    X_train,
+    y_train,
+    X_val,
+    y_val,
+    weight_val,
+    groups_val,
+    eval_metric,
+    task,
+    labels=None,
+    budget=None,
+    log_training_metric=False,
+    fit_kwargs={},
+    free_mem_ratio=0,
+):
+    start = time.time()
+    # if groups_val is not None:
+    #     fit_kwargs['groups_val'] = groups_val
+    #     fit_kwargs['X_val'] = X_val
+    #     fit_kwargs['y_val'] = y_val
+    estimator.fit(X_train, y_train, budget=budget, free_mem_ratio=free_mem_ratio, **fit_kwargs)
+    val_loss, metric_for_logging, pred_time, _ = _eval_estimator(
+        config,
+        estimator,
+        X_train,
+        y_train,
+        X_val,
+        y_val,
+        weight_val,
+        groups_val,
+        eval_metric,
+        task,
+        labels,
+        log_training_metric,
+        fit_kwargs,
+    )
+    if hasattr(estimator, "intermediate_results"):
+        metric_for_logging["intermediate_results"] = estimator.intermediate_results
+    train_time = time.time() - start
+    return val_loss, metric_for_logging, train_time, pred_time
+
+
+def default_cv_score_agg_func(val_loss_folds, log_metrics_folds):
+    metric_to_minimize = sum(val_loss_folds) / len(val_loss_folds)
+    metrics_to_log = None
+    for single_fold in log_metrics_folds:
+        if metrics_to_log is None:
+            metrics_to_log = single_fold
+        elif isinstance(metrics_to_log, dict):
+            metrics_to_log = {k: metrics_to_log[k] + v for k, v in single_fold.items()}
+        else:
+            metrics_to_log += single_fold
+    if metrics_to_log:
+        n = len(val_loss_folds)
+        metrics_to_log = (
+            {k: v / n for k, v in metrics_to_log.items()} if isinstance(metrics_to_log, dict) else metrics_to_log / n
+        )
+    return metric_to_minimize, metrics_to_log
+
+
+def _eval_estimator(
+    config,
+    estimator,
+    X_train,
+    y_train,
+    X_val,
+    y_val,
+    weight_val,
+    groups_val,
+    eval_metric,
+    task,
+    labels=None,
+    log_training_metric=False,
+    fit_kwargs={},
+):
+    if isinstance(eval_metric, str):
+        pred_start = time.time()
+        val_pred_y = get_y_pred(estimator, X_val, eval_metric, task)
+
+        # TODO: why are integer labels being cast to str in the first place?
+
+        if isinstance(val_pred_y, Series) or isinstance(val_pred_y, DataFrame) or isinstance(val_pred_y, np.ndarray):
+            test = val_pred_y if isinstance(val_pred_y, np.ndarray) else val_pred_y.values
+            if not np.issubdtype(test.dtype, np.number):
+                # some NLP models return a list
+                val_pred_y = val_pred_y.astype(str)
+
+        if isinstance(X_val, TimeSeriesDataset):
+            num_val_rows = len(X_val.test_data)
+            y_val = X_val.test_data[X_val.target_names].values.astype(val_pred_y.dtype)
+            y_train = X_val.train_data[X_val.target_names].values.astype(val_pred_y.dtype)
+        else:
+            num_val_rows = X_val.shape[0]
+
+        pred_time = (time.time() - pred_start) / num_val_rows
+
+        val_loss = metric_loss_score(
+            eval_metric,
+            y_processed_predict=val_pred_y,
+            y_processed_true=y_val,
+            labels=labels,
+            sample_weight=weight_val,
+            groups=groups_val,
+        )
+        metric_for_logging = {"pred_time": pred_time}
+        if log_training_metric:
+            train_pred_y = get_y_pred(estimator, X_train, eval_metric, task)
+            metric_for_logging["train_loss"] = metric_loss_score(
+                eval_metric,
+                train_pred_y,
+                y_train,
+                labels,
+                fit_kwargs.get("sample_weight"),
+                fit_kwargs.get("groups"),
+            )
+    else:  # customized metric function
+        val_loss, metric_for_logging = eval_metric(
+            X_val,
+            y_val,
+            estimator,
+            labels,
+            X_train,
+            y_train,
+            weight_val,
+            fit_kwargs.get("sample_weight"),
+            config,
+            groups_val,
+            fit_kwargs.get("groups"),
+        )
+        pred_time = metric_for_logging.get("pred_time", 0)
+        val_pred_y = None
+        # eval_metric may return val_pred_y but not necessarily. Setting None for now.
+    return val_loss, metric_for_logging, pred_time, val_pred_y
```

### Comparing `FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/data_collator.py` & `FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/data_collator.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/trainer.py` & `FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/trainer.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/training_args.py` & `FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/training_args.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/nlp/huggingface/utils.py` & `FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/nlp/utils.py` & `FLAML-2.0.0rc2/flaml/automl/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/spark/__init__.py` & `FLAML-2.0.0rc2/flaml/automl/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/spark/configs.py` & `FLAML-2.0.0rc2/flaml/automl/spark/configs.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/spark/metrics.py` & `FLAML-2.0.0rc2/flaml/automl/spark/metrics.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/spark/utils.py` & `FLAML-2.0.0rc2/flaml/automl/spark/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/automl/state.py` & `FLAML-2.0.0rc2/flaml/automl/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import inspect
+import copy
 import time
 from typing import Any, Optional
 import numpy as np
 from flaml import tune
 from flaml.automl.logger import logger
 from flaml.automl.ml import compute_estimator, train_estimator
-from flaml.automl.task.task import TS_FORECAST
+from flaml.automl.time_series.ts_data import TimeSeriesDataset
 from flaml.automl.spark import psDataFrame, psSeries, DataFrame, Series
 
 
 class SearchState:
     @property
     def search_space(self):
         return self._search_space_domain
@@ -51,35 +52,39 @@
             for name, value in starting_point.items()
             if name != "FLAML_sample_size"
         )
 
     def __init__(
         self,
         learner_class,
-        data_size,
+        data,
         task,
         starting_point=None,
         period=None,
         custom_hp=None,
         max_iter=None,
         budget=None,
     ):
         self.init_eci = learner_class.cost_relative2lgbm() if budget >= 0 else 1
         self._search_space_domain = {}
         self.init_config = None
         self.low_cost_partial_config = {}
         self.cat_hp_cost = {}
-        self.data_size = data_size
+
         self.ls_ever_converged = False
         self.learner_class = learner_class
         self._budget = budget
-        if task in TS_FORECAST:
-            search_space = learner_class.search_space(data_size=data_size, task=task, pred_horizon=period)
+
+        if task.is_ts_forecast():
+            data_size = data.train_data.shape
+            search_space = learner_class.search_space(data=data, task=task, pred_horizon=period)
         else:
+            data_size = data.shape
             search_space = learner_class.search_space(data_size=data_size, task=task)
+        self.data_size = data_size
 
         if custom_hp is not None:
             search_space.update(custom_hp)
 
         if isinstance(starting_point, dict):
             starting_point = AutoMLState.sanitize(starting_point)
             if max_iter > 1 and not self.valid_starting_point(starting_point, search_space):
@@ -207,25 +212,30 @@
 
     def est_retrain_time(self, retrain_sample_size):
         assert self.best_config_sample_size is not None, "need to first get best_config_sample_size"
         return self.time2eval_best * retrain_sample_size / self.best_config_sample_size
 
 
 class AutoMLState:
-    def _prepare_sample_train_data(self, sample_size: int):
+    def prepare_sample_train_data(self, sample_size: int):
         sampled_weight = groups = None
         if sample_size <= self.data_size[0]:
-            if isinstance(self.X_train, (DataFrame, psDataFrame)):
-                sampled_X_train = self.X_train.iloc[:sample_size]
+            if isinstance(self.X_train, TimeSeriesDataset):
+                sampled_X_train = copy.copy(self.X_train)
+                sampled_X_train.train_data = self.X_train.train_data.iloc[-sample_size:]
+                sampled_y_train = None
             else:
-                sampled_X_train = self.X_train[:sample_size]
-            if isinstance(self.y_train, (Series, psSeries)):
-                sampled_y_train = self.y_train.iloc[:sample_size]
-            else:
-                sampled_y_train = self.y_train[:sample_size]
+                if isinstance(self.X_train, (DataFrame, psDataFrame)):
+                    sampled_X_train = self.X_train.iloc[:sample_size]
+                else:
+                    sampled_X_train = self.X_train[:sample_size]
+                if isinstance(self.y_train, (Series, psSeries)):
+                    sampled_y_train = self.y_train.iloc[:sample_size]
+                else:
+                    sampled_y_train = self.y_train[:sample_size]
             weight = self.fit_kwargs.get(
                 "sample_weight"
             )  # NOTE: _prepare_sample_train_data is before kwargs is updated to fit_kwargs_by_estimator
             if weight is not None:
                 sampled_weight = (
                     weight.iloc[:sample_size] if isinstance(weight, (Series, psSeries)) else weight[:sample_size]
                 )
@@ -262,15 +272,15 @@
             estimator
         ).copy()  # NOTE: _compute_with_config_base is after kwargs is updated to fit_kwargs_by_estimator
         (
             sampled_X_train,
             sampled_y_train,
             sampled_weight,
             groups,
-        ) = state._prepare_sample_train_data(sample_size)
+        ) = state.task.prepare_sample_train_data(state, sample_size)
         if sampled_weight is not None:
             weight = this_estimator_kwargs["sample_weight"]
             this_estimator_kwargs["sample_weight"] = sampled_weight
         if groups is not None:
             this_estimator_kwargs["groups"] = groups
         config = config_w_resource.copy()
         if "FLAML_sample_size" in config:
@@ -350,15 +360,15 @@
             estimator
         ).copy()  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
         (
             sampled_X_train,
             sampled_y_train,
             sampled_weight,
             groups,
-        ) = self._prepare_sample_train_data(sample_size)
+        ) = self.task.prepare_sample_train_data(self, sample_size)
         if sampled_weight is not None:
             weight = this_estimator_kwargs[
                 "sample_weight"
             ]  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
             this_estimator_kwargs[
                 "sample_weight"
             ] = sampled_weight  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
```

### Comparing `FLAML-2.0.0rc1/flaml/automl/task/generic_task.py` & `FLAML-2.0.0rc2/flaml/automl/task/generic_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,14 @@
 import logging
 import time
 from typing import List, Optional
 import numpy as np
 from flaml.automl.data import TS_TIMESTAMP_COL, concat
-from flaml.automl.ml import EstimatorSubclass, default_cv_score_agg_func, get_val_loss
-from flaml.automl.model import (
-    XGBoostSklearnEstimator,
-    XGBoostLimitDepthEstimator,
-    RandomForestEstimator,
-    LGBMEstimator,
-    LRL1Classifier,
-    LRL2Classifier,
-    CatBoostEstimator,
-    ExtraTreesEstimator,
-    KNeighborsEstimator,
-    TransformersEstimator,
-    TransformersEstimatorModelSelection,
-    SparkLGBMEstimator,
-)
+from flaml.automl.ml import EstimatorSubclass, get_val_loss, default_cv_score_agg_func
+
 from flaml.automl.task.task import (
     Task,
     get_classification_objective,
     TS_FORECAST,
     TS_FORECASTPANEL,
 )
 from flaml.config import RANDOM_SEED
@@ -54,28 +41,48 @@
 except ImportError:
     pass
 
 logger = logging.getLogger(__name__)
 
 
 class GenericTask(Task):
-    estimators = {
-        "xgboost": XGBoostSklearnEstimator,
-        "xgb_limitdepth": XGBoostLimitDepthEstimator,
-        "rf": RandomForestEstimator,
-        "lgbm": LGBMEstimator,
-        "lrl1": LRL1Classifier,
-        "lrl2": LRL2Classifier,
-        "catboost": CatBoostEstimator,
-        "extra_tree": ExtraTreesEstimator,
-        "kneighbor": KNeighborsEstimator,
-        "transformer": TransformersEstimator,
-        "transformer_ms": TransformersEstimatorModelSelection,
-        "lgbm_spark": SparkLGBMEstimator,
-    }
+    @property
+    def estimators(self):
+        if self._estimators is None:
+            # put this into a function to avoid circular dependency
+            from flaml.automl.model import (
+                XGBoostSklearnEstimator,
+                XGBoostLimitDepthEstimator,
+                RandomForestEstimator,
+                LGBMEstimator,
+                LRL1Classifier,
+                LRL2Classifier,
+                CatBoostEstimator,
+                ExtraTreesEstimator,
+                KNeighborsEstimator,
+                TransformersEstimator,
+                TransformersEstimatorModelSelection,
+                SparkLGBMEstimator,
+            )
+
+            self._estimators = {
+                "xgboost": XGBoostSklearnEstimator,
+                "xgb_limitdepth": XGBoostLimitDepthEstimator,
+                "rf": RandomForestEstimator,
+                "lgbm": LGBMEstimator,
+                "lgbm_spark": SparkLGBMEstimator,
+                "lrl1": LRL1Classifier,
+                "lrl2": LRL2Classifier,
+                "catboost": CatBoostEstimator,
+                "extra_tree": ExtraTreesEstimator,
+                "kneighbor": KNeighborsEstimator,
+                "transformer": TransformersEstimator,
+                "transformer_ms": TransformersEstimatorModelSelection,
+            }
+        return self._estimators
 
     def validate_data(
         self,
         automl,
         state,
         X_train_all,
         y_train_all,
@@ -229,63 +236,15 @@
             state.groups_val = (
                 np.concatenate([[i] * c for i, c in enumerate(groups_val)]) if groups_val is not None else None
             )
         else:
             state.groups_val = groups_val
             state.groups = groups
 
-    @staticmethod
-    def _validate_ts_data(
-        dataframe,
-        y_train_all=None,
-    ):
-        assert (
-            dataframe[dataframe.columns[0]].dtype.name == "datetime64[ns]"
-        ), f"For '{TS_FORECAST}' task, the first column must contain timestamp values."
-        if y_train_all is not None:
-            if isinstance(y_train_all, pd.Series):
-                y_df = pd.DataFrame(y_train_all)
-            elif isinstance(y_train_all, np.ndarray):
-                y_df = pd.DataFrame(y_train_all, columns=["labels"])
-            elif isinstance(y_train_all, (psDataFrame, psSeries)):
-                # TODO: optimize this
-                set_option("compute.ops_on_diff_frames", True)
-                y_df = y_train_all
-            dataframe = dataframe.join(y_df)
-        duplicates = dataframe.duplicated()
-        if isinstance(dataframe, psDataFrame):
-            if duplicates.any():
-                logger.warning("Duplicate timestamp values found in timestamp column.")
-                dataframe = dataframe.drop_duplicates()
-                logger.warning("Removed duplicate rows based on all columns")
-                assert (
-                    dataframe[[dataframe.columns[0]]].duplicated().any() is False
-                ), "Duplicate timestamp values with different values for other columns."
-            ts_series = ps.to_datetime(dataframe[dataframe.columns[0]])
-            inferred_freq = None  # TODO: `pd.infer_freq()` is not implemented yet.
-        else:
-            if any(duplicates):
-                logger.warning(
-                    "Duplicate timestamp values found in timestamp column. "
-                    f"\n{dataframe.loc[duplicates, dataframe][dataframe.columns[0]]}"
-                )
-                dataframe = dataframe.drop_duplicates()
-                logger.warning("Removed duplicate rows based on all columns")
-                assert (
-                    dataframe[[dataframe.columns[0]]].duplicated() is None
-                ), "Duplicate timestamp values with different values for other columns."
-            ts_series = pd.to_datetime(dataframe[dataframe.columns[0]])
-            inferred_freq = pd.infer_freq(ts_series)
-        if inferred_freq is None:
-            logger.warning(
-                "Missing timestamps detected. To avoid error with estimators, set estimator list to ['prophet']. "
-            )
-        if y_train_all is not None:
-            return dataframe.iloc[:, :-1], dataframe.iloc[:, -1]
-        return dataframe
+        automl.data_size_full = len(automl._y_train_all)
 
     @staticmethod
     def _split_pyspark(state, X_train_all, y_train_all, split_ratio, stratify=None):
         # TODO: optimize this
         set_option("compute.ops_on_diff_frames", True)
         if not isinstance(y_train_all, (psDataFrame, psSeries)):
             raise ValueError("y_train_all must be a pyspark.pandas dataframe or series")
@@ -465,93 +424,58 @@
                 X_train_all.reset_index(drop=True, inplace=True)
             if isinstance(y_train_all, pd.Series):
                 y_train_all.reset_index(drop=True, inplace=True)
 
         X_train, y_train = X_train_all, y_train_all
         state.groups_all = state.groups
         if X_val is None and eval_method == "holdout":
-            # if eval_method = holdout, make holdout data
             if split_type == "time":
-                if self.is_ts_forecast():
-                    period = state.fit_kwargs[
-                        "period"
-                    ]  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                    if self.is_ts_forecastpanel():
-                        X_train_all["time_idx"] -= X_train_all["time_idx"].min()
-                        X_train_all["time_idx"] = X_train_all["time_idx"].astype("int")
-                        ids = state.fit_kwargs["group_ids"].copy()
-                        ids.append(TS_TIMESTAMP_COL)
-                        ids.append("time_idx")
-                        y_train_all = (
-                            pd.DataFrame(y_train_all)
-                            if not is_spark_dataframe
-                            else ps.DataFrame(y_train_all)
-                            if isinstance(y_train_all, psSeries)
-                            else y_train_all
-                        )
-                        y_train_all[ids] = X_train_all[ids]
-                        X_train_all = X_train_all.sort_values(ids)
-                        y_train_all = y_train_all.sort_values(ids)
-                        training_cutoff = X_train_all["time_idx"].max() - period
-                        X_train = X_train_all[X_train_all["time_idx"] <= training_cutoff]
-                        y_train = y_train_all[y_train_all["time_idx"] <= training_cutoff].drop(columns=ids)
-                        X_val = X_train_all[X_train_all["time_idx"] > training_cutoff]
-                        y_val = y_train_all[y_train_all["time_idx"] > training_cutoff].drop(columns=ids)
-                    else:
-                        num_samples = X_train_all.shape[0]
-                        assert period < num_samples, f"period={period}>#examples={num_samples}"
-                        split_idx = num_samples - period
-                        X_train = X_train_all[:split_idx]
-                        y_train = y_train_all[:split_idx]
-                        X_val = X_train_all[split_idx:]
-                        y_val = y_train_all[split_idx:]
+                assert not self.is_ts_forecast(), "For a TS forecast task, this code should never be called"
+
+                is_sample_weight = "sample_weight" in state.fit_kwargs
+                if not is_spark_dataframe and is_sample_weight:
+                    (
+                        X_train,
+                        X_val,
+                        y_train,
+                        y_val,
+                        state.fit_kwargs[
+                            "sample_weight"
+                        ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
+                        state.weight_val,
+                    ) = train_test_split(
+                        X_train_all,
+                        y_train_all,
+                        state.fit_kwargs[
+                            "sample_weight"
+                        ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
+                        test_size=split_ratio,
+                        shuffle=False,
+                    )
+                elif not is_spark_dataframe and not is_sample_weight:
+                    X_train, X_val, y_train, y_val = train_test_split(
+                        X_train_all,
+                        y_train_all,
+                        test_size=split_ratio,
+                        shuffle=False,
+                    )
+                elif is_spark_dataframe and is_sample_weight:
+                    (
+                        X_train,
+                        X_val,
+                        y_train,
+                        y_val,
+                        state.fit_kwargs[
+                            "sample_weight"
+                        ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
+                        state.weight_val,
+                    ) = self._split_pyspark(state, X_train_all, y_train_all, split_ratio)
                 else:
-                    is_sample_weight = "sample_weight" in state.fit_kwargs
-                    if not is_spark_dataframe and is_sample_weight:
-                        (
-                            X_train,
-                            X_val,
-                            y_train,
-                            y_val,
-                            state.fit_kwargs[
-                                "sample_weight"
-                            ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                            state.weight_val,
-                        ) = train_test_split(
-                            X_train_all,
-                            y_train_all,
-                            state.fit_kwargs[
-                                "sample_weight"
-                            ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                            test_size=split_ratio,
-                            shuffle=False,
-                        )
-                    elif not is_spark_dataframe and not is_sample_weight:
-                        X_train, X_val, y_train, y_val = train_test_split(
-                            X_train_all,
-                            y_train_all,
-                            test_size=split_ratio,
-                            shuffle=False,
-                        )
-                    elif is_spark_dataframe and is_sample_weight:
-                        (
-                            X_train,
-                            X_val,
-                            y_train,
-                            y_val,
-                            state.fit_kwargs[
-                                "sample_weight"
-                            ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                            state.weight_val,
-                        ) = self._split_pyspark(state, X_train_all, y_train_all, split_ratio)
-                    else:
-                        X_train, X_val, y_train, y_val = self._split_pyspark(
-                            state, X_train_all, y_train_all, split_ratio
-                        )
-            elif split_type == "group":
+                    X_train, X_val, y_train, y_val = self._split_pyspark(state, X_train_all, y_train_all, split_ratio)
+            if split_type == "group":
                 gss = GroupShuffleSplit(n_splits=1, test_size=split_ratio, random_state=RANDOM_SEED)
                 for train_idx, val_idx in gss.split(X_train_all, y_train_all, state.groups_all):
                     if data_is_df:
                         X_train = X_train_all.iloc[train_idx]
                         X_val = X_train_all.iloc[val_idx]
                     else:
                         X_train, X_val = X_train_all[train_idx], X_train_all[val_idx]
@@ -587,14 +511,15 @@
                 X_val = concat(X_first, X_val)
                 y_val = concat(label_set, y_val) if data_is_df else np.concatenate([label_set, y_val])
             elif self.is_regression():
                 X_train, X_val, y_train, y_val = self._train_test_split(
                     state, X_train_all, y_train_all, split_ratio=split_ratio
                 )
         state.data_size = X_train.shape
+        state.data_size_full = len(y_train_all)
         state.X_train, state.y_train = X_train, y_train
         state.X_val, state.y_val = X_val, y_val
         state.X_train_all = X_train_all
         state.y_train_all = y_train_all
         y_train_all_size = y_train_all.size
         if eval_method == "holdout":
             state.kf = None
@@ -632,14 +557,15 @@
                 state.kf = TimeSeriesSplit(n_splits=n_splits, test_size=period)
             elif self.is_ts_forecastpanel():
                 n_groups = len(X_train.groupby(state.fit_kwargs.get("group_ids")).size())
                 period = state.fit_kwargs.get("period")
                 state.kf = TimeSeriesSplit(n_splits=n_splits, test_size=period * n_groups)
             else:
                 state.kf = TimeSeriesSplit(n_splits=n_splits)
+            # state.kf = TimeSeriesSplit(n_splits=n_splits)
         elif isinstance(split_type, str):
             # logger.info("Using RepeatedKFold")
             state.kf = RepeatedKFold(n_splits=n_splits, n_repeats=1, random_state=RANDOM_SEED)
         else:
             # logger.info("Using splitter object")
             state.kf = split_type
         if isinstance(state.kf, (GroupKFold, StratifiedGroupKFold)):
@@ -649,39 +575,26 @@
     def decide_split_type(
         self,
         split_type,
         y_train_all,
         fit_kwargs,
         groups=None,
     ) -> str:
+        assert not self.is_ts_forecast(), "This function should never be called as part of a time-series task."
         if self.name == "classification":
             self.name = get_classification_objective(len_labels(y_train_all))
         if not isinstance(split_type, str):
             assert hasattr(split_type, "split") and hasattr(
                 split_type, "get_n_splits"
             ), "split_type must be a string or a splitter object with split and get_n_splits methods."
             assert (
                 not isinstance(split_type, GroupKFold) or groups is not None
             ), "GroupKFold requires groups to be provided."
             return split_type
 
-        elif self.is_ts_forecast():
-            assert split_type in ["auto", "time"]
-            assert isinstance(
-                fit_kwargs.get("period"),
-                int,  # NOTE: _decide_split_type is before kwargs is updated to fit_kwargs_by_estimator
-            ), f"missing a required integer 'period' for '{TS_FORECAST}' task."
-            if fit_kwargs.get("group_ids"):
-                # TODO (MARK) This will likely not play well with the task class
-                self.name = TS_FORECASTPANEL
-                assert isinstance(
-                    fit_kwargs.get("group_ids"), list
-                ), f"missing a required List[str] 'group_ids' for '{TS_FORECASTPANEL}' task."
-            return "time"
-
         elif self.is_classification():
             assert split_type in ["auto", "stratified", "uniform", "time", "group"]
             return split_type if split_type != "auto" else groups is None and "stratified" or "group"
 
         elif self.is_regression():
             assert split_type in ["auto", "uniform", "time", "group"]
             return split_type if split_type != "auto" else "uniform"
@@ -911,31 +824,31 @@
                     "lgbm",
                     "rf",
                     "xgboost",
                     "extra_tree",
                     "xgb_limitdepth",
                     "lgbm_spark",
                 ]
-            if self.is_ts_forecast():
-                # catboost is removed because it has a `name` parameter, making it incompatible with hcrystalball
-                if "catboost" in estimator_list:
-                    estimator_list.remove("catboost")
-                if self.is_ts_forecastregression():
-                    try:
-                        import prophet
-
-                        estimator_list += [
-                            "prophet",
-                            "arima",
-                            "sarimax",
-                            "holt-winters",
-                        ]
-                    except ImportError:
-                        estimator_list += ["arima", "sarimax", "holt-winters"]
-            elif not self.is_regression():
+            # if self.is_ts_forecast():
+            #     # catboost is removed because it has a `name` parameter, making it incompatible with hcrystalball
+            #     if "catboost" in estimator_list:
+            #         estimator_list.remove("catboost")
+            #     if self.is_ts_forecastregression():
+            #         try:
+            #             import prophet
+            #
+            #             estimator_list += [
+            #                 "prophet",
+            #                 "arima",
+            #                 "sarimax",
+            #                 "holt-winters",
+            #             ]
+            #         except ImportError:
+            #             estimator_list += ["arima", "sarimax", "holt-winters"]
+            if not self.is_regression():
                 estimator_list += ["lrl1"]
 
         estimator_list = [
             est
             for est in estimator_list
             if (est.endswith("_spark") if is_spark_dataframe else not est.endswith("_spark"))
         ]
@@ -957,7 +870,11 @@
             return "log_loss"
         elif self.is_ts_forecast():
             return "mape"
         elif self.is_rank():
             return "ndcg"
         else:
             return "r2"
+
+    @staticmethod
+    def prepare_sample_train_data(automlstate, sample_size):
+        return automlstate.prepare_sample_train_data(sample_size)
```

### Comparing `FLAML-2.0.0rc1/flaml/automl/task/task.py` & `FLAML-2.0.0rc2/flaml/automl/task/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,14 @@
     implemented. The implementation of a Task may optionally use the training data and labels to determine data and task
     specific details, such as in determining if a problem is single-label or multi-label.
 
     FLAML evaluates at runtime how to behave exactly, relying on the task instance to provide implementations of
     operations which vary between tasks.
     """
 
-    estimators = {}
-
     def __init__(
         self,
         task_name: str,
         X_train: Optional[Union[np.ndarray, DataFrame, psDataFrame]] = None,
         y_train: Optional[Union[np.ndarray, DataFrame, Series, psSeries]] = None,
     ):
         """Constructor.
@@ -84,14 +82,15 @@
                 types of sub-task.
             X_train: Optional. Some Task types may use the data shape or features to determine details of their usage,
                 such as in binary vs multilabel classification.
             y_train: Optional. Some Task types may use the data shape or features to determine details of their usage,
                 such as in binary vs multilabel classification.
         """
         self.name = task_name
+        self._estimators = None
 
     def __str__(self) -> str:
         """Name of this task type."""
         return self.name
 
     @abstractmethod
     def evaluate_model_CV(
@@ -322,28 +321,27 @@
     def is_regression(self) -> bool:
         return self.name in REGRESSION
 
     def __eq__(self, other: str) -> bool:
         """For backward compatibility with all the string comparisons to task"""
         return self.name == other
 
-    @classmethod
-    def estimator_class_from_str(cls, estimator_name: str) -> "flaml.automl.ml.BaseEstimator":
+    def estimator_class_from_str(self, estimator_name: str) -> "flaml.automl.ml.BaseEstimator":
         """Determine the estimator class corresponding to the provided name.
 
         Args:
             estimator_name: Name of the desired estimator.
 
         Returns:
             The estimator class corresponding to the provided name.
 
         Raises:
             ValueError: The provided estimator_name has not been registered for this task type.
         """
-        if estimator_name in cls.estimators:
-            return cls.estimators[estimator_name]
+        if estimator_name in self.estimators:
+            return self.estimators[estimator_name]
         else:
             raise ValueError(
                 f"{estimator_name} is not a built-in learner for this task type, "
-                f"only {list(cls.estimators.keys())} are supported."
+                f"only {list(self.estimators.keys())} are supported."
                 "Please use AutoML.add_learner() to add a customized learner."
             )
```

### Comparing `FLAML-2.0.0rc1/flaml/automl/training_log.py` & `FLAML-2.0.0rc2/flaml/automl/training_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         sample_size: int,
     ):
         self.record_id = record_id
         self.iter_per_learner = iter_per_learner
         self.logged_metric = logged_metric
         self.trial_time = trial_time
         self.wall_clock_time = wall_clock_time
-        self.validation_loss = validation_loss
+        self.validation_loss = float(validation_loss)
         self.config = config
         self.learner = learner
         self.sample_size = sample_size
 
     def dump(self, fp: IO[str]):
         d = vars(self)
         return json.dump(d, fp)
```

### Comparing `FLAML-2.0.0rc1/flaml/default/all/binary.json` & `FLAML-2.0.0rc2/flaml/default/all/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/all/multiclass.json` & `FLAML-2.0.0rc2/flaml/default/all/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/all/regression.json` & `FLAML-2.0.0rc2/flaml/default/all/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/estimator.py` & `FLAML-2.0.0rc2/flaml/default/estimator.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/extra_tree/binary.json` & `FLAML-2.0.0rc2/flaml/default/extra_tree/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/extra_tree/multiclass.json` & `FLAML-2.0.0rc2/flaml/default/extra_tree/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/extra_tree/regression.json` & `FLAML-2.0.0rc2/flaml/default/extra_tree/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/greedy.py` & `FLAML-2.0.0rc2/flaml/default/greedy.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/lgbm/binary.json` & `FLAML-2.0.0rc2/flaml/default/lgbm/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/lgbm/multiclass.json` & `FLAML-2.0.0rc2/flaml/default/lgbm/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/lgbm/regression.json` & `FLAML-2.0.0rc2/flaml/default/lgbm/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/portfolio.py` & `FLAML-2.0.0rc2/flaml/default/portfolio.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/regret.py` & `FLAML-2.0.0rc2/flaml/default/regret.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/rf/binary.json` & `FLAML-2.0.0rc2/flaml/default/rf/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/rf/multiclass.json` & `FLAML-2.0.0rc2/flaml/default/rf/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/rf/regression.json` & `FLAML-2.0.0rc2/flaml/default/rf/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/suggest.py` & `FLAML-2.0.0rc2/flaml/default/suggest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import logging
 import pathlib
 import json
 from flaml.automl.data import DataTransformer
 from flaml.automl.task.task import CLASSIFICATION, get_classification_objective
 from flaml.automl.task.generic_task import len_labels
-from flaml.automl.ml import get_estimator_class
+from flaml.automl.task.factory import task_factory
 from flaml.version import __version__
 
 try:
     from sklearn.neighbors import NearestNeighbors
 except ImportError:
     pass
 
@@ -158,17 +158,18 @@
 
     Returns:
         hyperparams: A dict of the hyperparameter configurations.
         estiamtor_class: A class of the underlying estimator, e.g., lightgbm.LGBMClassifier.
     """
     config = suggest_config(task, X, y, estimator_or_predictor, location=location, k=1)[0]
     estimator = config["class"]
-    model_class = get_estimator_class(task, estimator)
+    task = task_factory(task)
+    model_class = task.estimator_class_from_str(estimator)
     hyperparams = config["hyperparameters"]
-    model = model_class(task=task, **hyperparams)
+    model = model_class(task=task.name, **hyperparams)
     estimator_class = model.estimator_class
     hyperparams = hyperparams and model.params
     return hyperparams, estimator_class
 
 
 class AutoMLTransformer:
     def __init__(self, model, data_transformer):
@@ -242,15 +243,15 @@
             X,
             y,
             estimator_list=["xgb_limitdepth", "xgboost"],
             location=location,
         )
     config = suggest_config(task, X, y, estimator_or_predictor, location=location, k=1)[0]
     estimator = config["class"]
-    model_class = get_estimator_class(task, estimator)
+    model_class = task_factory(task).estimator_class_from_str(estimator)
     hyperparams = config["hyperparameters"]
     model = model_class(task=task, **hyperparams)
     if model.estimator_class is None:
         return hyperparams, model_class, X, y, None, None
     else:
         estimator_class = model.estimator_class
         X = model._preprocess(X)
```

### Comparing `FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/binary.json` & `FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/multiclass.json` & `FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/xgb_limitdepth/regression.json` & `FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/xgboost/binary.json` & `FLAML-2.0.0rc2/flaml/default/xgboost/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/xgboost/multiclass.json` & `FLAML-2.0.0rc2/flaml/default/xgboost/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/default/xgboost/regression.json` & `FLAML-2.0.0rc2/flaml/default/xgboost/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/onlineml/autovw.py` & `FLAML-2.0.0rc2/flaml/onlineml/autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/onlineml/trial.py` & `FLAML-2.0.0rc2/flaml/onlineml/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/onlineml/trial_runner.py` & `FLAML-2.0.0rc2/flaml/onlineml/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/__init__.py` & `FLAML-2.0.0rc2/flaml/tune/__init__.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/analysis.py` & `FLAML-2.0.0rc2/flaml/tune/analysis.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/result.py` & `FLAML-2.0.0rc2/flaml/tune/result.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/sample.py` & `FLAML-2.0.0rc2/flaml/tune/sample.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/scheduler/online_scheduler.py` & `FLAML-2.0.0rc2/flaml/tune/scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/scheduler/trial_scheduler.py` & `FLAML-2.0.0rc2/flaml/tune/scheduler/trial_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/searcher/blendsearch.py` & `FLAML-2.0.0rc2/flaml/tune/searcher/blendsearch.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/searcher/cfo_cat.py` & `FLAML-2.0.0rc2/flaml/tune/searcher/cfo_cat.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/searcher/flow2.py` & `FLAML-2.0.0rc2/flaml/tune/searcher/flow2.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/searcher/online_searcher.py` & `FLAML-2.0.0rc2/flaml/tune/searcher/online_searcher.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/searcher/search_thread.py` & `FLAML-2.0.0rc2/flaml/tune/searcher/search_thread.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/searcher/suggestion.py` & `FLAML-2.0.0rc2/flaml/tune/searcher/suggestion.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/searcher/variant_generator.py` & `FLAML-2.0.0rc2/flaml/tune/searcher/variant_generator.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/space.py` & `FLAML-2.0.0rc2/flaml/tune/space.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/spark/utils.py` & `FLAML-2.0.0rc2/flaml/tune/spark/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/trial.py` & `FLAML-2.0.0rc2/flaml/tune/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/trial_runner.py` & `FLAML-2.0.0rc2/flaml/tune/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/tune.py` & `FLAML-2.0.0rc2/flaml/tune/tune.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/flaml/tune/utils.py` & `FLAML-2.0.0rc2/flaml/tune/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/pyproject.toml` & `FLAML-2.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/setup.py` & `FLAML-2.0.0rc2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,16 +77,20 @@
             "mlflow",
             "pyspark>=3.2.0",
             "joblibspark>=0.5.0",
             "nbconvert",
             "nbformat",
             "ipykernel",
             "pytorch-lightning<1.9.1",  # test_forecast_panel
+            "tensorboardX==2.6",  # test_forecast_panel
             "requests<2.29.0",  # https://github.com/docker/docker-py/issues/3113
             "packaging",
+            "pydantic",
+            "sympy",
+            "wolframalpha",
         ],
         "catboost": ["catboost>=0.26"],
         "blendsearch": ["optuna==2.8.0"],
         "ray": [
             "ray[tune]~=1.13",
         ],
         "azureml": [
@@ -121,18 +125,21 @@
         ],
         "forecast": [
             "holidays<0.14",  # to prevent installation error for prophet
             "prophet>=1.0.1",
             "statsmodels>=0.12.2",
             "hcrystalball==0.1.10",
             "pytorch-forecasting>=0.9.0",
+            "pytorch-lightning==1.9.0",
+            "tensorboardX==2.6",
         ],
-        "benchmark": ["catboost>=0.26", "psutil==5.8.0", "xgboost==1.3.3"],
-        "openai": ["openai==0.27.4", "diskcache"],
-        "autogen": ["openai==0.27.4", "diskcache", "docker"],
+        "benchmark": ["catboost>=0.26", "psutil==5.8.0", "xgboost==1.3.3", "pandas==1.1.4"],
+        "openai": ["openai==0.27.8", "diskcache"],
+        "autogen": ["openai==0.27.8", "diskcache", "docker"],
+        "mathchat": ["openai==0.27.8", "diskcache", "docker", "sympy", "pydantic", "wolframalpha"],
         "synapse": [
             "joblibspark>=0.5.0",
             "optuna==2.8.0",
             "pyspark>=3.2.0",
         ],
         "autozero": ["scikit-learn", "pandas", "packaging"],
     },
```

### Comparing `FLAML-2.0.0rc1/test/test_autovw.py` & `FLAML-2.0.0rc2/test/test_autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/test/test_conda_distribution.py` & `FLAML-2.0.0rc2/test/test_conda_distribution.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/test/test_gpu.py` & `FLAML-2.0.0rc2/test/test_gpu.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc1/test/test_model.py` & `FLAML-2.0.0rc2/test/test_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,18 +6,16 @@
     KNeighborsEstimator,
     LRL2Classifier,
     BaseEstimator,
     LGBMEstimator,
     CatBoostEstimator,
     XGBoostEstimator,
     RandomForestEstimator,
-    Prophet,
-    ARIMA,
-    LGBM_TS,
 )
+from flaml.automl.time_series import Prophet, ARIMA, LGBM_TS, TimeSeriesDataset
 
 
 def test_lrl2():
     BaseEstimator.search_space(1, "")
     X, y = make_classification(100000, 1000)
     print("start")
     lr = LRL2Classifier()
@@ -97,39 +95,44 @@
     try:
         prophet.predict(4)
     except ValueError:
         # predict() with steps is only supported for arima/sarimax.
         pass
     prophet.predict(X)
 
-    arima = ARIMA()
+    # What's the point of callin ARIMA without parameters, or calling predict before fit?
+    arima = ARIMA(p=1, q=1, d=0)
     arima.predict(X)
     arima._model = False
     try:
         arima.predict(X)
     except ValueError:
         # X_test needs to be either a pandas Dataframe with dates as the first column or an int number of periods for predict().
         pass
-
-    lgbm = LGBM_TS(optimize_for_horizon=True, lags=1)
+    lgbm = LGBM_TS(lags=1)
     X = DataFrame(
         {
             "A": [
-                datetime(1900, 2, 3),
+                datetime(1900, 3, 1),
+                datetime(1900, 3, 2),
+                datetime(1900, 3, 3),
                 datetime(1900, 3, 4),
                 datetime(1900, 3, 4),
                 datetime(1900, 3, 4),
-                datetime(1900, 7, 2),
-                datetime(1900, 8, 9),
+                datetime(1900, 3, 5),
+                datetime(1900, 3, 6),
             ],
         }
     )
-    y = np.array([0, 1, 0, 1, 0, 0])
+    y = np.array([0, 1, 0, 1, 1, 1, 0, 0])
     lgbm.predict(X[:2])
-    lgbm.fit(X, y, period=2)
+    df = X.copy()
+    df["y"] = y
+    tsds = TimeSeriesDataset(df, time_col="A", target_names="y")
+    lgbm.fit(tsds, period=2)
     lgbm.predict(X[:2])
     print(lgbm.feature_names_in_)
     print(lgbm.feature_importances_)
 
 
 if __name__ == "__main__":
     test_prep()
```

