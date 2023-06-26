# Comparing `tmp/longship-2023.6.26.tar.gz` & `tmp/longship-2023.6.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longship-2023.6.26.tar", max compression
+gzip compressed data, was "longship-2023.6.27.tar", max compression
```

## Comparing `longship-2023.6.26.tar` & `longship-2023.6.27.tar`

### file list

```diff
@@ -1,275 +1,275 @@
--rw-r--r--   0        0        0     1072 2023-06-26 16:00:19.878825 longship-2023.6.26/LICENSE
--rw-r--r--   0        0        0     4633 2023-06-26 16:00:19.883966 longship-2023.6.26/README.md
--rw-r--r--   0        0        0     7215 2023-06-26 16:00:19.886579 longship-2023.6.26/longship/client.py
--rw-r--r--   0        0        0      112 2023-06-26 16:00:19.886682 longship-2023.6.26/longship/errors.py
--rw-r--r--   0        0        0     2954 2023-06-26 16:00:19.886885 longship-2023.6.26/longship/types.py
--rw-r--r--   0        0        0      156 2023-06-26 16:00:19.887019 longship-2023.6.26/longship_api_client/__init__.py
--rw-r--r--   0        0        0       47 2023-06-26 16:00:19.887155 longship-2023.6.26/longship_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.887208 longship-2023.6.26/longship_api_client/api/cdrs/__init__.py
--rw-r--r--   0        0        0     4619 2023-06-26 16:00:19.887462 longship-2023.6.26/longship_api_client/api/cdrs/cdr_get.py
--rw-r--r--   0        0        0    10429 2023-06-26 16:00:19.887727 longship-2023.6.26/longship_api_client/api/cdrs/get_all_cdrs.py
--rw-r--r--   0        0        0     8447 2023-06-26 16:00:19.887850 longship-2023.6.26/longship_api_client/api/cdrs/get_all_interchangeformat.py
--rw-r--r--   0        0        0     6309 2023-06-26 16:00:19.887973 longship-2023.6.26/longship_api_client/api/cdrs/get_file_full_download_cdrs.py
--rw-r--r--   0        0        0     6288 2023-06-26 16:00:19.888095 longship-2023.6.26/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.888157 longship-2023.6.26/longship_api_client/api/chargepoint_status/__init__.py
--rw-r--r--   0        0        0     4940 2023-06-26 16:00:19.888332 longship-2023.6.26/longship_api_client/api/chargepoint_status/chargepoint_status_get.py
--rw-r--r--   0        0        0     6787 2023-06-26 16:00:19.888455 longship-2023.6.26/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.888516 longship-2023.6.26/longship_api_client/api/chargepoints/__init__.py
--rw-r--r--   0        0        0     4795 2023-06-26 16:00:19.888699 longship-2023.6.26/longship_api_client/api/chargepoints/chargepoint_get.py
--rw-r--r--   0        0        0     5302 2023-06-26 16:00:19.888829 longship-2023.6.26/longship_api_client/api/chargepoints/chargepoint_put.py
--rw-r--r--   0        0        0    12511 2023-06-26 16:00:19.888975 longship-2023.6.26/longship_api_client/api/chargepoints/get_all_chargepointmessages.py
--rw-r--r--   0        0        0     8572 2023-06-26 16:00:19.889108 longship-2023.6.26/longship_api_client/api/chargepoints/get_all_chargepoints.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.889164 longship-2023.6.26/longship_api_client/api/commands/__init__.py
--rw-r--r--   0        0        0     5291 2023-06-26 16:00:19.889355 longship-2023.6.26/longship_api_client/api/commands/send_cancel_reservation_request.py
--rw-r--r--   0        0        0     5311 2023-06-26 16:00:19.889628 longship-2023.6.26/longship_api_client/api/commands/send_change_availability_request.py
--rw-r--r--   0        0        0     5331 2023-06-26 16:00:19.889795 longship-2023.6.26/longship_api_client/api/commands/send_change_configuration_request.py
--rw-r--r--   0        0        0     5151 2023-06-26 16:00:19.889931 longship-2023.6.26/longship_api_client/api/commands/send_clear_cache_request.py
--rw-r--r--   0        0        0     5352 2023-06-26 16:00:19.890060 longship-2023.6.26/longship_api_client/api/commands/send_clear_charging_profile_request.py
--rw-r--r--   0        0        0     5191 2023-06-26 16:00:19.890188 longship-2023.6.26/longship_api_client/api/commands/send_data_transfer_request.py
--rw-r--r--   0        0        0     5352 2023-06-26 16:00:19.890335 longship-2023.6.26/longship_api_client/api/commands/send_get_composite_schedule_request.py
--rw-r--r--   0        0        0     5271 2023-06-26 16:00:19.890534 longship-2023.6.26/longship_api_client/api/commands/send_get_configuration_request.py
--rw-r--r--   0        0        0     5231 2023-06-26 16:00:19.890672 longship-2023.6.26/longship_api_client/api/commands/send_get_diagnostics_request.py
--rw-r--r--   0        0        0     5333 2023-06-26 16:00:19.890880 longship-2023.6.26/longship_api_client/api/commands/send_get_local_list_version_request.py
--rw-r--r--   0        0        0     5381 2023-06-26 16:00:19.891176 longship-2023.6.26/longship_api_client/api/commands/send_remote_start_transaction_request.py
--rw-r--r--   0        0        0     5361 2023-06-26 16:00:19.891376 longship-2023.6.26/longship_api_client/api/commands/send_remote_stop_transaction_request.py
--rw-r--r--   0        0        0     5151 2023-06-26 16:00:19.891498 longship-2023.6.26/longship_api_client/api/commands/send_reserve_now_request.py
--rw-r--r--   0        0        0     5050 2023-06-26 16:00:19.891732 longship-2023.6.26/longship_api_client/api/commands/send_reset_request.py
--rw-r--r--   0        0        0     5212 2023-06-26 16:00:19.891864 longship-2023.6.26/longship_api_client/api/commands/send_send_local_list_request.py
--rw-r--r--   0        0        0     5312 2023-06-26 16:00:19.891993 longship-2023.6.26/longship_api_client/api/commands/send_set_charging_profile_request.py
--rw-r--r--   0        0        0     5231 2023-06-26 16:00:19.892118 longship-2023.6.26/longship_api_client/api/commands/send_trigger_message_request.py
--rw-r--r--   0        0        0     5251 2023-06-26 16:00:19.892369 longship-2023.6.26/longship_api_client/api/commands/send_unlock_connector_request.py
--rw-r--r--   0        0        0     5231 2023-06-26 16:00:19.892498 longship-2023.6.26/longship_api_client/api/commands/send_update_firmware_request.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.892562 longship-2023.6.26/longship_api_client/api/localtokengroups/__init__.py
--rw-r--r--   0        0        0     6805 2023-06-26 16:00:19.892749 longship-2023.6.26/longship_api_client/api/localtokengroups/get_all_localtokengroups.py
--rw-r--r--   0        0        0     4598 2023-06-26 16:00:19.892881 longship-2023.6.26/longship_api_client/api/localtokengroups/local_token_group_delete.py
--rw-r--r--   0        0        0     5198 2023-06-26 16:00:19.893124 longship-2023.6.26/longship_api_client/api/localtokengroups/local_token_group_post.py
--rw-r--r--   0        0        0     5383 2023-06-26 16:00:19.893249 longship-2023.6.26/longship_api_client/api/localtokengroups/local_token_group_put.py
--rw-r--r--   0        0        0     4937 2023-06-26 16:00:19.893381 longship-2023.6.26/longship_api_client/api/localtokengroups/localtokengroup_get.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.893447 longship-2023.6.26/longship_api_client/api/locations/__init__.py
--rw-r--r--   0        0        0     8422 2023-06-26 16:00:19.893637 longship-2023.6.26/longship_api_client/api/locations/get_all_locations.py
--rw-r--r--   0        0        0     4729 2023-06-26 16:00:19.893769 longship-2023.6.26/longship_api_client/api/locations/location_get.py
--rw-r--r--   0        0        0     5203 2023-06-26 16:00:19.893904 longship-2023.6.26/longship_api_client/api/locations/location_post.py
--rw-r--r--   0        0        0     5020 2023-06-26 16:00:19.894032 longship-2023.6.26/longship_api_client/api/locations/location_put.py
--rw-r--r--   0        0        0     5309 2023-06-26 16:00:19.894173 longship-2023.6.26/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py
--rw-r--r--   0        0        0     5624 2023-06-26 16:00:19.894313 longship-2023.6.26/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.894383 longship-2023.6.26/longship_api_client/api/mspreimbursement/__init__.py
--rw-r--r--   0        0        0     4660 2023-06-26 16:00:19.894562 longship-2023.6.26/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.894631 longship-2023.6.26/longship_api_client/api/organizationunits/__init__.py
--rw-r--r--   0        0        0     6828 2023-06-26 16:00:19.894949 longship-2023.6.26/longship_api_client/api/organizationunits/get_all_organizationunits.py
--rw-r--r--   0        0        0     4960 2023-06-26 16:00:19.895152 longship-2023.6.26/longship_api_client/api/organizationunits/organization_unit_get.py
--rw-r--r--   0        0        0     5219 2023-06-26 16:00:19.895279 longship-2023.6.26/longship_api_client/api/organizationunits/organization_unit_post.py
--rw-r--r--   0        0        0     5390 2023-06-26 16:00:19.895408 longship-2023.6.26/longship_api_client/api/organizationunits/organization_unit_put.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.895477 longship-2023.6.26/longship_api_client/api/reimbursement/__init__.py
--rw-r--r--   0        0        0    11074 2023-06-26 16:00:19.895698 longship-2023.6.26/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py
--rw-r--r--   0        0        0     5314 2023-06-26 16:00:19.895832 longship-2023.6.26/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py
--rw-r--r--   0        0        0     4906 2023-06-26 16:00:19.895962 longship-2023.6.26/longship_api_client/api/reimbursement/reimbursement_cdr_get.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.896026 longship-2023.6.26/longship_api_client/api/sessions/__init__.py
--rw-r--r--   0        0        0    11057 2023-06-26 16:00:19.896212 longship-2023.6.26/longship_api_client/api/sessions/get_all_sessions.py
--rw-r--r--   0        0        0     4707 2023-06-26 16:00:19.896340 longship-2023.6.26/longship_api_client/api/sessions/session_get.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.896408 longship-2023.6.26/longship_api_client/api/tariffdistributions/__init__.py
--rw-r--r--   0        0        0     6878 2023-06-26 16:00:19.896589 longship-2023.6.26/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py
--rw-r--r--   0        0        0     4856 2023-06-26 16:00:19.896717 longship-2023.6.26/longship_api_client/api/tariffdistributions/tariffdistribution_get.py
--rw-r--r--   0        0        0     5111 2023-06-26 16:00:19.896842 longship-2023.6.26/longship_api_client/api/tariffdistributions/tariffdistribution_post.py
--rw-r--r--   0        0        0     5765 2023-06-26 16:00:19.896981 longship-2023.6.26/longship_api_client/api/tariffdistributions/tariffdistribution_put.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.897051 longship-2023.6.26/longship_api_client/api/tariffs/__init__.py
--rw-r--r--   0        0        0     7732 2023-06-26 16:00:19.897369 longship-2023.6.26/longship_api_client/api/tariffs/get_all_tariffs.py
--rw-r--r--   0        0        0     4685 2023-06-26 16:00:19.897492 longship-2023.6.26/longship_api_client/api/tariffs/tariff_get.py
--rw-r--r--   0        0        0     5006 2023-06-26 16:00:19.897616 longship-2023.6.26/longship_api_client/api/tariffs/tariff_post.py
--rw-r--r--   0        0        0     5192 2023-06-26 16:00:19.897743 longship-2023.6.26/longship_api_client/api/tariffs/tariff_put.py
--rw-r--r--   0        0        0        0 2023-06-26 16:00:19.897804 longship-2023.6.26/longship_api_client/api/webhooks/__init__.py
--rw-r--r--   0        0        0     8568 2023-06-26 16:00:19.897979 longship-2023.6.26/longship_api_client/api/webhooks/get_all_webhooks.py
--rw-r--r--   0        0        0     4526 2023-06-26 16:00:19.898246 longship-2023.6.26/longship_api_client/api/webhooks/webhook_delete.py
--rw-r--r--   0        0        0     4747 2023-06-26 16:00:19.898373 longship-2023.6.26/longship_api_client/api/webhooks/webhook_get.py
--rw-r--r--   0        0        0     5026 2023-06-26 16:00:19.898488 longship-2023.6.26/longship_api_client/api/webhooks/webhook_post.py
--rw-r--r--   0        0        0     5388 2023-06-26 16:00:19.898609 longship-2023.6.26/longship_api_client/api/webhooks/webhook_put.py
--rw-r--r--   0        0        0     2817 2023-06-26 16:00:19.898736 longship-2023.6.26/longship_api_client/client.py
--rw-r--r--   0        0        0      470 2023-06-26 16:00:19.898849 longship-2023.6.26/longship_api_client/errors.py
--rw-r--r--   0        0        0    17634 2023-06-26 16:00:19.899028 longship-2023.6.26/longship_api_client/models/__init__.py
--rw-r--r--   0        0        0     2516 2023-06-26 16:00:19.899270 longship-2023.6.26/longship_api_client/models/additional_geo_location_dto.py
--rw-r--r--   0        0        0     2207 2023-06-26 16:00:19.899403 longship-2023.6.26/longship_api_client/models/authorization_data.py
--rw-r--r--   0        0        0     2385 2023-06-26 16:00:19.899529 longship-2023.6.26/longship_api_client/models/business_details_dto.py
--rw-r--r--   0        0        0     1520 2023-06-26 16:00:19.899640 longship-2023.6.26/longship_api_client/models/cancel_reservation_request.py
--rw-r--r--   0        0        0    13561 2023-06-26 16:00:19.899776 longship-2023.6.26/longship_api_client/models/cdr_dto.py
--rw-r--r--   0        0        0     1799 2023-06-26 16:00:19.899895 longship-2023.6.26/longship_api_client/models/cdr_geo_location_dto.py
--rw-r--r--   0        0        0     6718 2023-06-26 16:00:19.900079 longship-2023.6.26/longship_api_client/models/cdr_location_dto.py
--rw-r--r--   0        0        0      202 2023-06-26 16:00:19.900314 longship-2023.6.26/longship_api_client/models/cdr_location_dto_power_type.py
--rw-r--r--   0        0        0     5179 2023-06-26 16:00:19.900442 longship-2023.6.26/longship_api_client/models/cdr_started_by_info_dto.py
--rw-r--r--   0        0        0      668 2023-06-26 16:00:19.900557 longship-2023.6.26/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py
--rw-r--r--   0        0        0      185 2023-06-26 16:00:19.900677 longship-2023.6.26/longship_api_client/models/cdr_started_by_info_dto_roaming_platform_type.py
--rw-r--r--   0        0        0     5488 2023-06-26 16:00:19.900807 longship-2023.6.26/longship_api_client/models/cdr_started_by_token_dto.py
--rw-r--r--   0        0        0      221 2023-06-26 16:00:19.900930 longship-2023.6.26/longship_api_client/models/cdr_started_by_token_dto_auth_method.py
--rw-r--r--   0        0        0      230 2023-06-26 16:00:19.901050 longship-2023.6.26/longship_api_client/models/cdr_started_by_token_dto_token_type.py
--rw-r--r--   0        0        0     1918 2023-06-26 16:00:19.901179 longship-2023.6.26/longship_api_client/models/change_availability_request.py
--rw-r--r--   0        0        0      194 2023-06-26 16:00:19.901304 longship-2023.6.26/longship_api_client/models/change_availability_request_type.py
--rw-r--r--   0        0        0     1574 2023-06-26 16:00:19.901432 longship-2023.6.26/longship_api_client/models/change_configuration_request.py
--rw-r--r--   0        0        0     6026 2023-06-26 16:00:19.901570 longship-2023.6.26/longship_api_client/models/chargepoint_connector_dto.py
--rw-r--r--   0        0        0      176 2023-06-26 16:00:19.901703 longship-2023.6.26/longship_api_client/models/chargepoint_connector_dto_format.py
--rw-r--r--   0        0        0      405 2023-06-26 16:00:19.902100 longship-2023.6.26/longship_api_client/models/chargepoint_connector_dto_operational_status.py
--rw-r--r--   0        0        0      211 2023-06-26 16:00:19.902249 longship-2023.6.26/longship_api_client/models/chargepoint_connector_dto_power_type.py
--rw-r--r--   0        0        0     1100 2023-06-26 16:00:19.902449 longship-2023.6.26/longship_api_client/models/chargepoint_connector_dto_standard.py
--rw-r--r--   0        0        0    17517 2023-06-26 16:00:19.902653 longship-2023.6.26/longship_api_client/models/chargepoint_dto.py
--rw-r--r--   0        0        0      183 2023-06-26 16:00:19.902815 longship-2023.6.26/longship_api_client/models/chargepoint_dto_connectivity_status.py
--rw-r--r--   0        0        0     2540 2023-06-26 16:00:19.903151 longship-2023.6.26/longship_api_client/models/chargepoint_evse_dto.py
--rw-r--r--   0        0        0     3701 2023-06-26 16:00:19.903531 longship-2023.6.26/longship_api_client/models/chargepoint_put_dto.py
--rw-r--r--   0        0        0     7169 2023-06-26 16:00:19.903846 longship-2023.6.26/longship_api_client/models/chargepoint_status_dto.py
--rw-r--r--   0        0        0      189 2023-06-26 16:00:19.904003 longship-2023.6.26/longship_api_client/models/chargepoint_status_dto_connectivity_status.py
--rw-r--r--   0        0        0     3743 2023-06-26 16:00:19.904221 longship-2023.6.26/longship_api_client/models/charging_meter_value_dto.py
--rw-r--r--   0        0        0     1197 2023-06-26 16:00:19.904460 longship-2023.6.26/longship_api_client/models/charging_meter_value_dto_measurand.py
--rw-r--r--   0        0        0      402 2023-06-26 16:00:19.904625 longship-2023.6.26/longship_api_client/models/charging_meter_value_dto_unit.py
--rw-r--r--   0        0        0     2736 2023-06-26 16:00:19.904794 longship-2023.6.26/longship_api_client/models/charging_period_dto.py
--rw-r--r--   0        0        0     6103 2023-06-26 16:00:19.905086 longship-2023.6.26/longship_api_client/models/charging_profile.py
--rw-r--r--   0        0        0      219 2023-06-26 16:00:19.905228 longship-2023.6.26/longship_api_client/models/charging_profile_charging_profile_kind.py
--rw-r--r--   0        0        0      264 2023-06-26 16:00:19.905404 longship-2023.6.26/longship_api_client/models/charging_profile_charging_profile_purpose.py
--rw-r--r--   0        0        0      176 2023-06-26 16:00:19.905580 longship-2023.6.26/longship_api_client/models/charging_profile_recurrency_kind.py
--rw-r--r--   0        0        0     4307 2023-06-26 16:00:19.905728 longship-2023.6.26/longship_api_client/models/charging_schedule.py
--rw-r--r--   0        0        0      161 2023-06-26 16:00:19.905871 longship-2023.6.26/longship_api_client/models/charging_schedule_charging_rate_unit.py
--rw-r--r--   0        0        0     2007 2023-06-26 16:00:19.906409 longship-2023.6.26/longship_api_client/models/charging_schedule_period.py
--rw-r--r--   0        0        0     1180 2023-06-26 16:00:19.906577 longship-2023.6.26/longship_api_client/models/clear_cache_request.py
--rw-r--r--   0        0        0     3421 2023-06-26 16:00:19.906723 longship-2023.6.26/longship_api_client/models/clear_charging_profile_request.py
--rw-r--r--   0        0        0      276 2023-06-26 16:00:19.906886 longship-2023.6.26/longship_api_client/models/clear_charging_profile_request_charging_profile_purpose.py
--rw-r--r--   0        0        0     5744 2023-06-26 16:00:19.907051 longship-2023.6.26/longship_api_client/models/connector_dto.py
--rw-r--r--   0        0        0      165 2023-06-26 16:00:19.907200 longship-2023.6.26/longship_api_client/models/connector_dto_format.py
--rw-r--r--   0        0        0      200 2023-06-26 16:00:19.907337 longship-2023.6.26/longship_api_client/models/connector_dto_power_type.py
--rw-r--r--   0        0        0     1089 2023-06-26 16:00:19.907561 longship-2023.6.26/longship_api_client/models/connector_dto_standard.py
--rw-r--r--   0        0        0     3465 2023-06-26 16:00:19.907704 longship-2023.6.26/longship_api_client/models/connector_operational_status_dto.py
--rw-r--r--   0        0        0      411 2023-06-26 16:00:19.907830 longship-2023.6.26/longship_api_client/models/connector_operational_status_dto_operational_status.py
--rw-r--r--   0        0        0     6202 2023-06-26 16:00:19.907958 longship-2023.6.26/longship_api_client/models/cs_charging_profiles.py
--rw-r--r--   0        0        0      222 2023-06-26 16:00:19.908086 longship-2023.6.26/longship_api_client/models/cs_charging_profiles_charging_profile_kind.py
--rw-r--r--   0        0        0      267 2023-06-26 16:00:19.908346 longship-2023.6.26/longship_api_client/models/cs_charging_profiles_charging_profile_purpose.py
--rw-r--r--   0        0        0      179 2023-06-26 16:00:19.908522 longship-2023.6.26/longship_api_client/models/cs_charging_profiles_recurrency_kind.py
--rw-r--r--   0        0        0     1996 2023-06-26 16:00:19.908662 longship-2023.6.26/longship_api_client/models/data_transfer_request.py
--rw-r--r--   0        0        0     1726 2023-06-26 16:00:19.908786 longship-2023.6.26/longship_api_client/models/display_text_dto.py
--rw-r--r--   0        0        0     3730 2023-06-26 16:00:19.908920 longship-2023.6.26/longship_api_client/models/energy_mix_dto.py
--rw-r--r--   0        0        0     2229 2023-06-26 16:00:19.909045 longship-2023.6.26/longship_api_client/models/energy_source_dto.py
--rw-r--r--   0        0        0      316 2023-06-26 16:00:19.909172 longship-2023.6.26/longship_api_client/models/energy_source_dto_source.py
--rw-r--r--   0        0        0     2180 2023-06-26 16:00:19.909461 longship-2023.6.26/longship_api_client/models/entity_tag_header_value.py
--rw-r--r--   0        0        0     2340 2023-06-26 16:00:19.909584 longship-2023.6.26/longship_api_client/models/environmental_impact_dto.py
--rw-r--r--   0        0        0      209 2023-06-26 16:00:19.909709 longship-2023.6.26/longship_api_client/models/environmental_impact_dto_category.py
--rw-r--r--   0        0        0     2592 2023-06-26 16:00:19.909843 longship-2023.6.26/longship_api_client/models/exceptional_period_dto.py
--rw-r--r--   0        0        0     4622 2023-06-26 16:00:19.909979 longship-2023.6.26/longship_api_client/models/file_content_result.py
--rw-r--r--   0        0        0     1781 2023-06-26 16:00:19.910112 longship-2023.6.26/longship_api_client/models/geo_location_dto.py
--rw-r--r--   0        0        0      190 2023-06-26 16:00:19.910233 longship-2023.6.26/longship_api_client/models/get_all_cdrs_order_by.py
--rw-r--r--   0        0        0      224 2023-06-26 16:00:19.910360 longship-2023.6.26/longship_api_client/models/get_all_chargepoints_order_by.py
--rw-r--r--   0        0        0      191 2023-06-26 16:00:19.910499 longship-2023.6.26/longship_api_client/models/get_all_locations_order_by.py
--rw-r--r--   0        0        0      203 2023-06-26 16:00:19.910619 longship-2023.6.26/longship_api_client/models/get_all_reimbursementcdrs_order_by.py
--rw-r--r--   0        0        0      164 2023-06-26 16:00:19.910737 longship-2023.6.26/longship_api_client/models/get_all_sessions_order_by.py
--rw-r--r--   0        0        0      203 2023-06-26 16:00:19.910857 longship-2023.6.26/longship_api_client/models/get_all_tariffs_order_by.py
--rw-r--r--   0        0        0      144 2023-06-26 16:00:19.910971 longship-2023.6.26/longship_api_client/models/get_all_webhooks_order_by.py
--rw-r--r--   0        0        0     2844 2023-06-26 16:00:19.911220 longship-2023.6.26/longship_api_client/models/get_composite_schedule_request.py
--rw-r--r--   0        0        0      172 2023-06-26 16:00:19.911415 longship-2023.6.26/longship_api_client/models/get_composite_schedule_request_charging_rate_unit.py
--rw-r--r--   0        0        0     1621 2023-06-26 16:00:19.911532 longship-2023.6.26/longship_api_client/models/get_configuration_request.py
--rw-r--r--   0        0        0     3343 2023-06-26 16:00:19.911661 longship-2023.6.26/longship_api_client/models/get_diagnostics_request.py
--rw-r--r--   0        0        0     1231 2023-06-26 16:00:19.911780 longship-2023.6.26/longship_api_client/models/get_local_list_version_request.py
--rw-r--r--   0        0        0     4898 2023-06-26 16:00:19.911903 longship-2023.6.26/longship_api_client/models/hours_dto.py
--rw-r--r--   0        0        0     2581 2023-06-26 16:00:19.912026 longship-2023.6.26/longship_api_client/models/id_tag_info.py
--rw-r--r--   0        0        0      252 2023-06-26 16:00:19.912140 longship-2023.6.26/longship_api_client/models/id_tag_info_status.py
--rw-r--r--   0        0        0     3089 2023-06-26 16:00:19.912263 longship-2023.6.26/longship_api_client/models/image_dto.py
--rw-r--r--   0        0        0      287 2023-06-26 16:00:19.912517 longship-2023.6.26/longship_api_client/models/image_dto_category.py
--rw-r--r--   0        0        0     8559 2023-06-26 16:00:19.912653 longship-2023.6.26/longship_api_client/models/interchange_format_cdr.py
--rw-r--r--   0        0        0     5283 2023-06-26 16:00:19.912789 longship-2023.6.26/longship_api_client/models/local_token_group_get_dto.py
--rw-r--r--   0        0        0     3911 2023-06-26 16:00:19.912916 longship-2023.6.26/longship_api_client/models/local_token_group_post_dto.py
--rw-r--r--   0        0        0     3899 2023-06-26 16:00:19.913044 longship-2023.6.26/longship_api_client/models/local_token_group_put_dto.py
--rw-r--r--   0        0        0     2722 2023-06-26 16:00:19.913170 longship-2023.6.26/longship_api_client/models/local_token_group_token_get_dto.py
--rw-r--r--   0        0        0     2310 2023-06-26 16:00:19.913336 longship-2023.6.26/longship_api_client/models/local_token_group_token_post_dto.py
--rw-r--r--   0        0        0     2305 2023-06-26 16:00:19.913457 longship-2023.6.26/longship_api_client/models/local_token_group_token_put_dto.py
--rw-r--r--   0        0        0     1619 2023-06-26 16:00:19.913572 longship-2023.6.26/longship_api_client/models/location_charge_point_dto.py
--rw-r--r--   0        0        0    17497 2023-06-26 16:00:19.913731 longship-2023.6.26/longship_api_client/models/location_dto.py
--rw-r--r--   0        0        0      690 2023-06-26 16:00:19.913864 longship-2023.6.26/longship_api_client/models/location_dto_facilities_item.py
--rw-r--r--   0        0        0      341 2023-06-26 16:00:19.913988 longship-2023.6.26/longship_api_client/models/location_dto_parking_type.py
--rw-r--r--   0        0        0    11569 2023-06-26 16:00:19.914142 longship-2023.6.26/longship_api_client/models/location_evse_dto.py
--rw-r--r--   0        0        0      698 2023-06-26 16:00:19.914413 longship-2023.6.26/longship_api_client/models/location_evse_dto_capabilities_item.py
--rw-r--r--   0        0        0      277 2023-06-26 16:00:19.914536 longship-2023.6.26/longship_api_client/models/location_evse_dto_parking_restrictions_item.py
--rw-r--r--   0        0        0      364 2023-06-26 16:00:19.914656 longship-2023.6.26/longship_api_client/models/location_evse_dto_status.py
--rw-r--r--   0        0        0    17038 2023-06-26 16:00:19.914818 longship-2023.6.26/longship_api_client/models/location_post_dto.py
--rw-r--r--   0        0        0      694 2023-06-26 16:00:19.914939 longship-2023.6.26/longship_api_client/models/location_post_dto_facilities_item.py
--rw-r--r--   0        0        0      345 2023-06-26 16:00:19.915048 longship-2023.6.26/longship_api_client/models/location_post_dto_parking_type.py
--rw-r--r--   0        0        0    17258 2023-06-26 16:00:19.915198 longship-2023.6.26/longship_api_client/models/location_put_dto.py
--rw-r--r--   0        0        0      693 2023-06-26 16:00:19.915320 longship-2023.6.26/longship_api_client/models/location_put_dto_facilities_item.py
--rw-r--r--   0        0        0      344 2023-06-26 16:00:19.915650 longship-2023.6.26/longship_api_client/models/location_put_dto_parking_type.py
--rw-r--r--   0        0        0     1854 2023-06-26 16:00:19.915768 longship-2023.6.26/longship_api_client/models/location_tariff_distribution_dto.py
--rw-r--r--   0        0        0     2379 2023-06-26 16:00:19.915889 longship-2023.6.26/longship_api_client/models/longship_error.py
--rw-r--r--   0        0        0     1920 2023-06-26 16:00:19.916000 longship-2023.6.26/longship_api_client/models/longship_error_detail.py
--rw-r--r--   0        0        0     5923 2023-06-26 16:00:19.916126 longship-2023.6.26/longship_api_client/models/message_log_dto.py
--rw-r--r--   0        0        0      219 2023-06-26 16:00:19.916232 longship-2023.6.26/longship_api_client/models/message_log_dto_direction.py
--rw-r--r--   0        0        0     1335 2023-06-26 16:00:19.916490 longship-2023.6.26/longship_api_client/models/message_log_dto_ocpp_message_type.py
--rw-r--r--   0        0        0      227 2023-06-26 16:00:19.916750 longship-2023.6.26/longship_api_client/models/message_log_dto_wamp_message_type.py
--rw-r--r--   0        0        0     2135 2023-06-26 16:00:19.916889 longship-2023.6.26/longship_api_client/models/organization_unit_financial_details_dto.py
--rw-r--r--   0        0        0     8654 2023-06-26 16:00:19.917030 longship-2023.6.26/longship_api_client/models/organization_unit_get_dto.py
--rw-r--r--   0        0        0     7882 2023-06-26 16:00:19.917159 longship-2023.6.26/longship_api_client/models/organization_unit_post_dto.py
--rw-r--r--   0        0        0     7631 2023-06-26 16:00:19.917289 longship-2023.6.26/longship_api_client/models/organization_unit_put_dto.py
--rw-r--r--   0        0        0     4792 2023-06-26 16:00:19.917419 longship-2023.6.26/longship_api_client/models/price_info_dto.py
--rw-r--r--   0        0        0     3235 2023-06-26 16:00:19.917544 longship-2023.6.26/longship_api_client/models/private_emp_tariff_dto.py
--rw-r--r--   0        0        0      161 2023-06-26 16:00:19.917650 longship-2023.6.26/longship_api_client/models/private_emp_tariff_dto_power_type.py
--rw-r--r--   0        0        0     2984 2023-06-26 16:00:19.917824 longship-2023.6.26/longship_api_client/models/publish_token_type_dto.py
--rw-r--r--   0        0        0      224 2023-06-26 16:00:19.917985 longship-2023.6.26/longship_api_client/models/publish_token_type_dto_type.py
--rw-r--r--   0        0        0     2097 2023-06-26 16:00:19.918105 longship-2023.6.26/longship_api_client/models/regular_hours_dto.py
--rw-r--r--   0        0        0    11178 2023-06-26 16:00:19.918236 longship-2023.6.26/longship_api_client/models/reimburse_info_dto.py
--rw-r--r--   0        0        0      205 2023-06-26 16:00:19.918347 longship-2023.6.26/longship_api_client/models/reimburse_info_dto_type.py
--rw-r--r--   0        0        0     3914 2023-06-26 16:00:19.918467 longship-2023.6.26/longship_api_client/models/reimburse_started_by_info_dto.py
--rw-r--r--   0        0        0      674 2023-06-26 16:00:19.918586 longship-2023.6.26/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py
--rw-r--r--   0        0        0     5626 2023-06-26 16:00:19.918712 longship-2023.6.26/longship_api_client/models/reimburse_started_by_token_dto.py
--rw-r--r--   0        0        0      227 2023-06-26 16:00:19.918949 longship-2023.6.26/longship_api_client/models/reimburse_started_by_token_dto_auth_method.py
--rw-r--r--   0        0        0      236 2023-06-26 16:00:19.919062 longship-2023.6.26/longship_api_client/models/reimburse_started_by_token_dto_token_type.py
--rw-r--r--   0        0        0     2926 2023-06-26 16:00:19.919183 longship-2023.6.26/longship_api_client/models/reimbursement_bank_details_dto.py
--rw-r--r--   0        0        0    21317 2023-06-26 16:00:19.919340 longship-2023.6.26/longship_api_client/models/reimbursement_cdr_dto.py
--rw-r--r--   0        0        0     1867 2023-06-26 16:00:19.919476 longship-2023.6.26/longship_api_client/models/reimbursement_cdr_geo_location_dto.py
--rw-r--r--   0        0        0     7009 2023-06-26 16:00:19.919607 longship-2023.6.26/longship_api_client/models/reimbursement_cdr_location_dto.py
--rw-r--r--   0        0        0      215 2023-06-26 16:00:19.919855 longship-2023.6.26/longship_api_client/models/reimbursement_cdr_location_dto_power_type.py
--rw-r--r--   0        0        0     2330 2023-06-26 16:00:19.919972 longship-2023.6.26/longship_api_client/models/reimbursement_customer_share_dto.py
--rw-r--r--   0        0        0     1813 2023-06-26 16:00:19.920092 longship-2023.6.26/longship_api_client/models/reimbursement_price_dto.py
--rw-r--r--   0        0        0     4578 2023-06-26 16:00:19.920212 longship-2023.6.26/longship_api_client/models/reimbursement_tariff_dto.py
--rw-r--r--   0        0        0      209 2023-06-26 16:00:19.920328 longship-2023.6.26/longship_api_client/models/reimbursement_tariff_dto_status.py
--rw-r--r--   0        0        0     2720 2023-06-26 16:00:19.920443 longship-2023.6.26/longship_api_client/models/remote_start_transaction_request.py
--rw-r--r--   0        0        0     1543 2023-06-26 16:00:19.920556 longship-2023.6.26/longship_api_client/models/remote_stop_transaction_request.py
--rw-r--r--   0        0        0     2538 2023-06-26 16:00:19.920673 longship-2023.6.26/longship_api_client/models/reserve_now_request.py
--rw-r--r--   0        0        0     1524 2023-06-26 16:00:19.920881 longship-2023.6.26/longship_api_client/models/reset_request.py
--rw-r--r--   0        0        0      157 2023-06-26 16:00:19.920991 longship-2023.6.26/longship_api_client/models/reset_request_type.py
--rw-r--r--   0        0        0     3346 2023-06-26 16:00:19.921117 longship-2023.6.26/longship_api_client/models/send_local_list_request.py
--rw-r--r--   0        0        0      187 2023-06-26 16:00:19.921237 longship-2023.6.26/longship_api_client/models/send_local_list_request_update_type.py
--rw-r--r--   0        0        0    16519 2023-06-26 16:00:19.921384 longship-2023.6.26/longship_api_client/models/session_dto.py
--rw-r--r--   0        0        0      251 2023-06-26 16:00:19.921491 longship-2023.6.26/longship_api_client/models/session_dto_status.py
--rw-r--r--   0        0        0     1819 2023-06-26 16:00:19.921601 longship-2023.6.26/longship_api_client/models/session_geo_location_dto.py
--rw-r--r--   0        0        0     6802 2023-06-26 16:00:19.921722 longship-2023.6.26/longship_api_client/models/session_location_dto.py
--rw-r--r--   0        0        0      206 2023-06-26 16:00:19.921830 longship-2023.6.26/longship_api_client/models/session_location_dto_power_type.py
--rw-r--r--   0        0        0     2048 2023-06-26 16:00:19.921941 longship-2023.6.26/longship_api_client/models/set_charging_profile_request.py
--rw-r--r--   0        0        0     5085 2023-06-26 16:00:19.922062 longship-2023.6.26/longship_api_client/models/started_by_info_dto.py
--rw-r--r--   0        0        0      665 2023-06-26 16:00:19.922175 longship-2023.6.26/longship_api_client/models/started_by_info_dto_authorization_state.py
--rw-r--r--   0        0        0      182 2023-06-26 16:00:19.922285 longship-2023.6.26/longship_api_client/models/started_by_info_dto_roaming_platform_type.py
--rw-r--r--   0        0        0     5408 2023-06-26 16:00:19.922417 longship-2023.6.26/longship_api_client/models/started_by_token_dto.py
--rw-r--r--   0        0        0      218 2023-06-26 16:00:19.922533 longship-2023.6.26/longship_api_client/models/started_by_token_dto_auth_method.py
--rw-r--r--   0        0        0      227 2023-06-26 16:00:19.923113 longship-2023.6.26/longship_api_client/models/started_by_token_dto_token_type.py
--rw-r--r--   0        0        0     3296 2023-06-26 16:00:19.923404 longship-2023.6.26/longship_api_client/models/status_schedule_dto.py
--rw-r--r--   0        0        0      366 2023-06-26 16:00:19.923560 longship-2023.6.26/longship_api_client/models/status_schedule_dto_status.py
--rw-r--r--   0        0        0     2475 2023-06-26 16:00:19.923890 longship-2023.6.26/longship_api_client/models/string_segment.py
--rw-r--r--   0        0        0     2787 2023-06-26 16:00:19.924076 longship-2023.6.26/longship_api_client/models/tariff_assertion_dto.py
--rw-r--r--   0        0        0      283 2023-06-26 16:00:19.924212 longship-2023.6.26/longship_api_client/models/tariff_assertion_dto_tariff_type.py
--rw-r--r--   0        0        0     6447 2023-06-26 16:00:19.924335 longship-2023.6.26/longship_api_client/models/tariff_distribution_get_dto.py
--rw-r--r--   0        0        0     3617 2023-06-26 16:00:19.924485 longship-2023.6.26/longship_api_client/models/tariff_distribution_history_dto.py
--rw-r--r--   0        0        0     3409 2023-06-26 16:00:19.924751 longship-2023.6.26/longship_api_client/models/tariff_distribution_post_dto.py
--rw-r--r--   0        0        0     3404 2023-06-26 16:00:19.925022 longship-2023.6.26/longship_api_client/models/tariff_distribution_put_dto.py
--rw-r--r--   0        0        0    12525 2023-06-26 16:00:19.925189 longship-2023.6.26/longship_api_client/models/tariff_dto.py
--rw-r--r--   0        0        0      186 2023-06-26 16:00:19.925352 longship-2023.6.26/longship_api_client/models/tariff_dto_tariff_type.py
--rw-r--r--   0        0        0      241 2023-06-26 16:00:19.925490 longship-2023.6.26/longship_api_client/models/tariff_dto_usage_type.py
--rw-r--r--   0        0        0     5977 2023-06-26 16:00:19.925640 longship-2023.6.26/longship_api_client/models/tariff_info_dto.py
--rw-r--r--   0        0        0     6945 2023-06-26 16:00:19.925780 longship-2023.6.26/longship_api_client/models/tariff_post_dto.py
--rw-r--r--   0        0        0      245 2023-06-26 16:00:19.926087 longship-2023.6.26/longship_api_client/models/tariff_post_dto_usage_type.py
--rw-r--r--   0        0        0     7511 2023-06-26 16:00:19.926318 longship-2023.6.26/longship_api_client/models/tariff_price_dto.py
--rw-r--r--   0        0        0      209 2023-06-26 16:00:19.926463 longship-2023.6.26/longship_api_client/models/tariff_price_dto_approval_status.py
--rw-r--r--   0        0        0     6188 2023-06-26 16:00:19.926616 longship-2023.6.26/longship_api_client/models/tariff_put_dto.py
--rw-r--r--   0        0        0     2235 2023-06-26 16:00:19.926826 longship-2023.6.26/longship_api_client/models/trigger_message_request.py
--rw-r--r--   0        0        0      420 2023-06-26 16:00:19.927163 longship-2023.6.26/longship_api_client/models/trigger_message_request_requested_message.py
--rw-r--r--   0        0        0     1490 2023-06-26 16:00:19.928533 longship-2023.6.26/longship_api_client/models/unlock_connector_request.py
--rw-r--r--   0        0        0     2409 2023-06-26 16:00:19.928994 longship-2023.6.26/longship_api_client/models/update_firmware_request.py
--rw-r--r--   0        0        0     5393 2023-06-26 16:00:19.929113 longship-2023.6.26/longship_api_client/models/webhook_get_dto.py
--rw-r--r--   0        0        0      398 2023-06-26 16:00:19.929555 longship-2023.6.26/longship_api_client/models/webhook_get_dto_event_types_item.py
--rw-r--r--   0        0        0     1703 2023-06-26 16:00:19.929899 longship-2023.6.26/longship_api_client/models/webhook_header_dto.py
--rw-r--r--   0        0        0     4020 2023-06-26 16:00:19.930015 longship-2023.6.26/longship_api_client/models/webhook_post_dto.py
--rw-r--r--   0        0        0      399 2023-06-26 16:00:19.930121 longship-2023.6.26/longship_api_client/models/webhook_post_dto_event_types_item.py
--rw-r--r--   0        0        0     4009 2023-06-26 16:00:19.930238 longship-2023.6.26/longship_api_client/models/webhook_put_dto.py
--rw-r--r--   0        0        0      398 2023-06-26 16:00:19.930345 longship-2023.6.26/longship_api_client/models/webhook_put_dto_event_types_item.py
--rw-r--r--   0        0        0     4096 2023-06-26 16:00:19.930595 longship-2023.6.26/longship_api_client/models/webhook_summary_get_dto.py
--rw-r--r--   0        0        0      405 2023-06-26 16:00:19.930722 longship-2023.6.26/longship_api_client/models/webhook_summary_get_dto_event_types_item.py
--rw-r--r--   0        0        0       25 2023-06-26 16:00:19.930817 longship-2023.6.26/longship_api_client/py.typed
--rw-r--r--   0        0        0      993 2023-06-26 16:00:19.930917 longship-2023.6.26/longship_api_client/types.py
--rw-r--r--   0        0        0      818 2023-06-26 16:00:19.931382 longship-2023.6.26/pyproject.toml
--rw-r--r--   0        0        0     5236 1970-01-01 00:00:00.000000 longship-2023.6.26/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-26 16:00:19.878825 longship-2023.6.27/LICENSE
+-rw-r--r--   0        0        0     4661 2023-06-26 16:47:23.288883 longship-2023.6.27/README.md
+-rw-r--r--   0        0        0     7215 2023-06-26 16:00:19.886579 longship-2023.6.27/longship/client.py
+-rw-r--r--   0        0        0      112 2023-06-26 16:00:19.886682 longship-2023.6.27/longship/errors.py
+-rw-r--r--   0        0        0     3084 2023-06-26 21:07:50.182772 longship-2023.6.27/longship/types.py
+-rw-r--r--   0        0        0      156 2023-06-26 16:00:19.887019 longship-2023.6.27/longship_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-26 16:00:19.887155 longship-2023.6.27/longship_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.887208 longship-2023.6.27/longship_api_client/api/cdrs/__init__.py
+-rw-r--r--   0        0        0     4619 2023-06-26 16:00:19.887462 longship-2023.6.27/longship_api_client/api/cdrs/cdr_get.py
+-rw-r--r--   0        0        0    10429 2023-06-26 16:00:19.887727 longship-2023.6.27/longship_api_client/api/cdrs/get_all_cdrs.py
+-rw-r--r--   0        0        0     8447 2023-06-26 16:00:19.887850 longship-2023.6.27/longship_api_client/api/cdrs/get_all_interchangeformat.py
+-rw-r--r--   0        0        0     6309 2023-06-26 16:00:19.887973 longship-2023.6.27/longship_api_client/api/cdrs/get_file_full_download_cdrs.py
+-rw-r--r--   0        0        0     6288 2023-06-26 16:00:19.888095 longship-2023.6.27/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.888157 longship-2023.6.27/longship_api_client/api/chargepoint_status/__init__.py
+-rw-r--r--   0        0        0     4940 2023-06-26 16:00:19.888332 longship-2023.6.27/longship_api_client/api/chargepoint_status/chargepoint_status_get.py
+-rw-r--r--   0        0        0     6787 2023-06-26 16:00:19.888455 longship-2023.6.27/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.888516 longship-2023.6.27/longship_api_client/api/chargepoints/__init__.py
+-rw-r--r--   0        0        0     4795 2023-06-26 16:00:19.888699 longship-2023.6.27/longship_api_client/api/chargepoints/chargepoint_get.py
+-rw-r--r--   0        0        0     5302 2023-06-26 16:00:19.888829 longship-2023.6.27/longship_api_client/api/chargepoints/chargepoint_put.py
+-rw-r--r--   0        0        0    12511 2023-06-26 16:00:19.888975 longship-2023.6.27/longship_api_client/api/chargepoints/get_all_chargepointmessages.py
+-rw-r--r--   0        0        0     8572 2023-06-26 16:00:19.889108 longship-2023.6.27/longship_api_client/api/chargepoints/get_all_chargepoints.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.889164 longship-2023.6.27/longship_api_client/api/commands/__init__.py
+-rw-r--r--   0        0        0     5291 2023-06-26 16:00:19.889355 longship-2023.6.27/longship_api_client/api/commands/send_cancel_reservation_request.py
+-rw-r--r--   0        0        0     5311 2023-06-26 16:00:19.889628 longship-2023.6.27/longship_api_client/api/commands/send_change_availability_request.py
+-rw-r--r--   0        0        0     5331 2023-06-26 16:00:19.889795 longship-2023.6.27/longship_api_client/api/commands/send_change_configuration_request.py
+-rw-r--r--   0        0        0     5151 2023-06-26 16:00:19.889931 longship-2023.6.27/longship_api_client/api/commands/send_clear_cache_request.py
+-rw-r--r--   0        0        0     5352 2023-06-26 16:00:19.890060 longship-2023.6.27/longship_api_client/api/commands/send_clear_charging_profile_request.py
+-rw-r--r--   0        0        0     5191 2023-06-26 16:00:19.890188 longship-2023.6.27/longship_api_client/api/commands/send_data_transfer_request.py
+-rw-r--r--   0        0        0     5352 2023-06-26 16:00:19.890335 longship-2023.6.27/longship_api_client/api/commands/send_get_composite_schedule_request.py
+-rw-r--r--   0        0        0     5271 2023-06-26 16:00:19.890534 longship-2023.6.27/longship_api_client/api/commands/send_get_configuration_request.py
+-rw-r--r--   0        0        0     5231 2023-06-26 16:00:19.890672 longship-2023.6.27/longship_api_client/api/commands/send_get_diagnostics_request.py
+-rw-r--r--   0        0        0     5333 2023-06-26 16:00:19.890880 longship-2023.6.27/longship_api_client/api/commands/send_get_local_list_version_request.py
+-rw-r--r--   0        0        0     5381 2023-06-26 16:00:19.891176 longship-2023.6.27/longship_api_client/api/commands/send_remote_start_transaction_request.py
+-rw-r--r--   0        0        0     5361 2023-06-26 16:00:19.891376 longship-2023.6.27/longship_api_client/api/commands/send_remote_stop_transaction_request.py
+-rw-r--r--   0        0        0     5151 2023-06-26 16:00:19.891498 longship-2023.6.27/longship_api_client/api/commands/send_reserve_now_request.py
+-rw-r--r--   0        0        0     5050 2023-06-26 16:00:19.891732 longship-2023.6.27/longship_api_client/api/commands/send_reset_request.py
+-rw-r--r--   0        0        0     5212 2023-06-26 16:00:19.891864 longship-2023.6.27/longship_api_client/api/commands/send_send_local_list_request.py
+-rw-r--r--   0        0        0     5312 2023-06-26 16:00:19.891993 longship-2023.6.27/longship_api_client/api/commands/send_set_charging_profile_request.py
+-rw-r--r--   0        0        0     5231 2023-06-26 16:00:19.892118 longship-2023.6.27/longship_api_client/api/commands/send_trigger_message_request.py
+-rw-r--r--   0        0        0     5251 2023-06-26 16:00:19.892369 longship-2023.6.27/longship_api_client/api/commands/send_unlock_connector_request.py
+-rw-r--r--   0        0        0     5231 2023-06-26 16:00:19.892498 longship-2023.6.27/longship_api_client/api/commands/send_update_firmware_request.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.892562 longship-2023.6.27/longship_api_client/api/localtokengroups/__init__.py
+-rw-r--r--   0        0        0     6805 2023-06-26 16:00:19.892749 longship-2023.6.27/longship_api_client/api/localtokengroups/get_all_localtokengroups.py
+-rw-r--r--   0        0        0     4598 2023-06-26 16:00:19.892881 longship-2023.6.27/longship_api_client/api/localtokengroups/local_token_group_delete.py
+-rw-r--r--   0        0        0     5198 2023-06-26 16:00:19.893124 longship-2023.6.27/longship_api_client/api/localtokengroups/local_token_group_post.py
+-rw-r--r--   0        0        0     5383 2023-06-26 16:00:19.893249 longship-2023.6.27/longship_api_client/api/localtokengroups/local_token_group_put.py
+-rw-r--r--   0        0        0     4937 2023-06-26 16:00:19.893381 longship-2023.6.27/longship_api_client/api/localtokengroups/localtokengroup_get.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.893447 longship-2023.6.27/longship_api_client/api/locations/__init__.py
+-rw-r--r--   0        0        0     8422 2023-06-26 16:00:19.893637 longship-2023.6.27/longship_api_client/api/locations/get_all_locations.py
+-rw-r--r--   0        0        0     4729 2023-06-26 16:00:19.893769 longship-2023.6.27/longship_api_client/api/locations/location_get.py
+-rw-r--r--   0        0        0     5203 2023-06-26 16:00:19.893904 longship-2023.6.27/longship_api_client/api/locations/location_post.py
+-rw-r--r--   0        0        0     5020 2023-06-26 16:00:19.894032 longship-2023.6.27/longship_api_client/api/locations/location_put.py
+-rw-r--r--   0        0        0     5309 2023-06-26 16:00:19.894173 longship-2023.6.27/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py
+-rw-r--r--   0        0        0     5624 2023-06-26 16:00:19.894313 longship-2023.6.27/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.894383 longship-2023.6.27/longship_api_client/api/mspreimbursement/__init__.py
+-rw-r--r--   0        0        0     4660 2023-06-26 16:00:19.894562 longship-2023.6.27/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.894631 longship-2023.6.27/longship_api_client/api/organizationunits/__init__.py
+-rw-r--r--   0        0        0     6828 2023-06-26 16:00:19.894949 longship-2023.6.27/longship_api_client/api/organizationunits/get_all_organizationunits.py
+-rw-r--r--   0        0        0     4960 2023-06-26 16:00:19.895152 longship-2023.6.27/longship_api_client/api/organizationunits/organization_unit_get.py
+-rw-r--r--   0        0        0     5219 2023-06-26 16:00:19.895279 longship-2023.6.27/longship_api_client/api/organizationunits/organization_unit_post.py
+-rw-r--r--   0        0        0     5390 2023-06-26 16:00:19.895408 longship-2023.6.27/longship_api_client/api/organizationunits/organization_unit_put.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.895477 longship-2023.6.27/longship_api_client/api/reimbursement/__init__.py
+-rw-r--r--   0        0        0    11074 2023-06-26 16:00:19.895698 longship-2023.6.27/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py
+-rw-r--r--   0        0        0     5314 2023-06-26 16:00:19.895832 longship-2023.6.27/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py
+-rw-r--r--   0        0        0     4906 2023-06-26 16:00:19.895962 longship-2023.6.27/longship_api_client/api/reimbursement/reimbursement_cdr_get.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.896026 longship-2023.6.27/longship_api_client/api/sessions/__init__.py
+-rw-r--r--   0        0        0    11057 2023-06-26 16:00:19.896212 longship-2023.6.27/longship_api_client/api/sessions/get_all_sessions.py
+-rw-r--r--   0        0        0     4707 2023-06-26 16:00:19.896340 longship-2023.6.27/longship_api_client/api/sessions/session_get.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.896408 longship-2023.6.27/longship_api_client/api/tariffdistributions/__init__.py
+-rw-r--r--   0        0        0     6878 2023-06-26 16:00:19.896589 longship-2023.6.27/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py
+-rw-r--r--   0        0        0     4856 2023-06-26 16:00:19.896717 longship-2023.6.27/longship_api_client/api/tariffdistributions/tariffdistribution_get.py
+-rw-r--r--   0        0        0     5111 2023-06-26 16:00:19.896842 longship-2023.6.27/longship_api_client/api/tariffdistributions/tariffdistribution_post.py
+-rw-r--r--   0        0        0     5765 2023-06-26 16:00:19.896981 longship-2023.6.27/longship_api_client/api/tariffdistributions/tariffdistribution_put.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.897051 longship-2023.6.27/longship_api_client/api/tariffs/__init__.py
+-rw-r--r--   0        0        0     7732 2023-06-26 16:00:19.897369 longship-2023.6.27/longship_api_client/api/tariffs/get_all_tariffs.py
+-rw-r--r--   0        0        0     4685 2023-06-26 16:00:19.897492 longship-2023.6.27/longship_api_client/api/tariffs/tariff_get.py
+-rw-r--r--   0        0        0     5006 2023-06-26 16:00:19.897616 longship-2023.6.27/longship_api_client/api/tariffs/tariff_post.py
+-rw-r--r--   0        0        0     5192 2023-06-26 16:00:19.897743 longship-2023.6.27/longship_api_client/api/tariffs/tariff_put.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:00:19.897804 longship-2023.6.27/longship_api_client/api/webhooks/__init__.py
+-rw-r--r--   0        0        0     8568 2023-06-26 16:00:19.897979 longship-2023.6.27/longship_api_client/api/webhooks/get_all_webhooks.py
+-rw-r--r--   0        0        0     4526 2023-06-26 16:00:19.898246 longship-2023.6.27/longship_api_client/api/webhooks/webhook_delete.py
+-rw-r--r--   0        0        0     4747 2023-06-26 16:00:19.898373 longship-2023.6.27/longship_api_client/api/webhooks/webhook_get.py
+-rw-r--r--   0        0        0     5026 2023-06-26 16:00:19.898488 longship-2023.6.27/longship_api_client/api/webhooks/webhook_post.py
+-rw-r--r--   0        0        0     5388 2023-06-26 16:00:19.898609 longship-2023.6.27/longship_api_client/api/webhooks/webhook_put.py
+-rw-r--r--   0        0        0     2817 2023-06-26 16:00:19.898736 longship-2023.6.27/longship_api_client/client.py
+-rw-r--r--   0        0        0      470 2023-06-26 16:00:19.898849 longship-2023.6.27/longship_api_client/errors.py
+-rw-r--r--   0        0        0    17634 2023-06-26 16:00:19.899028 longship-2023.6.27/longship_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2516 2023-06-26 16:00:19.899270 longship-2023.6.27/longship_api_client/models/additional_geo_location_dto.py
+-rw-r--r--   0        0        0     2207 2023-06-26 16:00:19.899403 longship-2023.6.27/longship_api_client/models/authorization_data.py
+-rw-r--r--   0        0        0     2385 2023-06-26 16:00:19.899529 longship-2023.6.27/longship_api_client/models/business_details_dto.py
+-rw-r--r--   0        0        0     1520 2023-06-26 16:00:19.899640 longship-2023.6.27/longship_api_client/models/cancel_reservation_request.py
+-rw-r--r--   0        0        0    13561 2023-06-26 16:00:19.899776 longship-2023.6.27/longship_api_client/models/cdr_dto.py
+-rw-r--r--   0        0        0     1799 2023-06-26 16:00:19.899895 longship-2023.6.27/longship_api_client/models/cdr_geo_location_dto.py
+-rw-r--r--   0        0        0     6718 2023-06-26 16:00:19.900079 longship-2023.6.27/longship_api_client/models/cdr_location_dto.py
+-rw-r--r--   0        0        0      202 2023-06-26 16:00:19.900314 longship-2023.6.27/longship_api_client/models/cdr_location_dto_power_type.py
+-rw-r--r--   0        0        0     5179 2023-06-26 16:00:19.900442 longship-2023.6.27/longship_api_client/models/cdr_started_by_info_dto.py
+-rw-r--r--   0        0        0      668 2023-06-26 16:00:19.900557 longship-2023.6.27/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py
+-rw-r--r--   0        0        0      185 2023-06-26 16:00:19.900677 longship-2023.6.27/longship_api_client/models/cdr_started_by_info_dto_roaming_platform_type.py
+-rw-r--r--   0        0        0     5488 2023-06-26 16:00:19.900807 longship-2023.6.27/longship_api_client/models/cdr_started_by_token_dto.py
+-rw-r--r--   0        0        0      221 2023-06-26 16:00:19.900930 longship-2023.6.27/longship_api_client/models/cdr_started_by_token_dto_auth_method.py
+-rw-r--r--   0        0        0      230 2023-06-26 16:00:19.901050 longship-2023.6.27/longship_api_client/models/cdr_started_by_token_dto_token_type.py
+-rw-r--r--   0        0        0     1918 2023-06-26 16:00:19.901179 longship-2023.6.27/longship_api_client/models/change_availability_request.py
+-rw-r--r--   0        0        0      194 2023-06-26 16:00:19.901304 longship-2023.6.27/longship_api_client/models/change_availability_request_type.py
+-rw-r--r--   0        0        0     1574 2023-06-26 16:00:19.901432 longship-2023.6.27/longship_api_client/models/change_configuration_request.py
+-rw-r--r--   0        0        0     6026 2023-06-26 16:00:19.901570 longship-2023.6.27/longship_api_client/models/chargepoint_connector_dto.py
+-rw-r--r--   0        0        0      176 2023-06-26 16:00:19.901703 longship-2023.6.27/longship_api_client/models/chargepoint_connector_dto_format.py
+-rw-r--r--   0        0        0      405 2023-06-26 16:00:19.902100 longship-2023.6.27/longship_api_client/models/chargepoint_connector_dto_operational_status.py
+-rw-r--r--   0        0        0      211 2023-06-26 16:00:19.902249 longship-2023.6.27/longship_api_client/models/chargepoint_connector_dto_power_type.py
+-rw-r--r--   0        0        0     1100 2023-06-26 16:00:19.902449 longship-2023.6.27/longship_api_client/models/chargepoint_connector_dto_standard.py
+-rw-r--r--   0        0        0    17517 2023-06-26 16:00:19.902653 longship-2023.6.27/longship_api_client/models/chargepoint_dto.py
+-rw-r--r--   0        0        0      183 2023-06-26 16:00:19.902815 longship-2023.6.27/longship_api_client/models/chargepoint_dto_connectivity_status.py
+-rw-r--r--   0        0        0     2540 2023-06-26 16:00:19.903151 longship-2023.6.27/longship_api_client/models/chargepoint_evse_dto.py
+-rw-r--r--   0        0        0     3701 2023-06-26 16:00:19.903531 longship-2023.6.27/longship_api_client/models/chargepoint_put_dto.py
+-rw-r--r--   0        0        0     7169 2023-06-26 16:00:19.903846 longship-2023.6.27/longship_api_client/models/chargepoint_status_dto.py
+-rw-r--r--   0        0        0      189 2023-06-26 16:00:19.904003 longship-2023.6.27/longship_api_client/models/chargepoint_status_dto_connectivity_status.py
+-rw-r--r--   0        0        0     3743 2023-06-26 16:00:19.904221 longship-2023.6.27/longship_api_client/models/charging_meter_value_dto.py
+-rw-r--r--   0        0        0     1197 2023-06-26 16:00:19.904460 longship-2023.6.27/longship_api_client/models/charging_meter_value_dto_measurand.py
+-rw-r--r--   0        0        0      402 2023-06-26 16:00:19.904625 longship-2023.6.27/longship_api_client/models/charging_meter_value_dto_unit.py
+-rw-r--r--   0        0        0     2736 2023-06-26 16:00:19.904794 longship-2023.6.27/longship_api_client/models/charging_period_dto.py
+-rw-r--r--   0        0        0     6103 2023-06-26 16:00:19.905086 longship-2023.6.27/longship_api_client/models/charging_profile.py
+-rw-r--r--   0        0        0      219 2023-06-26 16:00:19.905228 longship-2023.6.27/longship_api_client/models/charging_profile_charging_profile_kind.py
+-rw-r--r--   0        0        0      264 2023-06-26 16:00:19.905404 longship-2023.6.27/longship_api_client/models/charging_profile_charging_profile_purpose.py
+-rw-r--r--   0        0        0      176 2023-06-26 16:00:19.905580 longship-2023.6.27/longship_api_client/models/charging_profile_recurrency_kind.py
+-rw-r--r--   0        0        0     4307 2023-06-26 16:00:19.905728 longship-2023.6.27/longship_api_client/models/charging_schedule.py
+-rw-r--r--   0        0        0      161 2023-06-26 16:00:19.905871 longship-2023.6.27/longship_api_client/models/charging_schedule_charging_rate_unit.py
+-rw-r--r--   0        0        0     2007 2023-06-26 16:00:19.906409 longship-2023.6.27/longship_api_client/models/charging_schedule_period.py
+-rw-r--r--   0        0        0     1180 2023-06-26 16:00:19.906577 longship-2023.6.27/longship_api_client/models/clear_cache_request.py
+-rw-r--r--   0        0        0     3421 2023-06-26 16:00:19.906723 longship-2023.6.27/longship_api_client/models/clear_charging_profile_request.py
+-rw-r--r--   0        0        0      276 2023-06-26 16:00:19.906886 longship-2023.6.27/longship_api_client/models/clear_charging_profile_request_charging_profile_purpose.py
+-rw-r--r--   0        0        0     5744 2023-06-26 16:00:19.907051 longship-2023.6.27/longship_api_client/models/connector_dto.py
+-rw-r--r--   0        0        0      165 2023-06-26 16:00:19.907200 longship-2023.6.27/longship_api_client/models/connector_dto_format.py
+-rw-r--r--   0        0        0      200 2023-06-26 16:00:19.907337 longship-2023.6.27/longship_api_client/models/connector_dto_power_type.py
+-rw-r--r--   0        0        0     1089 2023-06-26 16:00:19.907561 longship-2023.6.27/longship_api_client/models/connector_dto_standard.py
+-rw-r--r--   0        0        0     3465 2023-06-26 16:00:19.907704 longship-2023.6.27/longship_api_client/models/connector_operational_status_dto.py
+-rw-r--r--   0        0        0      411 2023-06-26 16:00:19.907830 longship-2023.6.27/longship_api_client/models/connector_operational_status_dto_operational_status.py
+-rw-r--r--   0        0        0     6202 2023-06-26 16:00:19.907958 longship-2023.6.27/longship_api_client/models/cs_charging_profiles.py
+-rw-r--r--   0        0        0      222 2023-06-26 16:00:19.908086 longship-2023.6.27/longship_api_client/models/cs_charging_profiles_charging_profile_kind.py
+-rw-r--r--   0        0        0      267 2023-06-26 16:00:19.908346 longship-2023.6.27/longship_api_client/models/cs_charging_profiles_charging_profile_purpose.py
+-rw-r--r--   0        0        0      179 2023-06-26 16:00:19.908522 longship-2023.6.27/longship_api_client/models/cs_charging_profiles_recurrency_kind.py
+-rw-r--r--   0        0        0     1996 2023-06-26 16:00:19.908662 longship-2023.6.27/longship_api_client/models/data_transfer_request.py
+-rw-r--r--   0        0        0     1726 2023-06-26 16:00:19.908786 longship-2023.6.27/longship_api_client/models/display_text_dto.py
+-rw-r--r--   0        0        0     3730 2023-06-26 16:00:19.908920 longship-2023.6.27/longship_api_client/models/energy_mix_dto.py
+-rw-r--r--   0        0        0     2229 2023-06-26 16:00:19.909045 longship-2023.6.27/longship_api_client/models/energy_source_dto.py
+-rw-r--r--   0        0        0      316 2023-06-26 16:00:19.909172 longship-2023.6.27/longship_api_client/models/energy_source_dto_source.py
+-rw-r--r--   0        0        0     2180 2023-06-26 16:00:19.909461 longship-2023.6.27/longship_api_client/models/entity_tag_header_value.py
+-rw-r--r--   0        0        0     2340 2023-06-26 16:00:19.909584 longship-2023.6.27/longship_api_client/models/environmental_impact_dto.py
+-rw-r--r--   0        0        0      209 2023-06-26 16:00:19.909709 longship-2023.6.27/longship_api_client/models/environmental_impact_dto_category.py
+-rw-r--r--   0        0        0     2592 2023-06-26 16:00:19.909843 longship-2023.6.27/longship_api_client/models/exceptional_period_dto.py
+-rw-r--r--   0        0        0     4622 2023-06-26 16:00:19.909979 longship-2023.6.27/longship_api_client/models/file_content_result.py
+-rw-r--r--   0        0        0     1781 2023-06-26 16:00:19.910112 longship-2023.6.27/longship_api_client/models/geo_location_dto.py
+-rw-r--r--   0        0        0      190 2023-06-26 16:00:19.910233 longship-2023.6.27/longship_api_client/models/get_all_cdrs_order_by.py
+-rw-r--r--   0        0        0      224 2023-06-26 16:00:19.910360 longship-2023.6.27/longship_api_client/models/get_all_chargepoints_order_by.py
+-rw-r--r--   0        0        0      191 2023-06-26 16:00:19.910499 longship-2023.6.27/longship_api_client/models/get_all_locations_order_by.py
+-rw-r--r--   0        0        0      203 2023-06-26 16:00:19.910619 longship-2023.6.27/longship_api_client/models/get_all_reimbursementcdrs_order_by.py
+-rw-r--r--   0        0        0      164 2023-06-26 16:00:19.910737 longship-2023.6.27/longship_api_client/models/get_all_sessions_order_by.py
+-rw-r--r--   0        0        0      203 2023-06-26 16:00:19.910857 longship-2023.6.27/longship_api_client/models/get_all_tariffs_order_by.py
+-rw-r--r--   0        0        0      144 2023-06-26 16:00:19.910971 longship-2023.6.27/longship_api_client/models/get_all_webhooks_order_by.py
+-rw-r--r--   0        0        0     2844 2023-06-26 16:00:19.911220 longship-2023.6.27/longship_api_client/models/get_composite_schedule_request.py
+-rw-r--r--   0        0        0      172 2023-06-26 16:00:19.911415 longship-2023.6.27/longship_api_client/models/get_composite_schedule_request_charging_rate_unit.py
+-rw-r--r--   0        0        0     1621 2023-06-26 16:00:19.911532 longship-2023.6.27/longship_api_client/models/get_configuration_request.py
+-rw-r--r--   0        0        0     3343 2023-06-26 16:00:19.911661 longship-2023.6.27/longship_api_client/models/get_diagnostics_request.py
+-rw-r--r--   0        0        0     1231 2023-06-26 16:00:19.911780 longship-2023.6.27/longship_api_client/models/get_local_list_version_request.py
+-rw-r--r--   0        0        0     4898 2023-06-26 16:00:19.911903 longship-2023.6.27/longship_api_client/models/hours_dto.py
+-rw-r--r--   0        0        0     2581 2023-06-26 16:00:19.912026 longship-2023.6.27/longship_api_client/models/id_tag_info.py
+-rw-r--r--   0        0        0      252 2023-06-26 16:00:19.912140 longship-2023.6.27/longship_api_client/models/id_tag_info_status.py
+-rw-r--r--   0        0        0     3089 2023-06-26 16:00:19.912263 longship-2023.6.27/longship_api_client/models/image_dto.py
+-rw-r--r--   0        0        0      287 2023-06-26 16:00:19.912517 longship-2023.6.27/longship_api_client/models/image_dto_category.py
+-rw-r--r--   0        0        0     8559 2023-06-26 16:00:19.912653 longship-2023.6.27/longship_api_client/models/interchange_format_cdr.py
+-rw-r--r--   0        0        0     5283 2023-06-26 16:00:19.912789 longship-2023.6.27/longship_api_client/models/local_token_group_get_dto.py
+-rw-r--r--   0        0        0     3911 2023-06-26 16:00:19.912916 longship-2023.6.27/longship_api_client/models/local_token_group_post_dto.py
+-rw-r--r--   0        0        0     3899 2023-06-26 16:00:19.913044 longship-2023.6.27/longship_api_client/models/local_token_group_put_dto.py
+-rw-r--r--   0        0        0     2722 2023-06-26 16:00:19.913170 longship-2023.6.27/longship_api_client/models/local_token_group_token_get_dto.py
+-rw-r--r--   0        0        0     2310 2023-06-26 16:00:19.913336 longship-2023.6.27/longship_api_client/models/local_token_group_token_post_dto.py
+-rw-r--r--   0        0        0     2305 2023-06-26 16:00:19.913457 longship-2023.6.27/longship_api_client/models/local_token_group_token_put_dto.py
+-rw-r--r--   0        0        0     1619 2023-06-26 16:00:19.913572 longship-2023.6.27/longship_api_client/models/location_charge_point_dto.py
+-rw-r--r--   0        0        0    17497 2023-06-26 16:00:19.913731 longship-2023.6.27/longship_api_client/models/location_dto.py
+-rw-r--r--   0        0        0      690 2023-06-26 16:00:19.913864 longship-2023.6.27/longship_api_client/models/location_dto_facilities_item.py
+-rw-r--r--   0        0        0      341 2023-06-26 16:00:19.913988 longship-2023.6.27/longship_api_client/models/location_dto_parking_type.py
+-rw-r--r--   0        0        0    11569 2023-06-26 16:00:19.914142 longship-2023.6.27/longship_api_client/models/location_evse_dto.py
+-rw-r--r--   0        0        0      698 2023-06-26 16:00:19.914413 longship-2023.6.27/longship_api_client/models/location_evse_dto_capabilities_item.py
+-rw-r--r--   0        0        0      277 2023-06-26 16:00:19.914536 longship-2023.6.27/longship_api_client/models/location_evse_dto_parking_restrictions_item.py
+-rw-r--r--   0        0        0      364 2023-06-26 16:00:19.914656 longship-2023.6.27/longship_api_client/models/location_evse_dto_status.py
+-rw-r--r--   0        0        0    17038 2023-06-26 16:00:19.914818 longship-2023.6.27/longship_api_client/models/location_post_dto.py
+-rw-r--r--   0        0        0      694 2023-06-26 16:00:19.914939 longship-2023.6.27/longship_api_client/models/location_post_dto_facilities_item.py
+-rw-r--r--   0        0        0      345 2023-06-26 16:00:19.915048 longship-2023.6.27/longship_api_client/models/location_post_dto_parking_type.py
+-rw-r--r--   0        0        0    17258 2023-06-26 16:00:19.915198 longship-2023.6.27/longship_api_client/models/location_put_dto.py
+-rw-r--r--   0        0        0      693 2023-06-26 16:00:19.915320 longship-2023.6.27/longship_api_client/models/location_put_dto_facilities_item.py
+-rw-r--r--   0        0        0      344 2023-06-26 16:00:19.915650 longship-2023.6.27/longship_api_client/models/location_put_dto_parking_type.py
+-rw-r--r--   0        0        0     1854 2023-06-26 16:00:19.915768 longship-2023.6.27/longship_api_client/models/location_tariff_distribution_dto.py
+-rw-r--r--   0        0        0     2379 2023-06-26 16:00:19.915889 longship-2023.6.27/longship_api_client/models/longship_error.py
+-rw-r--r--   0        0        0     1920 2023-06-26 16:00:19.916000 longship-2023.6.27/longship_api_client/models/longship_error_detail.py
+-rw-r--r--   0        0        0     5923 2023-06-26 16:00:19.916126 longship-2023.6.27/longship_api_client/models/message_log_dto.py
+-rw-r--r--   0        0        0      219 2023-06-26 16:00:19.916232 longship-2023.6.27/longship_api_client/models/message_log_dto_direction.py
+-rw-r--r--   0        0        0     1335 2023-06-26 16:00:19.916490 longship-2023.6.27/longship_api_client/models/message_log_dto_ocpp_message_type.py
+-rw-r--r--   0        0        0      227 2023-06-26 16:00:19.916750 longship-2023.6.27/longship_api_client/models/message_log_dto_wamp_message_type.py
+-rw-r--r--   0        0        0     2135 2023-06-26 16:00:19.916889 longship-2023.6.27/longship_api_client/models/organization_unit_financial_details_dto.py
+-rw-r--r--   0        0        0     8654 2023-06-26 16:00:19.917030 longship-2023.6.27/longship_api_client/models/organization_unit_get_dto.py
+-rw-r--r--   0        0        0     7882 2023-06-26 16:00:19.917159 longship-2023.6.27/longship_api_client/models/organization_unit_post_dto.py
+-rw-r--r--   0        0        0     7631 2023-06-26 16:00:19.917289 longship-2023.6.27/longship_api_client/models/organization_unit_put_dto.py
+-rw-r--r--   0        0        0     4792 2023-06-26 16:00:19.917419 longship-2023.6.27/longship_api_client/models/price_info_dto.py
+-rw-r--r--   0        0        0     3235 2023-06-26 16:00:19.917544 longship-2023.6.27/longship_api_client/models/private_emp_tariff_dto.py
+-rw-r--r--   0        0        0      161 2023-06-26 16:00:19.917650 longship-2023.6.27/longship_api_client/models/private_emp_tariff_dto_power_type.py
+-rw-r--r--   0        0        0     2984 2023-06-26 16:00:19.917824 longship-2023.6.27/longship_api_client/models/publish_token_type_dto.py
+-rw-r--r--   0        0        0      224 2023-06-26 16:00:19.917985 longship-2023.6.27/longship_api_client/models/publish_token_type_dto_type.py
+-rw-r--r--   0        0        0     2097 2023-06-26 16:00:19.918105 longship-2023.6.27/longship_api_client/models/regular_hours_dto.py
+-rw-r--r--   0        0        0    11178 2023-06-26 16:00:19.918236 longship-2023.6.27/longship_api_client/models/reimburse_info_dto.py
+-rw-r--r--   0        0        0      205 2023-06-26 16:00:19.918347 longship-2023.6.27/longship_api_client/models/reimburse_info_dto_type.py
+-rw-r--r--   0        0        0     3914 2023-06-26 16:00:19.918467 longship-2023.6.27/longship_api_client/models/reimburse_started_by_info_dto.py
+-rw-r--r--   0        0        0      674 2023-06-26 16:00:19.918586 longship-2023.6.27/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py
+-rw-r--r--   0        0        0     5626 2023-06-26 16:00:19.918712 longship-2023.6.27/longship_api_client/models/reimburse_started_by_token_dto.py
+-rw-r--r--   0        0        0      227 2023-06-26 16:00:19.918949 longship-2023.6.27/longship_api_client/models/reimburse_started_by_token_dto_auth_method.py
+-rw-r--r--   0        0        0      236 2023-06-26 16:00:19.919062 longship-2023.6.27/longship_api_client/models/reimburse_started_by_token_dto_token_type.py
+-rw-r--r--   0        0        0     2926 2023-06-26 16:00:19.919183 longship-2023.6.27/longship_api_client/models/reimbursement_bank_details_dto.py
+-rw-r--r--   0        0        0    21317 2023-06-26 16:00:19.919340 longship-2023.6.27/longship_api_client/models/reimbursement_cdr_dto.py
+-rw-r--r--   0        0        0     1867 2023-06-26 16:00:19.919476 longship-2023.6.27/longship_api_client/models/reimbursement_cdr_geo_location_dto.py
+-rw-r--r--   0        0        0     7009 2023-06-26 16:00:19.919607 longship-2023.6.27/longship_api_client/models/reimbursement_cdr_location_dto.py
+-rw-r--r--   0        0        0      215 2023-06-26 16:00:19.919855 longship-2023.6.27/longship_api_client/models/reimbursement_cdr_location_dto_power_type.py
+-rw-r--r--   0        0        0     2330 2023-06-26 16:00:19.919972 longship-2023.6.27/longship_api_client/models/reimbursement_customer_share_dto.py
+-rw-r--r--   0        0        0     1813 2023-06-26 16:00:19.920092 longship-2023.6.27/longship_api_client/models/reimbursement_price_dto.py
+-rw-r--r--   0        0        0     4578 2023-06-26 16:00:19.920212 longship-2023.6.27/longship_api_client/models/reimbursement_tariff_dto.py
+-rw-r--r--   0        0        0      209 2023-06-26 16:00:19.920328 longship-2023.6.27/longship_api_client/models/reimbursement_tariff_dto_status.py
+-rw-r--r--   0        0        0     2720 2023-06-26 16:00:19.920443 longship-2023.6.27/longship_api_client/models/remote_start_transaction_request.py
+-rw-r--r--   0        0        0     1543 2023-06-26 16:00:19.920556 longship-2023.6.27/longship_api_client/models/remote_stop_transaction_request.py
+-rw-r--r--   0        0        0     2538 2023-06-26 16:00:19.920673 longship-2023.6.27/longship_api_client/models/reserve_now_request.py
+-rw-r--r--   0        0        0     1524 2023-06-26 16:00:19.920881 longship-2023.6.27/longship_api_client/models/reset_request.py
+-rw-r--r--   0        0        0      157 2023-06-26 16:00:19.920991 longship-2023.6.27/longship_api_client/models/reset_request_type.py
+-rw-r--r--   0        0        0     3346 2023-06-26 16:00:19.921117 longship-2023.6.27/longship_api_client/models/send_local_list_request.py
+-rw-r--r--   0        0        0      187 2023-06-26 16:00:19.921237 longship-2023.6.27/longship_api_client/models/send_local_list_request_update_type.py
+-rw-r--r--   0        0        0    16519 2023-06-26 16:00:19.921384 longship-2023.6.27/longship_api_client/models/session_dto.py
+-rw-r--r--   0        0        0      251 2023-06-26 16:00:19.921491 longship-2023.6.27/longship_api_client/models/session_dto_status.py
+-rw-r--r--   0        0        0     1819 2023-06-26 16:00:19.921601 longship-2023.6.27/longship_api_client/models/session_geo_location_dto.py
+-rw-r--r--   0        0        0     6802 2023-06-26 16:00:19.921722 longship-2023.6.27/longship_api_client/models/session_location_dto.py
+-rw-r--r--   0        0        0      206 2023-06-26 16:00:19.921830 longship-2023.6.27/longship_api_client/models/session_location_dto_power_type.py
+-rw-r--r--   0        0        0     2048 2023-06-26 16:00:19.921941 longship-2023.6.27/longship_api_client/models/set_charging_profile_request.py
+-rw-r--r--   0        0        0     5085 2023-06-26 16:00:19.922062 longship-2023.6.27/longship_api_client/models/started_by_info_dto.py
+-rw-r--r--   0        0        0      665 2023-06-26 16:00:19.922175 longship-2023.6.27/longship_api_client/models/started_by_info_dto_authorization_state.py
+-rw-r--r--   0        0        0      182 2023-06-26 16:00:19.922285 longship-2023.6.27/longship_api_client/models/started_by_info_dto_roaming_platform_type.py
+-rw-r--r--   0        0        0     5408 2023-06-26 16:00:19.922417 longship-2023.6.27/longship_api_client/models/started_by_token_dto.py
+-rw-r--r--   0        0        0      218 2023-06-26 16:00:19.922533 longship-2023.6.27/longship_api_client/models/started_by_token_dto_auth_method.py
+-rw-r--r--   0        0        0      227 2023-06-26 16:00:19.923113 longship-2023.6.27/longship_api_client/models/started_by_token_dto_token_type.py
+-rw-r--r--   0        0        0     3296 2023-06-26 16:00:19.923404 longship-2023.6.27/longship_api_client/models/status_schedule_dto.py
+-rw-r--r--   0        0        0      366 2023-06-26 16:00:19.923560 longship-2023.6.27/longship_api_client/models/status_schedule_dto_status.py
+-rw-r--r--   0        0        0     2475 2023-06-26 16:00:19.923890 longship-2023.6.27/longship_api_client/models/string_segment.py
+-rw-r--r--   0        0        0     2787 2023-06-26 16:00:19.924076 longship-2023.6.27/longship_api_client/models/tariff_assertion_dto.py
+-rw-r--r--   0        0        0      283 2023-06-26 16:00:19.924212 longship-2023.6.27/longship_api_client/models/tariff_assertion_dto_tariff_type.py
+-rw-r--r--   0        0        0     6447 2023-06-26 16:00:19.924335 longship-2023.6.27/longship_api_client/models/tariff_distribution_get_dto.py
+-rw-r--r--   0        0        0     3617 2023-06-26 16:00:19.924485 longship-2023.6.27/longship_api_client/models/tariff_distribution_history_dto.py
+-rw-r--r--   0        0        0     3409 2023-06-26 16:00:19.924751 longship-2023.6.27/longship_api_client/models/tariff_distribution_post_dto.py
+-rw-r--r--   0        0        0     3404 2023-06-26 16:00:19.925022 longship-2023.6.27/longship_api_client/models/tariff_distribution_put_dto.py
+-rw-r--r--   0        0        0    12525 2023-06-26 16:00:19.925189 longship-2023.6.27/longship_api_client/models/tariff_dto.py
+-rw-r--r--   0        0        0      186 2023-06-26 16:00:19.925352 longship-2023.6.27/longship_api_client/models/tariff_dto_tariff_type.py
+-rw-r--r--   0        0        0      241 2023-06-26 16:00:19.925490 longship-2023.6.27/longship_api_client/models/tariff_dto_usage_type.py
+-rw-r--r--   0        0        0     5977 2023-06-26 16:00:19.925640 longship-2023.6.27/longship_api_client/models/tariff_info_dto.py
+-rw-r--r--   0        0        0     6945 2023-06-26 16:00:19.925780 longship-2023.6.27/longship_api_client/models/tariff_post_dto.py
+-rw-r--r--   0        0        0      245 2023-06-26 16:00:19.926087 longship-2023.6.27/longship_api_client/models/tariff_post_dto_usage_type.py
+-rw-r--r--   0        0        0     7511 2023-06-26 16:00:19.926318 longship-2023.6.27/longship_api_client/models/tariff_price_dto.py
+-rw-r--r--   0        0        0      209 2023-06-26 16:00:19.926463 longship-2023.6.27/longship_api_client/models/tariff_price_dto_approval_status.py
+-rw-r--r--   0        0        0     6188 2023-06-26 16:00:19.926616 longship-2023.6.27/longship_api_client/models/tariff_put_dto.py
+-rw-r--r--   0        0        0     2235 2023-06-26 16:00:19.926826 longship-2023.6.27/longship_api_client/models/trigger_message_request.py
+-rw-r--r--   0        0        0      420 2023-06-26 16:00:19.927163 longship-2023.6.27/longship_api_client/models/trigger_message_request_requested_message.py
+-rw-r--r--   0        0        0     1490 2023-06-26 16:00:19.928533 longship-2023.6.27/longship_api_client/models/unlock_connector_request.py
+-rw-r--r--   0        0        0     2409 2023-06-26 16:00:19.928994 longship-2023.6.27/longship_api_client/models/update_firmware_request.py
+-rw-r--r--   0        0        0     5393 2023-06-26 16:00:19.929113 longship-2023.6.27/longship_api_client/models/webhook_get_dto.py
+-rw-r--r--   0        0        0      398 2023-06-26 16:00:19.929555 longship-2023.6.27/longship_api_client/models/webhook_get_dto_event_types_item.py
+-rw-r--r--   0        0        0     1703 2023-06-26 16:00:19.929899 longship-2023.6.27/longship_api_client/models/webhook_header_dto.py
+-rw-r--r--   0        0        0     4020 2023-06-26 16:00:19.930015 longship-2023.6.27/longship_api_client/models/webhook_post_dto.py
+-rw-r--r--   0        0        0      399 2023-06-26 16:00:19.930121 longship-2023.6.27/longship_api_client/models/webhook_post_dto_event_types_item.py
+-rw-r--r--   0        0        0     4009 2023-06-26 16:00:19.930238 longship-2023.6.27/longship_api_client/models/webhook_put_dto.py
+-rw-r--r--   0        0        0      398 2023-06-26 16:00:19.930345 longship-2023.6.27/longship_api_client/models/webhook_put_dto_event_types_item.py
+-rw-r--r--   0        0        0     4096 2023-06-26 16:00:19.930595 longship-2023.6.27/longship_api_client/models/webhook_summary_get_dto.py
+-rw-r--r--   0        0        0      405 2023-06-26 16:00:19.930722 longship-2023.6.27/longship_api_client/models/webhook_summary_get_dto_event_types_item.py
+-rw-r--r--   0        0        0       25 2023-06-26 16:00:19.930817 longship-2023.6.27/longship_api_client/py.typed
+-rw-r--r--   0        0        0      993 2023-06-26 16:00:19.930917 longship-2023.6.27/longship_api_client/types.py
+-rw-r--r--   0        0        0      818 2023-06-26 21:10:23.752739 longship-2023.6.27/pyproject.toml
+-rw-r--r--   0        0        0     5264 1970-01-01 00:00:00.000000 longship-2023.6.27/PKG-INFO
```

### Comparing `longship-2023.6.26/LICENSE` & `longship-2023.6.27/LICENSE`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/README.md` & `longship-2023.6.27/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # longship-api-client
 
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/longship.svg)](https://pypi.python.org/pypi/longship/)
 [![Downloads](https://static.pepy.tech/personalized-badge/longship?period=total&units=international_system&left_color=blue&right_color=green&left_text=Downloads)](https://pepy.tech/project/longship)
 
 
-A client library for accessing Longship API
+A client library for accessing [Longship](https://www.longship.io/) API
 
 ## Usage
 First, create a client:
 
 ```python
 from longship_api_client import Client
