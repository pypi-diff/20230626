# Comparing `tmp/ask-smapi-model-1.9.1.tar.gz` & `tmp/ask-smapi-model-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ask-smapi-model-1.9.1.tar", last modified: Mon May 10 23:34:52 2021, max compression
+gzip compressed data, was "dist/ask-smapi-model-1.9.2.tar", last modified: Thu Jun 10 19:48:20 2021, max compression
```

## Comparing `ask-smapi-model-1.9.1.tar` & `ask-smapi-model-1.9.2.tar`

### file list

```diff
@@ -1,836 +1,835 @@
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6445 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/CHANGELOG.rst
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      142 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/requirements.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       67 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/setup.cfg
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      124 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/MANIFEST.in
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      974 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/README.rst
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1748 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/stage_type.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1076 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3938 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/validations_api_response_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3153 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/validations_api_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2005 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/validations_api_response_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1929 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/response_validation_importance.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1905 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/response_validation_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4526 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/validations_api_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5662 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/response_validation.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1817 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/agreement_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1746 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_stage_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3212 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/update_skill_with_package_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3522 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_feature.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6045 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2193 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/build_step_name.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3214 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/alexa_response_content.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4281 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/simulations_api_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3262 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/input.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4400 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/simulations_api_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1297 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4623 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/simulation_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1999 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/simulations_api_response_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3536 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/alexa_execution_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3522 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/device.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3606 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/invocation_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3960 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/alexa_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3465 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/session.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3584 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/metrics.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3288 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/invocation_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4765 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/invocation.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1847 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/session_mode.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1996 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/response_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2760 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3387 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/create_rollback_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      811 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1865 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/skill_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1807 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/stage_for_metric.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2361 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/metric.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1873 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/period.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4454 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/get_metric_data_response.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/private/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/private/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      824 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/private/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1829 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/private/accept_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3992 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/private/private_distribution_account.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4636 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/private/list_private_distribution_accounts_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4592 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/ssl_certificate_payload.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5431 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_status_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4389 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/build_step.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7245 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3292 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result_output.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3752 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/error_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3786 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/audio_asset.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3891 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/pagination_context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2046 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7040 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/annotation_with_audio_asset.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1687 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6210 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/annotation.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4585 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/list_asr_evaluations_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4280 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_metadata_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3557 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/skill.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7085 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_metadata.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3210 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/post_asr_evaluations_response_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7098 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/get_asr_evaluation_status_response_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5466 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1945 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3745 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/post_asr_evaluations_request_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4403 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/get_asr_evaluations_results_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3304 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/metrics.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3368 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/create_asr_annotation_set_request_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3786 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/audio_asset.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3891 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/pagination_context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7714 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_with_audio_asset.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5254 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_set_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1560 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7444 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/annotation.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4372 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/list_asr_annotation_sets_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3929 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/update_asr_annotation_set_contents_payload.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3180 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/create_asr_annotation_set_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4923 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_set_metadata.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5379 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/get_asr_annotation_set_annotations_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5088 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/get_asr_annotation_sets_properties_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3388 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/update_asr_annotation_set_properties_request_object.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3995 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication/skill_publication_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1923 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication/skill_publication_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3776 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication/publish_skill_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      799 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3544 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4528 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_version.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5010 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/standardized_error.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4286 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/distribution_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5549 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/review_tracking_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1178 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5647 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/certification_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5352 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/certification_summary.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4839 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/review_tracking_info_summary.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6036 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/list_certifications_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2049 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/certification_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3825 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/publication_failure.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4882 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/estimation_update.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3922 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/certification_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4853 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest_last_update_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    16940 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_details.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4342 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3989 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/submit_skill_for_certification_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3878 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/version_submission.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3531 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/connections_payload.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3648 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/extension_initialization_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1851 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/flash_briefing_update_frequency.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4009 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_localized_privacy_and_compliance.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3248 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/target_runtime_device.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      855 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3759 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/connection.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2833 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/suppressed_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4103 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/target_runtime.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1725 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/target_runtime_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3180 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_feature.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3454 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/dialog_delegation_strategy.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4097 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_endpoint.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3582 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_web_player_feature.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3279 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/authorized_client_lwa_application.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3462 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/extension_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3761 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/voice_profile_feature.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1927 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/ssl_certificate_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1880 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/viewport_mode.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5702 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_events.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3665 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1793 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/flash_briefing_content_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8285 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_privacy_and_compliance.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3614 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/authorized_client_lwa.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2828 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/interface_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7309 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_apis.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2066 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/distribution_mode.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4074 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_connections.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3732 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_capability.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1988 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/display_interface_apml_version.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3436 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/event_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3621 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/up_channel_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3017 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/house_hold_list.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4139 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_interfaces.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5034 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/permission_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5911 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3490 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/health_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3591 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/region.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3437 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_envelope.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6369 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3734 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/supported_controls.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3162 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/app_link_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8255 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_apis.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3302 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/lambda_endpoint.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5602 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/viewport_specification.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3884 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/catalog_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3172 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_alias.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4502 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_feature.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3571 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_content_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3858 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/friendly_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5357 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/manifest_gadget_support.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4451 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/source_language_for_locales.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4229 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/dialog_manager.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3936 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_fire_tv_catalog_ingestion.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6041 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/distribution_countries.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    10166 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_publishing_information.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1859 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/gadget_support_requirement.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3165 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_app_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8861 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_apis.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_dialog_management/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3458 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_dialog_management/session_start_delegation_strategy.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_dialog_management/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      696 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_dialog_management/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2334 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/flash_briefing_genre.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4775 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/linked_application.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3970 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/app_link.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7699 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/localized_flash_briefing_info_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3170 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_wordmark.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3909 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/knowledge_apis.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6284 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_apis_locale.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4558 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3173 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/game_engine_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4642 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/dialog_management.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3443 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/gadget_controller_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2023 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/smart_home_protocol.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7060 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_localized_publishing_information.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1729 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/version.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3118 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5692 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_apis.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3531 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/lambda_region.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3740 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_country_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8134 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1750 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/manifest_version.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3879 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/flash_briefing_apis.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3608 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/amazon_conversations_dialog_manager.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3395 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/permission_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5783 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/automatic_distribution.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3361 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/authorized_client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    30273 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/event_name_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3159 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/audio_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5580 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/smart_home_apis.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1849 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface_request_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3171 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/app_link_v2_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5083 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_for_business_apis.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4332 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_region.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3787 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/localized_knowledge_information.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1806 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/viewport_shape.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4178 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_presentation_apl_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6130 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/display_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1820 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/catalog_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1864 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_content_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3374 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/localized_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3512 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/authorized_client_lwa_application_android.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4146 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_localized_information_dialog_management.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1993 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/display_interface_template_version.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3205 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/event_publications.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4675 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/demand_response_apis.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3934 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_localized_information.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1732 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_prompt_name_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3718 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_prompt_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3532 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_task.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1823 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/supported_controls_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5305 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/localized_music_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3135 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_catalog_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4409 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/localized_flash_briefing_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3372 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_presentation_html_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5077 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model_last_update_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4378 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/image_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2852 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_failure_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2074 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/reason.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5333 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/hosted_skill_deployment_status_last_update_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3058 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_request_status.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5002 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4803 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/profile_nlu_selected_intent.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1985 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/confirmation_status_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3662 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/profile_nlu_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1888 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/dialog_act_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1376 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4449 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/slot_resolutions.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4643 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/slot.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2486 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_status_code.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5539 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/profile_nlu_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4468 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/multi_turn.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3854 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_value_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4199 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/dialog_act.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3779 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4557 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/intent.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6969 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_summary.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2032 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication_method.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3682 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/image_dimension.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4373 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/create_skill_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4506 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/list_skill_versions_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3705 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/image_size.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3915 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/hosted_skill_provisioning_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2180 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/rollback_request_status_types.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3465 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/confidence.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6532 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/intent_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1944 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/intent_request_locales.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1959 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/locale_in_query.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1863 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/publication_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1237 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3164 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/slot.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2123 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/intent_confidence_bin.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6128 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/intent_requests.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2166 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/sort_field_for_intent_request_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2060 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/confidence_bin.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3457 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/dialog_act.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2549 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/dialog_act_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2055 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/interaction_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4410 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/intent.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3961 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/import_response_skill.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4797 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/instance.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3724 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_messaging_credentials.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3152 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/version_submission_status.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/resource_schema/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/resource_schema/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      686 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/resource_schema/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3749 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/resource_schema/get_resource_schema_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3995 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/hosted_skill_deployment_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3464 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/create_rollback_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1814 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3207 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/regional_ssl_certificate.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4286 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_resource_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4938 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/import_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3703 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/withdraw_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3782 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/export_response_skill.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3719 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/build_details.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4504 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_interaction_model_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3533 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/create_skill_with_package_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3225 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/create_skill_response.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4933 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/beta_test.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      771 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2897 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/update_beta_test_response.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4858 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/tester_with_details.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      837 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4077 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/list_testers_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3161 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/tester.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1840 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/invitation_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3505 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/testers_list.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1871 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3289 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/test_body.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1862 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/overwrite_mode.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1746 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/format.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3668 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/upload_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3791 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_credentials.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4412 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/account_linking_platform_authorization_url.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    11049 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/account_linking_request_payload.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     9139 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/account_linking_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1876 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/access_token_scheme_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3861 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/account_linking_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1060 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1806 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/account_linking_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1835 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/platform_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2062 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_summary_apis.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3718 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_failure_reason.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3920 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/export_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4517 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4869 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/list_nlu_evaluations_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3375 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/pagination_context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2213 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5496 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_results_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1747 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/results_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3284 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/results.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2486 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_status_code.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4274 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/paged_results_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3112 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/expected_intent_slots_props.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3815 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/evaluate_nlu_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3407 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_response_links.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3565 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/actual.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4920 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/test_case.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5228 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/evaluation.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4972 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1805 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3776 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/paged_results_response_pagination_context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4961 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/evaluation_entity.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3627 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/links.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3575 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/inputs.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3653 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/expected.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1970 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/confirmation_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3811 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/evaluation_inputs.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4048 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/paged_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3148 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/evaluate_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4649 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3787 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/expected_intent.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4267 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/resolutions.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4599 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/slots_props.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5776 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3598 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_value.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3289 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/source.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4355 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/intent.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2933 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/update_nlu_annotation_set_annotations_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4794 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/list_nlu_annotation_sets_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3180 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/create_nlu_annotation_set_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3375 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/pagination_context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1315 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4513 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/get_nlu_annotation_set_properties_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3510 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/create_nlu_annotation_set_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4353 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/annotation_set_entity.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3627 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/links.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3234 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/update_nlu_annotation_set_properties_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4808 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/annotation_set.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6597 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/list_skill_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3474 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/hosted_skill_deployment_details.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3846 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/dialog_prompts.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3756 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/prompt_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2268 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3824 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/has_entity_resolution_match.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3420 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/multiple_values_config.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3245 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3530 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_input.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1132 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4287 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_definition_output.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4844 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/list_catalog_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3560 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/update_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1866 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_status_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4532 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/last_update_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3534 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_entity.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4343 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_item.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3747 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3880 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/definition_data.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3890 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_less_than.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3911 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_not_in_set.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5979 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/dialog_intents.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4574 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/interaction_model_schema.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3501 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/value_catalog.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3882 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_greater_than.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3757 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/fallback_intent_sensitivity.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3944 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_greater_than_or_equal_to.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2085 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/fallback_intent_sensitivity_level.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4864 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/slot_definition.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4162 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/interaction_model_data.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3876 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/inline_value_supplier.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4964 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/execution.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4457 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/trigger.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4909 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/catalog_auto_refresh.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4831 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/list_job_definitions_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6370 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/reference_version_update.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3159 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/job_api_pagination_context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1828 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3784 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/job_error_details.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3581 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/update_job_status_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3277 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/create_job_definition_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1811 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3623 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/validation_errors.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4755 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/get_executions_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3449 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/catalog.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4657 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/resource_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5274 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4142 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition_metadata.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3918 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/interaction_model.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4189 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/scheduled.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3957 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/create_job_definition_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3341 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/referenced_resource_jobs_complete.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3533 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/slot_type_reference.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3506 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/dynamic_update_error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3896 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/execution_metadata.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3828 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/dialog_intents_prompts.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3926 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_less_than_or_equal_to.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3901 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog_value_supplier.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4737 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/slot_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3897 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_configuration.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3729 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_value.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3891 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_in_set.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6054 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_in_duration.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6074 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_not_in_duration.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4150 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflicts_response_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3864 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/pagination_context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3958 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5000 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflicts_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1142 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3367 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_intent_slot.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4118 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflict_detection_job_status_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3905 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_intent.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1870 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_detection_job_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4044 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/paged_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4509 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/value_supplier.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1821 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/prompt_items_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5091 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/language_model.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5933 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/dialog_slot_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4739 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/dialog.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4043 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/prompt.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4069 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/version_data_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3628 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/version_data.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1119 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4514 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/list_slot_type_version_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3678 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_update.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3352 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_update_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3618 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/value_supplier_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4649 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_data_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3988 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_item.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3742 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_data.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3662 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3442 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1293 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3466 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/warning.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4284 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_item.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3716 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3358 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_update_definition.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3953 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_definition_output.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3698 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/update_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5135 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/last_update_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1868 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_status_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3544 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_input.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4323 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/list_slot_type_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3186 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_response_entity.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3931 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/definition_data.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3467 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_value_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6483 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/slot_validation.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5299 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/list_catalog_entity_versions_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4735 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/list_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3881 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/version_data.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1163 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4317 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/catalog_entity_version.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3365 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/value_schema_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3765 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/value_schema.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4782 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/catalog_values.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3274 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/links.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3330 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/catalog_update.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4189 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/catalog_version_data.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4249 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/version_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3513 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/input_source.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1986 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/delegation_strategy_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4332 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/intent.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3956 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_endpoint.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4667 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4158 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/alexa_hosted_config.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1750 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3862 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1885 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_runtime.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3989 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1527 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4194 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1724 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3584 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_metadata.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1841 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_region.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3974 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials_list.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3637 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3628 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosting_configuration.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1982 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4050 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1847 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/action.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1909 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/invocation_response_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1783 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/end_point_regions.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1085 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4190 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/invoke_skill_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4146 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/invocation_response_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3224 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3584 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/metrics.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4132 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/invoke_skill_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3360 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/skill_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3542 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4705 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/skill_execution_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5072 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/rollback_request_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4563 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/hosted_skill_provisioning_last_update_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1749 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/image_size_unit.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1876 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_data_types.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5268 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/resource_import_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1949 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_resources_enum.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3693 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/bad_request_error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3906 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      811 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3648 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/presigned_upload_part_items.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4154 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/pre_signed_url.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6088 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/get_content_upload_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2975 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/catalog_upload_base.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1914 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/file_upload_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1164 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4191 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/content_upload_file_summary.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3390 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/location.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1866 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/upload_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1877 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/ingestion_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5154 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/upload_ingestion_step.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3368 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/pre_signed_url_item.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1788 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/ingestion_step_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      840 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3613 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/create_content_upload_url_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4206 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/create_content_upload_url_response.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3402 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3251 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/requester_filter.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2071 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/sort_field.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1351 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3507 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/resource.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4986 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/request_pagination_context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3800 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/resource_filter.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1970 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/sort_direction.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7185 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/request_filters.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3646 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/operation_filter.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6113 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/audit_log.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5675 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/audit_logs_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3372 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/client_filter.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1882 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/resource_type_enum.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3369 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/requester.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3441 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/response_pagination_context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4908 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/audit_logs_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3382 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/operation.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4627 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/evaluate_sh_capability_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2893 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_capability_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5300 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/evaluation_object.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1740 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/stage.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3139 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/endpoint.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3420 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/pagination_context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3070 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/capability_test_plan.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1999 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3157 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/pagination_context_token.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2288 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_capability_error_code.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3274 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/list_sh_test_plan_item.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4208 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_evaluation_results_metric.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4402 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/list_sh_capability_evaluations_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6220 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/get_sh_capability_evaluation_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3739 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_capability_error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2895 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_capability_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4963 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/evaluate_sh_capability_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2887 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_capability_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7778 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/test_case_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1788 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/test_case_result_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3588 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/paged_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1837 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/evaluation_entity_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4445 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/list_sh_capability_test_plans_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4487 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/get_sh_capability_evaluation_results_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3062 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/link.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1825 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/editable_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3728 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/in_skill_product_summary_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3710 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/update_in_skill_product_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1849 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/product_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1804 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/currency.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4683 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/associated_skill_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3597 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/tax_information.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4151 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/summary_price_listing.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7484 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/localized_publishing_information.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2400 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1976 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/promotable_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8361 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/in_skill_product_definition.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4053 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/create_in_skill_product_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4508 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/subscription_information.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1853 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/subscription_payment_frequency.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3265 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/product_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6041 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/distribution_countries.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     9007 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/in_skill_product_summary.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2159 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/tax_information_category.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1924 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4003 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/price_listing.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2081 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/purchasable_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3827 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/privacy_and_compliance.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3504 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/localized_privacy_and_compliance.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4366 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/summary_marketplace_pricing.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4294 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/marketplace_pricing.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3741 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/list_in_skill_product_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4408 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/custom_product_prompts.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3294 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/isp_summary_links.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4643 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/list_in_skill_product.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3794 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/in_skill_product_definition_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6042 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/publishing_information.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1791 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/stage_v2_type.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/vendor_management/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/vendor_management/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      674 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/vendor_management/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3779 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/vendor_management/vendor.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3399 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/vendor_management/vendors.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3627 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v1/links.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5004 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3208 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/alexa_response_content.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1985 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/confirmation_status_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4279 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/simulations_api_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3262 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/input.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4400 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/simulations_api_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1661 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4449 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/slot_resolutions.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4641 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/slot.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4711 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/simulation_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2486 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_status_code.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1999 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/simulations_api_response_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3854 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_value_items.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4140 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/alexa_execution_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3522 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/device.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3960 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/alexa_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3465 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/session.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3779 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3415 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/skill_execution_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1847 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/session_mode.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4557 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/intent.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      784 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3606 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocation_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3584 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/metrics.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3288 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocation_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4621 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocation.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1909 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/invocation_response_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4196 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/invocations_api_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1816 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/end_point_regions.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      955 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3862 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/invocation_response_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3360 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/skill_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4138 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/invocations_api_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3693 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/bad_request_error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3644 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      690 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v2/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      994 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/__version__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/services/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/services/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/services/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/services/skill_management/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/services/skill_management/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      692 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/services/skill_management/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)   850764 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/ask_smapi_model/services/skill_management/skill_management_service_client.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3691 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/bad_request_error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3644 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      690 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      671 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4522 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/skill_review_publish.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3704 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/skill_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1183 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3513 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/actor_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1811 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/request_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3501 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/subscription_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5901 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/base_schema.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4805 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/skill_review_event_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4200 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/skill_review_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5200 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/skill_event_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3883 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/interaction_model_attributes.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5540 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/manifest_update.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      815 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5528 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/interaction_model_update.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5870 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/skill_publish.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5414 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/skill_certification.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5479 2021-05-10 23:33:21.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/interaction_model_event_attributes.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4477 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/list_catalogs_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5733 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/catalog_summary.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3607 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/create_content_upload_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6179 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/get_content_upload_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3497 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/presigned_upload_part.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1914 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/file_upload_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1409 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4029 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/content_upload_file_summary.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4493 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/list_uploads_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1863 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/upload_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3665 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/complete_upload_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4657 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/content_upload_summary.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1877 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/ingestion_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5112 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/upload_ingestion_step.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3368 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/pre_signed_url_item.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6508 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/create_content_upload_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1788 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/ingestion_step_name.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      898 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2284 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/catalog_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5733 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/catalog_details.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2576 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/catalog_usage.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4468 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/create_catalog_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4884 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/subscription_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      946 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3811 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/update_subscription_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4344 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/list_subscriptions_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4888 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/subscription_summary.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4087 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/event.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4539 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/create_subscription_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3897 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/endpoint.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3697 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/update_subscriber_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3622 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/endpoint_aws_authorization.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/py.typed
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1170 2021-05-10 23:33:35.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1906 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/subscriber_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4134 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/subscriber_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4241 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/endpoint_authorization.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3978 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/create_subscriber_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1794 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/endpoint_authorization_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5010 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/subscriber_summary.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4300 2021-05-10 23:33:20.000000 ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/list_subscribers_response.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/ask_smapi_model.egg-info/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    45851 2021-05-10 23:34:51.000000 ask-smapi-model-1.9.1/ask_smapi_model.egg-info/SOURCES.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2021-05-10 23:34:51.000000 ask-smapi-model-1.9.1/ask_smapi_model.egg-info/dependency_links.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       16 2021-05-10 23:34:51.000000 ask-smapi-model-1.9.1/ask_smapi_model.egg-info/top_level.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2021-05-10 23:34:51.000000 ask-smapi-model-1.9.1/ask_smapi_model.egg-info/not-zip-safe
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     9901 2021-05-10 23:34:51.000000 ask-smapi-model-1.9.1/ask_smapi_model.egg-info/PKG-INFO
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       79 2021-05-10 23:34:51.000000 ask-smapi-model-1.9.1/ask_smapi_model.egg-info/requires.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    11357 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/LICENSE
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     9901 2021-05-10 23:34:52.000000 ask-smapi-model-1.9.1/PKG-INFO
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2162 2021-05-10 23:33:22.000000 ask-smapi-model-1.9.1/setup.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6539 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/CHANGELOG.rst
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      142 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/requirements.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       67 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/setup.cfg
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      124 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/MANIFEST.in
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      974 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/README.rst
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1748 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/stage_type.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1076 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3938 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/validations_api_response_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3153 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/validations_api_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2005 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/validations_api_response_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1929 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/response_validation_importance.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1905 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/response_validation_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4526 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/validations_api_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5662 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/response_validation.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1817 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/agreement_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1746 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_stage_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3212 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/update_skill_with_package_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3522 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_feature.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6045 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2193 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/build_step_name.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3214 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/alexa_response_content.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4281 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/simulations_api_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3262 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/input.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4400 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/simulations_api_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1297 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4623 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/simulation_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1999 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/simulations_api_response_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3536 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/alexa_execution_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3522 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/device.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3606 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/invocation_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3960 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/alexa_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3465 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/session.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3584 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/metrics.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3288 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/invocation_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4765 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/invocation.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1847 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/session_mode.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1996 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/response_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2760 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3387 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/create_rollback_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      811 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1865 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/skill_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1807 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/stage_for_metric.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2361 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/metric.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1873 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/period.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4454 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/get_metric_data_response.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/private/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/private/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      824 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/private/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1829 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/private/accept_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3992 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/private/private_distribution_account.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4636 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/private/list_private_distribution_accounts_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4592 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/ssl_certificate_payload.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5431 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_status_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4389 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/build_step.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7245 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3292 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result_output.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3752 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/error_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3786 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/audio_asset.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3891 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/pagination_context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2046 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7040 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/annotation_with_audio_asset.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1687 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6210 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/annotation.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4585 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/list_asr_evaluations_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4280 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_metadata_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3557 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/skill.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7085 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_metadata.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3210 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/post_asr_evaluations_response_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7098 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/get_asr_evaluation_status_response_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5466 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1945 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3745 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/post_asr_evaluations_request_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4403 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/get_asr_evaluations_results_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3304 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/metrics.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3368 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/create_asr_annotation_set_request_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3786 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/audio_asset.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3891 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/pagination_context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7714 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_with_audio_asset.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5254 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_set_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1560 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7444 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/annotation.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4372 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/list_asr_annotation_sets_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3929 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/update_asr_annotation_set_contents_payload.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3180 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/create_asr_annotation_set_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4923 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_set_metadata.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5379 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/get_asr_annotation_set_annotations_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5088 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/get_asr_annotation_sets_properties_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3388 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/update_asr_annotation_set_properties_request_object.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3995 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication/skill_publication_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1923 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication/skill_publication_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3776 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication/publish_skill_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      799 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3544 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4528 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_version.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5010 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/standardized_error.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4286 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/distribution_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5549 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/review_tracking_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1178 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5647 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/certification_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5352 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/certification_summary.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4839 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/review_tracking_info_summary.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6036 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/list_certifications_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2049 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/certification_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3825 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/publication_failure.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4882 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/estimation_update.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3922 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/certification_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4853 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest_last_update_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    16940 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_details.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4342 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3989 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/submit_skill_for_certification_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3878 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/version_submission.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3531 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/connections_payload.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3648 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/extension_initialization_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1851 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/flash_briefing_update_frequency.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4009 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_localized_privacy_and_compliance.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3248 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/target_runtime_device.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      855 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3759 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/connection.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2833 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/suppressed_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4103 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/target_runtime.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1725 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/target_runtime_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3180 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_feature.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3454 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/dialog_delegation_strategy.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4097 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_endpoint.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3279 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/authorized_client_lwa_application.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3462 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/extension_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3761 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/voice_profile_feature.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1927 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/ssl_certificate_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1880 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/viewport_mode.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5702 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_events.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3665 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1793 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/flash_briefing_content_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8285 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_privacy_and_compliance.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4401 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/authorized_client_lwa.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2828 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/interface_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7309 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_apis.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2066 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/distribution_mode.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4074 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_connections.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3732 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_capability.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1988 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/display_interface_apml_version.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3436 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/event_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3621 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/up_channel_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3017 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/house_hold_list.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4139 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_interfaces.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5131 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/permission_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5911 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3490 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/health_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3591 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/region.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3437 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_envelope.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6309 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3734 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/supported_controls.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3162 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/app_link_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8255 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_apis.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3302 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/lambda_endpoint.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5602 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/viewport_specification.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3884 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/catalog_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3172 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_alias.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4258 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_feature.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3571 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_content_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3858 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/friendly_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5357 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/manifest_gadget_support.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4451 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/source_language_for_locales.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4229 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/dialog_manager.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3936 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_fire_tv_catalog_ingestion.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6041 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/distribution_countries.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    10166 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_publishing_information.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1859 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/gadget_support_requirement.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3165 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_app_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8861 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_apis.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_dialog_management/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3458 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_dialog_management/session_start_delegation_strategy.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_dialog_management/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      696 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_dialog_management/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2334 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/flash_briefing_genre.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4775 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/linked_application.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3970 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/app_link.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7699 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/localized_flash_briefing_info_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3170 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_wordmark.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3909 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/knowledge_apis.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6284 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_apis_locale.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4558 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3173 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/game_engine_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4642 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/dialog_management.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3443 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/gadget_controller_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2023 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/smart_home_protocol.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7060 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_localized_publishing_information.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1729 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/version.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3118 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5692 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_apis.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3531 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/lambda_region.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3740 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_country_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8134 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1750 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/manifest_version.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3879 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/flash_briefing_apis.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3460 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/amazon_conversations_dialog_manager.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3395 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/permission_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5783 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/automatic_distribution.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3361 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/authorized_client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    30273 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/event_name_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3159 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/audio_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5580 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/smart_home_apis.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1849 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface_request_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3171 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/app_link_v2_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5083 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_for_business_apis.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4332 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_region.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3787 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/localized_knowledge_information.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1806 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/viewport_shape.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4178 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_presentation_apl_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6130 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/display_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1820 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/catalog_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1864 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_content_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3374 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/localized_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4086 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/authorized_client_lwa_application_android.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4146 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_localized_information_dialog_management.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1993 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/display_interface_template_version.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3205 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/event_publications.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4675 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/demand_response_apis.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3934 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_localized_information.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1732 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_prompt_name_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3718 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_prompt_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3532 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_task.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1823 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/supported_controls_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5305 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/localized_music_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3135 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_catalog_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4409 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/localized_flash_briefing_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3372 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_presentation_html_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5077 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model_last_update_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4378 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/image_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2852 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_failure_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2074 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/reason.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5333 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/hosted_skill_deployment_status_last_update_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3058 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_request_status.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5002 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4803 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/profile_nlu_selected_intent.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1985 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/confirmation_status_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3662 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/profile_nlu_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1888 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/dialog_act_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1376 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4449 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/slot_resolutions.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4643 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/slot.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2486 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_status_code.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5539 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/profile_nlu_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4468 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/multi_turn.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3854 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_value_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4199 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/dialog_act.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3779 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4557 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/intent.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6969 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_summary.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2032 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication_method.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3682 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/image_dimension.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4373 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/create_skill_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4506 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/list_skill_versions_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3705 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/image_size.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3915 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/hosted_skill_provisioning_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2180 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/rollback_request_status_types.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3465 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/confidence.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6532 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/intent_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1944 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/intent_request_locales.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1959 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/locale_in_query.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1863 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/publication_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1237 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3164 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/slot.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2123 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/intent_confidence_bin.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6128 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/intent_requests.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2166 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/sort_field_for_intent_request_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2060 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/confidence_bin.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3457 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/dialog_act.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2549 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/dialog_act_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2055 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/interaction_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4410 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/intent.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3961 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/import_response_skill.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4797 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/instance.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3724 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_messaging_credentials.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3152 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/version_submission_status.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/resource_schema/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/resource_schema/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      686 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/resource_schema/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3749 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/resource_schema/get_resource_schema_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3995 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/hosted_skill_deployment_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3464 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/create_rollback_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1814 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3207 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/regional_ssl_certificate.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4286 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_resource_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4938 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/import_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3703 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/withdraw_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3782 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/export_response_skill.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3719 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/build_details.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4504 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_interaction_model_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3533 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/create_skill_with_package_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3225 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/create_skill_response.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4933 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/beta_test.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      771 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2897 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/update_beta_test_response.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4858 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/tester_with_details.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      837 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4077 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/list_testers_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3161 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/tester.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1840 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/invitation_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3505 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/testers_list.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1871 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3289 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/test_body.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1862 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/overwrite_mode.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1746 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/format.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3668 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/upload_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3791 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_credentials.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4412 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/account_linking_platform_authorization_url.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    11049 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/account_linking_request_payload.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     9139 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/account_linking_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1876 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/access_token_scheme_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3861 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/account_linking_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1060 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1806 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/account_linking_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1835 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/platform_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2062 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_summary_apis.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3718 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_failure_reason.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3920 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/export_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4517 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4869 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/list_nlu_evaluations_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3375 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/pagination_context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2213 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5496 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_results_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1747 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/results_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3284 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/results.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2486 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_status_code.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4274 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/paged_results_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3112 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/expected_intent_slots_props.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3815 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/evaluate_nlu_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3407 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_response_links.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3565 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/actual.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4920 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/test_case.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5228 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/evaluation.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4972 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1805 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3776 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/paged_results_response_pagination_context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4961 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/evaluation_entity.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3627 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/links.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3575 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/inputs.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3653 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/expected.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1970 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/confirmation_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3811 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/evaluation_inputs.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4048 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/paged_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3148 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/evaluate_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4649 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3787 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/expected_intent.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4267 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/resolutions.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4599 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/slots_props.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5776 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3598 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_value.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3289 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/source.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4355 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/intent.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2933 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/update_nlu_annotation_set_annotations_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4794 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/list_nlu_annotation_sets_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3180 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/create_nlu_annotation_set_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3375 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/pagination_context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1315 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4513 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/get_nlu_annotation_set_properties_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3510 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/create_nlu_annotation_set_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4353 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/annotation_set_entity.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3627 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/links.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3234 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/update_nlu_annotation_set_properties_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4808 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/annotation_set.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6597 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/list_skill_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3474 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/hosted_skill_deployment_details.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3846 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/dialog_prompts.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3756 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/prompt_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2268 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3824 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/has_entity_resolution_match.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3420 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/multiple_values_config.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3245 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3530 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_input.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1132 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4287 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_definition_output.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4844 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/list_catalog_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3560 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/update_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1866 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_status_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4532 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/last_update_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3534 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_entity.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4343 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3747 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3880 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/definition_data.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3890 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_less_than.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3911 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_not_in_set.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5979 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/dialog_intents.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4574 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/interaction_model_schema.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3501 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/value_catalog.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3882 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_greater_than.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3757 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/fallback_intent_sensitivity.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3944 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_greater_than_or_equal_to.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2085 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/fallback_intent_sensitivity_level.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4864 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/slot_definition.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4162 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/interaction_model_data.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3876 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/inline_value_supplier.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4964 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/execution.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4457 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/trigger.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4909 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/catalog_auto_refresh.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4831 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/list_job_definitions_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6370 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/reference_version_update.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3159 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/job_api_pagination_context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1828 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3784 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/job_error_details.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3581 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/update_job_status_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3277 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/create_job_definition_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1811 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3623 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/validation_errors.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4755 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/get_executions_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3449 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/catalog.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4657 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/resource_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5274 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4142 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition_metadata.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3918 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/interaction_model.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4189 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/scheduled.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3957 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/create_job_definition_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3341 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/referenced_resource_jobs_complete.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3533 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/slot_type_reference.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3506 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/dynamic_update_error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3896 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/execution_metadata.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3828 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/dialog_intents_prompts.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3926 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_less_than_or_equal_to.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3901 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog_value_supplier.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4737 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/slot_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3897 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_configuration.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3729 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_value.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3891 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_in_set.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6054 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_in_duration.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6074 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_not_in_duration.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4150 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflicts_response_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3864 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/pagination_context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3958 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5000 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflicts_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1142 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3367 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_intent_slot.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4118 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflict_detection_job_status_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3905 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_intent.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1870 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_detection_job_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4044 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/paged_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4509 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/value_supplier.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1821 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/prompt_items_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5091 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/language_model.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5933 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/dialog_slot_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4739 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/dialog.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4043 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/prompt.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4069 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/version_data_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3628 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/version_data.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1119 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4514 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/list_slot_type_version_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3678 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_update.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3352 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_update_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3618 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/value_supplier_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4649 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_data_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3988 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3742 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_data.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3662 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3442 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1293 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3466 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/warning.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4284 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3716 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3358 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_update_definition.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3953 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_definition_output.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3698 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/update_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5135 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/last_update_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1868 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_status_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3544 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_input.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4323 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/list_slot_type_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3186 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_response_entity.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3931 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/definition_data.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3467 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_value_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6483 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/slot_validation.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5299 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/list_catalog_entity_versions_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4735 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/list_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3881 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/version_data.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1163 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4317 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/catalog_entity_version.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3365 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/value_schema_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3765 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/value_schema.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4782 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/catalog_values.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3274 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/links.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3330 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/catalog_update.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4189 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/catalog_version_data.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4249 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/version_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3513 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/input_source.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1986 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/delegation_strategy_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4332 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/intent.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3956 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_endpoint.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4667 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4158 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/alexa_hosted_config.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1750 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3862 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1885 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_runtime.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3989 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1527 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4194 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1724 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3584 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_metadata.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1841 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_region.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3974 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials_list.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3637 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3628 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosting_configuration.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1982 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4050 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1847 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/action.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1909 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/invocation_response_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1783 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/end_point_regions.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1085 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4190 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/invoke_skill_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4146 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/invocation_response_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3224 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3584 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/metrics.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4132 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/invoke_skill_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3476 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/skill_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3542 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4705 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/skill_execution_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5072 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/rollback_request_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4563 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/hosted_skill_provisioning_last_update_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1749 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/image_size_unit.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1876 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_data_types.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5268 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/resource_import_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1949 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_resources_enum.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3693 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/bad_request_error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3906 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      811 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3648 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/presigned_upload_part_items.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4154 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/pre_signed_url.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6088 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/get_content_upload_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2975 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/catalog_upload_base.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1914 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/file_upload_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1164 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4191 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/content_upload_file_summary.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3390 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/location.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1866 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/upload_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1877 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/ingestion_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5154 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/upload_ingestion_step.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3368 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/pre_signed_url_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1788 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/ingestion_step_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      840 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3613 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/create_content_upload_url_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4206 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/create_content_upload_url_response.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3402 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3251 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/requester_filter.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2071 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/sort_field.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1351 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3507 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/resource.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4986 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/request_pagination_context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3800 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/resource_filter.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1970 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/sort_direction.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7185 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/request_filters.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3646 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/operation_filter.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6113 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/audit_log.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5675 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/audit_logs_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3372 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/client_filter.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1882 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/resource_type_enum.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3369 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/requester.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3441 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/response_pagination_context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4908 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/audit_logs_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3382 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/operation.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4627 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/evaluate_sh_capability_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2893 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_capability_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5300 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/evaluation_object.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1740 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/stage.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3139 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/endpoint.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3420 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/pagination_context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3070 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/capability_test_plan.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1999 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3157 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/pagination_context_token.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2288 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_capability_error_code.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3274 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/list_sh_test_plan_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4208 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_evaluation_results_metric.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4402 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/list_sh_capability_evaluations_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6220 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/get_sh_capability_evaluation_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3739 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_capability_error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2895 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_capability_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4963 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/evaluate_sh_capability_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2887 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_capability_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7778 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/test_case_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1788 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/test_case_result_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3588 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/paged_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1837 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/evaluation_entity_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4445 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/list_sh_capability_test_plans_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4487 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/get_sh_capability_evaluation_results_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3062 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/link.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1825 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/editable_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3728 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/in_skill_product_summary_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3710 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/update_in_skill_product_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1849 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/product_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1804 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/currency.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4683 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/associated_skill_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3597 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/tax_information.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4151 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/summary_price_listing.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7484 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/localized_publishing_information.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2400 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1976 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/promotable_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8361 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/in_skill_product_definition.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4053 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/create_in_skill_product_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4508 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/subscription_information.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1853 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/subscription_payment_frequency.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3265 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/product_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6041 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/distribution_countries.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     9007 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/in_skill_product_summary.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2159 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/tax_information_category.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1924 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4003 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/price_listing.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2081 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/purchasable_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3827 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/privacy_and_compliance.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3504 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/localized_privacy_and_compliance.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4366 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/summary_marketplace_pricing.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4294 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/marketplace_pricing.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3741 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/list_in_skill_product_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4408 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/custom_product_prompts.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3294 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/isp_summary_links.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4643 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/list_in_skill_product.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3794 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/in_skill_product_definition_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6042 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/publishing_information.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1791 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/stage_v2_type.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/vendor_management/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/vendor_management/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      674 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/vendor_management/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3779 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/vendor_management/vendor.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3399 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/vendor_management/vendors.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3627 2021-06-10 19:45:18.000000 ask-smapi-model-1.9.2/ask_smapi_model/v1/links.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5004 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3208 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/alexa_response_content.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1985 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/confirmation_status_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4279 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/simulations_api_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3262 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/input.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4400 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/simulations_api_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1661 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4449 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/slot_resolutions.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4641 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/slot.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4711 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/simulation_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2486 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_status_code.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1999 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/simulations_api_response_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3854 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_value_items.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4140 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/alexa_execution_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3522 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/device.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3960 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/alexa_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3465 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/session.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3779 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3415 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/skill_execution_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1847 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/session_mode.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4557 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/intent.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      784 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3606 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocation_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3584 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/metrics.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3288 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocation_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4621 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocation.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1913 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/invocation_response_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4196 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/invocations_api_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1816 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/end_point_regions.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      955 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3862 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/invocation_response_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3476 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/skill_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4138 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/invocations_api_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3693 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/bad_request_error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3644 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      690 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v2/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      994 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/__version__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/services/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/services/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/services/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/services/skill_management/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/services/skill_management/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      692 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/services/skill_management/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)   850764 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/ask_smapi_model/services/skill_management/skill_management_service_client.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3691 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/bad_request_error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3644 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      690 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      671 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4522 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/skill_review_publish.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3704 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/skill_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1183 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3513 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/actor_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1811 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/request_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3501 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/subscription_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5901 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/base_schema.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4805 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/skill_review_event_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4200 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/skill_review_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5200 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/skill_event_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4165 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/interaction_model_attributes.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5540 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/manifest_update.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      815 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5528 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/interaction_model_update.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5870 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/skill_publish.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5414 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/skill_certification.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5479 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/interaction_model_event_attributes.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4477 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/list_catalogs_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5733 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/catalog_summary.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3607 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/create_content_upload_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6179 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/get_content_upload_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3497 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/presigned_upload_part.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1914 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/file_upload_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1409 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4029 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/content_upload_file_summary.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4493 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/list_uploads_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1863 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/upload_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3665 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/complete_upload_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4657 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/content_upload_summary.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1877 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/ingestion_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5112 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/upload_ingestion_step.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3368 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/pre_signed_url_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6508 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/create_content_upload_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1788 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/ingestion_step_name.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      898 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2284 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/catalog_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5733 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/catalog_details.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2576 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/catalog_usage.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4468 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/create_catalog_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4884 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/subscription_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      946 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3811 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/update_subscription_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4344 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/list_subscriptions_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4888 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/subscription_summary.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4087 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/event.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4539 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/create_subscription_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3897 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/endpoint.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3697 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/update_subscriber_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3622 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/endpoint_aws_authorization.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/py.typed
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1170 2021-06-10 19:47:02.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1906 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/subscriber_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4134 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/subscriber_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4241 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/endpoint_authorization.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3978 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/create_subscriber_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1794 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/endpoint_authorization_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5010 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/subscriber_summary.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4300 2021-06-10 19:45:17.000000 ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/list_subscribers_response.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model.egg-info/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    45789 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model.egg-info/SOURCES.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model.egg-info/dependency_links.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       16 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model.egg-info/top_level.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model.egg-info/not-zip-safe
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    10059 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model.egg-info/PKG-INFO
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       79 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/ask_smapi_model.egg-info/requires.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    11357 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/LICENSE
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    10059 2021-06-10 19:48:20.000000 ask-smapi-model-1.9.2/PKG-INFO
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2162 2021-06-10 19:45:19.000000 ask-smapi-model-1.9.2/setup.py
```

### Comparing `ask-smapi-model-1.9.1/CHANGELOG.rst` & `ask-smapi-model-1.9.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -169,7 +169,15 @@
 ^^^^^
 
 This release contains the following changes :
 
 - General bug fixes and updates.
 - Model definition updates to support `AlexaCustomerFeedbackEvent.SkillReviewPublish <https://developer.amazon.com/en-US/docs/alexa/sdns/skill-development-event-schemas.html#events-summary>`__ event notifications for skill developers in SMAPI.
 - Developers can subscribe to this `new event and get notified <https://developer.amazon.com/en-US/docs/alexa/sdns/use-skill-development-notifications.html>`__ whenever there is a customer-review published for their skills.
