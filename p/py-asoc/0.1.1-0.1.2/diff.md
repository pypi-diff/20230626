# Comparing `tmp/py_asoc-0.1.1.tar.gz` & `tmp/py_asoc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_asoc-0.1.1.tar", max compression
+gzip compressed data, was "py_asoc-0.1.2.tar", max compression
```

## Comparing `py_asoc-0.1.1.tar` & `py_asoc-0.1.2.tar`

### file list

```diff
@@ -1,193 +1,193 @@
--rw-r--r--   0        0        0     1056 2023-06-21 19:57:13.234134 py_asoc-0.1.1/LICENSE
--rw-r--r--   0        0        0      458 2023-06-21 19:57:28.902167 py_asoc-0.1.1/README.md
--rw-r--r--   0        0        0     3663 2023-06-26 15:02:23.612944 py_asoc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      701 2023-06-26 15:02:23.612944 py_asoc-0.1.1/src/pyasoc/__init__.py
--rw-r--r--   0        0        0       47 2023-06-20 17:19:48.801799 py_asoc-0.1.1/src/pyasoc/api/__init__.py
--rw-r--r--   0        0        0    26867 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/api/account_api.py
--rw-r--r--   0        0        0    80163 2023-06-23 20:09:33.904449 py_asoc-0.1.1/src/pyasoc/api/apps_api.py
--rw-r--r--   0        0        0    31131 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/api/asset_groups_api.py
--rw-r--r--   0        0        0    27522 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/api/business_units_api.py
--rw-r--r--   0        0        0    22350 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/api/domains_api.py
--rw-r--r--   0        0        0     7576 2023-06-22 14:55:38.934298 py_asoc-0.1.1/src/pyasoc/api/file_upload_api.py
--rw-r--r--   0        0        0    34193 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/api/fix_groups_api.py
--rw-r--r--   0        0        0    79429 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/api/issues_api.py
--rw-r--r--   0        0        0     8329 2023-06-21 20:05:15.455147 py_asoc-0.1.1/src/pyasoc/api/os_libraries_api.py
--rw-r--r--   0        0        0    24024 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/api/policies_api.py
--rw-r--r--   0        0        0    37288 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/api/presences_api.py
--rw-r--r--   0        0        0    50499 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/api/reports_api.py
--rw-r--r--   0        0        0    21218 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/api/roles_api.py
--rw-r--r--   0        0        0   155783 2023-06-23 20:09:25.456419 py_asoc-0.1.1/src/pyasoc/api/scans_api.py
--rw-r--r--   0        0        0    15380 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/api/tools_api.py
--rw-r--r--   0        0        0    26696 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/api/users_api.py
--rw-r--r--   0        0        0    35869 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/api/webhooks_api.py
--rw-r--r--   0        0        0    24160 2023-06-21 20:04:54.927105 py_asoc-0.1.1/src/pyasoc/api_client.py
--rw-r--r--   0        0        0    10950 2023-06-26 15:01:22.048673 py_asoc-0.1.1/src/pyasoc/asoc.py
--rw-r--r--   0        0        0     3320 2023-06-23 20:09:32.672444 py_asoc-0.1.1/src/pyasoc/cli.py
--rw-r--r--   0        0        0     8378 2023-06-21 20:11:19.303897 py_asoc-0.1.1/src/pyasoc/configuration.py
--rw-r--r--   0        0        0    18394 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/__init__.py
--rw-r--r--   0        0        0     3826 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_controllers_scans_controller_data.py
--rw-r--r--   0        0        0     4055 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_controllers_scans_controller_is_valid_url_response.py
--rw-r--r--   0        0        0     5705 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_business_unit_model.py
--rw-r--r--   0        0        0     5224 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_change.py
--rw-r--r--   0        0        0    42691 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_dynamic_analyzer_scan.py
--rw-r--r--   0        0        0    48251 2023-06-21 20:05:40.203199 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_dynamic_analyzer_scan_execution.py
--rw-r--r--   0        0        0     5289 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_error_response.py
--rw-r--r--   0        0        0     7949 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_explore_data_counters_model.py
--rw-r--r--   0        0        0    34679 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_iast_analyzer.py
--rw-r--r--   0        0        0    40601 2023-06-21 20:05:40.115198 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_iast_analyzer_scan_execution.py
--rw-r--r--   0        0        0     6675 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_issue_change_set.py
--rw-r--r--   0        0        0    21886 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_license_library_model.py
--rw-r--r--   0        0        0     5042 2023-06-21 20:05:40.611199 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_min_presence_data.py
--rw-r--r--   0        0        0    25346 2023-06-23 19:47:24.863396 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_min_scan_data.py
--rw-r--r--   0        0        0    30048 2023-06-21 20:05:40.063198 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_min_scan_execution.py
--rw-r--r--   0        0        0     5125 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_new_business_unit_model.py
--rw-r--r--   0        0        0     7784 2023-06-21 20:05:39.899198 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_new_webhook.py
--rw-r--r--   0        0        0    34361 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_sca_analyzer_scan.py
--rw-r--r--   0        0        0    44118 2023-06-21 20:05:40.139198 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_sca_analyzer_scan_execution.py
--rw-r--r--   0        0        0    32810 2023-06-21 20:05:15.455147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scan.py
--rw-r--r--   0        0        0    32951 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scan1.py
--rw-r--r--   0        0        0    38717 2023-06-21 20:05:40.479199 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution.py
--rw-r--r--   0        0        0    38874 2023-06-21 20:05:40.691199 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution1.py
--rw-r--r--   0        0        0     5431 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution_info.py
--rw-r--r--   0        0        0     5007 2023-06-21 20:05:40.431199 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_status.py
--rw-r--r--   0        0        0     5201 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_technology.py
--rw-r--r--   0        0        0     4569 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_user.py
--rw-r--r--   0        0        0    34912 2023-06-23 18:00:16.145229 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_static_analyzer_scan.py
--rw-r--r--   0        0        0    44637 2023-06-21 20:05:40.515199 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_static_analyzer_scan_execution.py
--rw-r--r--   0        0        0     6219 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_update_business_unit_model.py
--rw-r--r--   0        0        0     5586 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_update_webhook.py
--rw-r--r--   0        0        0     8265 2023-06-21 20:05:40.639199 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_webhook.py
--rw-r--r--   0        0        0     5065 2023-06-21 20:05:40.547199 py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_webhook_association.py
--rw-r--r--   0        0        0     5565 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/application_reset_model.py
--rw-r--r--   0        0        0    11688 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/common_models_asm_models_app_license.py
--rw-r--r--   0        0        0    25610 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/common_models_asm_models_application_create_model.py
--rw-r--r--   0        0        0    50861 2023-06-21 20:05:15.455147 py_asoc-0.1.1/src/pyasoc/models/common_models_asm_models_application_model.py
--rw-r--r--   0        0        0    25368 2023-06-21 20:05:15.483147 py_asoc-0.1.1/src/pyasoc/models/common_models_asm_models_application_update_model.py
--rw-r--r--   0        0        0     9351 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/common_models_asm_models_compliance_status.py
--rw-r--r--   0        0        0     8875 2023-06-21 20:06:00.227240 py_asoc-0.1.1/src/pyasoc/models/common_models_domain_model.py
--rw-r--r--   0        0        0    20402 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/common_models_scx_account_scx_subscription.py
--rw-r--r--   0        0        0     8650 2023-06-21 20:05:15.479147 py_asoc-0.1.1/src/pyasoc/models/common_models_scx_account_scx_user_info.py
--rw-r--r--   0        0        0    22521 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/common_models_scx_account_tenant_info.py
--rw-r--r--   0        0        0     3802 2023-06-21 20:05:15.451147 py_asoc-0.1.1/src/pyasoc/models/common_models_update_domain_model.py
--rw-r--r--   0        0        0     5958 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/edit_policy.py
--rw-r--r--   0        0        0     5159 2023-06-21 20:05:15.479147 py_asoc-0.1.1/src/pyasoc/models/import_app_result_model.py
--rw-r--r--   0        0        0     3282 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_annotations_i_edm_direct_value_annotations_manager.py
--rw-r--r--   0        0        0     5745 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_annotations_i_edm_vocabulary_annotation.py
--rw-r--r--   0        0        0     7720 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_model.py
--rw-r--r--   0        0        0     5937 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_schema_element.py
--rw-r--r--   0        0        0     6908 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_term.py
--rw-r--r--   0        0        0     4294 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_type.py
--rw-r--r--   0        0        0     4750 2023-06-21 20:05:15.479147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_type_reference.py
--rw-r--r--   0        0        0     3187 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_vocabulary_annotatable.py
--rw-r--r--   0        0        0     6213 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_filter_clause.py
--rw-r--r--   0        0        0     8362 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_order_by_clause.py
--rw-r--r--   0        0        0     5620 2023-06-21 20:05:15.483147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_range_variable.py
--rw-r--r--   0        0        0     5223 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_select_expand_clause.py
--rw-r--r--   0        0        0     3202 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_select_item.py
--rw-r--r--   0        0        0     5900 2023-06-21 20:06:00.107240 py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_single_value_node.py
--rw-r--r--   0        0        0     5045 2023-06-21 20:05:15.483147 py_asoc-0.1.1/src/pyasoc/models/name_value_pair.py
--rw-r--r--   0        0        0     6179 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/new_policy.py
--rw-r--r--   0        0        0    12235 2023-06-21 20:06:00.459240 py_asoc-0.1.1/src/pyasoc/models/policy.py
--rw-r--r--   0        0        0    14244 2023-06-21 20:06:00.495241 py_asoc-0.1.1/src/pyasoc/models/policy_association.py
--rw-r--r--   0        0        0     4469 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/policy_configuration.py
--rw-r--r--   0        0        0     7432 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/scan_manager_scan_models_postman_collection_files.py
--rw-r--r--   0        0        0    32842 2023-06-21 20:05:15.495147 py_asoc-0.1.1/src/pyasoc/models/shared_components_configurations_dast_user_scan_configuration.py
--rw-r--r--   0        0        0     5717 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_o_data_query_context.py
--rw-r--r--   0        0        0     6015 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_business_unit_model.py
--rw-r--r--   0        0        0     6101 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_license_library_model.py
--rw-r--r--   0        0        0     6001 2023-06-21 21:02:08.078528 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_min_scan_data.py
--rw-r--r--   0        0        0     5742 2023-06-21 20:05:15.479147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_scan.py
--rw-r--r--   0        0        0     6036 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_common_models_asm_models_application_model.py
--rw-r--r--   0        0        0     5742 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_common_models_domain_model.py
--rw-r--r--   0        0        0     5354 2023-06-21 20:05:15.451147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_policy.py
--rw-r--r--   0        0        0     5994 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_asset_group_model.py
--rw-r--r--   0        0        0     5847 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_fix_group.py
--rw-r--r--   0        0        0     5868 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_user_model.py
--rw-r--r--   0        0        0     5742 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_utilities_issue_model.py
--rw-r--r--   0        0        0     6211 2023-06-21 20:05:15.451147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_utilities_shared_models_correlation_group_model.py
--rw-r--r--   0        0        0     6879 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_filter_query_option.py
--rw-r--r--   0        0        0     5839 2023-06-21 20:05:40.183198 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_inline_count_query_option.py
--rw-r--r--   0        0        0    15871 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_business_unit_model.py
--rw-r--r--   0        0        0    15977 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_license_library_model.py
--rw-r--r--   0        0        0    15518 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_min_scan_data.py
--rw-r--r--   0        0        0    15130 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_scan1.py
--rw-r--r--   0        0        0    15924 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_common_models_asm_models_application_model.py
--rw-r--r--   0        0        0    15077 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_common_models_domain_model.py
--rw-r--r--   0        0        0    14176 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_policy.py
--rw-r--r--   0        0        0    15818 2023-06-21 20:05:15.451147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_asset_group_model.py
--rw-r--r--   0        0        0    15386 2023-06-21 20:05:15.483147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_fix_group.py
--rw-r--r--   0        0        0    15439 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_user_model.py
--rw-r--r--   0        0        0    14865 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_utilities_issue_model.py
--rw-r--r--   0        0        0    16189 2023-06-21 20:05:15.479147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_utilities_shared_models_correlation_group_model.py
--rw-r--r--   0        0        0     9966 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_raw_query_options.py
--rw-r--r--   0        0        0     4215 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_order_by_node.py
--rw-r--r--   0        0        0     7978 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_order_by_query_option.py
--rw-r--r--   0        0        0     8036 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_select_expand_query_option.py
--rw-r--r--   0        0        0     6498 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_skip_query_option.py
--rw-r--r--   0        0        0     6473 2023-06-21 20:05:15.451147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_top_query_option.py
--rw-r--r--   0        0        0     3247 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_filter_query_validator.py
--rw-r--r--   0        0        0     3242 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_o_data_query_validator.py
--rw-r--r--   0        0        0     3252 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_order_by_query_validator.py
--rw-r--r--   0        0        0     3277 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_select_expand_query_validator.py
--rw-r--r--   0        0        0     3237 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_skip_query_validator.py
--rw-r--r--   0        0        0     3232 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_top_query_validator.py
--rw-r--r--   0        0        0     4509 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_access_token_data.py
--rw-r--r--   0        0        0     5295 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_api_key.py
--rw-r--r--   0        0        0    10536 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_asset_group_model.py
--rw-r--r--   0        0        0     4877 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_asset_group_short_model.py
--rw-r--r--   0        0        0     6744 2023-06-21 20:05:15.479147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_basic_user_info.py
--rw-r--r--   0        0        0     4346 2023-06-21 20:05:15.455147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_comment_model.py
--rw-r--r--   0        0        0     5691 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_comment_model_response.py
--rw-r--r--   0        0        0     6073 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_count_group_model.py
--rw-r--r--   0        0        0     3767 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_count_model.py
--rw-r--r--   0        0        0     4559 2023-06-21 20:05:15.483147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_explore_item.py
--rw-r--r--   0        0        0    22081 2023-06-21 20:05:40.355199 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_fix_group.py
--rw-r--r--   0        0        0     6172 2023-06-21 20:05:40.535199 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_fix_group_update.py
--rw-r--r--   0        0        0     4560 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_group_count_element_model.py
--rw-r--r--   0        0        0     5566 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_group_count_model.py
--rw-r--r--   0        0        0     5385 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_import_issue_status_model.py
--rw-r--r--   0        0        0     5350 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_invite_model.py
--rw-r--r--   0        0        0     5079 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_invite_result.py
--rw-r--r--   0        0        0     5510 2023-06-21 20:05:15.455147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_invite_users_model.py
--rw-r--r--   0        0        0     5692 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_issue_merge_model.py
--rw-r--r--   0        0        0     5062 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_issues_count_by_severity.py
--rw-r--r--   0        0        0     4953 2023-06-21 20:05:40.763200 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_issues_count_by_status.py
--rw-r--r--   0        0        0     6160 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_issues_report_job.py
--rw-r--r--   0        0        0     5073 2023-06-21 20:05:15.483147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_license_report_job.py
--rw-r--r--   0        0        0     8222 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_asset_group_model.py
--rw-r--r--   0        0        0    50631 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan.py
--rw-r--r--   0        0        0    54044 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan_by_template.py
--rw-r--r--   0        0        0    56257 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan_with_files.py
--rw-r--r--   0        0        0    14222 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_iast_analyzer_scan.py
--rw-r--r--   0        0        0     3727 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_iast_key.py
--rw-r--r--   0        0        0     5301 2023-06-21 20:05:15.451147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_key.py
--rw-r--r--   0        0        0     4663 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_presence.py
--rw-r--r--   0        0        0     8846 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_role_model.py
--rw-r--r--   0        0        0    13343 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_static_analyzer_scan.py
--rw-r--r--   0        0        0     8594 2023-06-21 20:05:40.687199 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_presence.py
--rw-r--r--   0        0        0     7366 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_regulation_report_job.py
--rw-r--r--   0        0        0     9906 2023-06-21 20:05:40.515199 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_report_status_model.py
--rw-r--r--   0        0        0    11625 2023-06-21 20:05:15.455147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_role_model.py
--rw-r--r--   0        0        0     5017 2023-06-21 20:05:15.451147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_scan_execute.py
--rw-r--r--   0        0        0     5490 2023-06-21 20:05:15.455147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_scan_results_model.py
--rw-r--r--   0        0        0     7316 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_security_report_job.py
--rw-r--r--   0        0        0    14507 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_subscription_info_model.py
--rw-r--r--   0        0        0     6944 2023-06-21 20:05:15.459147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_triage_result.py
--rw-r--r--   0        0        0    11080 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_update_dast_scan.py
--rw-r--r--   0        0        0     8273 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_update_iast_scan.py
--rw-r--r--   0        0        0     4690 2023-06-21 20:05:15.475147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_update_presence.py
--rw-r--r--   0        0        0     4730 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_update_user_model.py
--rw-r--r--   0        0        0     5748 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_upload_view_model.py
--rw-r--r--   0        0        0     4868 2023-06-21 20:05:15.479147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_user_grouping_model.py
--rw-r--r--   0        0        0    13900 2023-06-21 20:05:40.823200 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_user_model.py
--rw-r--r--   0        0        0     4732 2023-06-21 20:05:15.467147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_users_count_model.py
--rw-r--r--   0        0        0     4977 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_ver_and_hashes.py
--rw-r--r--   0        0        0    43304 2023-06-21 20:05:40.355199 py_asoc-0.1.1/src/pyasoc/models/utilities_issue_model.py
--rw-r--r--   0        0        0    15446 2023-06-21 20:08:02.467492 py_asoc-0.1.1/src/pyasoc/models/utilities_shared_models_correlation_group_model.py
--rw-r--r--   0        0        0     6602 2023-06-21 20:05:15.471147 py_asoc-0.1.1/src/pyasoc/models/utilities_structures_license_report_options.py
--rw-r--r--   0        0        0     8717 2023-06-21 20:05:15.487147 py_asoc-0.1.1/src/pyasoc/models/utilities_structures_regulation_report_options.py
--rw-r--r--   0        0        0    15574 2023-06-21 20:05:15.491147 py_asoc-0.1.1/src/pyasoc/models/utilities_structures_security_report_options.py
--rw-r--r--   0        0        0     9252 2023-06-21 20:05:15.463147 py_asoc-0.1.1/src/pyasoc/models/utilities_structures_tenant_info_model.py
--rw-r--r--   0        0        0     6607 2023-06-21 20:05:40.579199 py_asoc-0.1.1/src/pyasoc/models/utilities_update_issue.py
--rw-r--r--   0        0        0    13319 2023-06-21 20:11:19.463897 py_asoc-0.1.1/src/pyasoc/rest.py
--rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 py_asoc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-21 19:57:13.234134 py_asoc-0.1.2/LICENSE
+-rw-r--r--   0        0        0      458 2023-06-21 19:57:28.902167 py_asoc-0.1.2/README.md
+-rw-r--r--   0        0        0     3663 2023-06-26 21:14:12.578962 py_asoc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      701 2023-06-26 21:14:12.578962 py_asoc-0.1.2/src/pyasoc/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-20 17:19:48.801799 py_asoc-0.1.2/src/pyasoc/api/__init__.py
+-rw-r--r--   0        0        0    26867 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/api/account_api.py
+-rw-r--r--   0        0        0    80163 2023-06-23 20:09:33.904449 py_asoc-0.1.2/src/pyasoc/api/apps_api.py
+-rw-r--r--   0        0        0    31131 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/api/asset_groups_api.py
+-rw-r--r--   0        0        0    27522 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/api/business_units_api.py
+-rw-r--r--   0        0        0    22350 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/api/domains_api.py
+-rw-r--r--   0        0        0     7576 2023-06-22 14:55:38.934298 py_asoc-0.1.2/src/pyasoc/api/file_upload_api.py
+-rw-r--r--   0        0        0    34193 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/api/fix_groups_api.py
+-rw-r--r--   0        0        0    79429 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/api/issues_api.py
+-rw-r--r--   0        0        0     8329 2023-06-21 20:05:15.455147 py_asoc-0.1.2/src/pyasoc/api/os_libraries_api.py
+-rw-r--r--   0        0        0    24024 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/api/policies_api.py
+-rw-r--r--   0        0        0    37288 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/api/presences_api.py
+-rw-r--r--   0        0        0    50499 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/api/reports_api.py
+-rw-r--r--   0        0        0    21218 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/api/roles_api.py
+-rw-r--r--   0        0        0   155783 2023-06-23 20:09:25.456419 py_asoc-0.1.2/src/pyasoc/api/scans_api.py
+-rw-r--r--   0        0        0    15380 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/api/tools_api.py
+-rw-r--r--   0        0        0    26696 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/api/users_api.py
+-rw-r--r--   0        0        0    35869 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/api/webhooks_api.py
+-rw-r--r--   0        0        0    24160 2023-06-21 20:04:54.927105 py_asoc-0.1.2/src/pyasoc/api_client.py
+-rw-r--r--   0        0        0    11425 2023-06-26 21:12:48.770764 py_asoc-0.1.2/src/pyasoc/asoc.py
+-rw-r--r--   0        0        0     3320 2023-06-23 20:09:32.672444 py_asoc-0.1.2/src/pyasoc/cli.py
+-rw-r--r--   0        0        0     8378 2023-06-21 20:11:19.303897 py_asoc-0.1.2/src/pyasoc/configuration.py
+-rw-r--r--   0        0        0    18394 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/__init__.py
+-rw-r--r--   0        0        0     3826 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_controllers_scans_controller_data.py
+-rw-r--r--   0        0        0     4055 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_controllers_scans_controller_is_valid_url_response.py
+-rw-r--r--   0        0        0     5705 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_business_unit_model.py
+-rw-r--r--   0        0        0     5224 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_change.py
+-rw-r--r--   0        0        0    42691 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_dynamic_analyzer_scan.py
+-rw-r--r--   0        0        0    48251 2023-06-21 20:05:40.203199 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_dynamic_analyzer_scan_execution.py
+-rw-r--r--   0        0        0     5289 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_error_response.py
+-rw-r--r--   0        0        0     7949 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_explore_data_counters_model.py
+-rw-r--r--   0        0        0    34679 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_iast_analyzer.py
+-rw-r--r--   0        0        0    40601 2023-06-21 20:05:40.115198 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_iast_analyzer_scan_execution.py
+-rw-r--r--   0        0        0     6675 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_issue_change_set.py
+-rw-r--r--   0        0        0    21886 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_license_library_model.py
+-rw-r--r--   0        0        0     5042 2023-06-21 20:05:40.611199 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_min_presence_data.py
+-rw-r--r--   0        0        0    25346 2023-06-23 19:47:24.863396 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_min_scan_data.py
+-rw-r--r--   0        0        0    30048 2023-06-21 20:05:40.063198 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_min_scan_execution.py
+-rw-r--r--   0        0        0     5125 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_new_business_unit_model.py
+-rw-r--r--   0        0        0     7784 2023-06-21 20:05:39.899198 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_new_webhook.py
+-rw-r--r--   0        0        0    34361 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_sca_analyzer_scan.py
+-rw-r--r--   0        0        0    44118 2023-06-21 20:05:40.139198 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_sca_analyzer_scan_execution.py
+-rw-r--r--   0        0        0    32810 2023-06-21 20:05:15.455147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scan.py
+-rw-r--r--   0        0        0    32951 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scan1.py
+-rw-r--r--   0        0        0    38717 2023-06-21 20:05:40.479199 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution.py
+-rw-r--r--   0        0        0    38874 2023-06-21 20:05:40.691199 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution1.py
+-rw-r--r--   0        0        0     5431 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution_info.py
+-rw-r--r--   0        0        0     5007 2023-06-21 20:05:40.431199 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_status.py
+-rw-r--r--   0        0        0     5201 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_technology.py
+-rw-r--r--   0        0        0     4569 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_user.py
+-rw-r--r--   0        0        0    34912 2023-06-23 18:00:16.145229 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_static_analyzer_scan.py
+-rw-r--r--   0        0        0    44637 2023-06-21 20:05:40.515199 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_static_analyzer_scan_execution.py
+-rw-r--r--   0        0        0     6219 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_update_business_unit_model.py
+-rw-r--r--   0        0        0     5586 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_update_webhook.py
+-rw-r--r--   0        0        0     8265 2023-06-21 20:05:40.639199 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_webhook.py
+-rw-r--r--   0        0        0     5065 2023-06-21 20:05:40.547199 py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_webhook_association.py
+-rw-r--r--   0        0        0     5565 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/application_reset_model.py
+-rw-r--r--   0        0        0    11688 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/common_models_asm_models_app_license.py
+-rw-r--r--   0        0        0    25610 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/common_models_asm_models_application_create_model.py
+-rw-r--r--   0        0        0    50861 2023-06-21 20:05:15.455147 py_asoc-0.1.2/src/pyasoc/models/common_models_asm_models_application_model.py
+-rw-r--r--   0        0        0    25368 2023-06-21 20:05:15.483147 py_asoc-0.1.2/src/pyasoc/models/common_models_asm_models_application_update_model.py
+-rw-r--r--   0        0        0     9351 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/common_models_asm_models_compliance_status.py
+-rw-r--r--   0        0        0     8875 2023-06-21 20:06:00.227240 py_asoc-0.1.2/src/pyasoc/models/common_models_domain_model.py
+-rw-r--r--   0        0        0    20402 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/common_models_scx_account_scx_subscription.py
+-rw-r--r--   0        0        0     8650 2023-06-21 20:05:15.479147 py_asoc-0.1.2/src/pyasoc/models/common_models_scx_account_scx_user_info.py
+-rw-r--r--   0        0        0    22521 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/common_models_scx_account_tenant_info.py
+-rw-r--r--   0        0        0     3802 2023-06-21 20:05:15.451147 py_asoc-0.1.2/src/pyasoc/models/common_models_update_domain_model.py
+-rw-r--r--   0        0        0     5958 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/edit_policy.py
+-rw-r--r--   0        0        0     5159 2023-06-21 20:05:15.479147 py_asoc-0.1.2/src/pyasoc/models/import_app_result_model.py
+-rw-r--r--   0        0        0     3282 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_annotations_i_edm_direct_value_annotations_manager.py
+-rw-r--r--   0        0        0     5745 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_annotations_i_edm_vocabulary_annotation.py
+-rw-r--r--   0        0        0     7720 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_model.py
+-rw-r--r--   0        0        0     5937 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_schema_element.py
+-rw-r--r--   0        0        0     6908 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_term.py
+-rw-r--r--   0        0        0     4294 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_type.py
+-rw-r--r--   0        0        0     4750 2023-06-21 20:05:15.479147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_type_reference.py
+-rw-r--r--   0        0        0     3187 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_vocabulary_annotatable.py
+-rw-r--r--   0        0        0     6213 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_filter_clause.py
+-rw-r--r--   0        0        0     8362 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_order_by_clause.py
+-rw-r--r--   0        0        0     5620 2023-06-21 20:05:15.483147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_range_variable.py
+-rw-r--r--   0        0        0     5223 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_select_expand_clause.py
+-rw-r--r--   0        0        0     3202 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_select_item.py
+-rw-r--r--   0        0        0     5900 2023-06-21 20:06:00.107240 py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_single_value_node.py
+-rw-r--r--   0        0        0     5045 2023-06-21 20:05:15.483147 py_asoc-0.1.2/src/pyasoc/models/name_value_pair.py
+-rw-r--r--   0        0        0     6179 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/new_policy.py
+-rw-r--r--   0        0        0    12235 2023-06-21 20:06:00.459240 py_asoc-0.1.2/src/pyasoc/models/policy.py
+-rw-r--r--   0        0        0    14244 2023-06-21 20:06:00.495241 py_asoc-0.1.2/src/pyasoc/models/policy_association.py
+-rw-r--r--   0        0        0     4469 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/policy_configuration.py
+-rw-r--r--   0        0        0     7432 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/scan_manager_scan_models_postman_collection_files.py
+-rw-r--r--   0        0        0    32842 2023-06-21 20:05:15.495147 py_asoc-0.1.2/src/pyasoc/models/shared_components_configurations_dast_user_scan_configuration.py
+-rw-r--r--   0        0        0     5717 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_o_data_query_context.py
+-rw-r--r--   0        0        0     6015 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_business_unit_model.py
+-rw-r--r--   0        0        0     6101 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_license_library_model.py
+-rw-r--r--   0        0        0     6001 2023-06-21 21:02:08.078528 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_min_scan_data.py
+-rw-r--r--   0        0        0     5742 2023-06-21 20:05:15.479147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_scan.py
+-rw-r--r--   0        0        0     6036 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_common_models_asm_models_application_model.py
+-rw-r--r--   0        0        0     5742 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_common_models_domain_model.py
+-rw-r--r--   0        0        0     5354 2023-06-21 20:05:15.451147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_policy.py
+-rw-r--r--   0        0        0     5994 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_asset_group_model.py
+-rw-r--r--   0        0        0     5847 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_fix_group.py
+-rw-r--r--   0        0        0     5868 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_user_model.py
+-rw-r--r--   0        0        0     5742 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_utilities_issue_model.py
+-rw-r--r--   0        0        0     6211 2023-06-21 20:05:15.451147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_utilities_shared_models_correlation_group_model.py
+-rw-r--r--   0        0        0     6879 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_filter_query_option.py
+-rw-r--r--   0        0        0     5839 2023-06-21 20:05:40.183198 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_inline_count_query_option.py
+-rw-r--r--   0        0        0    15871 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_business_unit_model.py
+-rw-r--r--   0        0        0    15977 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_license_library_model.py
+-rw-r--r--   0        0        0    15518 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_min_scan_data.py
+-rw-r--r--   0        0        0    15130 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_scan1.py
+-rw-r--r--   0        0        0    15924 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_common_models_asm_models_application_model.py
+-rw-r--r--   0        0        0    15077 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_common_models_domain_model.py
+-rw-r--r--   0        0        0    14176 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_policy.py
+-rw-r--r--   0        0        0    15818 2023-06-21 20:05:15.451147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_asset_group_model.py
+-rw-r--r--   0        0        0    15386 2023-06-21 20:05:15.483147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_fix_group.py
+-rw-r--r--   0        0        0    15439 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_user_model.py
+-rw-r--r--   0        0        0    14865 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_utilities_issue_model.py
+-rw-r--r--   0        0        0    16189 2023-06-21 20:05:15.479147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_utilities_shared_models_correlation_group_model.py
+-rw-r--r--   0        0        0     9966 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_raw_query_options.py
+-rw-r--r--   0        0        0     4215 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_order_by_node.py
+-rw-r--r--   0        0        0     7978 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_order_by_query_option.py
+-rw-r--r--   0        0        0     8036 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_select_expand_query_option.py
+-rw-r--r--   0        0        0     6498 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_skip_query_option.py
+-rw-r--r--   0        0        0     6473 2023-06-21 20:05:15.451147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_top_query_option.py
+-rw-r--r--   0        0        0     3247 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_filter_query_validator.py
+-rw-r--r--   0        0        0     3242 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_o_data_query_validator.py
+-rw-r--r--   0        0        0     3252 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_order_by_query_validator.py
+-rw-r--r--   0        0        0     3277 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_select_expand_query_validator.py
+-rw-r--r--   0        0        0     3237 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_skip_query_validator.py
+-rw-r--r--   0        0        0     3232 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_top_query_validator.py
+-rw-r--r--   0        0        0     4509 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_access_token_data.py
+-rw-r--r--   0        0        0     5295 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_api_key.py
+-rw-r--r--   0        0        0    10536 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_asset_group_model.py
+-rw-r--r--   0        0        0     4877 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_asset_group_short_model.py
+-rw-r--r--   0        0        0     6744 2023-06-21 20:05:15.479147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_basic_user_info.py
+-rw-r--r--   0        0        0     4346 2023-06-21 20:05:15.455147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_comment_model.py
+-rw-r--r--   0        0        0     5691 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_comment_model_response.py
+-rw-r--r--   0        0        0     6073 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_count_group_model.py
+-rw-r--r--   0        0        0     3767 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_count_model.py
+-rw-r--r--   0        0        0     4559 2023-06-21 20:05:15.483147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_explore_item.py
+-rw-r--r--   0        0        0    22081 2023-06-21 20:05:40.355199 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_fix_group.py
+-rw-r--r--   0        0        0     6172 2023-06-21 20:05:40.535199 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_fix_group_update.py
+-rw-r--r--   0        0        0     4560 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_group_count_element_model.py
+-rw-r--r--   0        0        0     5566 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_group_count_model.py
+-rw-r--r--   0        0        0     5385 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_import_issue_status_model.py
+-rw-r--r--   0        0        0     5350 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_invite_model.py
+-rw-r--r--   0        0        0     5079 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_invite_result.py
+-rw-r--r--   0        0        0     5510 2023-06-21 20:05:15.455147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_invite_users_model.py
+-rw-r--r--   0        0        0     5692 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_issue_merge_model.py
+-rw-r--r--   0        0        0     5062 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_issues_count_by_severity.py
+-rw-r--r--   0        0        0     4953 2023-06-21 20:05:40.763200 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_issues_count_by_status.py
+-rw-r--r--   0        0        0     6160 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_issues_report_job.py
+-rw-r--r--   0        0        0     5073 2023-06-21 20:05:15.483147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_license_report_job.py
+-rw-r--r--   0        0        0     8222 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_asset_group_model.py
+-rw-r--r--   0        0        0    50631 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan.py
+-rw-r--r--   0        0        0    54044 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan_by_template.py
+-rw-r--r--   0        0        0    56257 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan_with_files.py
+-rw-r--r--   0        0        0    14222 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_iast_analyzer_scan.py
+-rw-r--r--   0        0        0     3727 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_iast_key.py
+-rw-r--r--   0        0        0     5301 2023-06-21 20:05:15.451147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_key.py
+-rw-r--r--   0        0        0     4663 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_presence.py
+-rw-r--r--   0        0        0     8846 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_role_model.py
+-rw-r--r--   0        0        0    13343 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_static_analyzer_scan.py
+-rw-r--r--   0        0        0     8594 2023-06-21 20:05:40.687199 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_presence.py
+-rw-r--r--   0        0        0     7366 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_regulation_report_job.py
+-rw-r--r--   0        0        0     9906 2023-06-21 20:05:40.515199 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_report_status_model.py
+-rw-r--r--   0        0        0    11625 2023-06-21 20:05:15.455147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_role_model.py
+-rw-r--r--   0        0        0     5017 2023-06-21 20:05:15.451147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_scan_execute.py
+-rw-r--r--   0        0        0     5490 2023-06-21 20:05:15.455147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_scan_results_model.py
+-rw-r--r--   0        0        0     7316 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_security_report_job.py
+-rw-r--r--   0        0        0    14507 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_subscription_info_model.py
+-rw-r--r--   0        0        0     6944 2023-06-21 20:05:15.459147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_triage_result.py
+-rw-r--r--   0        0        0    11080 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_update_dast_scan.py
+-rw-r--r--   0        0        0     8273 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_update_iast_scan.py
+-rw-r--r--   0        0        0     4690 2023-06-21 20:05:15.475147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_update_presence.py
+-rw-r--r--   0        0        0     4730 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_update_user_model.py
+-rw-r--r--   0        0        0     5748 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_upload_view_model.py
+-rw-r--r--   0        0        0     4868 2023-06-21 20:05:15.479147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_user_grouping_model.py
+-rw-r--r--   0        0        0    13900 2023-06-21 20:05:40.823200 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_user_model.py
+-rw-r--r--   0        0        0     4732 2023-06-21 20:05:15.467147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_users_count_model.py
+-rw-r--r--   0        0        0     4977 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_ver_and_hashes.py
+-rw-r--r--   0        0        0    43304 2023-06-21 20:05:40.355199 py_asoc-0.1.2/src/pyasoc/models/utilities_issue_model.py
+-rw-r--r--   0        0        0    15446 2023-06-21 20:08:02.467492 py_asoc-0.1.2/src/pyasoc/models/utilities_shared_models_correlation_group_model.py
+-rw-r--r--   0        0        0     6602 2023-06-21 20:05:15.471147 py_asoc-0.1.2/src/pyasoc/models/utilities_structures_license_report_options.py
+-rw-r--r--   0        0        0     8717 2023-06-21 20:05:15.487147 py_asoc-0.1.2/src/pyasoc/models/utilities_structures_regulation_report_options.py
+-rw-r--r--   0        0        0    15574 2023-06-21 20:05:15.491147 py_asoc-0.1.2/src/pyasoc/models/utilities_structures_security_report_options.py
+-rw-r--r--   0        0        0     9252 2023-06-21 20:05:15.463147 py_asoc-0.1.2/src/pyasoc/models/utilities_structures_tenant_info_model.py
+-rw-r--r--   0        0        0     6607 2023-06-21 20:05:40.579199 py_asoc-0.1.2/src/pyasoc/models/utilities_update_issue.py
+-rw-r--r--   0        0        0    13319 2023-06-21 20:11:19.463897 py_asoc-0.1.2/src/pyasoc/rest.py
+-rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 py_asoc-0.1.2/PKG-INFO
```

### Comparing `py_asoc-0.1.1/LICENSE` & `py_asoc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/pyproject.toml` & `py_asoc-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # region Poetry
 [tool.poetry]
 name = "py-asoc"