```

### Comparing `longship-2023.6.26/longship/client.py` & `longship-2023.6.27/longship/client.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship/types.py` & `longship-2023.6.27/longship/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Union
+from typing import Optional, Union
 
 import attr
 
 from longship_api_client.models.chargepoint_dto_connectivity_status import ChargepointDtoConnectivityStatus
 from longship_api_client.models.connector_operational_status_dto_operational_status import (
     ConnectorOperationalStatusDtoOperationalStatus,
 )
@@ -35,17 +35,18 @@
 
 
 @attr.s(auto_attribs=True)
 class OperationalStatusChangedData:
     status: ConnectorOperationalStatusDtoOperationalStatus
     errorcode: str
     connectornumber: int
-    locationid: str
-    evseid: str
     statussource: str
+    locationid: Optional[str] = attr.ib(default=None)
+    evseid: Optional[str] = attr.ib(default=None)
+    vendorid: Optional[str] = attr.ib(default=None)
 
 
 @attr.s(auto_attribs=True)
 class ConnectivityStatusChangedData:
     # TODO: Longship uses uppercase for the status, but the webhook response uses CamelCase
     status: ChargepointDtoConnectivityStatus
```

### Comparing `longship-2023.6.26/longship_api_client/api/cdrs/cdr_get.py` & `longship-2023.6.27/longship_api_client/api/cdrs/cdr_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/cdrs/get_all_cdrs.py` & `longship-2023.6.27/longship_api_client/api/cdrs/get_all_cdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/cdrs/get_all_interchangeformat.py` & `longship-2023.6.27/longship_api_client/api/cdrs/get_all_interchangeformat.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/cdrs/get_file_full_download_cdrs.py` & `longship-2023.6.27/longship_api_client/api/cdrs/get_file_full_download_cdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py` & `longship-2023.6.27/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/chargepoint_status/chargepoint_status_get.py` & `longship-2023.6.27/longship_api_client/api/chargepoint_status/chargepoint_status_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py` & `longship-2023.6.27/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/chargepoints/chargepoint_get.py` & `longship-2023.6.27/longship_api_client/api/chargepoints/chargepoint_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/chargepoints/chargepoint_put.py` & `longship-2023.6.27/longship_api_client/api/chargepoints/chargepoint_put.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/chargepoints/get_all_chargepointmessages.py` & `longship-2023.6.27/longship_api_client/api/chargepoints/get_all_chargepointmessages.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/chargepoints/get_all_chargepoints.py` & `longship-2023.6.27/longship_api_client/api/chargepoints/get_all_chargepoints.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_cancel_reservation_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_cancel_reservation_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_change_availability_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_change_availability_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_change_configuration_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_change_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_clear_cache_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_clear_cache_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_clear_charging_profile_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_clear_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_data_transfer_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_data_transfer_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_get_composite_schedule_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_get_composite_schedule_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_get_configuration_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_get_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_get_diagnostics_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_get_diagnostics_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_get_local_list_version_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_get_local_list_version_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_remote_start_transaction_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_remote_start_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_remote_stop_transaction_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_remote_stop_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_reserve_now_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_reserve_now_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_reset_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_reset_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_send_local_list_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_send_local_list_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_set_charging_profile_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_set_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_trigger_message_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_trigger_message_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_unlock_connector_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_unlock_connector_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/commands/send_update_firmware_request.py` & `longship-2023.6.27/longship_api_client/api/commands/send_update_firmware_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/localtokengroups/get_all_localtokengroups.py` & `longship-2023.6.27/longship_api_client/api/localtokengroups/get_all_localtokengroups.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/localtokengroups/local_token_group_delete.py` & `longship-2023.6.27/longship_api_client/api/localtokengroups/local_token_group_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/localtokengroups/local_token_group_post.py` & `longship-2023.6.27/longship_api_client/api/localtokengroups/local_token_group_post.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/localtokengroups/local_token_group_put.py` & `longship-2023.6.27/longship_api_client/api/localtokengroups/local_token_group_put.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/localtokengroups/localtokengroup_get.py` & `longship-2023.6.27/longship_api_client/api/localtokengroups/localtokengroup_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/locations/get_all_locations.py` & `longship-2023.6.27/longship_api_client/api/locations/get_all_locations.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/locations/location_get.py` & `longship-2023.6.27/longship_api_client/api/locations/location_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/locations/location_post.py` & `longship-2023.6.27/longship_api_client/api/locations/location_post.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/locations/location_put.py` & `longship-2023.6.27/longship_api_client/api/locations/location_put.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py` & `longship-2023.6.27/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py` & `longship-2023.6.27/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py` & `longship-2023.6.27/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/organizationunits/get_all_organizationunits.py` & `longship-2023.6.27/longship_api_client/api/organizationunits/get_all_organizationunits.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/organizationunits/organization_unit_get.py` & `longship-2023.6.27/longship_api_client/api/organizationunits/organization_unit_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/organizationunits/organization_unit_post.py` & `longship-2023.6.27/longship_api_client/api/organizationunits/organization_unit_post.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/organizationunits/organization_unit_put.py` & `longship-2023.6.27/longship_api_client/api/organizationunits/organization_unit_put.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py` & `longship-2023.6.27/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py` & `longship-2023.6.27/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/reimbursement/reimbursement_cdr_get.py` & `longship-2023.6.27/longship_api_client/api/reimbursement/reimbursement_cdr_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/sessions/get_all_sessions.py` & `longship-2023.6.27/longship_api_client/api/sessions/get_all_sessions.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/sessions/session_get.py` & `longship-2023.6.27/longship_api_client/api/sessions/session_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py` & `longship-2023.6.27/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/tariffdistributions/tariffdistribution_get.py` & `longship-2023.6.27/longship_api_client/api/tariffdistributions/tariffdistribution_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/tariffdistributions/tariffdistribution_post.py` & `longship-2023.6.27/longship_api_client/api/tariffdistributions/tariffdistribution_post.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/tariffdistributions/tariffdistribution_put.py` & `longship-2023.6.27/longship_api_client/api/tariffdistributions/tariffdistribution_put.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/tariffs/get_all_tariffs.py` & `longship-2023.6.27/longship_api_client/api/tariffs/get_all_tariffs.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/tariffs/tariff_get.py` & `longship-2023.6.27/longship_api_client/api/tariffs/tariff_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/tariffs/tariff_post.py` & `longship-2023.6.27/longship_api_client/api/tariffs/tariff_post.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/tariffs/tariff_put.py` & `longship-2023.6.27/longship_api_client/api/tariffs/tariff_put.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/webhooks/get_all_webhooks.py` & `longship-2023.6.27/longship_api_client/api/webhooks/get_all_webhooks.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/webhooks/webhook_delete.py` & `longship-2023.6.27/longship_api_client/api/webhooks/webhook_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/webhooks/webhook_get.py` & `longship-2023.6.27/longship_api_client/api/webhooks/webhook_get.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/webhooks/webhook_post.py` & `longship-2023.6.27/longship_api_client/api/webhooks/webhook_post.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/api/webhooks/webhook_put.py` & `longship-2023.6.27/longship_api_client/api/webhooks/webhook_put.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/client.py` & `longship-2023.6.27/longship_api_client/client.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/__init__.py` & `longship-2023.6.27/longship_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/additional_geo_location_dto.py` & `longship-2023.6.27/longship_api_client/models/additional_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/authorization_data.py` & `longship-2023.6.27/longship_api_client/models/authorization_data.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/business_details_dto.py` & `longship-2023.6.27/longship_api_client/models/business_details_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/cancel_reservation_request.py` & `longship-2023.6.27/longship_api_client/models/cancel_reservation_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/cdr_dto.py` & `longship-2023.6.27/longship_api_client/models/cdr_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/cdr_geo_location_dto.py` & `longship-2023.6.27/longship_api_client/models/cdr_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/cdr_location_dto.py` & `longship-2023.6.27/longship_api_client/models/cdr_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/cdr_started_by_info_dto.py` & `longship-2023.6.27/longship_api_client/models/cdr_started_by_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py` & `longship-2023.6.27/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/cdr_started_by_token_dto.py` & `longship-2023.6.27/longship_api_client/models/cdr_started_by_token_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/change_availability_request.py` & `longship-2023.6.27/longship_api_client/models/change_availability_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/change_configuration_request.py` & `longship-2023.6.27/longship_api_client/models/change_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/chargepoint_connector_dto.py` & `longship-2023.6.27/longship_api_client/models/chargepoint_connector_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/chargepoint_connector_dto_standard.py` & `longship-2023.6.27/longship_api_client/models/chargepoint_connector_dto_standard.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/chargepoint_dto.py` & `longship-2023.6.27/longship_api_client/models/chargepoint_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/chargepoint_evse_dto.py` & `longship-2023.6.27/longship_api_client/models/chargepoint_evse_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/chargepoint_put_dto.py` & `longship-2023.6.27/longship_api_client/models/chargepoint_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/chargepoint_status_dto.py` & `longship-2023.6.27/longship_api_client/models/chargepoint_status_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/charging_meter_value_dto.py` & `longship-2023.6.27/longship_api_client/models/charging_meter_value_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/charging_meter_value_dto_measurand.py` & `longship-2023.6.27/longship_api_client/models/charging_meter_value_dto_measurand.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/charging_period_dto.py` & `longship-2023.6.27/longship_api_client/models/charging_period_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/charging_profile.py` & `longship-2023.6.27/longship_api_client/models/charging_profile.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/charging_schedule.py` & `longship-2023.6.27/longship_api_client/models/charging_schedule.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/charging_schedule_period.py` & `longship-2023.6.27/longship_api_client/models/charging_schedule_period.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/clear_cache_request.py` & `longship-2023.6.27/longship_api_client/models/clear_cache_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/clear_charging_profile_request.py` & `longship-2023.6.27/longship_api_client/models/clear_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/connector_dto.py` & `longship-2023.6.27/longship_api_client/models/connector_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/connector_dto_standard.py` & `longship-2023.6.27/longship_api_client/models/connector_dto_standard.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/connector_operational_status_dto.py` & `longship-2023.6.27/longship_api_client/models/connector_operational_status_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/cs_charging_profiles.py` & `longship-2023.6.27/longship_api_client/models/cs_charging_profiles.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/data_transfer_request.py` & `longship-2023.6.27/longship_api_client/models/data_transfer_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/display_text_dto.py` & `longship-2023.6.27/longship_api_client/models/display_text_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/energy_mix_dto.py` & `longship-2023.6.27/longship_api_client/models/energy_mix_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/energy_source_dto.py` & `longship-2023.6.27/longship_api_client/models/energy_source_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/entity_tag_header_value.py` & `longship-2023.6.27/longship_api_client/models/entity_tag_header_value.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/environmental_impact_dto.py` & `longship-2023.6.27/longship_api_client/models/environmental_impact_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/exceptional_period_dto.py` & `longship-2023.6.27/longship_api_client/models/exceptional_period_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/file_content_result.py` & `longship-2023.6.27/longship_api_client/models/file_content_result.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/geo_location_dto.py` & `longship-2023.6.27/longship_api_client/models/geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/get_composite_schedule_request.py` & `longship-2023.6.27/longship_api_client/models/get_composite_schedule_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/get_configuration_request.py` & `longship-2023.6.27/longship_api_client/models/get_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/get_diagnostics_request.py` & `longship-2023.6.27/longship_api_client/models/get_diagnostics_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/get_local_list_version_request.py` & `longship-2023.6.27/longship_api_client/models/get_local_list_version_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/hours_dto.py` & `longship-2023.6.27/longship_api_client/models/hours_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/id_tag_info.py` & `longship-2023.6.27/longship_api_client/models/id_tag_info.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/image_dto.py` & `longship-2023.6.27/longship_api_client/models/image_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/interchange_format_cdr.py` & `longship-2023.6.27/longship_api_client/models/interchange_format_cdr.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/local_token_group_get_dto.py` & `longship-2023.6.27/longship_api_client/models/local_token_group_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/local_token_group_post_dto.py` & `longship-2023.6.27/longship_api_client/models/local_token_group_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/local_token_group_put_dto.py` & `longship-2023.6.27/longship_api_client/models/local_token_group_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/local_token_group_token_get_dto.py` & `longship-2023.6.27/longship_api_client/models/local_token_group_token_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/local_token_group_token_post_dto.py` & `longship-2023.6.27/longship_api_client/models/local_token_group_token_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/local_token_group_token_put_dto.py` & `longship-2023.6.27/longship_api_client/models/local_token_group_token_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/location_charge_point_dto.py` & `longship-2023.6.27/longship_api_client/models/location_charge_point_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/location_dto.py` & `longship-2023.6.27/longship_api_client/models/location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/location_dto_facilities_item.py` & `longship-2023.6.27/longship_api_client/models/location_dto_facilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/location_evse_dto.py` & `longship-2023.6.27/longship_api_client/models/location_evse_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/location_evse_dto_capabilities_item.py` & `longship-2023.6.27/longship_api_client/models/location_evse_dto_capabilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/location_post_dto.py` & `longship-2023.6.27/longship_api_client/models/location_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/location_post_dto_facilities_item.py` & `longship-2023.6.27/longship_api_client/models/location_post_dto_facilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/location_put_dto.py` & `longship-2023.6.27/longship_api_client/models/location_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/location_put_dto_facilities_item.py` & `longship-2023.6.27/longship_api_client/models/location_put_dto_facilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/location_tariff_distribution_dto.py` & `longship-2023.6.27/longship_api_client/models/location_tariff_distribution_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/longship_error.py` & `longship-2023.6.27/longship_api_client/models/longship_error.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/longship_error_detail.py` & `longship-2023.6.27/longship_api_client/models/longship_error_detail.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/message_log_dto.py` & `longship-2023.6.27/longship_api_client/models/message_log_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/message_log_dto_ocpp_message_type.py` & `longship-2023.6.27/longship_api_client/models/message_log_dto_ocpp_message_type.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/organization_unit_financial_details_dto.py` & `longship-2023.6.27/longship_api_client/models/organization_unit_financial_details_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/organization_unit_get_dto.py` & `longship-2023.6.27/longship_api_client/models/organization_unit_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/organization_unit_post_dto.py` & `longship-2023.6.27/longship_api_client/models/organization_unit_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/organization_unit_put_dto.py` & `longship-2023.6.27/longship_api_client/models/organization_unit_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/price_info_dto.py` & `longship-2023.6.27/longship_api_client/models/price_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/private_emp_tariff_dto.py` & `longship-2023.6.27/longship_api_client/models/private_emp_tariff_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/publish_token_type_dto.py` & `longship-2023.6.27/longship_api_client/models/publish_token_type_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/regular_hours_dto.py` & `longship-2023.6.27/longship_api_client/models/regular_hours_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimburse_info_dto.py` & `longship-2023.6.27/longship_api_client/models/reimburse_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimburse_started_by_info_dto.py` & `longship-2023.6.27/longship_api_client/models/reimburse_started_by_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py` & `longship-2023.6.27/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimburse_started_by_token_dto.py` & `longship-2023.6.27/longship_api_client/models/reimburse_started_by_token_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimbursement_bank_details_dto.py` & `longship-2023.6.27/longship_api_client/models/reimbursement_bank_details_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimbursement_cdr_dto.py` & `longship-2023.6.27/longship_api_client/models/reimbursement_cdr_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimbursement_cdr_geo_location_dto.py` & `longship-2023.6.27/longship_api_client/models/reimbursement_cdr_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimbursement_cdr_location_dto.py` & `longship-2023.6.27/longship_api_client/models/reimbursement_cdr_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimbursement_customer_share_dto.py` & `longship-2023.6.27/longship_api_client/models/reimbursement_customer_share_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimbursement_price_dto.py` & `longship-2023.6.27/longship_api_client/models/reimbursement_price_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reimbursement_tariff_dto.py` & `longship-2023.6.27/longship_api_client/models/reimbursement_tariff_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/remote_start_transaction_request.py` & `longship-2023.6.27/longship_api_client/models/remote_start_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/remote_stop_transaction_request.py` & `longship-2023.6.27/longship_api_client/models/remote_stop_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reserve_now_request.py` & `longship-2023.6.27/longship_api_client/models/reserve_now_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/reset_request.py` & `longship-2023.6.27/longship_api_client/models/reset_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/send_local_list_request.py` & `longship-2023.6.27/longship_api_client/models/send_local_list_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/session_dto.py` & `longship-2023.6.27/longship_api_client/models/session_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/session_geo_location_dto.py` & `longship-2023.6.27/longship_api_client/models/session_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/session_location_dto.py` & `longship-2023.6.27/longship_api_client/models/session_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/set_charging_profile_request.py` & `longship-2023.6.27/longship_api_client/models/set_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/started_by_info_dto.py` & `longship-2023.6.27/longship_api_client/models/started_by_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/started_by_info_dto_authorization_state.py` & `longship-2023.6.27/longship_api_client/models/started_by_info_dto_authorization_state.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/started_by_token_dto.py` & `longship-2023.6.27/longship_api_client/models/started_by_token_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/status_schedule_dto.py` & `longship-2023.6.27/longship_api_client/models/status_schedule_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/string_segment.py` & `longship-2023.6.27/longship_api_client/models/string_segment.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/tariff_assertion_dto.py` & `longship-2023.6.27/longship_api_client/models/tariff_assertion_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/tariff_distribution_get_dto.py` & `longship-2023.6.27/longship_api_client/models/tariff_distribution_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/tariff_distribution_history_dto.py` & `longship-2023.6.27/longship_api_client/models/tariff_distribution_history_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/tariff_distribution_post_dto.py` & `longship-2023.6.27/longship_api_client/models/tariff_distribution_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/tariff_distribution_put_dto.py` & `longship-2023.6.27/longship_api_client/models/tariff_distribution_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/tariff_dto.py` & `longship-2023.6.27/longship_api_client/models/tariff_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/tariff_info_dto.py` & `longship-2023.6.27/longship_api_client/models/tariff_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/tariff_post_dto.py` & `longship-2023.6.27/longship_api_client/models/tariff_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/tariff_price_dto.py` & `longship-2023.6.27/longship_api_client/models/tariff_price_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/tariff_put_dto.py` & `longship-2023.6.27/longship_api_client/models/tariff_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/trigger_message_request.py` & `longship-2023.6.27/longship_api_client/models/trigger_message_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/unlock_connector_request.py` & `longship-2023.6.27/longship_api_client/models/unlock_connector_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/update_firmware_request.py` & `longship-2023.6.27/longship_api_client/models/update_firmware_request.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/webhook_get_dto.py` & `longship-2023.6.27/longship_api_client/models/webhook_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/webhook_header_dto.py` & `longship-2023.6.27/longship_api_client/models/webhook_header_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/webhook_post_dto.py` & `longship-2023.6.27/longship_api_client/models/webhook_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/webhook_put_dto.py` & `longship-2023.6.27/longship_api_client/models/webhook_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/models/webhook_summary_get_dto.py` & `longship-2023.6.27/longship_api_client/models/webhook_summary_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/longship_api_client/types.py` & `longship-2023.6.27/longship_api_client/types.py`

 * *Files identical despite different names*

### Comparing `longship-2023.6.26/pyproject.toml` & `longship-2023.6.27/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "longship"
-version = "2023.06.26"
+version = "2023.06.27"
 description = "A client library for accessing Longship API"
 
 authors = ["Wojtek Siudzinski <admin@suda.pl>"]
 
 readme = "README.md"
 packages = [
     {include = "longship_api_client"},
```

### Comparing `longship-2023.6.26/PKG-INFO` & `longship-2023.6.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longship
-Version: 2023.6.26
+Version: 2023.6.27
 Summary: A client library for accessing Longship API
 Author: Wojtek Siudzinski
 Author-email: admin@suda.pl
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,15 @@
 # longship-api-client
 
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/longship.svg)](https://pypi.python.org/pypi/longship/)
 [![Downloads](https://static.pepy.tech/personalized-badge/longship?period=total&units=international_system&left_color=blue&right_color=green&left_text=Downloads)](https://pepy.tech/project/longship)
 
 
-A client library for accessing Longship API
+A client library for accessing [Longship](https://www.longship.io/) API
 
 ## Usage
 First, create a client:
 
 ```python
 from longship_api_client import Client
```