+
+
+1.9.2
+^^^^^
+
+This release contains the following changes :
+
+- general bug fixes and updates
```

### Comparing `ask-smapi-model-1.9.1/README.rst` & `ask-smapi-model-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/stage_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/stage_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/validations_api_response_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/validations_api_response_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/validations_api_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/validations_api_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/validations_api_response_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/validations_api_response_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/response_validation_importance.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/response_validation_importance.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/response_validation_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/response_validation_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/validations_api_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/validations_api_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validations/response_validation.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validations/response_validation.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/agreement_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/agreement_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_stage_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_stage_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/update_skill_with_package_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/update_skill_with_package_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_feature.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_feature.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/build_step_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/build_step_name.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/alexa_response_content.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/alexa_response_content.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/simulations_api_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/simulations_api_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/input.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/input.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/simulations_api_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/simulations_api_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/simulation_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/simulation_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/simulations_api_response_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/simulations_api_response_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/alexa_execution_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/alexa_execution_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/device.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/device.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/invocation_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/invocation_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/alexa_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/alexa_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/session.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/session.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/metrics.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/metrics.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/invocation_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/invocation_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/invocation.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/invocation.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/simulations/session_mode.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/simulations/session_mode.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/response_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/response_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/create_rollback_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/create_rollback_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/skill_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/skill_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/stage_for_metric.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/stage_for_metric.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/metric.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/period.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/period.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/metrics/get_metric_data_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/metrics/get_metric_data_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/private/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/private/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/private/accept_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/private/accept_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/private/private_distribution_account.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/private/private_distribution_account.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/private/list_private_distribution_accounts_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/private/list_private_distribution_accounts_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/ssl_certificate_payload.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/ssl_certificate_payload.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_status_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_status_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/build_step.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/build_step.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result_output.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result_output.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/error_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/error_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/audio_asset.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/audio_asset.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/pagination_context.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/pagination_context.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/annotation_with_audio_asset.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/annotation_with_audio_asset.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/annotation.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/annotation.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/list_asr_evaluations_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/list_asr_evaluations_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_metadata_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_metadata_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/skill.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/skill.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_metadata.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_metadata.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/post_asr_evaluations_response_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/post_asr_evaluations_response_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/get_asr_evaluation_status_response_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/get_asr_evaluation_status_response_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/evaluation_result_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/post_asr_evaluations_request_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/post_asr_evaluations_request_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/get_asr_evaluations_results_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/get_asr_evaluations_results_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/evaluations/metrics.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/evaluations/metrics.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/create_asr_annotation_set_request_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/create_asr_annotation_set_request_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/audio_asset.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/audio_asset.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/pagination_context.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/pagination_context.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_with_audio_asset.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_with_audio_asset.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_set_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_set_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/annotation.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/annotation.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/list_asr_annotation_sets_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/list_asr_annotation_sets_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/update_asr_annotation_set_contents_payload.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/update_asr_annotation_set_contents_payload.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/create_asr_annotation_set_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/create_asr_annotation_set_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_set_metadata.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/annotation_set_metadata.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/get_asr_annotation_set_annotations_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/get_asr_annotation_set_annotations_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/get_asr_annotation_sets_properties_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/get_asr_annotation_sets_properties_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/asr/annotation_sets/update_asr_annotation_set_properties_request_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/asr/annotation_sets/update_asr_annotation_set_properties_request_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication/skill_publication_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication/skill_publication_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication/skill_publication_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication/skill_publication_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication/publish_skill_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication/publish_skill_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_version.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_version.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/standardized_error.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/standardized_error.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/distribution_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/distribution_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/review_tracking_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/review_tracking_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/certification_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/certification_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/certification_summary.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/certification_summary.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/review_tracking_info_summary.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/review_tracking_info_summary.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/list_certifications_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/list_certifications_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/certification_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/certification_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/publication_failure.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/publication_failure.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/estimation_update.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/estimation_update.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/certification/certification_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/certification/certification_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest_last_update_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest_last_update_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_details.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_details.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/submit_skill_for_certification_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/submit_skill_for_certification_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/version_submission.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/version_submission.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/connections_payload.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/connections_payload.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/extension_initialization_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/extension_initialization_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/flash_briefing_update_frequency.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/flash_briefing_update_frequency.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_localized_privacy_and_compliance.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_localized_privacy_and_compliance.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/target_runtime_device.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/target_runtime_device.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/connection.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/connection.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/suppressed_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/suppressed_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/target_runtime.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/target_runtime.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom/target_runtime_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom/target_runtime_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_feature.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_feature.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/dialog_delegation_strategy.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/dialog_delegation_strategy.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_endpoint.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_endpoint.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_web_player_feature.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/voice_profile_feature.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class VideoWebPlayerFeature(VideoFeature):
+class VoiceProfileFeature(VideoFeature):
     """
-    Feature for allowing and supporting directives and CX for casting content to video web players.
+    Feature for allowing for querying for available partner voice profiles, linking Alexa Speaker ID profiles to partner speaker profiles, and sending partner speaker profiles in directives.
 
 
     :param version: 
     :type version: (optional) str
 
     """
     deserialized_types = {
@@ -44,23 +44,23 @@
         'version': 'version',
         'name': 'name'
     }  # type: Dict
     supports_multiple_types = False
 
     def __init__(self, version=None):
         # type: (Optional[str], ) -> None