-version = "0.1.1"
+version = "0.1.2"
 description = "Description"
 authors = ["Daniel Sullivan <daniel.j.sullivan@state.mn.us>"]
 license = "MIT"
 repository = "https://github.com/mumblepins/py-asoc/"
 documentation = "https://mumblepins.github.io/py-asoc/"
 readme = "README.md"
 packages = [{ include = "pyasoc", from = "src" }]
```

### Comparing `py_asoc-0.1.1/src/pyasoc/__init__.py` & `py_asoc-0.1.2/src/pyasoc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 
     This API allows you to interact with the service. The API allows you to perform many of the operations available in the UI and more.</br>For authentication, use the relevant APIs in the Account section. A successful authentication response includes a bearer token for use in subsequent API calls. Pasting this token in the 'Access token' field above will automatically add the authorization header to any API call that requires a valid session.
 
     OpenAPI spec version: v2
 
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
-__version__: str = "0.1.1"
+__version__: str = "0.1.2"
 
 # import apis into sdk package
 
 # import ApiClient
 
 # import models into sdk package
```

### Comparing `py_asoc-0.1.1/src/pyasoc/api/account_api.py` & `py_asoc-0.1.2/src/pyasoc/api/account_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/apps_api.py` & `py_asoc-0.1.2/src/pyasoc/api/apps_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/asset_groups_api.py` & `py_asoc-0.1.2/src/pyasoc/api/asset_groups_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/business_units_api.py` & `py_asoc-0.1.2/src/pyasoc/api/business_units_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/domains_api.py` & `py_asoc-0.1.2/src/pyasoc/api/domains_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/file_upload_api.py` & `py_asoc-0.1.2/src/pyasoc/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/fix_groups_api.py` & `py_asoc-0.1.2/src/pyasoc/api/fix_groups_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/issues_api.py` & `py_asoc-0.1.2/src/pyasoc/api/issues_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/os_libraries_api.py` & `py_asoc-0.1.2/src/pyasoc/api/os_libraries_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/policies_api.py` & `py_asoc-0.1.2/src/pyasoc/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/presences_api.py` & `py_asoc-0.1.2/src/pyasoc/api/presences_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/reports_api.py` & `py_asoc-0.1.2/src/pyasoc/api/reports_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/roles_api.py` & `py_asoc-0.1.2/src/pyasoc/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/scans_api.py` & `py_asoc-0.1.2/src/pyasoc/api/scans_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/tools_api.py` & `py_asoc-0.1.2/src/pyasoc/api/tools_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/users_api.py` & `py_asoc-0.1.2/src/pyasoc/api/users_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api/webhooks_api.py` & `py_asoc-0.1.2/src/pyasoc/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/api_client.py` & `py_asoc-0.1.2/src/pyasoc/api_client.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/asoc.py` & `py_asoc-0.1.2/src/pyasoc/asoc.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,15 +133,16 @@
     def _old_scan_start(self, scan_id: str, file_id: str) -> AppScanSaaSModelsV2ScanExecution:
         return self._scans.scans_execute_scan_by_scanid(
             scan_id=scan_id, model=UserSiteCommonModelsScanExecute(file_id=file_id)
         )
 
     # region external issue handling
     def get_external_issues(self) -> list[UtilitiesIssueModel]:
-        r: SystemWebHttpODataPageResultUtilitiesIssueModel = self._issues.issues_get_issues_for_scope_by_scope_and_scopeid(
+        r: SystemWebHttpODataPageResultUtilitiesIssueModel
+        r = self._issues.issues_get_issues_for_scope_by_scope_and_scopeid(
             scope="Application",
             scope_id=self.app_id,
             top=5000,
             filter="length(ExternalId) gt 1",
             # _request_timeout=10,
         )
         return r.items
@@ -157,31 +158,50 @@
                         if iss["External Id"] not in issues:
                             issues[iss["External Id"]] = iss
                         # break
             except (json.JSONDecodeError, KeyError):
                 pass
         existing_issues = self.get_external_issues()
         existing_open: dict[str, UtilitiesIssueModel] = {
-            a.external_id: a for a in existing_issues if a.status in ("Open", "Reopened", "New")
+            a.external_id: a
+            for a in existing_issues
+            if a.status
+            in (
+                "Open",
+                "Reopened",
+                "New",
+            )
         }
         existing_fixed: dict[str, UtilitiesIssueModel] = {
             a.external_id: a for a in existing_issues if a.status in ("Fixed",)
         }
+        existing_passed: dict[str, UtilitiesIssueModel] = {
+            a.external_id: a
+            for a in existing_issues
+            if a.status
+            in (
+                "Passed",
+                "Noise",
+            )
+        }
 
         new_issues: list[dict] = []
         to_fix: list[UtilitiesIssueModel] = []
         to_reopen: list[UtilitiesIssueModel] = []
         stay_open: list[UtilitiesIssueModel] = []
         for eid, v in issues.items():
             if eid in existing_open:
                 # is already open
                 stay_open.append(existing_open.pop(eid))
             elif eid in existing_fixed:
                 # need to reopen
                 to_reopen.append(existing_fixed.pop(eid))
+            elif eid in existing_passed:
+                # has been changed to passed or fixed, ignore
+                pass
             else:
                 new_issues.append(v)
         for v in existing_open.values():
             to_fix.append(v)
         return new_issues, to_fix, to_reopen, stay_open
 
     def change_issue_status(self, issue_id: str, status):
```

### Comparing `py_asoc-0.1.1/src/pyasoc/cli.py` & `py_asoc-0.1.2/src/pyasoc/cli.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/configuration.py` & `py_asoc-0.1.2/src/pyasoc/configuration.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/__init__.py` & `py_asoc-0.1.2/src/pyasoc/models/__init__.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_controllers_scans_controller_data.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_controllers_scans_controller_data.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_controllers_scans_controller_is_valid_url_response.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_controllers_scans_controller_is_valid_url_response.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_business_unit_model.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_business_unit_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_change.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_change.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_dynamic_analyzer_scan.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_dynamic_analyzer_scan.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_dynamic_analyzer_scan_execution.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_dynamic_analyzer_scan_execution.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_error_response.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_error_response.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_explore_data_counters_model.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_explore_data_counters_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_iast_analyzer.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_iast_analyzer.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_iast_analyzer_scan_execution.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_iast_analyzer_scan_execution.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_issue_change_set.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_issue_change_set.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_license_library_model.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_license_library_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_min_presence_data.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_min_presence_data.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_min_scan_data.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_min_scan_data.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_min_scan_execution.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_min_scan_execution.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_new_business_unit_model.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_new_business_unit_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_new_webhook.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_new_webhook.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_sca_analyzer_scan.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_sca_analyzer_scan.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_sca_analyzer_scan_execution.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_sca_analyzer_scan_execution.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scan.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scan.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scan1.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scan1.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution1.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution1.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution_info.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scan_execution_info.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_status.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_status.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_technology.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_technology.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_user.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_scans_count_by_user.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_static_analyzer_scan.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_static_analyzer_scan.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_static_analyzer_scan_execution.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_static_analyzer_scan_execution.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_update_business_unit_model.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_update_business_unit_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_update_webhook.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_update_webhook.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_webhook.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_webhook.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/app_scan_saa_s_models_v2_webhook_association.py` & `py_asoc-0.1.2/src/pyasoc/models/app_scan_saa_s_models_v2_webhook_association.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/application_reset_model.py` & `py_asoc-0.1.2/src/pyasoc/models/application_reset_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/common_models_asm_models_app_license.py` & `py_asoc-0.1.2/src/pyasoc/models/common_models_asm_models_app_license.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/common_models_asm_models_application_create_model.py` & `py_asoc-0.1.2/src/pyasoc/models/common_models_asm_models_application_create_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/common_models_asm_models_application_model.py` & `py_asoc-0.1.2/src/pyasoc/models/common_models_asm_models_application_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/common_models_asm_models_application_update_model.py` & `py_asoc-0.1.2/src/pyasoc/models/common_models_asm_models_application_update_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/common_models_asm_models_compliance_status.py` & `py_asoc-0.1.2/src/pyasoc/models/common_models_asm_models_compliance_status.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/common_models_domain_model.py` & `py_asoc-0.1.2/src/pyasoc/models/common_models_domain_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/common_models_scx_account_scx_subscription.py` & `py_asoc-0.1.2/src/pyasoc/models/common_models_scx_account_scx_subscription.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/common_models_scx_account_scx_user_info.py` & `py_asoc-0.1.2/src/pyasoc/models/common_models_scx_account_scx_user_info.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/common_models_scx_account_tenant_info.py` & `py_asoc-0.1.2/src/pyasoc/models/common_models_scx_account_tenant_info.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/common_models_update_domain_model.py` & `py_asoc-0.1.2/src/pyasoc/models/common_models_update_domain_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/edit_policy.py` & `py_asoc-0.1.2/src/pyasoc/models/edit_policy.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/import_app_result_model.py` & `py_asoc-0.1.2/src/pyasoc/models/import_app_result_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_annotations_i_edm_direct_value_annotations_manager.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_annotations_i_edm_direct_value_annotations_manager.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_annotations_i_edm_vocabulary_annotation.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_annotations_i_edm_vocabulary_annotation.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_model.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_schema_element.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_schema_element.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_term.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_term.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_type.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_type.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_type_reference.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_type_reference.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_edm_i_edm_vocabulary_annotatable.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_edm_i_edm_vocabulary_annotatable.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_filter_clause.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_filter_clause.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_order_by_clause.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_order_by_clause.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_range_variable.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_range_variable.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_select_expand_clause.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_select_expand_clause.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_select_item.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_select_item.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_single_value_node.py` & `py_asoc-0.1.2/src/pyasoc/models/microsoft_data_o_data_query_semantic_ast_single_value_node.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/name_value_pair.py` & `py_asoc-0.1.2/src/pyasoc/models/name_value_pair.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/new_policy.py` & `py_asoc-0.1.2/src/pyasoc/models/new_policy.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/policy.py` & `py_asoc-0.1.2/src/pyasoc/models/policy.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/policy_association.py` & `py_asoc-0.1.2/src/pyasoc/models/policy_association.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/policy_configuration.py` & `py_asoc-0.1.2/src/pyasoc/models/policy_configuration.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/scan_manager_scan_models_postman_collection_files.py` & `py_asoc-0.1.2/src/pyasoc/models/scan_manager_scan_models_postman_collection_files.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/shared_components_configurations_dast_user_scan_configuration.py` & `py_asoc-0.1.2/src/pyasoc/models/shared_components_configurations_dast_user_scan_configuration.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_o_data_query_context.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_o_data_query_context.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_business_unit_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_business_unit_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_license_library_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_license_library_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_min_scan_data.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_min_scan_data.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_scan.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_app_scan_saa_s_models_v2_scan.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_common_models_asm_models_application_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_common_models_asm_models_application_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_common_models_domain_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_common_models_domain_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_policy.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_policy.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_asset_group_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_asset_group_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_fix_group.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_fix_group.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_user_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_user_site_common_models_user_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_utilities_issue_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_utilities_issue_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_page_result_utilities_shared_models_correlation_group_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_page_result_utilities_shared_models_correlation_group_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_filter_query_option.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_filter_query_option.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_inline_count_query_option.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_inline_count_query_option.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_business_unit_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_business_unit_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_license_library_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_license_library_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_min_scan_data.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_min_scan_data.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_scan1.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_app_scan_saa_s_models_v2_scan1.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_common_models_asm_models_application_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_common_models_asm_models_application_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_common_models_domain_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_common_models_domain_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_policy.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_policy.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_asset_group_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_asset_group_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_fix_group.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_fix_group.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_user_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_user_site_common_models_user_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_utilities_issue_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_utilities_issue_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_utilities_shared_models_correlation_group_model.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_query_options_utilities_shared_models_correlation_group_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_o_data_raw_query_options.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_o_data_raw_query_options.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_order_by_node.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_order_by_node.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_order_by_query_option.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_order_by_query_option.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_select_expand_query_option.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_select_expand_query_option.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_skip_query_option.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_skip_query_option.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_top_query_option.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_top_query_option.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_filter_query_validator.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_filter_query_validator.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_o_data_query_validator.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_o_data_query_validator.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_order_by_query_validator.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_order_by_query_validator.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_select_expand_query_validator.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_select_expand_query_validator.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_skip_query_validator.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_skip_query_validator.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/system_web_http_o_data_query_validators_top_query_validator.py` & `py_asoc-0.1.2/src/pyasoc/models/system_web_http_o_data_query_validators_top_query_validator.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_access_token_data.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_access_token_data.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_api_key.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_api_key.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_asset_group_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_asset_group_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_asset_group_short_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_asset_group_short_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_basic_user_info.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_basic_user_info.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_comment_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_comment_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_comment_model_response.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_comment_model_response.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_count_group_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_count_group_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_count_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_count_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_explore_item.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_explore_item.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_fix_group.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_fix_group.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_fix_group_update.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_fix_group_update.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_group_count_element_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_group_count_element_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_group_count_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_group_count_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_import_issue_status_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_import_issue_status_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_invite_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_invite_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_invite_result.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_invite_result.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_invite_users_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_invite_users_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_issue_merge_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_issue_merge_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_issues_count_by_severity.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_issues_count_by_severity.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_issues_count_by_status.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_issues_count_by_status.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_issues_report_job.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_issues_report_job.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_license_report_job.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_license_report_job.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_asset_group_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_asset_group_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan_by_template.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan_by_template.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan_with_files.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_dynamic_analyzer_scan_with_files.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_iast_analyzer_scan.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_iast_analyzer_scan.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_iast_key.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_iast_key.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_key.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_key.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_presence.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_presence.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_role_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_role_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_new_static_analyzer_scan.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_new_static_analyzer_scan.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_presence.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_presence.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_regulation_report_job.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_regulation_report_job.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_report_status_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_report_status_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_role_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_role_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_scan_execute.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_scan_execute.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_scan_results_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_scan_results_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_security_report_job.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_security_report_job.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_subscription_info_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_subscription_info_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_triage_result.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_triage_result.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_update_dast_scan.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_update_dast_scan.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_update_iast_scan.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_update_iast_scan.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_update_presence.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_update_presence.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_update_user_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_update_user_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_upload_view_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_upload_view_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_user_grouping_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_user_grouping_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_user_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_user_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_users_count_model.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_users_count_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/user_site_common_models_ver_and_hashes.py` & `py_asoc-0.1.2/src/pyasoc/models/user_site_common_models_ver_and_hashes.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/utilities_issue_model.py` & `py_asoc-0.1.2/src/pyasoc/models/utilities_issue_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/utilities_shared_models_correlation_group_model.py` & `py_asoc-0.1.2/src/pyasoc/models/utilities_shared_models_correlation_group_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/utilities_structures_license_report_options.py` & `py_asoc-0.1.2/src/pyasoc/models/utilities_structures_license_report_options.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/utilities_structures_regulation_report_options.py` & `py_asoc-0.1.2/src/pyasoc/models/utilities_structures_regulation_report_options.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/utilities_structures_security_report_options.py` & `py_asoc-0.1.2/src/pyasoc/models/utilities_structures_security_report_options.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/utilities_structures_tenant_info_model.py` & `py_asoc-0.1.2/src/pyasoc/models/utilities_structures_tenant_info_model.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/models/utilities_update_issue.py` & `py_asoc-0.1.2/src/pyasoc/models/utilities_update_issue.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/src/pyasoc/rest.py` & `py_asoc-0.1.2/src/pyasoc/rest.py`

 * *Files identical despite different names*

### Comparing `py_asoc-0.1.1/PKG-INFO` & `py_asoc-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-asoc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Description
 Home-page: https://github.com/mumblepins/py-asoc/
 License: MIT
 Author: Daniel Sullivan
 Author-email: daniel.j.sullivan@state.mn.us
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