-        """Feature for allowing and supporting directives and CX for casting content to video web players.
+        """Feature for allowing for querying for available partner voice profiles, linking Alexa Speaker ID profiles to partner speaker profiles, and sending partner speaker profiles in directives.
 
         :param version: 
         :type version: (optional) str
         """
-        self.__discriminator_value = "VIDEO_WEB_PLAYER"  # type: str
+        self.__discriminator_value = "VIDEO_VOICE_PROFILE"  # type: str
 
         self.name = self.__discriminator_value
-        super(VideoWebPlayerFeature, self).__init__(version=version, name=self.__discriminator_value)
+        super(VoiceProfileFeature, self).__init__(version=version, name=self.__discriminator_value)
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -97,15 +97,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, VideoWebPlayerFeature):
+        if not isinstance(other, VoiceProfileFeature):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/authorized_client_lwa_application.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/authorized_client_lwa_application.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/extension_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/extension_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/voice_profile_feature.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_presentation_html_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,53 +14,47 @@
 #
 
 import pprint
 import re  # noqa: F401
 import six
 import typing
 from enum import Enum
-from ask_smapi_model.v1.skill.manifest.video_feature import VideoFeature
+from ask_smapi_model.v1.skill.manifest.interface import Interface
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class VoiceProfileFeature(VideoFeature):
+class AlexaPresentationHtmlInterface(Interface):
     """
-    Feature for allowing for querying for available partner voice profiles, linking Alexa Speaker ID profiles to partner speaker profiles, and sending partner speaker profiles in directives.
+    Used to declare that the skill uses the Alexa.Presentation.HTML interface.
 
 
-    :param version: 
-    :type version: (optional) str
 
     """
     deserialized_types = {
-        'version': 'str',
-        'name': 'str'
+        'object_type': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'version': 'version',
-        'name': 'name'
+        'object_type': 'type'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, version=None):
-        # type: (Optional[str], ) -> None
-        """Feature for allowing for querying for available partner voice profiles, linking Alexa Speaker ID profiles to partner speaker profiles, and sending partner speaker profiles in directives.
+    def __init__(self):
+        # type: () -> None
+        """Used to declare that the skill uses the Alexa.Presentation.HTML interface.
 
-        :param version: 
-        :type version: (optional) str
         """
-        self.__discriminator_value = "VIDEO_VOICE_PROFILE"  # type: str
+        self.__discriminator_value = "ALEXA_PRESENTATION_HTML"  # type: str
 
-        self.name = self.__discriminator_value
-        super(VoiceProfileFeature, self).__init__(version=version, name=self.__discriminator_value)
+        self.object_type = self.__discriminator_value
+        super(AlexaPresentationHtmlInterface, self).__init__(object_type=self.__discriminator_value)
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -97,15 +91,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, VoiceProfileFeature):
+        if not isinstance(other, AlexaPresentationHtmlInterface):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/ssl_certificate_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/ssl_certificate_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/viewport_mode.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/viewport_mode.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_events.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_events.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/flash_briefing_content_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/flash_briefing_content_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_privacy_and_compliance.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_privacy_and_compliance.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/authorized_client_lwa.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/authorized_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,25 +14,24 @@
 #
 
 import pprint
 import re  # noqa: F401
 import six
 import typing
 from enum import Enum
-from ask_smapi_model.v1.skill.manifest.authorized_client import AuthorizedClient
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class AuthorizedClientLwa(AuthorizedClient):
+class AuthorizedClient(object):
     """
-    Defines client using Login With Amazon authentication provider, corresponds to LWA Security Profile.
+    Defines a client authorized for a skill.
 
 
     :param authentication_provider: 
     :type authentication_provider: (optional) str
 
     """
     deserialized_types = {
@@ -42,22 +41,22 @@
     attribute_map = {
         'authentication_provider': 'authenticationProvider'
     }  # type: Dict
     supports_multiple_types = False
 
     def __init__(self, authentication_provider=None):
         # type: (Optional[str]) -> None
-        """Defines client using Login With Amazon authentication provider, corresponds to LWA Security Profile.
+        """Defines a client authorized for a skill.
 
         :param authentication_provider: 
         :type authentication_provider: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
-        super(AuthorizedClientLwa, self).__init__(authentication_provider=authentication_provider)
+        self.authentication_provider = authentication_provider
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -94,15 +93,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, AuthorizedClientLwa):
+        if not isinstance(other, AuthorizedClient):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/interface_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/interface_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_apis.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_apis.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/distribution_mode.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/distribution_mode.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_connections.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_connections.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_capability.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_capability.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/display_interface_apml_version.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/display_interface_apml_version.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/event_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/event_name.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/up_channel_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/up_channel_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/house_hold_list.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/house_hold_list.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_interfaces.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_interfaces.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/permission_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/permission_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 class PermissionName(Enum):
     """
     Name of the required permission.
 
 
 
-    Allowed enum values: [alexa_device_id_read, alexa_personality_explicit_read, alexa_authenticate_2_mandatory, alexa_devices_all_address_country_and_postal_code_read, alexa_profile_mobile_number_read, alexa_async_event_write, alexa_device_type_read, alexa_skill_proactive_enablement, alexa_personality_explicit_write, alexa_household_lists_read, alexa_utterance_id_read, alexa_user_experience_guidance_read, alexa_devices_all_notifications_write, avs_distributed_audio, alexa_devices_all_address_full_read, alexa_devices_all_notifications_urgent_write, payments_autopay_consent, alexa_alerts_timers_skill_readwrite, alexa_customer_id_read, alexa_skill_cds_monetization, alexa_music_cast, alexa_profile_given_name_read, alexa_alerts_reminders_skill_readwrite, alexa_household_lists_write, alexa_profile_email_read, alexa_profile_name_read, alexa_devices_all_geolocation_read, alexa_raw_person_id_read, alexa_authenticate_2_optional, alexa_health_profile_write, alexa_person_id_read, alexa_skill_products_entitlements, alexa_energy_devices_state_read]
+    Allowed enum values: [alexa_device_id_read, alexa_personality_explicit_read, alexa_authenticate_2_mandatory, alexa_devices_all_address_country_and_postal_code_read, alexa_profile_mobile_number_read, alexa_async_event_write, alexa_device_type_read, alexa_skill_proactive_enablement, alexa_personality_explicit_write, alexa_household_lists_read, alexa_utterance_id_read, alexa_user_experience_guidance_read, alexa_devices_all_notifications_write, avs_distributed_audio, alexa_devices_all_address_full_read, alexa_devices_all_notifications_urgent_write, payments_autopay_consent, alexa_alerts_timers_skill_readwrite, alexa_customer_id_read, alexa_skill_cds_monetization, alexa_music_cast, alexa_profile_given_name_read, alexa_alerts_reminders_skill_readwrite, alexa_household_lists_write, alexa_profile_email_read, alexa_profile_name_read, alexa_devices_all_geolocation_read, alexa_raw_person_id_read, alexa_authenticate_2_optional, alexa_health_profile_write, alexa_person_id_read, alexa_skill_products_entitlements, alexa_energy_devices_state_read, alexa_origin_ip_address_read]
     """
     alexa_device_id_read = "alexa::device_id:read"
     alexa_personality_explicit_read = "alexa::personality:explicit:read"
     alexa_authenticate_2_mandatory = "alexa::authenticate:2:mandatory"
     alexa_devices_all_address_country_and_postal_code_read = "alexa:devices:all:address:country_and_postal_code:read"
     alexa_profile_mobile_number_read = "alexa::profile:mobile_number:read"
     alexa_async_event_write = "alexa::async_event:write"
@@ -62,14 +62,15 @@
     alexa_devices_all_geolocation_read = "alexa::devices:all:geolocation:read"
     alexa_raw_person_id_read = "alexa::raw_person_id:read"
     alexa_authenticate_2_optional = "alexa::authenticate:2:optional"
     alexa_health_profile_write = "alexa::health:profile:write"
     alexa_person_id_read = "alexa::person_id:read"
     alexa_skill_products_entitlements = "alexa::skill:products:entitlements"
     alexa_energy_devices_state_read = "alexa::energy:devices:state:read"
+    alexa_origin_ip_address_read = "alexa::origin_ip_address:read"
 
     def to_dict(self):
         # type: () -> Dict[str, Any]
         """Returns the model properties as a dict"""
         result = {self.name: self.value}
         return result
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/health_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/health_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/region.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/region.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_envelope.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_envelope.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from .connections_payload import ConnectionsPayload
 from .extension_initialization_request import ExtensionInitializationRequest
 from .flash_briefing_update_frequency import FlashBriefingUpdateFrequency
 from .skill_manifest_localized_privacy_and_compliance import SkillManifestLocalizedPrivacyAndCompliance
 from .music_feature import MusicFeature
 from .dialog_delegation_strategy import DialogDelegationStrategy
 from .skill_manifest_endpoint import SkillManifestEndpoint
-from .video_web_player_feature import VideoWebPlayerFeature
 from .authorized_client_lwa_application import AuthorizedClientLwaApplication
 from .extension_request import ExtensionRequest
 from .voice_profile_feature import VoiceProfileFeature
 from .ssl_certificate_type import SSLCertificateType
 from .viewport_mode import ViewportMode
 from .skill_manifest_events import SkillManifestEvents
 from .alexa_for_business_interface_request import AlexaForBusinessInterfaceRequest
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/supported_controls.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/supported_controls.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/app_link_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/app_link_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_apis.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_apis.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/lambda_endpoint.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/lambda_endpoint.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/viewport_specification.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/viewport_specification.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/catalog_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/catalog_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_alias.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_alias.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_feature.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,33 +37,30 @@
     :type name: (optional) str
 
     .. note::
 
         This is an abstract class. Use the following mapping, to figure out
         the model class to be instantiated, that sets ``name`` variable.
 
-        | VIDEO_VOICE_PROFILE: :py:class:`ask_smapi_model.v1.skill.manifest.voice_profile_feature.VoiceProfileFeature`,
-        |
-        | VIDEO_WEB_PLAYER: :py:class:`ask_smapi_model.v1.skill.manifest.video_web_player_feature.VideoWebPlayerFeature`
+        | VIDEO_VOICE_PROFILE: :py:class:`ask_smapi_model.v1.skill.manifest.voice_profile_feature.VoiceProfileFeature`
 
     """
     deserialized_types = {
         'version': 'str',
         'name': 'str'
     }  # type: Dict
 
     attribute_map = {
         'version': 'version',
         'name': 'name'
     }  # type: Dict
     supports_multiple_types = False
 
     discriminator_value_class_map = {
-        'VIDEO_VOICE_PROFILE': 'ask_smapi_model.v1.skill.manifest.voice_profile_feature.VoiceProfileFeature',
-        'VIDEO_WEB_PLAYER': 'ask_smapi_model.v1.skill.manifest.video_web_player_feature.VideoWebPlayerFeature'
+        'VIDEO_VOICE_PROFILE': 'ask_smapi_model.v1.skill.manifest.voice_profile_feature.VoiceProfileFeature'
     }
 
     json_discriminator_key = "name"
 
     __metaclass__ = ABCMeta
 
     @abstractmethod
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_content_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_content_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/friendly_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/friendly_name.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/manifest_gadget_support.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/manifest_gadget_support.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/source_language_for_locales.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/source_language_for_locales.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/dialog_manager.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/dialog_manager.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_fire_tv_catalog_ingestion.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_fire_tv_catalog_ingestion.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/distribution_countries.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/distribution_countries.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_publishing_information.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_publishing_information.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/gadget_support_requirement.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/gadget_support_requirement.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_app_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_app_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_apis.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_apis.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_dialog_management/session_start_delegation_strategy.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_dialog_management/session_start_delegation_strategy.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_dialog_management/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_dialog_management/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/flash_briefing_genre.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/flash_briefing_genre.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/linked_application.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/linked_application.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/app_link.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/app_link.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/localized_flash_briefing_info_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/localized_flash_briefing_info_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_wordmark.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_wordmark.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/knowledge_apis.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/knowledge_apis.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_apis_locale.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_apis_locale.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/game_engine_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/game_engine_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/dialog_management.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/dialog_management.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/gadget_controller_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/gadget_controller_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/smart_home_protocol.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/smart_home_protocol.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest_localized_publishing_information.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest_localized_publishing_information.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/version.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/version.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_apis.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_apis.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/lambda_region.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/lambda_region.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_country_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_country_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/skill_manifest.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/skill_manifest.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/manifest_version.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/manifest_version.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/flash_briefing_apis.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/flash_briefing_apis.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/amazon_conversations_dialog_manager.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/amazon_conversations_dialog_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
 class AMAZONConversationsDialogManager(DialogManager):
     """
-    The type of dialog manager:  * AMAZON.Conversations - The Alexa Conversations (Coltrane) model for this skill. See https://w.amazon.com/bin/view/Digital/Alexa/ConversationalAI/Coltrane
+    The type of dialog manager:  * AMAZON.Conversations - The Alexa Conversations (Coltrane) model for this skill.
 
 
 
     """
     deserialized_types = {
         'object_type': 'str'
     }  # type: Dict
@@ -40,15 +40,15 @@
     attribute_map = {
         'object_type': 'type'
     }  # type: Dict
     supports_multiple_types = False
 
     def __init__(self):
         # type: () -> None
-        """The type of dialog manager:  * AMAZON.Conversations - The Alexa Conversations (Coltrane) model for this skill. See https://w.amazon.com/bin/view/Digital/Alexa/ConversationalAI/Coltrane
+        """The type of dialog manager:  * AMAZON.Conversations - The Alexa Conversations (Coltrane) model for this skill.
 
         """
         self.__discriminator_value = "AMAZON.Conversations"  # type: str
 
         self.object_type = self.__discriminator_value
         super(AMAZONConversationsDialogManager, self).__init__(object_type=self.__discriminator_value)
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/permission_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/permission_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/automatic_distribution.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/automatic_distribution.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/authorized_client.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/pagination_context_token.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,42 +21,40 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class AuthorizedClient(object):
+class PaginationContextToken(object):
     """
-    Defines a client authorized for a skill.
 
-
-    :param authentication_provider: 
-    :type authentication_provider: (optional) str
+    :param next_token: 
+    :type next_token: (optional) str
 
     """
     deserialized_types = {
-        'authentication_provider': 'str'
+        'next_token': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'authentication_provider': 'authenticationProvider'
+        'next_token': 'nextToken'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, authentication_provider=None):
+    def __init__(self, next_token=None):
         # type: (Optional[str]) -> None
-        """Defines a client authorized for a skill.
+        """
 
-        :param authentication_provider: 
-        :type authentication_provider: (optional) str
+        :param next_token: 
+        :type next_token: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
-        self.authentication_provider = authentication_provider
+        self.next_token = next_token
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -93,15 +91,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, AuthorizedClient):
+        if not isinstance(other, PaginationContextToken):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/event_name_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/event_name_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/audio_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/audio_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/smart_home_apis.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/smart_home_apis.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface_request_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_for_business_interface_request_name.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/app_link_v2_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/app_link_v2_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_for_business_apis.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_for_business_apis.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_region.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_region.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/localized_knowledge_information.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/localized_knowledge_information.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/viewport_shape.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/viewport_shape.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_presentation_apl_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/alexa_presentation_apl_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/display_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/display_interface.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/catalog_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/catalog_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/music_content_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/music_content_name.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/localized_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/localized_name.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/authorized_client_lwa_application_android.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_intent_slot.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,50 +14,54 @@
 #
 
 import pprint
 import re  # noqa: F401
 import six
 import typing
 from enum import Enum
-from ask_smapi_model.v1.skill.manifest.authorized_client_lwa_application import AuthorizedClientLwaApplication
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class AuthorizedClientLwaApplicationAndroid(AuthorizedClientLwaApplication):
+class ConflictIntentSlot(object):
     """
-    Defines an android application for LWA authentication provider.
-
 
+    :param value: 
+    :type value: (optional) str
     :param object_type: 
     :type object_type: (optional) str
 
     """
     deserialized_types = {
+        'value': 'str',
         'object_type': 'str'
     }  # type: Dict
 
     attribute_map = {
+        'value': 'value',
         'object_type': 'type'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, object_type=None):
-        # type: (Optional[str]) -> None
-        """Defines an android application for LWA authentication provider.
+    def __init__(self, value=None, object_type=None):
+        # type: (Optional[str], Optional[str]) -> None
+        """
 
+        :param value: 
+        :type value: (optional) str
         :param object_type: 
         :type object_type: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
-        super(AuthorizedClientLwaApplicationAndroid, self).__init__(object_type=object_type)
+        self.value = value
+        self.object_type = object_type
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -94,15 +98,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, AuthorizedClientLwaApplicationAndroid):
+        if not isinstance(other, ConflictIntentSlot):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_localized_information_dialog_management.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_localized_information_dialog_management.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/display_interface_template_version.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/display_interface_template_version.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/event_publications.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/event_publications.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/demand_response_apis.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/demand_response_apis.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_localized_information.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_localized_information.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_prompt_name_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_prompt_name_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_prompt_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_prompt_name.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/custom_task.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/custom_task.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/supported_controls_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/supported_controls_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/localized_music_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/localized_music_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/video_catalog_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/video_catalog_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/localized_flash_briefing_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/localized_flash_briefing_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest/alexa_presentation_html_interface.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/slot.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,47 +14,47 @@
 #
 
 import pprint
 import re  # noqa: F401
 import six
 import typing
 from enum import Enum
-from ask_smapi_model.v1.skill.manifest.interface import Interface
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class AlexaPresentationHtmlInterface(Interface):
+class Slot(object):
     """
-    Used to declare that the skill uses the Alexa.Presentation.HTML interface.
-
 
+    :param name: Name of the slot that was used in this interaction.
+    :type name: (optional) str
 
     """
     deserialized_types = {
-        'object_type': 'str'
+        'name': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'object_type': 'type'
+        'name': 'name'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self):
-        # type: () -> None
-        """Used to declare that the skill uses the Alexa.Presentation.HTML interface.
+    def __init__(self, name=None):
+        # type: (Optional[str]) -> None
+        """
 
+        :param name: Name of the slot that was used in this interaction.
+        :type name: (optional) str
         """
-        self.__discriminator_value = "ALEXA_PRESENTATION_HTML"  # type: str
+        self.__discriminator_value = None  # type: str
 
-        self.object_type = self.__discriminator_value
-        super(AlexaPresentationHtmlInterface, self).__init__(object_type=self.__discriminator_value)
+        self.name = name
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -91,15 +91,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, AlexaPresentationHtmlInterface):
+        if not isinstance(other, Slot):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model_last_update_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model_last_update_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/image_attributes.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/image_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_failure_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_failure_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/reason.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/reason.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/hosted_skill_deployment_status_last_update_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/hosted_skill_deployment_status_last_update_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_request_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_request_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/profile_nlu_selected_intent.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/profile_nlu_selected_intent.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/confirmation_status_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/confirmation_status_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/profile_nlu_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/profile_nlu_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/dialog_act_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/dialog_act_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/slot_resolutions.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/slot_resolutions.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/slot.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/slot.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_status_code.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_status_code.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/profile_nlu_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/profile_nlu_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/multi_turn.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/multi_turn.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_value_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_value_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/dialog_act.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/dialog_act.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/resolutions_per_authority_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/evaluations/intent.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/evaluations/intent.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_summary.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_summary.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/publication_method.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/publication_method.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/image_dimension.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/image_dimension.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/create_skill_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/create_skill_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/list_skill_versions_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/list_skill_versions_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/image_size.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/image_size.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/hosted_skill_provisioning_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/hosted_skill_provisioning_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/rollback_request_status_types.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/rollback_request_status_types.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/confidence.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/confidence.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/intent_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/intent_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/intent_request_locales.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/intent_request_locales.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/locale_in_query.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/locale_in_query.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/publication_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/publication_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/slot.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/endpoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,40 +21,40 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class Slot(object):
+class Endpoint(object):
     """
 
-    :param name: Name of the slot that was used in this interaction.
-    :type name: (optional) str
+    :param endpoint_id: 
+    :type endpoint_id: (optional) str
 
     """
     deserialized_types = {
-        'name': 'str'
+        'endpoint_id': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'name': 'name'
+        'endpoint_id': 'endpointId'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, name=None):
+    def __init__(self, endpoint_id=None):
         # type: (Optional[str]) -> None
         """
 
-        :param name: Name of the slot that was used in this interaction.
-        :type name: (optional) str
+        :param endpoint_id: 
+        :type endpoint_id: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
-        self.name = name
+        self.endpoint_id = endpoint_id
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -91,15 +91,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, Slot):
+        if not isinstance(other, Endpoint):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/intent_confidence_bin.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/intent_confidence_bin.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/intent_requests.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/intent_requests.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/sort_field_for_intent_request_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/sort_field_for_intent_request_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/confidence_bin.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/confidence_bin.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/dialog_act.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/dialog_act.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/dialog_act_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/dialog_act_name.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/interaction_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/interaction_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/history/intent.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/history/intent.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/import_response_skill.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/import_response_skill.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/instance.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/instance.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_messaging_credentials.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_messaging_credentials.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/version_submission_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/version_submission_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/resource_schema/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/resource_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/resource_schema/get_resource_schema_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/resource_schema/get_resource_schema_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/hosted_skill_deployment_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/hosted_skill_deployment_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/create_rollback_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/create_rollback_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/regional_ssl_certificate.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/regional_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_resource_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_resource_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/import_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/import_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/withdraw_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/withdraw_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/export_response_skill.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/export_response_skill.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/build_details.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/build_details.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_interaction_model_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_interaction_model_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/create_skill_with_package_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/create_skill_with_package_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/create_skill_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/create_skill_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/beta_test.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/beta_test.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/update_beta_test_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/update_beta_test_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/tester_with_details.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/tester_with_details.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/list_testers_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/list_testers_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/tester.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/tester.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/invitation_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/invitation_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/testers/testers_list.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/testers/testers_list.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/beta_test/test_body.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/beta_test/test_body.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/overwrite_mode.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/overwrite_mode.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/format.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/format.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/upload_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/upload_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_credentials.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_credentials.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/account_linking_platform_authorization_url.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/account_linking_platform_authorization_url.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/account_linking_request_payload.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/account_linking_request_payload.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/account_linking_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/account_linking_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/access_token_scheme_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/access_token_scheme_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/account_linking_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/account_linking_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/account_linking_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/account_linking_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/account_linking/platform_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/account_linking/platform_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_summary_apis.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_summary_apis.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_failure_reason.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_failure_reason.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/export_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/export_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/clone_locale_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/clone_locale_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/list_nlu_evaluations_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/list_nlu_evaluations_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/pagination_context.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/pagination_context.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_results_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_results_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/results_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/results_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/results.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/results.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_status_code.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_status_code.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/paged_results_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/paged_results_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/expected_intent_slots_props.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/expected_intent_slots_props.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/evaluate_nlu_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/evaluate_nlu_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_response_links.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_response_links.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/actual.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/actual.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/test_case.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/test_case.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/evaluation.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/evaluation.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/paged_results_response_pagination_context.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/paged_results_response_pagination_context.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/evaluation_entity.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/evaluation_entity.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/links.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/links.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/inputs.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/inputs.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/expected.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/expected.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/confirmation_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/confirmation_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/evaluation_inputs.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/evaluation_inputs.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/paged_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/paged_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/evaluate_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/evaluate_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/expected_intent.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/expected_intent.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/resolutions.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/resolutions.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/slots_props.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/slots_props.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/get_nlu_evaluation_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_value.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/resolutions_per_authority_value.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/source.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/source.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/evaluations/intent.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/evaluations/intent.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/update_nlu_annotation_set_annotations_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/update_nlu_annotation_set_annotations_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/list_nlu_annotation_sets_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/list_nlu_annotation_sets_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/create_nlu_annotation_set_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/create_nlu_annotation_set_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/pagination_context.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/pagination_context.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/get_nlu_annotation_set_properties_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/get_nlu_annotation_set_properties_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/create_nlu_annotation_set_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/create_nlu_annotation_set_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/annotation_set_entity.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/annotation_set_entity.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/links.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/links.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/update_nlu_annotation_set_properties_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/update_nlu_annotation_set_properties_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/nlu/annotation_sets/annotation_set.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/nlu/annotation_sets/annotation_set.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/list_skill_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/list_skill_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/hosted_skill_deployment_details.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/hosted_skill_deployment_details.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/dialog_prompts.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/dialog_prompts.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/prompt_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/prompt_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/has_entity_resolution_match.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/has_entity_resolution_match.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/multiple_values_config.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/multiple_values_config.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_input.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_input.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_definition_output.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_definition_output.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/list_catalog_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/list_catalog_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/update_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/update_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_status_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_status_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/last_update_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/last_update_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_entity.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_entity.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_item.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_item.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/catalog_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog/definition_data.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog/definition_data.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_less_than.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_less_than.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_not_in_set.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_not_in_set.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/dialog_intents.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/dialog_intents.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/interaction_model_schema.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/interaction_model_schema.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/value_catalog.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/value_catalog.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_greater_than.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_greater_than.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/fallback_intent_sensitivity.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/fallback_intent_sensitivity.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_greater_than_or_equal_to.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_greater_than_or_equal_to.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/fallback_intent_sensitivity_level.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/fallback_intent_sensitivity_level.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/slot_definition.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/slot_definition.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/interaction_model_data.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/interaction_model_data.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/inline_value_supplier.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/inline_value_supplier.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/execution.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/execution.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/trigger.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/trigger.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/catalog_auto_refresh.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/catalog_auto_refresh.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/list_job_definitions_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/list_job_definitions_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/reference_version_update.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/reference_version_update.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/job_api_pagination_context.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/job_api_pagination_context.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/job_error_details.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/job_error_details.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/update_job_status_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/update_job_status_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/create_job_definition_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/create_job_definition_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/validation_errors.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/validation_errors.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/get_executions_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/get_executions_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/catalog.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/catalog.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/resource_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/resource_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition_metadata.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/job_definition_metadata.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/interaction_model.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/interaction_model.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/scheduled.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/scheduled.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/create_job_definition_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/create_job_definition_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/referenced_resource_jobs_complete.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/referenced_resource_jobs_complete.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/slot_type_reference.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/slot_type_reference.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/dynamic_update_error.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/dynamic_update_error.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/jobs/execution_metadata.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/jobs/execution_metadata.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/dialog_intents_prompts.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/dialog_intents_prompts.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_less_than_or_equal_to.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_less_than_or_equal_to.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/catalog_value_supplier.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/catalog_value_supplier.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/slot_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/slot_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_configuration.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_configuration.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_value.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_value.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_in_set.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_in_set.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_in_duration.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_in_duration.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/is_not_in_duration.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/is_not_in_duration.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflicts_response_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflicts_response_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/pagination_context.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/pagination_context.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflicts_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflicts_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_intent_slot.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/list_sh_test_plan_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,47 +21,47 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class ConflictIntentSlot(object):
+class ListSHTestPlanItem(object):
     """
 
-    :param value: 
-    :type value: (optional) str
-    :param object_type: 
-    :type object_type: (optional) str
+    :param id: 
+    :type id: (optional) str
+    :param name: 
+    :type name: (optional) str
 
     """
     deserialized_types = {
-        'value': 'str',
-        'object_type': 'str'
+        'id': 'str',
+        'name': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'value': 'value',
-        'object_type': 'type'
+        'id': 'id',
+        'name': 'name'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, value=None, object_type=None):
+    def __init__(self, id=None, name=None):
         # type: (Optional[str], Optional[str]) -> None
         """
 
-        :param value: 
-        :type value: (optional) str
-        :param object_type: 
-        :type object_type: (optional) str
+        :param id: 
+        :type id: (optional) str
+        :param name: 
+        :type name: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
-        self.value = value
-        self.object_type = object_type
+        self.id = id
+        self.name = name
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -98,15 +98,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, ConflictIntentSlot):
+        if not isinstance(other, ListSHTestPlanItem):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflict_detection_job_status_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/get_conflict_detection_job_status_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_intent.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_intent.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_detection_job_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/conflict_detection_job_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/conflict_detection/paged_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/conflict_detection/paged_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/value_supplier.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/value_supplier.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/prompt_items_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/prompt_items_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/language_model.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/language_model.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/dialog_slot_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/dialog_slot_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/dialog.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/dialog.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/prompt.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/prompt.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/version_data_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/version_data_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/version_data.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/version_data.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/list_slot_type_version_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/list_slot_type_version_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_update.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_update.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_update_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_update_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/value_supplier_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/value_supplier_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_data_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_data_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_item.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_item.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_data.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_version/slot_type_version_data.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/error.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/error.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/warning.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/warning.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_item.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_item.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_update_definition.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_update_definition.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_definition_output.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_definition_output.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/update_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/update_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/last_update_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/last_update_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_status_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_status_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_input.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_input.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/list_slot_type_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/list_slot_type_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_response_entity.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/slot_type_response_entity.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/model_type/definition_data.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/model_type/definition_data.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/type_value_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/type_value_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/slot_validation.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/slot_validation.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/list_catalog_entity_versions_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/list_catalog_entity_versions_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/list_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/list_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/version_data.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/version_data.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/catalog_entity_version.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/catalog_entity_version.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/value_schema_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/value_schema_name.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/value_schema.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/value_schema.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/catalog_values.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/catalog_values.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/links.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/links.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/catalog_update.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/catalog_update.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/catalog_version_data.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/catalog_version_data.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/version_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/version_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/version/input_source.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/version/input_source.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/delegation_strategy_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/delegation_strategy_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/interaction_model/intent.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/interaction_model/intent.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_endpoint.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_endpoint.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/alexa_hosted_config.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/alexa_hosted_config.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_runtime.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_runtime.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_metadata.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_metadata.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_region.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_region.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials_list.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials_list.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_repository_credentials_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosting_configuration.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosting_configuration.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/alexa_hosted/hosted_skill_permission_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/manifest_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/action.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/action.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/invocation_response_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/invocation_response_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/end_point_regions.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/end_point_regions.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/invoke_skill_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/invoke_skill_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/invocation_response_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/invocation_response_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/metrics.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/metrics.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/invoke_skill_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/invoke_skill_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/skill_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/skill_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
 class SkillRequest(object):
     """
 
-    :param body: ASK request body schema as defined in the public facing documentation (https://tiny.amazon.com/1h8keglep/deveamazpublsolualexalexdocs) 
+    :param body: ASK request body schema as defined in the public facing documentation (https://developer.amazon.com/en-US/docs/alexa/custom-skills/request-and-response-json-reference.html#request-body-syntax) 
     :type body: (optional) object
 
     """
     deserialized_types = {
         'body': 'object'
     }  # type: Dict
 
@@ -41,15 +41,15 @@
     }  # type: Dict
     supports_multiple_types = False
 
     def __init__(self, body=None):
         # type: (Optional[object]) -> None
         """
 
-        :param body: ASK request body schema as defined in the public facing documentation (https://tiny.amazon.com/1h8keglep/deveamazpublsolualexalexdocs) 
+        :param body: ASK request body schema as defined in the public facing documentation (https://developer.amazon.com/en-US/docs/alexa/custom-skills/request-and-response-json-reference.html#request-body-syntax) 
         :type body: (optional) object
         """
         self.__discriminator_value = None  # type: str
 
         self.body = body
 
     def to_dict(self):
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/invocations/skill_execution_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/invocations/skill_execution_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/rollback_request_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/rollback_request_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/hosted_skill_provisioning_last_update_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/hosted_skill_provisioning_last_update_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/image_size_unit.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/image_size_unit.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/validation_data_types.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/validation_data_types.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/resource_import_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/resource_import_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/skill/skill_resources_enum.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/skill_resources_enum.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/bad_request_error.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/bad_request_error.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/error.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/error.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/presigned_upload_part_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/presigned_upload_part_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/pre_signed_url.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/pre_signed_url.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/get_content_upload_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/get_content_upload_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/catalog_upload_base.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/catalog_upload_base.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/file_upload_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/file_upload_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/content_upload_file_summary.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/content_upload_file_summary.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/location.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/location.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/upload_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/upload_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/ingestion_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/ingestion_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/upload_ingestion_step.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/upload_ingestion_step.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/pre_signed_url_item.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/pre_signed_url_item.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/upload/ingestion_step_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/upload/ingestion_step_name.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/create_content_upload_url_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/create_content_upload_url_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/catalog/create_content_upload_url_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/catalog/create_content_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/client.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/client.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/requester_filter.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/requester_filter.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/sort_field.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/sort_field.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/resource.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/resource.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/request_pagination_context.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/request_pagination_context.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/resource_filter.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/resource_filter.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/sort_direction.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/sort_direction.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/request_filters.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/request_filters.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/operation_filter.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/operation_filter.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/audit_log.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/audit_log.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/audit_logs_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/audit_logs_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/client_filter.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/client_filter.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/resource_type_enum.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/requester.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/requester.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/response_pagination_context.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/response_pagination_context.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/audit_logs_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/audit_logs_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/audit_logs/operation.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/audit_logs/operation.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/evaluate_sh_capability_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/evaluate_sh_capability_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_capability_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_capability_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/evaluation_object.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/evaluation_object.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/stage.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/stage.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/endpoint.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/capability_test_plan.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,40 +21,40 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class Endpoint(object):
+class CapabilityTestPlan(object):
     """
 
-    :param endpoint_id: 
-    :type endpoint_id: (optional) str
+    :param id: 
+    :type id: (optional) str
 
     """
     deserialized_types = {
-        'endpoint_id': 'str'
+        'id': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'endpoint_id': 'endpointId'
+        'id': 'id'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, endpoint_id=None):
+    def __init__(self, id=None):
         # type: (Optional[str]) -> None
         """
 
-        :param endpoint_id: 
-        :type endpoint_id: (optional) str
+        :param id: 
+        :type id: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
-        self.endpoint_id = endpoint_id
+        self.id = id
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -91,15 +91,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, Endpoint):
+        if not isinstance(other, CapabilityTestPlan):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/pagination_context.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/pagination_context.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/capability_test_plan.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/link.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,40 +21,40 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class CapabilityTestPlan(object):
+class Link(object):
     """
 
-    :param id: 
-    :type id: (optional) str
+    :param href: 
+    :type href: (optional) str
 
     """
     deserialized_types = {
-        'id': 'str'
+        'href': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'id': 'id'
+        'href': 'href'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, id=None):
+    def __init__(self, href=None):
         # type: (Optional[str]) -> None
         """
 
-        :param id: 
-        :type id: (optional) str
+        :param href: 
+        :type href: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
-        self.id = id
+        self.href = href
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -91,15 +91,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, CapabilityTestPlan):
+        if not isinstance(other, Link):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/pagination_context_token.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocation_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,40 +21,40 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class PaginationContextToken(object):
+class InvocationResponse(object):
     """
 
-    :param next_token: 
-    :type next_token: (optional) str
+    :param body: Payload that was returned by the skill&#39;s Lambda or HTTPS endpoint. 
+    :type body: (optional) dict(str, object)
 
     """
     deserialized_types = {
-        'next_token': 'str'
+        'body': 'dict(str, object)'
     }  # type: Dict
 
     attribute_map = {
-        'next_token': 'nextToken'
+        'body': 'body'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, next_token=None):
-        # type: (Optional[str]) -> None
+    def __init__(self, body=None):
+        # type: (Optional[Dict[str, object]]) -> None
         """
 
-        :param next_token: 
-        :type next_token: (optional) str
+        :param body: Payload that was returned by the skill&#39;s Lambda or HTTPS endpoint. 
+        :type body: (optional) dict(str, object)
         """
         self.__discriminator_value = None  # type: str
 
-        self.next_token = next_token
+        self.body = body
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -91,15 +91,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, PaginationContextToken):
+        if not isinstance(other, InvocationResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_capability_error_code.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_capability_error_code.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/list_sh_test_plan_item.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/skill_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,47 +21,40 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class ListSHTestPlanItem(object):
+class SkillRequest(object):
     """
 
-    :param id: 
-    :type id: (optional) str
-    :param name: 
-    :type name: (optional) str
+    :param body: ASK request body schema as defined in the public facing documentation (https://developer.amazon.com/en-US/docs/alexa/custom-skills/request-and-response-json-reference.html#request-body-syntax) 
+    :type body: (optional) object
 
     """
     deserialized_types = {
-        'id': 'str',
-        'name': 'str'
+        'body': 'object'
     }  # type: Dict
 
     attribute_map = {
-        'id': 'id',
-        'name': 'name'
+        'body': 'body'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, id=None, name=None):
-        # type: (Optional[str], Optional[str]) -> None
+    def __init__(self, body=None):
+        # type: (Optional[object]) -> None
         """
 
-        :param id: 
-        :type id: (optional) str
-        :param name: 
-        :type name: (optional) str
+        :param body: ASK request body schema as defined in the public facing documentation (https://developer.amazon.com/en-US/docs/alexa/custom-skills/request-and-response-json-reference.html#request-body-syntax) 
+        :type body: (optional) object
         """
         self.__discriminator_value = None  # type: str
 
-        self.id = id
-        self.name = name
+        self.body = body
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -98,15 +91,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, ListSHTestPlanItem):
+        if not isinstance(other, SkillRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_evaluation_results_metric.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_evaluation_results_metric.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/list_sh_capability_evaluations_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/list_sh_capability_evaluations_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/get_sh_capability_evaluation_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/get_sh_capability_evaluation_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_capability_error.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_capability_error.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_capability_directive.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_capability_directive.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/evaluate_sh_capability_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/evaluate_sh_capability_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/sh_capability_state.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/sh_capability_state.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/test_case_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/test_case_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/test_case_result_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/test_case_result_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/paged_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/paged_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/evaluation_entity_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/evaluation_entity_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/list_sh_capability_test_plans_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/list_sh_capability_test_plans_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/smart_home_evaluation/get_sh_capability_evaluation_results_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/smart_home_evaluation/get_sh_capability_evaluation_results_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/link.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/input.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,40 +21,40 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class Link(object):
+class Input(object):
     """
 
-    :param href: 
-    :type href: (optional) str
+    :param content: A string corresponding to the utterance text of what a customer would say to Alexa. 
+    :type content: (optional) str
 
     """
     deserialized_types = {
-        'href': 'str'
+        'content': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'href': 'href'
+        'content': 'content'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, href=None):
+    def __init__(self, content=None):
         # type: (Optional[str]) -> None
         """
 
-        :param href: 
-        :type href: (optional) str
+        :param content: A string corresponding to the utterance text of what a customer would say to Alexa. 
+        :type content: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
-        self.href = href
+        self.content = content
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -91,15 +91,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, Link):
+        if not isinstance(other, Input):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/editable_state.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/editable_state.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/in_skill_product_summary_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/in_skill_product_summary_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/update_in_skill_product_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/update_in_skill_product_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/product_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/product_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/currency.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/currency.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/associated_skill_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/associated_skill_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/tax_information.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/tax_information.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/summary_price_listing.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/summary_price_listing.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/localized_publishing_information.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/localized_publishing_information.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/promotable_state.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/promotable_state.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/in_skill_product_definition.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/in_skill_product_definition.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/create_in_skill_product_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/create_in_skill_product_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/subscription_information.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/subscription_information.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/subscription_payment_frequency.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/subscription_payment_frequency.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/product_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/product_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/distribution_countries.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/distribution_countries.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/in_skill_product_summary.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/in_skill_product_summary.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/tax_information_category.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/tax_information_category.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/price_listing.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/price_listing.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/purchasable_state.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/purchasable_state.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/privacy_and_compliance.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/privacy_and_compliance.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/localized_privacy_and_compliance.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/localized_privacy_and_compliance.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/summary_marketplace_pricing.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/summary_marketplace_pricing.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/marketplace_pricing.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/marketplace_pricing.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/list_in_skill_product_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/list_in_skill_product_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/custom_product_prompts.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/custom_product_prompts.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/isp_summary_links.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/isp_summary_links.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/list_in_skill_product.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/list_in_skill_product.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/in_skill_product_definition_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/in_skill_product_definition_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/isp/publishing_information.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/isp/publishing_information.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/stage_v2_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/stage_v2_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/vendor_management/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/vendor_management/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/vendor_management/vendor.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/vendor_management/vendor.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/vendor_management/vendors.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/vendor_management/vendors.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v1/links.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/links.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/alexa_response_content.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/alexa_response_content.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/confirmation_status_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/confirmation_status_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/simulations_api_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/simulations_api_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/input.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/endpoint_aws_authorization.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,47 +14,54 @@
 #
 
 import pprint
 import re  # noqa: F401
 import six
 import typing
 from enum import Enum
+from ask_smapi_model.v0.development_events.subscriber.endpoint_authorization import EndpointAuthorization
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class Input(object):
+class EndpointAwsAuthorization(EndpointAuthorization):
     """
+    Authorization for accessing AWS SNS endpoint.
 
-    :param content: A string corresponding to the utterance text of what a customer would say to Alexa. 
-    :type content: (optional) str
+
+    :param arn: IAM Role arn to use/assumeRole for authorization.
+    :type arn: (optional) str
 
     """
     deserialized_types = {
-        'content': 'str'
+        'object_type': 'str',
+        'arn': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'content': 'content'
+        'object_type': 'type',
+        'arn': 'arn'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, content=None):
+    def __init__(self, arn=None):
         # type: (Optional[str]) -> None
-        """
+        """Authorization for accessing AWS SNS endpoint.
 
-        :param content: A string corresponding to the utterance text of what a customer would say to Alexa. 
-        :type content: (optional) str
+        :param arn: IAM Role arn to use/assumeRole for authorization.
+        :type arn: (optional) str
         """
-        self.__discriminator_value = None  # type: str
+        self.__discriminator_value = "AWS_IAM"  # type: str
 
-        self.content = content
+        self.object_type = self.__discriminator_value
+        super(EndpointAwsAuthorization, self).__init__(object_type=self.__discriminator_value)
+        self.arn = arn
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -91,15 +98,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, Input):
+        if not isinstance(other, EndpointAwsAuthorization):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/simulations_api_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/simulations_api_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/slot_resolutions.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/slot_resolutions.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/slot.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/slot.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/simulation_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/simulation_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_status_code.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_status_code.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/simulations_api_response_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/simulations_api_response_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_value_items.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_value_items.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/alexa_execution_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/alexa_execution_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/device.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/device.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/alexa_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/alexa_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/session.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/session.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/resolutions_per_authority_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/skill_execution_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/skill_execution_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/session_mode.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/session_mode.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/simulations/intent.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/simulations/intent.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocation_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocation_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/metrics.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/metrics.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocation_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/update_subscriber_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,42 +19,50 @@
 import typing
 from enum import Enum
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
+    from ask_smapi_model.v0.development_events.subscriber.endpoint import Endpoint as Endpoint_7e4d296f
 
 
-class InvocationResponse(object):
+class UpdateSubscriberRequest(object):
     """
 
-    :param body: Payload that was returned by the skill&#39;s Lambda or HTTPS endpoint. 
-    :type body: (optional) dict(str, object)
+    :param name: Name of the subscriber.
+    :type name: (optional) str
+    :param endpoint: 
+    :type endpoint: (optional) ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint
 
     """
     deserialized_types = {
-        'body': 'dict(str, object)'
+        'name': 'str',
+        'endpoint': 'ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint'
     }  # type: Dict
 
     attribute_map = {
-        'body': 'body'
+        'name': 'name',
+        'endpoint': 'endpoint'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, body=None):
-        # type: (Optional[Dict[str, object]]) -> None
+    def __init__(self, name=None, endpoint=None):
+        # type: (Optional[str], Optional[Endpoint_7e4d296f]) -> None
         """
 
-        :param body: Payload that was returned by the skill&#39;s Lambda or HTTPS endpoint. 
-        :type body: (optional) dict(str, object)
+        :param name: Name of the subscriber.
+        :type name: (optional) str
+        :param endpoint: 
+        :type endpoint: (optional) ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint
         """
         self.__discriminator_value = None  # type: str
 
-        self.body = body
+        self.name = name
+        self.endpoint = endpoint
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -91,15 +99,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, InvocationResponse):
+        if not isinstance(other, UpdateSubscriberRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocation.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocation.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/invocation_response_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/request_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class InvocationResponseStatus(Enum):
+class RequestStatus(Enum):
     """
-    String that specifies the status of skill invocation. Possible values are \&quot;SUCCEEDED\&quot;, and \&quot;FAILED\&quot;. 
+    Represents the completion status of the request. 
 
 
 
     Allowed enum values: [SUCCEEDED, FAILED]
     """
     SUCCEEDED = "SUCCEEDED"
     FAILED = "FAILED"
@@ -51,15 +51,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, InvocationResponseStatus):
+        if not isinstance(other, RequestStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/invocations_api_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/invocations_api_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/end_point_regions.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/end_point_regions.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/invocation_response_result.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/invocation_response_result.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/skill_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/subscription_attributes.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,40 +21,42 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class SkillRequest(object):
+class SubscriptionAttributes(object):
     """
+    Represents attributes of a subscription for development notification. 
 
-    :param body: ASK request body schema as defined in the public facing documentation (https://tiny.amazon.com/1h8keglep/deveamazpublsolualexalexdocs) 
-    :type body: (optional) object
+
+    :param subscription_id: Unique subscription id that triggered the development notification event. 
+    :type subscription_id: (optional) str
 
     """
     deserialized_types = {
-        'body': 'object'
+        'subscription_id': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'body': 'body'
+        'subscription_id': 'subscriptionId'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, body=None):
-        # type: (Optional[object]) -> None
-        """
+    def __init__(self, subscription_id=None):
+        # type: (Optional[str]) -> None
+        """Represents attributes of a subscription for development notification. 
 
-        :param body: ASK request body schema as defined in the public facing documentation (https://tiny.amazon.com/1h8keglep/deveamazpublsolualexalexdocs) 
-        :type body: (optional) object
+        :param subscription_id: Unique subscription id that triggered the development notification event. 
+        :type subscription_id: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
-        self.body = body
+        self.subscription_id = subscription_id
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -91,15 +93,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, SkillRequest):
+        if not isinstance(other, SubscriptionAttributes):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/skill/invocations/invocations_api_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/invocations_api_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/bad_request_error.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/bad_request_error.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/error.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/error.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v2/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/__version__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for
 # the specific language governing permissions and limitations under the License.
 #
 
 __pip_package_name__ = 'ask-smapi-model'
 __description__ = 'The SMAPI SDK Model package provides model definitions for making Skill Management API calls.'
 __url__ = 'https://github.com/alexa/alexa-apis-for-python'
-__version__ = '1.9.1'
+__version__ = '1.9.2'
 __author__ = 'Alexa Skills Kit'
 __author_email__ = 'ask-sdk-dynamic@amazon.com'
 __license__ = 'Apache 2.0'
 __keywords__ = ['SMAPI SDK', 'ASK SDK', 'Alexa Skills Kit', 'Alexa', 'Models', 'Smapi']
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/services/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/services/skill_management/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/services/skill_management/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/services/skill_management/skill_management_service_client.py` & `ask-smapi-model-1.9.2/ask_smapi_model/services/skill_management/skill_management_service_client.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/bad_request_error.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/bad_request_error.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/error.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/error.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/skill_review_publish.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_customer_feedback_event/skill_review_publish.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/skill_attributes.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/skill_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/actor_attributes.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/actor_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/request_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/upload_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,24 +21,26 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class RequestStatus(Enum):
+class UploadStatus(Enum):
     """
-    Represents the completion status of the request. 
+    Status of the entire upload.
 
 
 
-    Allowed enum values: [SUCCEEDED, FAILED]
+    Allowed enum values: [PENDING, PROCESSING, FAILED, SUCCEEDED]
     """
-    SUCCEEDED = "SUCCEEDED"
+    PENDING = "PENDING"
+    PROCESSING = "PROCESSING"
     FAILED = "FAILED"
+    SUCCEEDED = "SUCCEEDED"
 
     def to_dict(self):
         # type: () -> Dict[str, Any]
         """Returns the model properties as a dict"""
         result = {self.name: self.value}
         return result
 
@@ -51,15 +53,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, RequestStatus):
+        if not isinstance(other, UploadStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/subscription_attributes.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/update_subscription_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,44 +19,50 @@
 import typing
 from enum import Enum
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
+    from ask_smapi_model.v0.development_events.subscription.event import Event as Event_a93e65dc
 
 
-class SubscriptionAttributes(object):
+class UpdateSubscriptionRequest(object):
     """
-    Represents attributes of a subscription for development notification. 
 
-
-    :param subscription_id: Unique subscription id that triggered the development notification event. 
-    :type subscription_id: (optional) str
+    :param name: Name of the subscription.
+    :type name: (optional) str
+    :param events: The list of events that the subscriber should be notified for.
+    :type events: (optional) list[ask_smapi_model.v0.development_events.subscription.event.Event]
 
     """
     deserialized_types = {
-        'subscription_id': 'str'
+        'name': 'str',
+        'events': 'list[ask_smapi_model.v0.development_events.subscription.event.Event]'
     }  # type: Dict
 
     attribute_map = {
-        'subscription_id': 'subscriptionId'
+        'name': 'name',
+        'events': 'events'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, subscription_id=None):
-        # type: (Optional[str]) -> None
-        """Represents attributes of a subscription for development notification. 
+    def __init__(self, name=None, events=None):
+        # type: (Optional[str], Optional[List[Event_a93e65dc]]) -> None
+        """
 
-        :param subscription_id: Unique subscription id that triggered the development notification event. 
-        :type subscription_id: (optional) str
+        :param name: Name of the subscription.
+        :type name: (optional) str
+        :param events: The list of events that the subscriber should be notified for.
+        :type events: (optional) list[ask_smapi_model.v0.development_events.subscription.event.Event]
         """
         self.__discriminator_value = None  # type: str
 
-        self.subscription_id = subscription_id
+        self.name = name
+        self.events = events
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -93,15 +99,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, SubscriptionAttributes):
+        if not isinstance(other, UpdateSubscriptionRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/base_schema.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/skill_review_event_attributes.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/skill_review_event_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/skill_review_attributes.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/skill_review_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/skill_event_attributes.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/skill_event_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/interaction_model_attributes.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/interaction_model_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,39 +31,46 @@
     Represents a set of attributes specific to interaction model of an Alexa Skill. 
 
 
     :param skill_id: Unique identifier of an Alexa skill. 
     :type skill_id: (optional) str
     :param vendor_id: Unique identifier of vendor account to which this skill belongs. 
     :type vendor_id: (optional) str
+    :param locale: Locale of interaction model. 
+    :type locale: (optional) str
 
     """
     deserialized_types = {
         'skill_id': 'str',
-        'vendor_id': 'str'
+        'vendor_id': 'str',
+        'locale': 'str'
     }  # type: Dict
 
     attribute_map = {
         'skill_id': 'skillId',
-        'vendor_id': 'vendorId'
+        'vendor_id': 'vendorId',
+        'locale': 'locale'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, skill_id=None, vendor_id=None):
-        # type: (Optional[str], Optional[str]) -> None
+    def __init__(self, skill_id=None, vendor_id=None, locale=None):
+        # type: (Optional[str], Optional[str], Optional[str]) -> None
         """Represents a set of attributes specific to interaction model of an Alexa Skill. 
 
         :param skill_id: Unique identifier of an Alexa skill. 
         :type skill_id: (optional) str
         :param vendor_id: Unique identifier of vendor account to which this skill belongs. 
         :type vendor_id: (optional) str
+        :param locale: Locale of interaction model. 
+        :type locale: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
         super(InteractionModelAttributes, self).__init__(skill_id=skill_id, vendor_id=vendor_id)
+        self.locale = locale
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/manifest_update.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/manifest_update.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/interaction_model_update.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/interaction_model_update.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/skill_publish.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/skill_publish.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/alexa_development_event/skill_certification.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/alexa_development_event/skill_certification.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/event_schema/interaction_model_event_attributes.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/event_schema/interaction_model_event_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/list_catalogs_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/list_catalogs_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/catalog_summary.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/catalog_summary.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/create_content_upload_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/create_content_upload_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/get_content_upload_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/get_content_upload_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/presigned_upload_part.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/presigned_upload_part.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/file_upload_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/file_upload_status.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/content_upload_file_summary.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/content_upload_file_summary.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/list_uploads_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/list_uploads_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/upload_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/ingestion_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,26 +21,25 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class UploadStatus(Enum):
+class IngestionStatus(Enum):
     """
-    Status of the entire upload.
 
 
-
-    Allowed enum values: [PENDING, PROCESSING, FAILED, SUCCEEDED]
+    Allowed enum values: [PENDING, IN_PROGRESS, FAILED, SUCCEEDED, CANCELLED]
     """
     PENDING = "PENDING"
-    PROCESSING = "PROCESSING"
+    IN_PROGRESS = "IN_PROGRESS"
     FAILED = "FAILED"
     SUCCEEDED = "SUCCEEDED"
+    CANCELLED = "CANCELLED"
 
     def to_dict(self):
         # type: () -> Dict[str, Any]
         """Returns the model properties as a dict"""
         result = {self.name: self.value}
         return result
 
@@ -53,15 +52,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, UploadStatus):
+        if not isinstance(other, IngestionStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/complete_upload_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/complete_upload_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/content_upload_summary.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/content_upload_summary.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/ingestion_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/ingestion_step_name.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,25 +21,22 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class IngestionStatus(Enum):
+class IngestionStepName(Enum):
     """
 
 
-    Allowed enum values: [PENDING, IN_PROGRESS, FAILED, SUCCEEDED, CANCELLED]
+    Allowed enum values: [UPLOAD, SCHEMA_VALIDATION]
     """
-    PENDING = "PENDING"
-    IN_PROGRESS = "IN_PROGRESS"
-    FAILED = "FAILED"
-    SUCCEEDED = "SUCCEEDED"
-    CANCELLED = "CANCELLED"
+    UPLOAD = "UPLOAD"
+    SCHEMA_VALIDATION = "SCHEMA_VALIDATION"
 
     def to_dict(self):
         # type: () -> Dict[str, Any]
         """Returns the model properties as a dict"""
         result = {self.name: self.value}
         return result
 
@@ -52,15 +49,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, IngestionStatus):
+        if not isinstance(other, IngestionStepName):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/upload_ingestion_step.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/upload_ingestion_step.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/pre_signed_url_item.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/pre_signed_url_item.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/create_content_upload_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/upload/create_content_upload_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/upload/ingestion_step_name.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/subscriber_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,22 +21,24 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class IngestionStepName(Enum):
+class SubscriberStatus(Enum):
     """
+    Status of the subscriber. This enum may get extended with new values in future. Clients are expected to gracefully handle any unknown values.
 
 
-    Allowed enum values: [UPLOAD, SCHEMA_VALIDATION]
+
+    Allowed enum values: [ACTIVE, INACTIVE]
     """
-    UPLOAD = "UPLOAD"
-    SCHEMA_VALIDATION = "SCHEMA_VALIDATION"
+    ACTIVE = "ACTIVE"
+    INACTIVE = "INACTIVE"
 
     def to_dict(self):
         # type: () -> Dict[str, Any]
         """Returns the model properties as a dict"""
         result = {self.name: self.value}
         return result
 
@@ -49,15 +51,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, IngestionStepName):
+        if not isinstance(other, SubscriberStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/catalog_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/catalog_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/catalog_details.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/catalog_details.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/catalog_usage.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/catalog_usage.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/catalog/create_catalog_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/catalog/create_catalog_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/subscription_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/subscription_info.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/update_subscription_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/create_subscriber_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,50 +19,57 @@
 import typing
 from enum import Enum
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
-    from ask_smapi_model.v0.development_events.subscription.event import Event as Event_a93e65dc
+    from ask_smapi_model.v0.development_events.subscriber.endpoint import Endpoint as Endpoint_7e4d296f
 
 
-class UpdateSubscriptionRequest(object):
+class CreateSubscriberRequest(object):
     """
 
-    :param name: Name of the subscription.
+    :param name: Name of the subscriber.
     :type name: (optional) str
-    :param events: The list of events that the subscriber should be notified for.
-    :type events: (optional) list[ask_smapi_model.v0.development_events.subscription.event.Event]
+    :param vendor_id: The Vendor ID.
+    :type vendor_id: (optional) str
+    :param endpoint: 
+    :type endpoint: (optional) ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint
 
     """
     deserialized_types = {
         'name': 'str',
-        'events': 'list[ask_smapi_model.v0.development_events.subscription.event.Event]'
+        'vendor_id': 'str',
+        'endpoint': 'ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint'
     }  # type: Dict
 
     attribute_map = {
         'name': 'name',
-        'events': 'events'
+        'vendor_id': 'vendorId',
+        'endpoint': 'endpoint'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, name=None, events=None):
-        # type: (Optional[str], Optional[List[Event_a93e65dc]]) -> None
+    def __init__(self, name=None, vendor_id=None, endpoint=None):
+        # type: (Optional[str], Optional[str], Optional[Endpoint_7e4d296f]) -> None
         """
 
-        :param name: Name of the subscription.
+        :param name: Name of the subscriber.
         :type name: (optional) str
-        :param events: The list of events that the subscriber should be notified for.
-        :type events: (optional) list[ask_smapi_model.v0.development_events.subscription.event.Event]
+        :param vendor_id: The Vendor ID.
+        :type vendor_id: (optional) str
+        :param endpoint: 
+        :type endpoint: (optional) ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint
         """
         self.__discriminator_value = None  # type: str
 
         self.name = name
-        self.events = events
+        self.vendor_id = vendor_id
+        self.endpoint = endpoint
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -99,15 +106,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, UpdateSubscriptionRequest):
+        if not isinstance(other, CreateSubscriberRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/list_subscriptions_response.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/list_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/subscription_summary.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/subscription_summary.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/event.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/event.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscription/create_subscription_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscription/create_subscription_request.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/endpoint.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/endpoint.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/update_subscriber_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/subscriber_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,45 +22,54 @@
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
     from ask_smapi_model.v0.development_events.subscriber.endpoint import Endpoint as Endpoint_7e4d296f
 
 
-class UpdateSubscriberRequest(object):
+class SubscriberInfo(object):
     """
+    Information about the subscriber.
 
+
+    :param subscriber_id: Unique identifier of the subscriber resource.
+    :type subscriber_id: (optional) str
     :param name: Name of the subscriber.
     :type name: (optional) str
     :param endpoint: 
     :type endpoint: (optional) ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint
 
     """
     deserialized_types = {
+        'subscriber_id': 'str',
         'name': 'str',
         'endpoint': 'ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint'
     }  # type: Dict
 
     attribute_map = {
+        'subscriber_id': 'subscriberId',
         'name': 'name',
         'endpoint': 'endpoint'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, name=None, endpoint=None):
-        # type: (Optional[str], Optional[Endpoint_7e4d296f]) -> None
-        """
+    def __init__(self, subscriber_id=None, name=None, endpoint=None):
+        # type: (Optional[str], Optional[str], Optional[Endpoint_7e4d296f]) -> None
+        """Information about the subscriber.
 
+        :param subscriber_id: Unique identifier of the subscriber resource.
+        :type subscriber_id: (optional) str
         :param name: Name of the subscriber.
         :type name: (optional) str
         :param endpoint: 
         :type endpoint: (optional) ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint
         """
         self.__discriminator_value = None  # type: str
 
+        self.subscriber_id = subscriber_id
         self.name = name
         self.endpoint = endpoint
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
@@ -99,15 +108,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, UpdateSubscriberRequest):
+        if not isinstance(other, SubscriberInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/__init__.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/subscriber_status.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v2/skill/invocations/invocation_response_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
 
 
-class SubscriberStatus(Enum):
+class InvocationResponseStatus(Enum):
     """
-    Status of the subscriber. This enum may get extended with new values in future. Clients are expected to gracefully handle any unknown values.
+    String that specifies the status of skill invocation. Possible values are \&quot;SUCCESSFUL\&quot;, and \&quot;FAILED\&quot;. 
 
 
 
-    Allowed enum values: [ACTIVE, INACTIVE]
+    Allowed enum values: [SUCCESSFUL, FAILED]
     """
-    ACTIVE = "ACTIVE"
-    INACTIVE = "INACTIVE"
+    SUCCESSFUL = "SUCCESSFUL"
+    FAILED = "FAILED"
 
     def to_dict(self):
         # type: () -> Dict[str, Any]
         """Returns the model properties as a dict"""
         result = {self.name: self.value}
         return result
 
@@ -51,15 +51,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, SubscriberStatus):
+        if not isinstance(other, InvocationResponseStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (Any) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/subscriber_info.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v1/skill/manifest/authorized_client_lwa_application_android.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,64 +14,64 @@
 #
 
 import pprint
 import re  # noqa: F401
 import six
 import typing
 from enum import Enum
+from ask_smapi_model.v1.skill.manifest.authorized_client_lwa_application import AuthorizedClientLwaApplication
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
-    from ask_smapi_model.v0.development_events.subscriber.endpoint import Endpoint as Endpoint_7e4d296f
 
 
-class SubscriberInfo(object):
+class AuthorizedClientLwaApplicationAndroid(AuthorizedClientLwaApplication):
     """
-    Information about the subscriber.
+    Defines an android application for LWA authentication provider.
 
 
-    :param subscriber_id: Unique identifier of the subscriber resource.
-    :type subscriber_id: (optional) str
-    :param name: Name of the subscriber.
-    :type name: (optional) str
-    :param endpoint: 
-    :type endpoint: (optional) ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint
+    :param object_type: 
+    :type object_type: (optional) str
+    :param app_store_app_id: 
+    :type app_store_app_id: (optional) str
+    :param client_id: 
+    :type client_id: (optional) str
 
     """
     deserialized_types = {
-        'subscriber_id': 'str',
-        'name': 'str',
-        'endpoint': 'ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint'
+        'object_type': 'str',
+        'app_store_app_id': 'str',
+        'client_id': 'str'
     }  # type: Dict
 
     attribute_map = {
-        'subscriber_id': 'subscriberId',
-        'name': 'name',
-        'endpoint': 'endpoint'
+        'object_type': 'type',
+        'app_store_app_id': 'appStoreAppId',
+        'client_id': 'clientId'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, subscriber_id=None, name=None, endpoint=None):
-        # type: (Optional[str], Optional[str], Optional[Endpoint_7e4d296f]) -> None
-        """Information about the subscriber.
-
-        :param subscriber_id: Unique identifier of the subscriber resource.
-        :type subscriber_id: (optional) str
-        :param name: Name of the subscriber.
-        :type name: (optional) str
-        :param endpoint: 
-        :type endpoint: (optional) ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint
+    def __init__(self, object_type=None, app_store_app_id=None, client_id=None):
+        # type: (Optional[str], Optional[str], Optional[str]) -> None
+        """Defines an android application for LWA authentication provider.
+
+        :param object_type: 
+        :type object_type: (optional) str
+        :param app_store_app_id: 
+        :type app_store_app_id: (optional) str
+        :param client_id: 
+        :type client_id: (optional) str
         """
         self.__discriminator_value = None  # type: str
 
-        self.subscriber_id = subscriber_id
-        self.name = name
-        self.endpoint = endpoint
+        super(AuthorizedClientLwaApplicationAndroid, self).__init__(object_type=object_type)
+        self.app_store_app_id = app_store_app_id
+        self.client_id = client_id
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -108,15 +108,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, SubscriberInfo):
+        if not isinstance(other, AuthorizedClientLwaApplicationAndroid):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/endpoint_authorization.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/endpoint_authorization.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/create_subscriber_request.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/list_subscribers_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,57 +19,58 @@
 import typing
 from enum import Enum
 
 
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any
     from datetime import datetime
-    from ask_smapi_model.v0.development_events.subscriber.endpoint import Endpoint as Endpoint_7e4d296f
+    from ask_smapi_model.v1.links import Links as Links_bc43467b
+    from ask_smapi_model.v0.development_events.subscriber.subscriber_summary import SubscriberSummary as SubscriberSummary_3b34977e
 
 
-class CreateSubscriberRequest(object):
+class ListSubscribersResponse(object):
     """
 
-    :param name: Name of the subscriber.
-    :type name: (optional) str
-    :param vendor_id: The Vendor ID.
-    :type vendor_id: (optional) str
-    :param endpoint: 
-    :type endpoint: (optional) ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint
+    :param links: 
+    :type links: (optional) ask_smapi_model.v1.links.Links
+    :param next_token: 
+    :type next_token: (optional) str
+    :param subscribers: List containing subscriber summary.
+    :type subscribers: (optional) list[ask_smapi_model.v0.development_events.subscriber.subscriber_summary.SubscriberSummary]
 
     """
     deserialized_types = {
-        'name': 'str',
-        'vendor_id': 'str',
-        'endpoint': 'ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint'
+        'links': 'ask_smapi_model.v1.links.Links',
+        'next_token': 'str',
+        'subscribers': 'list[ask_smapi_model.v0.development_events.subscriber.subscriber_summary.SubscriberSummary]'
     }  # type: Dict
 
     attribute_map = {
-        'name': 'name',
-        'vendor_id': 'vendorId',
-        'endpoint': 'endpoint'
+        'links': '_links',
+        'next_token': 'nextToken',
+        'subscribers': 'subscribers'
     }  # type: Dict
     supports_multiple_types = False
 
-    def __init__(self, name=None, vendor_id=None, endpoint=None):
-        # type: (Optional[str], Optional[str], Optional[Endpoint_7e4d296f]) -> None
+    def __init__(self, links=None, next_token=None, subscribers=None):
+        # type: (Optional[Links_bc43467b], Optional[str], Optional[List[SubscriberSummary_3b34977e]]) -> None
         """
 
-        :param name: Name of the subscriber.
-        :type name: (optional) str
-        :param vendor_id: The Vendor ID.
-        :type vendor_id: (optional) str
-        :param endpoint: 
-        :type endpoint: (optional) ask_smapi_model.v0.development_events.subscriber.endpoint.Endpoint
+        :param links: 
+        :type links: (optional) ask_smapi_model.v1.links.Links
+        :param next_token: 
+        :type next_token: (optional) str
+        :param subscribers: List containing subscriber summary.
+        :type subscribers: (optional) list[ask_smapi_model.v0.development_events.subscriber.subscriber_summary.SubscriberSummary]
         """
         self.__discriminator_value = None  # type: str
 
-        self.name = name
-        self.vendor_id = vendor_id
-        self.endpoint = endpoint
+        self.links = links
+        self.next_token = next_token
+        self.subscribers = subscribers
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}  # type: Dict
 
         for attr, _ in six.iteritems(self.deserialized_types):
@@ -106,15 +107,15 @@
         # type: () -> str
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateSubscriberRequest):
+        if not isinstance(other, ListSubscribersResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         # type: (object) -> bool
         """Returns true if both objects are not equal"""
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/endpoint_authorization_type.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/endpoint_authorization_type.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model/v0/development_events/subscriber/subscriber_summary.py` & `ask-smapi-model-1.9.2/ask_smapi_model/v0/development_events/subscriber/subscriber_summary.py`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model.egg-info/SOURCES.txt` & `ask-smapi-model-1.9.2/ask_smapi_model.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,14 @@
 ask_smapi_model/v1/skill/manifest/video_catalog_info.py
 ask_smapi_model/v1/skill/manifest/video_country_info.py
 ask_smapi_model/v1/skill/manifest/video_feature.py
 ask_smapi_model/v1/skill/manifest/video_fire_tv_catalog_ingestion.py
 ask_smapi_model/v1/skill/manifest/video_prompt_name.py
 ask_smapi_model/v1/skill/manifest/video_prompt_name_type.py
 ask_smapi_model/v1/skill/manifest/video_region.py
-ask_smapi_model/v1/skill/manifest/video_web_player_feature.py
 ask_smapi_model/v1/skill/manifest/viewport_mode.py
 ask_smapi_model/v1/skill/manifest/viewport_shape.py
 ask_smapi_model/v1/skill/manifest/viewport_specification.py
 ask_smapi_model/v1/skill/manifest/voice_profile_feature.py
 ask_smapi_model/v1/skill/manifest/custom/__init__.py
 ask_smapi_model/v1/skill/manifest/custom/connection.py
 ask_smapi_model/v1/skill/manifest/custom/py.typed
```

### Comparing `ask-smapi-model-1.9.1/ask_smapi_model.egg-info/PKG-INFO` & `ask-smapi-model-1.9.2/ask_smapi_model.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ask-smapi-model
-Version: 1.9.1
+Version: 1.9.2
 Summary: The SMAPI SDK Model package provides model definitions for making Skill Management API calls.
 Home-page: https://github.com/alexa/alexa-apis-for-python
 Author: Alexa Skills Kit
 Author-email: ask-sdk-dynamic@amazon.com
 License: Apache 2.0
 Description: =================================================
         ASK SMAPI Model - Model definitions for SMAPI SDK
@@ -198,14 +198,22 @@
         
         This release contains the following changes :
         
         - General bug fixes and updates.
         - Model definition updates to support `AlexaCustomerFeedbackEvent.SkillReviewPublish <https://developer.amazon.com/en-US/docs/alexa/sdns/skill-development-event-schemas.html#events-summary>`__ event notifications for skill developers in SMAPI.
         - Developers can subscribe to this `new event and get notified <https://developer.amazon.com/en-US/docs/alexa/sdns/use-skill-development-notifications.html>`__ whenever there is a customer-review published for their skills.
         
+        
+        1.9.2
+        ^^^^^
+        
+        This release contains the following changes :
+        
+        - general bug fixes and updates
+        
 Keywords: SMAPI SDK,ASK SDK,Alexa Skills Kit,Alexa,Models,Smapi
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ask-smapi-model-1.9.1/LICENSE` & `ask-smapi-model-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ask-smapi-model-1.9.1/PKG-INFO` & `ask-smapi-model-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ask-smapi-model
-Version: 1.9.1
+Version: 1.9.2
 Summary: The SMAPI SDK Model package provides model definitions for making Skill Management API calls.
 Home-page: https://github.com/alexa/alexa-apis-for-python
 Author: Alexa Skills Kit
 Author-email: ask-sdk-dynamic@amazon.com
 License: Apache 2.0
 Description: =================================================
         ASK SMAPI Model - Model definitions for SMAPI SDK
@@ -198,14 +198,22 @@
         
         This release contains the following changes :
         
         - General bug fixes and updates.
         - Model definition updates to support `AlexaCustomerFeedbackEvent.SkillReviewPublish <https://developer.amazon.com/en-US/docs/alexa/sdns/skill-development-event-schemas.html#events-summary>`__ event notifications for skill developers in SMAPI.
         - Developers can subscribe to this `new event and get notified <https://developer.amazon.com/en-US/docs/alexa/sdns/use-skill-development-notifications.html>`__ whenever there is a customer-review published for their skills.
         
+        
+        1.9.2
+        ^^^^^
+        
+        This release contains the following changes :
+        
+        - general bug fixes and updates
+        
 Keywords: SMAPI SDK,ASK SDK,Alexa Skills Kit,Alexa,Models,Smapi
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ask-smapi-model-1.9.1/setup.py` & `ask-smapi-model-1.9.2/setup.py`

 * *Files identical despite different names*

