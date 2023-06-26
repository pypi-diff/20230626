# Comparing `tmp/carbon-black-cloud-sdk-1.4.2.tar.gz` & `tmp/carbon-black-cloud-sdk-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbon-black-cloud-sdk-1.4.2.tar", last modified: Wed Mar 22 17:07:10 2023, max compression
+gzip compressed data, was "carbon-black-cloud-sdk-1.4.3.tar", last modified: Mon Jun 26 19:01:17 2023, max compression
```

## Comparing `carbon-black-cloud-sdk-1.4.2.tar` & `carbon-black-cloud-sdk-1.4.3.tar`

### file list

```diff
@@ -1,128 +1,130 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:10.274602 carbon-black-cloud-sdk-1.4.2/
--rw-rw-rw-   0        0        0       55 2021-04-27 16:36:08.000000 carbon-black-cloud-sdk-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     8561 2023-03-22 17:07:10.277565 carbon-black-cloud-sdk-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     6406 2023-03-22 17:03:40.000000 carbon-black-cloud-sdk-1.4.2/README.md
--rw-rw-rw-   0        0        0        7 2023-03-22 17:03:40.000000 carbon-black-cloud-sdk-1.4.2/VERSION
--rw-rw-rw-   0        0        0      322 2023-03-22 17:07:10.283985 carbon-black-cloud-sdk-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     2225 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:08.809195 carbon-black-cloud-sdk-1.4.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:08.992796 carbon-black-cloud-sdk-1.4.2/src/carbon_black_cloud_sdk.egg-info/
--rw-rw-rw-   0        0        0     8561 2023-03-22 17:07:07.000000 carbon-black-cloud-sdk-1.4.2/src/carbon_black_cloud_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4775 2023-03-22 17:07:08.000000 carbon-black-cloud-sdk-1.4.2/src/carbon_black_cloud_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 17:07:07.000000 carbon-black-cloud-sdk-1.4.2/src/carbon_black_cloud_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-06-15 17:27:55.000000 carbon-black-cloud-sdk-1.4.2/src/carbon_black_cloud_sdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      282 2023-03-22 17:07:07.000000 carbon-black-cloud-sdk-1.4.2/src/carbon_black_cloud_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-22 17:07:07.000000 carbon-black-cloud-sdk-1.4.2/src/carbon_black_cloud_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:09.135942 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/
--rw-rw-rw-   0        0        0      275 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:09.180286 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/
--rw-rw-rw-   0        0        0      477 2022-10-21 15:48:52.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/__init__.py
--rw-rw-rw-   0        0        0    64039 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/base.py
--rw-rw-rw-   0        0        0     9812 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/differential.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:09.251687 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/
--rw-rw-rw-   0        0        0     1765 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/device_summary.yaml
--rw-rw-rw-   0        0        0     2538 2022-10-21 15:48:52.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/differential.yaml
--rw-rw-rw-   0        0        0      652 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/facet.yaml
--rw-rw-rw-   0        0        0     1217 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/result.yaml
--rw-rw-rw-   0        0        0     3989 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/run.yaml
--rw-rw-rw-   0        0        0     4212 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/template.yaml
--rw-rw-rw-   0        0        0    87496 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/base.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:09.278423 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/cache/
--rw-rw-rw-   0        0        0       50 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/cache/__init__.py
--rw-rw-rw-   0        0        0    11344 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/cache/lru.py
--rw-rw-rw-   0        0        0    31345 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/connection.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:09.383551 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/
--rw-rw-rw-   0        0        0      459 2022-01-26 21:52:03.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/__init__.py
--rw-rw-rw-   0        0        0     2816 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/aws_sm_credential_provider.py
--rw-rw-rw-   0        0        0     2485 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/default.py
--rw-rw-rw-   0        0        0     2196 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/environ_credential_provider.py
--rw-rw-rw-   0        0        0     6531 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/file_credential_provider.py
--rw-rw-rw-   0        0        0     3517 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/keychain_credential_provider.py
--rw-rw-rw-   0        0        0     8180 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/registry_credential_provider.py
--rw-rw-rw-   0        0        0     9366 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credentials.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:09.443040 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/
--rw-rw-rw-   0        0        0      405 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/__init__.py
--rw-rw-rw-   0        0        0    20642 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/base.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:09.567073 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/
--rw-rw-rw-   0        0        0     4647 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/deviceInfo.yaml
--rw-rw-rw-   0        0        0     2189 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/enriched_event_facet.yaml
--rw-rw-rw-   0        0        0      358 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/policyInfo.yaml
--rw-rw-rw-   0        0        0     2997 2021-10-12 17:01:04.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/recommendation.yaml
--rw-rw-rw-   0        0        0      153 2021-10-12 17:01:04.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/recommendation_application.yaml
--rw-rw-rw-   0        0        0      543 2021-10-12 17:01:04.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/recommendation_impact.yaml
--rw-rw-rw-   0        0        0      929 2021-10-12 17:01:04.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/recommendation_new_rule.yaml
--rw-rw-rw-   0        0        0      686 2021-10-12 17:01:04.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/recommendation_workflow.yaml
--rw-rw-rw-   0        0        0     2340 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/usbDevice.yaml
--rw-rw-rw-   0        0        0     1135 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/usbDeviceApproval.yaml
--rw-rw-rw-   0        0        0      425 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/usbDeviceBlock.yaml
--rw-rw-rw-   0        0        0    20832 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/recommendation.py
--rw-rw-rw-   0        0        0    32770 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/usb_device_control.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:09.625968 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/
--rw-rw-rw-   0        0        0      494 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/__init__.py
--rw-rw-rw-   0        0        0    28393 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/auth_events.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:09.722773 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/
--rw-rw-rw-   0        0        0     1189 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/auth_events.yaml
--rw-rw-rw-   0        0        0     2011 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/auth_events_facet.yaml
--rw-rw-rw-   0        0        0     2412 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/binary.yaml
--rw-rw-rw-   0        0        0      722 2021-08-09 21:04:43.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/feed.yaml
--rw-rw-rw-   0        0        0      494 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/ioc_v2.yaml
--rw-rw-rw-   0        0        0      671 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/iocs.yaml
--rw-rw-rw-   0        0        0     1082 2021-08-09 21:04:43.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/report.yaml
--rw-rw-rw-   0        0        0      248 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/report_severity.yaml
--rw-rw-rw-   0        0        0     1054 2021-08-09 21:04:43.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/watchlist.yaml
--rw-rw-rw-   0        0        0    66139 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/threat_intelligence.py
--rw-rw-rw-   0        0        0     6586 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/ubs.py
--rw-rw-rw-   0        0        0    10259 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/errors.py
--rw-rw-rw-   0        0        0     7589 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/helpers.py
--rw-rw-rw-   0        0        0    60554 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/live_response_api.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:09.933317 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/
--rw-rw-rw-   0        0        0     1104 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/__init__.py
--rw-rw-rw-   0        0        0    67903 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/alerts.py
--rw-rw-rw-   0        0        0     1642 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/base.py
--rw-rw-rw-   0        0        0    37986 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/devices.py
--rw-rw-rw-   0        0        0    13486 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/events.py
--rw-rw-rw-   0        0        0    25992 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/grants.py
--rw-rw-rw-   0        0        0     9230 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/jobs.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:10.142038 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/
--rw-rw-rw-   0        0        0     3963 2022-04-19 21:51:06.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/base_alert.yaml
--rw-rw-rw-   0        0        0      325 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/base_alert_note.yaml
--rw-rw-rw-   0        0        0     8787 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/device.yaml
--rw-rw-rw-   0        0        0      487 2022-04-19 21:51:06.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/device_facet.yaml
--rw-rw-rw-   0        0        0     2627 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/grant.yaml
--rw-rw-rw-   0        0        0     1461 2022-01-26 21:52:04.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/job.yaml
--rw-rw-rw-   0        0        0      530 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/network_threat_metadata.yaml
--rw-rw-rw-   0        0        0     1491 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/observation.yaml
--rw-rw-rw-   0        0        0     2011 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/observation_facet.yaml
--rw-rw-rw-   0        0        0     6003 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/policy.yaml
--rw-rw-rw-   0        0        0     1173 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/policy_rule.yaml
--rw-rw-rw-   0        0        0      547 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/policy_ruleconfig.yaml
--rw-rw-rw-   0        0        0     2184 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/process_facets.yaml
--rw-rw-rw-   0        0        0     1288 2021-06-15 17:25:33.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/profile.yaml
--rw-rw-rw-   0        0        0     1378 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/reputation_override.yaml
--rw-rw-rw-   0        0        0      395 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/stub.yaml
--rw-rw-rw-   0        0        0     1145 2021-06-15 17:25:33.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/user.yaml
--rw-rw-rw-   0        0        0      644 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/workflow.yaml
--rw-rw-rw-   0        0        0     1520 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/workflow_status.yaml
--rw-rw-rw-   0        0        0     2711 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/network_threat_metadata.py
--rw-rw-rw-   0        0        0    25693 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/observations.py
--rw-rw-rw-   0        0        0    64633 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/policies.py
--rw-rw-rw-   0        0        0    11191 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/policy_ruleconfigs.py
--rw-rw-rw-   0        0        0    40005 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/processes.py
--rw-rw-rw-   0        0        0    11651 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/reputation.py
--rw-rw-rw-   0        0        0    25013 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/users.py
--rw-rw-rw-   0        0        0    40470 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/vulnerability_assessment.py
--rw-rw-rw-   0        0        0    18580 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/rest_api.py
--rw-rw-rw-   0        0        0     1455 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/utils.py
--rw-rw-rw-   0        0        0   118761 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/winerror.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:10.198941 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/
--rw-rw-rw-   0        0        0      457 2022-10-21 15:48:52.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:07:10.265397 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/
--rw-rw-rw-   0        0        0     2560 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/computeResource.yaml
--rw-rw-rw-   0        0        0     1666 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/deviceVulnerabilitySummary.yaml
--rw-rw-rw-   0        0        0     1316 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/sensorKit.yaml
--rw-rw-rw-   0        0        0     5047 2021-06-15 17:25:33.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/vulnerability.yaml
--rw-rw-rw-   0        0        0     1765 2021-06-15 17:25:33.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/vulnerabilityAssetView.yaml
--rw-rw-rw-   0        0        0    11959 2021-06-15 17:25:33.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/vulnerabilityOrgSummary.yaml
--rw-rw-rw-   0        0        0     5548 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/nsx_remediation.py
--rw-rw-rw-   0        0        0    11414 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/sensor_lifecycle.py
--rw-rw-rw-   0        0        0    71174 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/vm_workloads_search.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:17.341489 carbon-black-cloud-sdk-1.4.3/
+-rw-rw-rw-   0        0        0       55 2021-04-27 16:36:08.000000 carbon-black-cloud-sdk-1.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     8560 2023-06-26 19:01:17.344033 carbon-black-cloud-sdk-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6405 2023-06-26 18:56:26.000000 carbon-black-cloud-sdk-1.4.3/README.md
+-rw-rw-rw-   0        0        0        7 2023-06-26 18:56:26.000000 carbon-black-cloud-sdk-1.4.3/VERSION
+-rw-rw-rw-   0        0        0      322 2023-06-26 19:01:17.346178 carbon-black-cloud-sdk-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     2225 2023-06-26 18:56:26.000000 carbon-black-cloud-sdk-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:15.965812 carbon-black-cloud-sdk-1.4.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:16.122336 carbon-black-cloud-sdk-1.4.3/src/carbon_black_cloud_sdk.egg-info/
+-rw-rw-rw-   0        0        0     8560 2023-06-26 19:01:15.000000 carbon-black-cloud-sdk-1.4.3/src/carbon_black_cloud_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4875 2023-06-26 19:01:15.000000 carbon-black-cloud-sdk-1.4.3/src/carbon_black_cloud_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 19:01:15.000000 carbon-black-cloud-sdk-1.4.3/src/carbon_black_cloud_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-06-15 17:27:55.000000 carbon-black-cloud-sdk-1.4.3/src/carbon_black_cloud_sdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      282 2023-06-26 19:01:15.000000 carbon-black-cloud-sdk-1.4.3/src/carbon_black_cloud_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-26 19:01:15.000000 carbon-black-cloud-sdk-1.4.3/src/carbon_black_cloud_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:16.254276 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/
+-rw-rw-rw-   0        0        0      275 2023-06-26 18:56:26.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:16.300112 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/
+-rw-rw-rw-   0        0        0      477 2022-10-21 15:48:52.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/__init__.py
+-rw-rw-rw-   0        0        0    64127 2023-06-26 18:56:26.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/base.py
+-rw-rw-rw-   0        0        0     9812 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/differential.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:16.361542 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/
+-rw-rw-rw-   0        0        0     1765 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/device_summary.yaml
+-rw-rw-rw-   0        0        0     2538 2022-10-21 15:48:52.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/differential.yaml
+-rw-rw-rw-   0        0        0      652 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/facet.yaml
+-rw-rw-rw-   0        0        0     1217 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/result.yaml
+-rw-rw-rw-   0        0        0     3989 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/run.yaml
+-rw-rw-rw-   0        0        0     4212 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/template.yaml
+-rw-rw-rw-   0        0        0    87754 2023-06-26 18:56:26.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/base.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:16.386404 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/cache/
+-rw-rw-rw-   0        0        0       50 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/cache/__init__.py
+-rw-rw-rw-   0        0        0    11344 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/cache/lru.py
+-rw-rw-rw-   0        0        0    30672 2023-06-26 18:56:26.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/connection.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:16.496809 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/
+-rw-rw-rw-   0        0        0      459 2022-01-26 21:52:03.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/__init__.py
+-rw-rw-rw-   0        0        0     2816 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/aws_sm_credential_provider.py
+-rw-rw-rw-   0        0        0     2485 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/default.py
+-rw-rw-rw-   0        0        0     2196 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/environ_credential_provider.py
+-rw-rw-rw-   0        0        0     6531 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/file_credential_provider.py
+-rw-rw-rw-   0        0        0     3517 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/keychain_credential_provider.py
+-rw-rw-rw-   0        0        0     8180 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/registry_credential_provider.py
+-rw-rw-rw-   0        0        0     9366 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credentials.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:16.558366 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/
+-rw-rw-rw-   0        0        0      405 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/__init__.py
+-rw-rw-rw-   0        0        0    20642 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/base.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:16.655317 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/
+-rw-rw-rw-   0        0        0     4647 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/deviceInfo.yaml
+-rw-rw-rw-   0        0        0     2189 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/enriched_event_facet.yaml
+-rw-rw-rw-   0        0        0      358 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/policyInfo.yaml
+-rw-rw-rw-   0        0        0     2997 2021-10-12 17:01:04.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/recommendation.yaml
+-rw-rw-rw-   0        0        0      153 2021-10-12 17:01:04.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/recommendation_application.yaml
+-rw-rw-rw-   0        0        0      543 2021-10-12 17:01:04.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/recommendation_impact.yaml
+-rw-rw-rw-   0        0        0      929 2021-10-12 17:01:04.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/recommendation_new_rule.yaml
+-rw-rw-rw-   0        0        0      686 2021-10-12 17:01:04.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/recommendation_workflow.yaml
+-rw-rw-rw-   0        0        0     2340 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/usbDevice.yaml
+-rw-rw-rw-   0        0        0     1135 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/usbDeviceApproval.yaml
+-rw-rw-rw-   0        0        0      425 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/usbDeviceBlock.yaml
+-rw-rw-rw-   0        0        0    20832 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/recommendation.py
+-rw-rw-rw-   0        0        0    32822 2023-06-26 18:56:26.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/usb_device_control.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:16.718138 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/
+-rw-rw-rw-   0        0        0      494 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/__init__.py
+-rw-rw-rw-   0        0        0    28393 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/auth_events.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:16.800430 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/
+-rw-rw-rw-   0        0        0     1189 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/auth_events.yaml
+-rw-rw-rw-   0        0        0     2011 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/auth_events_facet.yaml
+-rw-rw-rw-   0        0        0     2412 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/binary.yaml
+-rw-rw-rw-   0        0        0      722 2021-08-09 21:04:43.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/feed.yaml
+-rw-rw-rw-   0        0        0      494 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/ioc_v2.yaml
+-rw-rw-rw-   0        0        0      671 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/iocs.yaml
+-rw-rw-rw-   0        0        0     1082 2021-08-09 21:04:43.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/report.yaml
+-rw-rw-rw-   0        0        0      248 2021-04-27 16:36:09.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/report_severity.yaml
+-rw-rw-rw-   0        0        0     1054 2021-08-09 21:04:43.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/watchlist.yaml
+-rw-rw-rw-   0        0        0    66298 2023-06-26 18:56:26.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/threat_intelligence.py
+-rw-rw-rw-   0        0        0     6586 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/ubs.py
+-rw-rw-rw-   0        0        0    10690 2023-06-26 18:56:27.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/errors.py
+-rw-rw-rw-   0        0        0     7589 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/helpers.py
+-rw-rw-rw-   0        0        0    60554 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/live_response_api.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:17.024293 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/
+-rw-rw-rw-   0        0        0     1104 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/__init__.py
+-rw-rw-rw-   0        0        0    67903 2023-06-12 16:32:34.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/alerts.py
+-rw-rw-rw-   0        0        0     1642 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/base.py
+-rw-rw-rw-   0        0        0    38026 2023-06-26 18:56:27.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/devices.py
+-rw-rw-rw-   0        0        0    13486 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/events.py
+-rw-rw-rw-   0        0        0    25992 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/grants.py
+-rw-rw-rw-   0        0        0     9230 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/jobs.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:17.214737 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/
+-rw-rw-rw-   0        0        0     3963 2022-04-19 21:51:06.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/base_alert.yaml
+-rw-rw-rw-   0        0        0      325 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/base_alert_note.yaml
+-rw-rw-rw-   0        0        0     8787 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/device.yaml
+-rw-rw-rw-   0        0        0      487 2022-04-19 21:51:06.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/device_facet.yaml
+-rw-rw-rw-   0        0        0     1370 2023-06-26 18:56:27.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/firewall_rule.yaml
+-rw-rw-rw-   0        0        0      310 2023-06-26 18:56:27.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/firewall_rule_group.yaml
+-rw-rw-rw-   0        0        0     2627 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/grant.yaml
+-rw-rw-rw-   0        0        0     1461 2022-01-26 21:52:04.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/job.yaml
+-rw-rw-rw-   0        0        0      530 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/network_threat_metadata.yaml
+-rw-rw-rw-   0        0        0     1491 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/observation.yaml
+-rw-rw-rw-   0        0        0     2011 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/observation_facet.yaml
+-rw-rw-rw-   0        0        0     6003 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/policy.yaml
+-rw-rw-rw-   0        0        0     1173 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/policy_rule.yaml
+-rw-rw-rw-   0        0        0      547 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/policy_ruleconfig.yaml
+-rw-rw-rw-   0        0        0     2184 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/process_facets.yaml
+-rw-rw-rw-   0        0        0     1288 2021-06-15 17:25:33.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/profile.yaml
+-rw-rw-rw-   0        0        0     1378 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/reputation_override.yaml
+-rw-rw-rw-   0        0        0      395 2022-07-26 17:35:55.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/stub.yaml
+-rw-rw-rw-   0        0        0     1145 2021-06-15 17:25:33.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/user.yaml
+-rw-rw-rw-   0        0        0      644 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/workflow.yaml
+-rw-rw-rw-   0        0        0     1520 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/workflow_status.yaml
+-rw-rw-rw-   0        0        0     2711 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/network_threat_metadata.py
+-rw-rw-rw-   0        0        0    25693 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/observations.py
+-rw-rw-rw-   0        0        0    67241 2023-06-26 18:56:27.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/policies.py
+-rw-rw-rw-   0        0        0    30547 2023-06-26 18:56:27.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/policy_ruleconfigs.py
+-rw-rw-rw-   0        0        0    40005 2023-03-22 17:03:41.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/processes.py
+-rw-rw-rw-   0        0        0    11672 2023-06-26 18:56:27.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/reputation.py
+-rw-rw-rw-   0        0        0    25022 2023-06-26 18:56:27.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/users.py
+-rw-rw-rw-   0        0        0    40470 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/vulnerability_assessment.py
+-rw-rw-rw-   0        0        0    18647 2023-06-26 18:56:27.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/rest_api.py
+-rw-rw-rw-   0        0        0     1455 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/utils.py
+-rw-rw-rw-   0        0        0   118761 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/winerror.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:17.267212 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/
+-rw-rw-rw-   0        0        0      457 2022-10-21 15:48:52.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:01:17.331263 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/
+-rw-rw-rw-   0        0        0     2560 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/computeResource.yaml
+-rw-rw-rw-   0        0        0     1666 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/deviceVulnerabilitySummary.yaml
+-rw-rw-rw-   0        0        0     1316 2021-04-27 16:36:10.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/sensorKit.yaml
+-rw-rw-rw-   0        0        0     5047 2021-06-15 17:25:33.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/vulnerability.yaml
+-rw-rw-rw-   0        0        0     1765 2021-06-15 17:25:33.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/vulnerabilityAssetView.yaml
+-rw-rw-rw-   0        0        0    11959 2021-06-15 17:25:33.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/vulnerabilityOrgSummary.yaml
+-rw-rw-rw-   0        0        0     5557 2023-06-26 18:56:27.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/nsx_remediation.py
+-rw-rw-rw-   0        0        0    11414 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/sensor_lifecycle.py
+-rw-rw-rw-   0        0        0    71174 2023-03-22 17:03:42.000000 carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/vm_workloads_search.py
```

### Comparing `carbon-black-cloud-sdk-1.4.2/PKG-INFO` & `carbon-black-cloud-sdk-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: carbon-black-cloud-sdk
-Version: 1.4.2
+Version: 1.4.3
 Summary: VMware Carbon Black Cloud Python SDK
 Home-page: https://github.com/carbonblack/carbon-black-cloud-sdk-python
 Author: VMware Carbon Black
 Author-email: cb-developer-network@vmware.com
 License: MIT
 Description: # VMware Carbon Black Cloud Python SDK
         
-        **Latest Version:** 1.4.2
+        **Latest Version:** 1.4.3
         <br>
-        **Release Date:** March 22, 2023
+        **Release Date:** June 26, 2023
         
         [![Coverage Status](https://coveralls.io/repos/github/carbonblack/carbon-black-cloud-sdk-python/badge.svg?t=Id6Baf)](https://coveralls.io/github/carbonblack/carbon-black-cloud-sdk-python)
         [![Codeship Status for carbonblack/carbon-black-cloud-sdk-python](https://app.codeship.com/projects/9e55a370-a772-0138-aae4-129773225755/status?branch=develop)](https://app.codeship.com/projects/402767)
         
         
         
         ## Recent updates
@@ -62,15 +62,15 @@
         - jsonschema
         - validators
         - keyring (for MacOS)
         
         If developing the SDK, you also need:
         
         - pytest==5.4.2
-        - pymox==0.7.8
+        - pymox==1.0.0
         - coverage==5.1
         - coveralls==2.0.0
         - flake8==3.8.1
         - flake8-colors==0.1.6
         - flake8-docstrings==1.5.0
         - pre-commit>=2.15.0
```

### Comparing `carbon-black-cloud-sdk-1.4.2/README.md` & `carbon-black-cloud-sdk-1.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # VMware Carbon Black Cloud Python SDK
 
-**Latest Version:** 1.4.2
+**Latest Version:** 1.4.3
 <br>
-**Release Date:** March 22, 2023
+**Release Date:** June 26, 2023
 
 [![Coverage Status](https://coveralls.io/repos/github/carbonblack/carbon-black-cloud-sdk-python/badge.svg?t=Id6Baf)](https://coveralls.io/github/carbonblack/carbon-black-cloud-sdk-python)
 [![Codeship Status for carbonblack/carbon-black-cloud-sdk-python](https://app.codeship.com/projects/9e55a370-a772-0138-aae4-129773225755/status?branch=develop)](https://app.codeship.com/projects/402767)
 
 
 
 ## Recent updates
@@ -54,15 +54,15 @@
 - jsonschema
 - validators
 - keyring (for MacOS)
 
 If developing the SDK, you also need:
 
 - pytest==5.4.2
-- pymox==0.7.8
+- pymox==1.0.0
 - coverage==5.1
 - coveralls==2.0.0
 - flake8==3.8.1
 - flake8-colors==0.1.6
 - flake8-docstrings==1.5.0
 - pre-commit>=2.15.0
```

### Comparing `carbon-black-cloud-sdk-1.4.2/setup.py` & `carbon-black-cloud-sdk-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "keyring;platform_system=='Darwin'",
     'boto3'
 ]
 
 extras_require = {
     "test": [
         'pytest==7.2.1',
-        'pymox==0.7.8',
+        'pymox==1.0.0',
         'coverage==6.5.0',
         'coveralls==3.3.1',
         'flake8==5.0.4',
         'flake8-colors==0.1.9',
         'flake8-docstrings==1.7.0',
         'pre-commit>=2.15.0',
         'requests-mock==1.10.0'
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/carbon_black_cloud_sdk.egg-info/PKG-INFO` & `carbon-black-cloud-sdk-1.4.3/src/carbon_black_cloud_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: carbon-black-cloud-sdk
-Version: 1.4.2
+Version: 1.4.3
 Summary: VMware Carbon Black Cloud Python SDK
 Home-page: https://github.com/carbonblack/carbon-black-cloud-sdk-python
 Author: VMware Carbon Black
 Author-email: cb-developer-network@vmware.com
 License: MIT
 Description: # VMware Carbon Black Cloud Python SDK
         
-        **Latest Version:** 1.4.2
+        **Latest Version:** 1.4.3
         <br>
-        **Release Date:** March 22, 2023
+        **Release Date:** June 26, 2023
         
         [![Coverage Status](https://coveralls.io/repos/github/carbonblack/carbon-black-cloud-sdk-python/badge.svg?t=Id6Baf)](https://coveralls.io/github/carbonblack/carbon-black-cloud-sdk-python)
         [![Codeship Status for carbonblack/carbon-black-cloud-sdk-python](https://app.codeship.com/projects/9e55a370-a772-0138-aae4-129773225755/status?branch=develop)](https://app.codeship.com/projects/402767)
         
         
         
         ## Recent updates
@@ -62,15 +62,15 @@
         - jsonschema
         - validators
         - keyring (for MacOS)
         
         If developing the SDK, you also need:
         
         - pytest==5.4.2
-        - pymox==0.7.8
+        - pymox==1.0.0
         - coverage==5.1
         - coveralls==2.0.0
         - flake8==3.8.1
         - flake8-colors==0.1.6
         - flake8-docstrings==1.5.0
         - pre-commit>=2.15.0
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/carbon_black_cloud_sdk.egg-info/SOURCES.txt` & `carbon-black-cloud-sdk-1.4.3/src/carbon_black_cloud_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,16 @@
 src/cbc_sdk/platform/reputation.py
 src/cbc_sdk/platform/users.py
 src/cbc_sdk/platform/vulnerability_assessment.py
 src/cbc_sdk/platform/models/base_alert.yaml
 src/cbc_sdk/platform/models/base_alert_note.yaml
 src/cbc_sdk/platform/models/device.yaml
 src/cbc_sdk/platform/models/device_facet.yaml
+src/cbc_sdk/platform/models/firewall_rule.yaml
+src/cbc_sdk/platform/models/firewall_rule_group.yaml
 src/cbc_sdk/platform/models/grant.yaml
 src/cbc_sdk/platform/models/job.yaml
 src/cbc_sdk/platform/models/network_threat_metadata.yaml
 src/cbc_sdk/platform/models/observation.yaml
 src/cbc_sdk/platform/models/observation_facet.yaml
 src/cbc_sdk/platform/models/policy.yaml
 src/cbc_sdk/platform/models/policy_rule.yaml
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/base.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,16 @@
         result = self._cb.put_object(url, {'status': 'CANCELLED'})
         if result.status_code == 200:
             try:
                 self._info = result.json()
                 self._last_refresh_time = time.time()
                 return True
             except Exception:
-                raise ServerError(result.status_code, "Cannot parse response as JSON: {0:s}".format(result.content))
+                raise ServerError(result.status_code, "Cannot parse response as JSON: {0:s}".format(result.content),
+                                  uri=url)
         return False
 
     def delete(self):
         """
         Delete a query.
 
         Required Permissions:
@@ -587,15 +588,16 @@
         result = self._cb.put_object(url, self._info)
         if (result.status_code == 200):
             try:
                 self._info = result.json()
                 self._last_refresh_time = time.time()
                 return True
             except Exception:
-                raise ServerError(result.status_code, "Cannot parse response as JSON: {0:s}".format(result.content))
+                raise ServerError(result.status_code, "Cannot parse response as JSON: {0:s}".format(result.content),
+                                  uri=url)
         return False
 
     def query_runs(self):
         """
         Create a RunHistory query that searches for all runs created by this template ID.
 
         The query may be further augmented with additional criteria prior to enumerating its results.
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/differential.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/differential.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/device_summary.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/device_summary.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/differential.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/differential.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/facet.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/facet.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/result.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/result.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/run.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/run.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/audit_remediation/models/template.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/audit_remediation/models/template.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/base.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -820,14 +820,21 @@
                 self._set(attrname, val)
             else:
                 print("Trying to set attribute {0:s}".format(attrname))
         else:
             object.__setattr__(self, attrname, val)
 
     def _set(self, attrname, new_value):
+        """
+        Sets the value of an attribute on the object.
+
+        Args:
+            attrname (str): Name of the attribute.
+            new_value (Any): Value of the attribute.
+        """
         # ensure that we are operating on the full object first
         if not self._full_init and self._model_unique_id is not None:
             self.refresh()
 
         # extract unique ID if we're updating a "joined" field
         if isinstance(new_value, NewBaseModel):
             new_value = new_value._model_unique_id
@@ -894,35 +901,36 @@
         Returns:
             Any: The unique ID of this object.
         """
         refresh_required = False
 
         if request_ret.status_code not in range(200, 300):
             try:
-                message = json.loads(request_ret.text)[0]
+                result = json.loads(request_ret.text)[0]
             except Exception:
-                message = request_ret.text
+                result = request_ret.text
 
-            raise ServerError(request_ret.status_code, message,
-                              result="Did not update {} record.".format(self.__class__.__name__))
+            raise ServerError(request_ret.status_code, f"Did not update {self.__class__.__name__} record.",
+                              result=result, uri=request_ret.url)
         else:
             try:
-                message = request_ret.json()
-                log.debug("Received response: %s" % message)
-                if list(message.keys()) == ["result"]:
-                    post_result = message.get("result", None)
+                result = request_ret.json()
+                log.debug("Received response: %s" % result)
+                if list(result.keys()) == ["result"]:
+                    post_result = result.get("result", None)
 
                     if post_result and post_result != "success":
-                        raise ServerError(request_ret.status_code, post_result,
-                                          result="Did not update {0:s} record.".format(self.__class__.__name__))
+                        raise ServerError(request_ret.status_code,
+                                          f"Did not update {self.__class__.__name__} record.",
+                                          result=post_result, uri=request_ret.url)
                     else:
                         refresh_required = True
                 else:
                     self._info = json.loads(request_ret.text)
-                    if message.keys() == ["id"]:
+                    if result.keys() == ["id"]:
                         # if all we got back was an ID, try refreshing to get the entire record.
                         log.debug("Only received an ID back from the server, forcing a refresh")
                         refresh_required = True
                     else:
                         self._full_init = True
             except Exception:
                 refresh_required = True
@@ -965,18 +973,18 @@
         if self._model_unique_id:
             ret = self._cb.delete_object(self._build_api_request_uri())
         else:
             return
 
         if ret.status_code not in (200, 204):
             try:
-                message = json.loads(ret.text)[0]
+                result = json.loads(ret.text)[0]
             except Exception:
-                message = ret.text
-            raise ServerError(ret.status_code, message, result="Did not delete {0:s}.".format(str(self)))
+                result = ret.text
+            raise ServerError(ret.status_code, f"Did not delete {str(self)}.", result=result, uri=None)
 
     def validate(self):
         """
         Validates this object.
 
         Returns:
             bool: True if the object is validated.
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/cache/lru.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/cache/lru.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/connection.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,23 +317,23 @@
                                   .format(self.server, str(connection_error)),
                                   original_exception=connection_error)
         except Exception as e:
             raise ApiError("Unknown exception when connecting to server: {0:s}".format(str(e)),
                            original_exception=e)
         else:
             if r.status_code >= 500:
-                raise ServerError(error_code=r.status_code, message=r.text)
+                raise ServerError(error_code=r.status_code, message=r.text, uri=uri)
             elif r.status_code == 404:
                 raise ObjectNotFoundError(uri=uri, message=r.text)
             elif r.status_code == 401:
                 raise UnauthorizedError(uri=uri, action=method, message=r.text)
             elif r.status_code == 400 and try_json(r).get('reason') == 'query_malformed_syntax':
                 raise QuerySyntaxError(uri=uri, message=r.text)
             elif r.status_code >= 400:
-                raise ClientError(error_code=r.status_code, message=r.text)
+                raise ClientError(error_code=r.status_code, message=r.text, uri=uri)
             return r
 
     def get(self, url, **kwargs):
         """
         Submit a GET request on this connection.
 
         Args:
@@ -432,33 +432,14 @@
                                   timeout=timeout,
                                   max_retries=max_retries,
                                   proxy_session=proxy_session,
                                   pool_connections=pool_connections,
                                   pool_maxsize=pool_maxsize,
                                   pool_block=pool_block)
 
-    def raise_unless_json(self, ret, expected):
-        """
-        Raise a ServerError unless we got back an HTTP 200 response with JSON containing all the expected values.
-
-        Args:
-            ret (object): Return value to be checked.
-            expected (dict): Expected keys and values that need to be found in the JSON response.
-
-        Raises:
-            ServerError: If the HTTP response is anything but 200, or if the expected values are not found.
-        """
-        if ret.status_code == 200:
-            message = ret.json()
-            for k, v in iter(expected.items()):
-                if k not in message or message[k] != v:
-                    raise ServerError(ret.status_code, message)
-        else:
-            raise ServerError(ret.status_code, "{0}".format(ret.content), )
-
     def get_object(self, uri, query_parameters=None, default=None):
         """
         Submit a GET request to the server and parse the result as JSON before returning.
 
         Args:
             uri (str): The URI to send the GET request to.
             query_parameters (object): Parameters for the query.
@@ -468,20 +449,22 @@
             object: Result of the GET request.
         """
         result = self.api_json_request("GET", uri, params=query_parameters)
         if result.status_code == 200:
             try:
                 return result.json()
             except Exception:
-                raise ServerError(result.status_code, "Cannot parse response as JSON: {0:s}".format(result.content))
+                raise ServerError(result.status_code, "Cannot parse response as JSON: {0:s}".format(result.content),
+                                  uri=uri)
         elif result.status_code == 204:
             # empty response
             return default
         else:
-            raise ServerError(error_code=result.status_code, message="Unknown error: {0}".format(result.content))
+            raise ServerError(error_code=result.status_code, message="Unknown error: {0}".format(result.content),
+                              uri=uri)
 
     def get_raw_data(self, uri, query_parameters=None, default=None, **kwargs):
         """
         Submit a GET request to the server and return the result without parsing it.
 
         Args:
             uri (str): The URI to send the GET request to.
@@ -496,15 +479,16 @@
         result = self.api_json_request("GET", uri, headers=hdrs, params=query_parameters)
         if result.status_code == 200:
             return result.text
         elif result.status_code == 204:
             # empty response
             return default
         else:
-            raise ServerError(error_code=result.status_code, message="Unknown error: {0}".format(result.content))
+            raise ServerError(error_code=result.status_code, message="Unknown error: {0}".format(result.content),
+                              uri=uri)
 
     def api_json_request(self, method, uri, **kwargs):
         """
         Submit a request to the server.
 
         Args:
             method (str): HTTP method to use.
@@ -532,15 +516,15 @@
 
         try:
             resp = result.json()
         except ValueError:
             return result
 
         if "errorMessage" in resp:
-            raise ServerError(error_code=result.status_code, message=resp["errorMessage"])
+            raise ServerError(error_code=result.status_code, message=resp["errorMessage"], uri=uri)
 
         return result
 
     def api_request_stream(self, method, uri, stream_output, **kwargs):
         """
         Submit a request to the specified URI and stream the results back into the given stream object.
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/aws_sm_credential_provider.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/aws_sm_credential_provider.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/default.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/default.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/environ_credential_provider.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/environ_credential_provider.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/file_credential_provider.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/file_credential_provider.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/keychain_credential_provider.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/keychain_credential_provider.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credential_providers/registry_credential_provider.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credential_providers/registry_credential_provider.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/credentials.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/credentials.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/base.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/base.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/deviceInfo.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/deviceInfo.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/enriched_event_facet.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/enriched_event_facet.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/recommendation.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/recommendation.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/recommendation_impact.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/recommendation_impact.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/recommendation_new_rule.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/recommendation_new_rule.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/recommendation_workflow.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/recommendation_workflow.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/usbDevice.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/usbDevice.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/models/usbDeviceApproval.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/models/usbDeviceApproval.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/recommendation.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/recommendation.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/endpoint_standard/usb_device_control.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/endpoint_standard/usb_device_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,18 +238,19 @@
         if self._model_unique_id:
             ret = self._cb.delete_object(self._build_api_request_uri())
         else:
             return
 
         if ret.status_code not in (200, 204):
             try:
-                message = json.loads(ret.text)[0]
+                result = json.loads(ret.text)[0]
             except Exception:
-                message = ret.text
-            raise ServerError(ret.status_code, message, result="Did not delete {0:s}.".format(str(self)))
+                result = ret.text
+            raise ServerError(ret.status_code, f"Did not delete {str(self)}.", result=result,
+                              uri=self._build_api_request_uri())
 
     @classmethod
     def create(cls, cb, policy_id):
         """
         Creates a USBDeviceBlock for a given policy ID.
 
         Args:
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/auth_events.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/auth_events.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/auth_events.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/auth_events.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/auth_events_facet.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/auth_events_facet.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/binary.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/binary.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/feed.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/feed.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/iocs.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/iocs.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/report.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/report.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/models/watchlist.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/models/watchlist.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/threat_intelligence.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/threat_intelligence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1177,16 +1177,16 @@
         Checks to ensure this report contains valid data.
 
         Raises:
             InvalidObjectError: If the report contains invalid data.
         """
         super(Report, self).validate()
 
-        if self.link and not validators.url(self.link):
-            raise InvalidObjectError("link should be a valid URL")
+        if self.link and not (validators.ipv4(self.link) or validators.url(self.link) or validators.domain(self.link)):
+            raise InvalidObjectError(f"link should be a valid URL or domain: {self.link}")
 
         if self.iocs_v2:
             [ioc.validate() for ioc in self._iocs_v2]
         if self._iocs_v2_need_rebuild:
             self._info['iocs_v2'] = [ioc._info for ioc in self._iocs_v2]
             self._iocs_v2_need_rebuild = False
 
@@ -1721,16 +1721,16 @@
         Checks to ensure this IOC contains valid FQDN.
 
         Raises:
             InvalidObjectError: If the IOC contains invalid data.
         """
         super(IOC_V2, self).validate()
 
-        if self.link and not validators.domain(self.link):
-            raise InvalidObjectError("link should be a valid domain URL (FQDN)")
+        if self.link and not (validators.ipv4(self.link) or validators.url(self.link) or validators.domain(self.link)):
+            raise InvalidObjectError(f"link should be a valid URL or domain: {self.link}")
 
     @property
     def ignored(self):
         """
         Returns whether or not this IOC is ignored.
 
         Only watchlist IOCs have an ignore status.
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/enterprise_edr/ubs.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/enterprise_edr/ubs.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/errors.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,28 +40,30 @@
         """
         return self.message
 
 
 class ClientError(ApiError):
     """A ClientError is raised when an HTTP 4xx error code is returned from the Carbon Black server."""
 
-    def __init__(self, error_code, message, result=None, original_exception=None):
+    def __init__(self, error_code, message, **kwargs):
         """
         Initialize the ClientError.
 
         Args:
             error_code (int): The error code that was received from the server.
             message (str): The actual error message.
-            result (object): The result of the operation from the server.
-            original_exception (Exception): The exception that caused this one to be raised.
+            kwargs (dict): Additional arguments, which may include 'result' (server operation result),
+                          'original_exception' (exception causing this one to be raised), and 'uri' (URI being accessed
+                           when this error was raised).
         """
-        super(ClientError, self).__init__(message=message, original_exception=original_exception)
+        super(ClientError, self).__init__(message=message, original_exception=kwargs.get('original_exception', None))
 
         self.error_code = error_code
-        self.result = result
+        self.result = kwargs.get('result', None)
+        self.uri = kwargs.get('uri', None)
 
     def __str__(self):
         """
         Convert the exception to a string.
 
         Returns:
             str: String equivalent of the exception.
@@ -105,45 +107,49 @@
 
         return msg
 
 
 class ServerError(ApiError):
     """A ServerError is raised when an HTTP 5xx error code is returned from the Carbon Black server."""
 
-    def __init__(self, error_code, message, result=None, original_exception=None):
+    def __init__(self, error_code, message, **kwargs):
         """
         Initialize the ServerError.
 
         Args:
             error_code (int): The error code that was received from the server.
             message (str): The actual error message.
-            result (object): The result of the operation from the server.
-            original_exception (Exception): The exception that caused this one to be raised.
+            kwargs (dict): Additional arguments, which may include 'result' (server operation result),
+                          'original_exception' (exception causing this one to be raised), and 'uri' (URI being accessed
+                           when this error was raised).
         """
-        super(ServerError, self).__init__(message=message, original_exception=original_exception)
+        super(ServerError, self).__init__(message=message, original_exception=kwargs.get('original_exception', None))
 
         self.error_code = error_code
-        self.result = result
+        self.result = kwargs.get('result', None)
+        self.uri = kwargs.get('uri', None)
 
     def __str__(self):
         """
         Convert the exception to a string.
 
         Returns:
             str: String equivalent of the exception.
         """
         msg = "Received error code {0:d} from API".format(self.error_code)
+        if self.uri:
+            msg += f" <{self.uri}>"
+        details = ""
         if self.message:
-            msg += ": {0:s}".format(self.message)
-        else:
-            msg += " (No further information provided)"
-
+            details += f" ({self.message})"
         if self.result:
-            msg += ". {}".format(self.result)
-        return msg
+            details += f" ({self.result})"
+        if not details:
+            details = " (No further information provided)"
+        return msg + details
 
 
 class ObjectNotFoundError(ApiError):
     """The requested object could not be found in the Carbon Black datastore."""
 
     def __init__(self, uri, message=None, original_exception=None):
         """
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/helpers.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/live_response_api.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/live_response_api.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/__init__.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/alerts.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/alerts.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/base.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/base.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/devices.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,16 @@
 
         resp = self._cb.post_object(url, body=request)
         if resp.status_code == 200:
             return resp.json()
         elif resp.status_code == 204:
             return None
         else:
-            raise ServerError(error_code=resp.status_code, message="Device action error: {0}".format(resp.content))
+            raise ServerError(error_code=resp.status_code, message="Device action error: {0}".format(resp.content),
+                              uri=url)
 
     def get_vulnerability_summary(self, category=None):
         """
         Get the vulnerabilities associated with this device
 
         Required Permissions:
             vulnerabilityAssessment.data (READ)
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/events.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/events.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/grants.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/grants.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/jobs.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/jobs.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/base_alert.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/base_alert.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/device.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/device.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/grant.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/grant.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/job.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/job.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/network_threat_metadata.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/network_threat_metadata.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/observation.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/observation.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/observation_facet.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/observation_facet.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/policy.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/policy.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/policy_rule.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/policy_rule.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/policy_ruleconfig.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/policy_ruleconfig.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/process_facets.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/process_facets.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/profile.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/profile.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/reputation_override.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/reputation_override.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/user.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/user.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/workflow.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/workflow.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/models/workflow_status.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/models/workflow_status.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/network_threat_metadata.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/network_threat_metadata.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/observations.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/observations.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/policies.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,23 @@
 # * NON-INFRINGEMENT AND FITNESS FOR A PARTICULAR PURPOSE.
 
 """Policy implementation as part of Platform API"""
 import copy
 import json
 from types import MappingProxyType
 from cbc_sdk.base import MutableBaseModel, BaseQuery, IterableQueryMixin, AsyncQueryMixin
-from cbc_sdk.platform.policy_ruleconfigs import PolicyRuleConfig, CorePreventionRuleConfig
+from cbc_sdk.platform.policy_ruleconfigs import (PolicyRuleConfig, CorePreventionRuleConfig,
+                                                 HostBasedFirewallRuleConfig, DataCollectionRuleConfig)
 from cbc_sdk.errors import ApiError, ServerError, InvalidObjectError
 
 
 SPECIFIC_RULECONFIGS = MappingProxyType({
-    "core_prevention": CorePreventionRuleConfig
+    "core_prevention": CorePreventionRuleConfig,
+    "host_based_firewall": HostBasedFirewallRuleConfig,
+    "data_collection": DataCollectionRuleConfig
 })
 
 
 class Policy(MutableBaseModel):
     """
     Represents a policy within the organization.
 
@@ -619,14 +622,32 @@
             True if the refresh was successful.
         """
         rc = super(Policy, self)._refresh()
         self._object_rules_need_load = True
         self._object_rule_configs_need_load = True
         return rc
 
+    def is_dirty(self):
+        """
+        Returns whether or not any fields of this object have been changed.
+
+        Returns:
+            bool: True if any fields of this object have been changed, False if not.
+        """
+        if super(Policy, self).is_dirty():
+            return True
+        # we need to check the rules and rule configs as well
+        if not self._object_rules_need_load:
+            if any(rule.is_dirty() for rule in self._object_rules.values()):
+                return True
+        if not self._object_rule_configs_need_load:
+            if any(rule_config.is_dirty() for rule_config in self._object_rule_configs.values()):
+                return True
+        return False
+
     @property
     def rules(self):
         """
         Returns a dictionary of rules and rule IDs for this Policy.
 
         Returns:
             dict: A dictionary with rule IDs as keys and rule data as values.
@@ -691,14 +712,54 @@
         Returns a list of core prevention rule configuration objects for this Policy.
 
         Returns:
             list: A list of CorePreventionRuleConfig objects.
         """
         return [rconf for rconf in self.object_rule_configs.values() if isinstance(rconf, CorePreventionRuleConfig)]
 
+    @property
+    def host_based_firewall_rule_config(self):
+        """
+        Returns the host-based firewall rule configuration for this policy.
+
+        Returns:
+            HostBasedFirewallRuleConfig: The host-based firewall rule configuration, or None.
+
+        Raises:
+            InvalidObjectError: If there's more than one host-based firewall rule configuration (should not happen).
+        """
+        tmp = [rconf for rconf in self.object_rule_configs.values() if isinstance(rconf, HostBasedFirewallRuleConfig)]
+        if not tmp:
+            return None
+        if len(tmp) > 1:
+            raise InvalidObjectError("found multiple host-based firewall rule configurations")
+        return tmp[0]
+
+    @property
+    def data_collection_rule_configs(self):
+        """
+        Returns a dictionary of data collection rule configuration IDs and objects for this Policy.
+
+        Returns:
+            dict: A dictionary with data collection rule configuration IDs as keys and DataCollectionRuleConfig objects
+                  as values.
+        """
+        return {key: rconf for (key, rconf) in self.object_rule_configs.items()
+                if isinstance(rconf, DataCollectionRuleConfig)}
+
+    @property
+    def data_collection_rule_configs_list(self):
+        """
+        Returns a list of data collection rule configuration objects for this Policy.
+
+        Returns:
+            list: A list of DataCollectionRuleConfig objects.
+        """
+        return [rconf for rconf in self.object_rule_configs.values() if isinstance(rconf, DataCollectionRuleConfig)]
+
     def valid_rule_configs(self):
         """
         Returns a dictionary identifying all valid rule configurations for this policy.
 
         Returns:
             dict: A dictionary mapping string ID values (UUIDs) to dicts containing entries for name, description,
                   and category.
@@ -1191,23 +1252,25 @@
         Required Permissions:
             org.policies(UPDATE)
         """
         if "id" in self._dirty_attributes.keys() or self._model_unique_id is None:
             new_object_info = copy.deepcopy(self._info)
             if "id" in new_object_info:
                 del new_object_info["id"]
-            ret = self._cb.post_object(self._parent._build_api_request_uri() + "/rules", new_object_info)
+            url = self._parent._build_api_request_uri() + "/rules"
+            ret = self._cb.post_object(url, new_object_info)
         else:
-            ret = self._cb.put_object(self._parent._build_api_request_uri() + f"/rules/{self.id}", self._info)
+            url = self._parent._build_api_request_uri() + f"/rules/{self.id}"
+            ret = self._cb.put_object(url, self._info)
         if ret.status_code not in range(200, 300):
             try:
-                message = json.loads(ret.text)[0]
+                result = json.loads(ret.text)[0]
             except Exception:
-                message = ret.text
-            raise ServerError(ret.status_code, message, result="Unable to update policy rule")
+                result = ret.text
+            raise ServerError(ret.status_code, "Unable to update policy rule", result=result, uri=url)
         self._info = json.loads(ret.text)
         self._full_init = True
         self._parent._on_updated_rule(self)
 
     def _delete_object(self):
         """
         Deletes this rule object from the policy on the server.
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/policy_ruleconfigs.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/reputation.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,268 +7,321 @@
 # *
 # * DISCLAIMER. THIS PROGRAM IS PROVIDED TO YOU "AS IS" WITHOUT
 # * WARRANTIES OR CONDITIONS OF ANY KIND, WHETHER ORAL OR WRITTEN,
 # * EXPRESS OR IMPLIED. THE AUTHOR SPECIFICALLY DISCLAIMS ANY IMPLIED
 # * WARRANTIES OR CONDITIONS OF MERCHANTABILITY, SATISFACTORY QUALITY,
 # * NON-INFRINGEMENT AND FITNESS FOR A PARTICULAR PURPOSE.
 
-"""Policy rule configuration implementation as part of Platform API"""
+"""Model and Query Classes for Reputation"""
 
-import copy
-import jsonschema
-from cbc_sdk.base import MutableBaseModel
-from cbc_sdk.errors import ApiError, InvalidObjectError
+from cbc_sdk.errors import ApiError, ServerError
+from cbc_sdk.platform import PlatformModel
+from cbc_sdk.base import (BaseQuery, QueryBuilder, QueryBuilderSupportMixin,
+                          IterableQueryMixin, AsyncQueryMixin)
 
+import time
+import json
 
-class PolicyRuleConfig(MutableBaseModel):
-    """
-    Represents a rule configuration in the policy.
+""""Reputation Override Models"""
 
-    Create one of these objects, associating it with a Policy, and set its properties, then call its save() method to
-    add the rule configuration to the policy. This requires the org.policies(UPDATE) permission.
 
-    To update a PolicyRuleConfig, change the values of its property fields, then call its save() method.  This
-    requires the org.policies(UPDATE) permission.
-
-    To delete an existing PolicyRuleConfig, call its delete() method. This requires the org.policies(DELETE) permission.
-
-    """
-    urlobject = "/policyservice/v1/orgs/{0}/policies"
+class ReputationOverride(PlatformModel):
+    """Represents a reputation override."""
+    urlobject = "/appservices/v6/orgs/{0}/reputations/overrides"
+    urlobject_single = "/appservices/v6/orgs/{0}/reputations/overrides/{1}"
     primary_key = "id"
-    swagger_meta_file = "platform/models/policy_ruleconfig.yaml"
+    swagger_meta_file = "platform/models/reputation_override.yaml"
+    _is_deleted = False
 
-    def __init__(self, cb, parent, model_unique_id=None, initial_data=None, force_init=False, full_doc=False):
+    def __init__(self, cb, model_unique_id, initial_data=None):
         """
-        Initialize the PolicyRuleConfig object.
+        Initialize the ReputationOverride object.
 
         Args:
             cb (BaseAPI): Reference to API object used to communicate with the server.
-            parent (Policy): The "parent" policy of this rule configuration.
-            model_unique_id (str): ID of the rule configuration.
-            initial_data (dict): Initial data used to populate the rule configuration.
-            force_init (bool): If True, forces the object to be refreshed after constructing.  Default False.
-            full_doc (bool): If True, object is considered "fully" initialized. Default False.
+            model_unique_id (str): ID of the alert represented.
+            initial_data (dict): Initial data used to populate the alert.
         """
-        super(PolicyRuleConfig, self).__init__(cb, model_unique_id=model_unique_id, initial_data=initial_data,
-                                               force_init=force_init, full_doc=full_doc)
-        self._parent = parent
-        if model_unique_id is None:
-            self.touch(True)
+        super(ReputationOverride, self).__init__(cb, model_unique_id, initial_data, full_doc=True)
+        if model_unique_id is not None and initial_data is None:
+            self._refresh()
 
-    def _base_url(self):
+    @classmethod
+    def _query_implementation(cls, cb, **kwargs):
         """
-        Calculates the base URL for these particular rule configs, including the org key and the parent policy ID.
+        Returns the appropriate query object for the ReputationOverride.
 
-        Returns:
-            str: The base URL for these particular rule configs.
+        Args:
+            cb (BaseAPI): Reference to API object used to communicate with the server.
+            **kwargs (dict): Not used, retained for compatibility.
 
-        Raises:
-            InvalidObjectError: If the rule config object is unparented.
+        Returns:
+            ReputationOverrideQuery: The query object for this alert type.
         """
-        if self._parent is None:
-            raise InvalidObjectError("no parent for rule config")
-        return PolicyRuleConfig.urlobject.format(self._cb.credentials.org_key) \
-            + f"/{self._parent._model_unique_id}/rule_configs"
+        return ReputationOverrideQuery(cls, cb)
 
     def _refresh(self):
         """
-        Refreshes the rule configuration object from the server.
-
-        Required Permissions:
-            org.policies (READ)
+        Rereads the device data from the server.
 
         Returns:
-            bool: True if the refresh was successful.
+            bool: True if refresh was successful, False if not.
         """
-        if self._model_unique_id is not None:
-            rc = self._parent._refresh()
-            if rc:
-                newobj = self._parent.object_rule_configs.get(self.id, None)
-                if newobj:
-                    self._info = newobj._info
-            return rc
+        if self._is_deleted:
+            raise ApiError("Cannot refresh a deleted ReputationOverride")
+        url = self.urlobject_single.format(self._cb.credentials.org_key, self._model_unique_id)
+        resp = self._cb.get_object(url)
+        self._info = resp
+        self._last_refresh_time = time.time()
+        self._full_init = True
+        return True
 
-    def _update_ruleconfig(self):
-        """Perform the internal update of the rule configuration object."""
-        raise NotImplementedError("update not defined for this category of rule configuration")
+    def delete(self):
+        """Delete this object."""
+        if self._model_unique_id is None:
+            return
+
+        resp = self._cb.delete_object(self.urlobject_single.format(self._cb.credentials.org_key, self._model_unique_id))
+        if resp.status_code not in (200, 204):
+            try:
+                result = json.loads(resp.text)[0]
+            except Exception:
+                result = resp.text
+            raise ServerError(resp.status_code, f"Did not delete {str(self)}.", result=result, uri=None)
+        self._is_deleted = True
 
-    def _update_object(self):
+    @classmethod
+    def create(cls, cb, initial_data):
         """
-        Updates the rule configuration object on the policy on the server.
+        Returns all vendors and products that have been seen for the organization.
 
-        Required Permissions:
-            org.policies(UPDATE)
-        """
-        self._update_ruleconfig()
-        self._full_init = True
-        self._parent._on_updated_rule_config(self)
+        Args:
+            cb (BaseAPI): Reference to API object used to communicate with the server.
+            initial_data (Object): The initial data for a ReputationOverride
 
-    def _delete_ruleconfig(self):
-        """Perform the internal delete of the rule configuration object."""
-        raise NotImplementedError("delete not defined for this category of rule configuration")
+        Example:
+            >>>
+            {
+                "description": "Banned as known malware",
+                "override_list": "BLACK_LIST",
+                "override_type": "SHA256",
+                "sha256_hash": "dd191a5b23df92e13a8852291f9fb5ed594b76a28a5a464418442584afd1e048",
+                "filename": "foo.exe"
+            }
 
-    def _delete_object(self):
-        """
-        Deletes this rule configuration object from the policy on the server.
+        Returns:
+            ReputationOverride: The created ReputationOverride object based on the specified properties
 
-        Required Permissions:
-            org.policies(DELETE)
         """
-        self._delete_ruleconfig()
-        self._parent._on_deleted_rule_config(self)
+        resp = cb.post_object(cls.urlobject.format(cb.credentials.org_key), body=initial_data)
+        resp_json = resp.json()
+        return cls(cb, resp_json["id"], resp_json)
 
-    def get_parameter(self, name):
+    @classmethod
+    def bulk_delete(cls, cb, overrides):
         """
-        Returns a parameter value from the rule configuration.
+        Deletes reputation overrides in bulk by id.
 
         Args:
-            name (str): The parameter name.
+            cb (BaseAPI): Reference to API object used to communicate with the server.
+            overrides (List): List if reputation override ids
+
+        Example:
+            >>>
+            [
+               "e9410b754ea011ebbfd0db2585a41b07"
+            ]
 
-        Returns:
-            Any: The parameter value, or None if there is no value.
         """
-        params = self._info['parameters']
-        return params.get(name, None)
+        url = cls.urlobject.format(cb.credentials.org_key) + "/_delete"
+        resp = cb.post_object(url, overrides)
+        if resp.status_code not in (200, 204):
+            try:
+                result = json.loads(resp.text)[0]
+            except Exception:
+                result = resp.text
+            raise ServerError(resp.status_code, "Did not delete overrides.", result=result, uri=url)
+
+        return resp.json()
+
 
-    def set_parameter(self, name, value):
+class ReputationOverrideQuery(BaseQuery, QueryBuilderSupportMixin, IterableQueryMixin, AsyncQueryMixin):
+    """Represents a query that is used to locate ReputationOverride objects."""
+    VALID_DIRECTIONS = ["ASC", "DESC", "asc", "desc"]
+
+    def __init__(self, doc_class, cb):
         """
-        Sets a parameter value into the rule configuration.
+        Initialize the ReputationOverrideQuery.
 
         Args:
-            name (str): The parameter name.
-            value (Any): The new value to be set.
+            doc_class (class): The model class that will be returned by this query.
+            cb (BaseAPI): Reference to API object used to communicate with the server.
         """
-        params = self._info['parameters']
-        old_value = params.get(name, None)
-        if old_value != value:
-            if 'parameters' not in self._dirty_attributes:
-                self._dirty_attributes['parameters'] = params
-                new_params = copy.deepcopy(params)
-            else:
-                new_params = params
-            new_params[name] = value
-            self._info['parameters'] = new_params
+        self._doc_class = doc_class
+        self._cb = cb
+        self._count_valid = False
+        super(ReputationOverrideQuery, self).__init__()
+
+        self._query_builder = QueryBuilder()
+        self._criteria = {}
+        self._sortcriteria = {}
 
-    def validate(self):
-        """
-        Validates this rule configuration against its constraints.
+    def set_override_list(self, override_list):
+        """Sets the override_list criteria filter.
 
-        Raises:
-            InvalidObjectError: If the rule object is not valid.
+        Arguments:
+            override_list (str): Override List to filter on.
+
+        Returns:
+            The ReputationOverrideQuery with specified override_list.
         """
-        super(PolicyRuleConfig, self).validate()
+        if not isinstance(override_list, str) and override_list in ["WHITE_LIST", "BLACK_LIST"]:
+            raise ApiError("Invalid override_list must be one of WHITE_LIST, BLACK_LIST")
+        self._criteria["override_list"] = override_list
+        return self
 
-        if self._parent is not None:
-            # set high-level fields
-            valid_configs = self._parent.valid_rule_configs()
-            data = valid_configs.get(self._model_unique_id, {})
-            self._info.update(data)
-            if 'inherited_from' not in self._info:
-                self._info['inherited_from'] = 'psc:region'
-
-        # validate parameters
-        if self._parent is None:
-            parameter_validations = self._cb.get_policy_ruleconfig_parameter_schema(self._model_unique_id)
-        else:
-            parameter_validations = self._parent.get_ruleconfig_parameter_schema(self._model_unique_id)
-        my_parameters = self._info.get('parameters', {})
-        try:
-            jsonschema.validate(instance=my_parameters, schema=parameter_validations)
-        except jsonschema.ValidationError as e:
-            raise InvalidObjectError(f"parameter error: {e.message}", e)
-        except jsonschema.exceptions.SchemaError as e:
-            raise ApiError(f"internal error: {e.message}", e)
-        self._info['parameters'] = my_parameters
-
-
-class CorePreventionRuleConfig(PolicyRuleConfig):
-    """
-    Represents a core prevention rule configuration in the policy.
-
-    Create one of these objects, associating it with a Policy, and set its properties, then call its save() method to
-    add the rule configuration to the policy. This requires the org.policies(UPDATE) permission.
-
-    To update a CorePreventionRuleConfig, change the values of its property fields, then call its save() method.  This
-    requires the org.policies(UPDATE) permission.
-
-    To delete an existing CorePreventionRuleConfig, call its delete() method. This requires the org.policies(DELETE)
-    permission.
+    def set_override_type(self, override_type):
+        """Sets the override_type criteria filter.
 
-    """
-    swagger_meta_file = "platform/models/policy_ruleconfig.yaml"
+        Arguments:
+            override_type (str): Override List to filter on.
 
-    def __init__(self, cb, parent, model_unique_id=None, initial_data=None, force_init=False, full_doc=False):
+        Returns:
+            The ReputationOverrideQuery with specified override_type.
         """
-        Initialize the CorePreventionRuleConfig object.
+        if not isinstance(override_type, str) and override_type in ["SHA256", "CERT", "IT_TOOL"]:
+            raise ApiError("Invalid override_type must be one of SHA256, CERT, IT_TOOL")
+        self._criteria["override_type"] = override_type
+        return self
 
-        Args:
-            cb (BaseAPI): Reference to API object used to communicate with the server.
-            parent (Policy): The "parent" policy of this rule configuration.
-            model_unique_id (str): ID of the rule configuration.
-            initial_data (dict): Initial data used to populate the rule configuration.
-            force_init (bool): If True, forces the object to be refreshed after constructing.  Default False.
-            full_doc (bool): If True, object is considered "fully" initialized. Default False.
+    def sort_by(self, key, direction="ASC"):
         """
-        super(CorePreventionRuleConfig, self).__init__(cb, parent, model_unique_id, initial_data, force_init, full_doc)
+        Sets the sorting behavior on a query's results.
 
-    def _base_url(self):
-        """
-        Calculates the base URL for these particular rule configs, including the org key and the parent policy ID.
+        Example:
+            >>> cb.select(ReputationOverride).sort_by("create_time")
+
+        Args:
+            key (str): The key in the schema to sort by.
+            direction (str): The sort order, either "ASC" or "DESC".
 
         Returns:
-            str: The base URL for these particular rule configs.
+            ReputationOverrideQuery: This instance.
 
         Raises:
-            InvalidObjectError: If the rule config object is unparented.
+            ApiError: If an invalid direction value is passed.
         """
-        return super(CorePreventionRuleConfig, self)._base_url() + "/core_prevention"
+        if direction not in ReputationOverrideQuery.VALID_DIRECTIONS:
+            raise ApiError("invalid sort direction specified")
+        self._sortcriteria = {"sort_field": key, "sort_order": direction}
+        return self
 
-    def _refresh(self):
+    def _build_request(self, from_row, max_rows):
         """
-        Refreshes the rule configuration object from the server.
+        Creates the request body for an API call.
 
-        Required Permissions:
-            org.policies (READ)
+        Args:
+            from_row (int): The row to start the query at.
+            max_rows (int): The maximum number of rows to be returned.
 
         Returns:
-            bool: True if the refresh was successful.
+            dict: The complete request body.
+        """
+        request = {
+            "criteria": self._criteria,
+            "query": self._query_builder._collapse()
+        }
+        if from_row > 0:
+            request["start"] = from_row
+        if max_rows >= 0:
+            request["rows"] = max_rows
+        if self._sortcriteria != {}:
+            request.update(self._sortcriteria)
+        return request
 
-        Raises:
-            InvalidObjectError: If the object is unparented or its ID is invalid.
+    def _build_url(self, tail_end):
         """
-        return_data = self._cb.get_object(self._base_url())
-        ruleconfig_data = [d for d in return_data.get("results", []) if d.get("id", "") == self._model_unique_id]
-        if ruleconfig_data:
-            self._info = ruleconfig_data[0]
-        else:
-            raise InvalidObjectError(f"invalid core prevention ID: {self._model_unique_id}")
-        return True
+        Creates the URL to be used for an API call.
 
-    def _update_ruleconfig(self):
-        """Perform the internal update of the rule configuration object."""
-        body = [{"id": self.id, "parameters": self.parameters}]
-        self._cb.put_object(self._base_url(), body)
+        Args:
+            tail_end (str): String to be appended to the end of the generated URL.
 
-    def _delete_ruleconfig(self):
-        """Perform the internal delete of the rule configuration object."""
-        self._cb.delete_object(self._base_url() + f"/{self.id}")
-        self._info["parameters"] = copy.deepcopy({"WindowsAssignmentMode": "BLOCK"})  # mirror server side
+        Returns:
+            str: The complete URL.
+        """
+        url = self._doc_class.urlobject.format(self._cb.credentials.org_key) + tail_end
+        return url
 
-    def get_assignment_mode(self):
+    def _count(self):
         """
-        Returns the assignment mode of this core prevention rule configuration.
+        Returns the number of results from the run of this query.
 
         Returns:
-            str: The assignment mode, either "REPORT" or "BLOCK".
+            int: The number of results from the run of this query.
         """
-        return self.get_parameter("WindowsAssignmentMode")
+        if self._count_valid:
+            return self._total_results
 
-    def set_assignment_mode(self, mode):
+        url = self._build_url("/_search")
+        request = self._build_request(0, -1)
+        resp = self._cb.post_object(url, body=request)
+        result = resp.json()
+
+        self._total_results = result["num_found"]
+        self._count_valid = True
+
+        return self._total_results
+
+    def _perform_query(self, from_row=0, max_rows=-1):
         """
-        Sets the assignment mode of this core prevention rule configuration.
+        Performs the query and returns the results of the query in an iterable fashion.
 
         Args:
-            mode (str): The new mode to set, either "REPORT" or "BLOCK". The default is "BLOCK".
+            from_row (int): The row to start the query at (default 0).
+            max_rows (int): The maximum number of rows to be returned (default -1, meaning "all").
+
+        Returns:
+            Iterable: The iterated query.
+        """
+        url = self._build_url("/_search")
+        current = from_row
+        numrows = 0
+        still_querying = True
+        while still_querying:
+            request = self._build_request(current, max_rows)
+            resp = self._cb.post_object(url, body=request)
+            result = resp.json()
+
+            self._total_results = result["num_found"]
+            self._count_valid = True
+
+            results = result.get("results", [])
+            for item in results:
+                yield self._doc_class(self._cb, item["id"], item)
+                current += 1
+                numrows += 1
+
+                if max_rows > 0 and numrows == max_rows:
+                    still_querying = False
+                    break
+
+            if current >= self._total_results:
+                break
+
+    def _run_async_query(self, context):
+        """
+        Executed in the background to run an asynchronous query.
+
+        Args:
+            context (object): Not used, always None.
+
+        Returns:
+            list: Result of the async query, which is then returned by the future.
         """
-        if mode not in ("REPORT", "BLOCK"):
-            raise ApiError(f"invalid assignment mode: {mode}")
-        self.set_parameter("WindowsAssignmentMode", mode)
+        url = self._build_url("/_search")
+        request = self._build_request(0, -1)
+        resp = self._cb.post_object(url, body=request)
+        result = resp.json()
+        self._total_results = result["num_found"]
+        self._count_valid = True
+        results = result.get("results", [])
+        return [self._doc_class(self._cb, item["id"], item) for item in results]
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/processes.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/processes.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/reputation.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/sensor_lifecycle.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,320 +7,269 @@
 # *
 # * DISCLAIMER. THIS PROGRAM IS PROVIDED TO YOU "AS IS" WITHOUT
 # * WARRANTIES OR CONDITIONS OF ANY KIND, WHETHER ORAL OR WRITTEN,
 # * EXPRESS OR IMPLIED. THE AUTHOR SPECIFICALLY DISCLAIMS ANY IMPLIED
 # * WARRANTIES OR CONDITIONS OF MERCHANTABILITY, SATISFACTORY QUALITY,
 # * NON-INFRINGEMENT AND FITNESS FOR A PARTICULAR PURPOSE.
 
-"""Model and Query Classes for Reputation"""
+"""Sensor Lifecycle Management for Workloads"""
 
-from cbc_sdk.errors import ApiError, ServerError
-from cbc_sdk.platform import PlatformModel
-from cbc_sdk.base import (BaseQuery, QueryBuilder, QueryBuilderSupportMixin,
+from cbc_sdk.errors import ApiError
+from cbc_sdk.base import (UnrefreshableModel, BaseQuery, CriteriaBuilderSupportMixin,
                           IterableQueryMixin, AsyncQueryMixin)
 
-import time
+import logging
 import json
 
-""""Reputation Override Models"""
+log = logging.getLogger(__name__)
 
+_GET_SENSOR_KIT_TRANS_TABLE = {'sensor_url_request': {'filename': 'sensor.json', 'type': 'application/json'},
+                               'configParams': {'filename': 'config.ini', 'type': 'text/plain'}}
+_SENSOR_INSTALL_TRANS_TABLE = {'action_type': {},
+                               'install_request': {'filename': 'request.json', 'type': 'application/json'},
+                               'file': {'filename': 'config.ini', 'type': 'text/plain'}}
 
-class ReputationOverride(PlatformModel):
-    """Represents a reputation override."""
-    urlobject = "/appservices/v6/orgs/{0}/reputations/overrides"
-    urlobject_single = "/appservices/v6/orgs/{0}/reputations/overrides/{1}"
-    primary_key = "id"
-    swagger_meta_file = "platform/models/reputation_override.yaml"
-    _is_deleted = False
 
-    def __init__(self, cb, model_unique_id, initial_data=None):
+class SensorKit(UnrefreshableModel):
+    """Represents the information about a sensor, including installation file URLs."""
+    swagger_meta_file = "workload/models/sensorKit.yaml"
+
+    VALID_DEVICE_TYPES = ["WINDOWS", "LINUX", "MAC"]
+    VALID_ARCHITECTURES = ["32", "64", "OTHER"]
+    VALID_TYPES = ["WINDOWS", "MAC", "RHEL", "UBUNTU", "SUSE", "AMAZON_LINUX"]
+    COMPUTE_RESOURCE_MAP = {'SLES': 'SUSE', 'CENTOS': 'RHEL', 'ORACLE': 'RHEL'}
+
+    def __init__(self, cb, initial_data=None):
         """
-        Initialize the ReputationOverride object.
+        Initialize the SensorKit object.
 
         Args:
             cb (BaseAPI): Reference to API object used to communicate with the server.
-            model_unique_id (str): ID of the alert represented.
-            initial_data (dict): Initial data used to populate the alert.
+            initial_data (dict): Initial data used to populate the sensor kit data.
         """
-        super(ReputationOverride, self).__init__(cb, model_unique_id, initial_data, full_doc=True)
-        if model_unique_id is not None and initial_data is None:
-            self._refresh()
+        super(SensorKit, self).__init__(cb, None, initial_data)
+        self._full_init = (initial_data is not None and not initial_data.get('_pseudo', False))
 
     @classmethod
-    def _query_implementation(cls, cb, **kwargs):
+    def from_type(cls, cb, device_type, architecture, sensor_type, version):
         """
-        Returns the appropriate query object for the ReputationOverride.
+        Helper method used to create a temporary SensorKit object from its four components.
+
+        This method CANNOT be used to create an object that will be persisted to the server.
 
         Args:
             cb (BaseAPI): Reference to API object used to communicate with the server.
-            **kwargs (dict): Not used, retained for compatibility.
+            device_type (str): Device type to be used.  Valid values are "WINDOWS", "LINUX", and "MAC".
+            architecture (str): Architecture to be used.  Valid values are "32", "64", and "OTHER".
+            sensor_type (str): Sensor type to be used.  Valid values are "WINDOWS", "MAC", "RHEL", "UBUNTU", "SUSE",
+                               and "AMAZON_LINUX".
+            version (str): Sensor version number to be used.
 
         Returns:
-            ReputationOverrideQuery: The query object for this alert type.
-        """
-        return ReputationOverrideQuery(cls, cb)
-
-    def _refresh(self):
-        """
-        Rereads the device data from the server.
+            SensorType: A SensorType object with those specified values.
 
-        Returns:
-            bool: True if refresh was successful, False if not.
+        Raises:
+            ApiError: If an invalid value was used for one of the three limited values.
         """
-        if self._is_deleted:
-            raise ApiError("Cannot refresh a deleted ReputationOverride")
-        url = self.urlobject_single.format(self._cb.credentials.org_key, self._model_unique_id)
-        resp = self._cb.get_object(url)
-        self._info = resp
-        self._last_refresh_time = time.time()
-        self._full_init = True
-        return True
-
-    def delete(self):
-        """Delete this object."""
-        if self._model_unique_id is None:
-            return
-
-        resp = self._cb.delete_object(self.urlobject_single.format(self._cb.credentials.org_key, self._model_unique_id))
-        if resp.status_code not in (200, 204):
-            try:
-                message = json.loads(resp.text)[0]
-            except Exception:
-                message = resp.text
-            raise ServerError(resp.status_code, message, result="Did not delete {0:s}.".format(str(self)))
-        self._is_deleted = True
+        sensor_type_data = {}
+        if device_type is not None:
+            if device_type not in SensorKit.VALID_DEVICE_TYPES:
+                raise ApiError("invalid device_type specified for SensorKit")
+            sensor_type_data['device_type'] = device_type
+        if architecture is not None:
+            if architecture not in SensorKit.VALID_ARCHITECTURES:
+                raise ApiError("invalid architecture specified for SensorKit")
+            sensor_type_data['architecture'] = architecture
+        if sensor_type is not None:
+            if sensor_type not in SensorKit.VALID_TYPES:
+                raise ApiError("invalid type specified for SensorKit")
+            sensor_type_data['type'] = sensor_type
+        if version is not None:
+            sensor_type_data['version'] = version
+        return SensorKit(cb, {'sensor_type': sensor_type_data, '_pseudo': True})
 
     @classmethod
-    def create(cls, cb, initial_data):
+    def get_config_template(cls, cb):
         """
-        Returns all vendors and products that have been seen for the organization.
+        Retrieve the sample config.ini file with the properties populated from the server.
 
         Args:
             cb (BaseAPI): Reference to API object used to communicate with the server.
-            initial_data (Object): The initial data for a ReputationOverride
-
-        Example:
-            >>>
-            {
-                "description": "Banned as known malware",
-                "override_list": "BLACK_LIST",
-                "override_type": "SHA256",
-                "sha256_hash": "dd191a5b23df92e13a8852291f9fb5ed594b76a28a5a464418442584afd1e048",
-                "filename": "foo.exe"
-            }
 
         Returns:
-            ReputationOverride: The created ReputationOverride object based on the specified properties
-
+            str: Text of the sample configuration file.
         """
-        resp = cb.post_object(cls.urlobject.format(cb.credentials.org_key), body=initial_data)
-        resp_json = resp.json()
-        return cls(cb, resp_json["id"], resp_json)
+        url = "/lcm/v1/orgs/{0}/sensor/config_template".format(cb.credentials.org_key)
+        return cb.get_raw_data(url)
 
     @classmethod
-    def bulk_delete(cls, cb, overrides):
+    def _query_implementation(cls, cb, **kwargs):
         """
-        Deletes reputation overrides in bulk by id.
+        Returns the appropriate query object for this object type.
 
         Args:
             cb (BaseAPI): Reference to API object used to communicate with the server.
-            overrides (List): List if reputation override ids
-
-        Example:
-            >>>
-            [
-               "e9410b754ea011ebbfd0db2585a41b07"
-            ]
+            **kwargs (dict): Not used, retained for compatibility.
 
+        Returns:
+            USBDeviceQuery: The query object for this alert type.
         """
-        resp = cb.post_object(cls.urlobject.format(cb.credentials.org_key) + "/_delete", overrides)
-        if resp.status_code not in (200, 204):
-            try:
-                message = json.loads(resp.text)[0]
-            except Exception:
-                message = resp.text
-            raise ServerError(resp.status_code, message, result="Did not delete overrides.")
-
-        return resp.json()
+        return SensorKitQuery(cls, cb)
 
 
-class ReputationOverrideQuery(BaseQuery, QueryBuilderSupportMixin, IterableQueryMixin, AsyncQueryMixin):
-    """Represents a query that is used to locate ReputationOverride objects."""
-    VALID_DIRECTIONS = ["ASC", "DESC", "asc", "desc"]
+class SensorKitQuery(BaseQuery, CriteriaBuilderSupportMixin, IterableQueryMixin, AsyncQueryMixin):
+    """Query class used to read in SensorKit objects."""
 
     def __init__(self, doc_class, cb):
         """
-        Initialize the ReputationOverrideQuery.
+        Initialize the SensorKitQuery.
 
         Args:
             doc_class (class): The model class that will be returned by this query.
             cb (BaseAPI): Reference to API object used to communicate with the server.
         """
         self._doc_class = doc_class
         self._cb = cb
         self._count_valid = False
-        super(ReputationOverrideQuery, self).__init__()
-
-        self._query_builder = QueryBuilder()
+        super(BaseQuery, self).__init__()
         self._criteria = {}
-        self._sortcriteria = {}
-
-    def set_override_list(self, override_list):
-        """Sets the override_list criteria filter.
-
-        Arguments:
-            override_list (str): Override List to filter on.
+        self._expires = None
+        self._config_params = None
+        self._total_results = 0
 
-        Returns:
-            The ReputationOverrideQuery with specified override_list.
+    def add_sensor_kit_type(self, skit=None, **kwargs):
         """
-        if not isinstance(override_list, str) and override_list in ["WHITE_LIST", "BLACK_LIST"]:
-            raise ApiError("Invalid override_list must be one of WHITE_LIST, BLACK_LIST")
-        self._criteria["override_list"] = override_list
-        return self
-
-    def set_override_type(self, override_type):
-        """Sets the override_type criteria filter.
+        Add a sensor kit type to the request.
 
-        Arguments:
-            override_type (str): Override List to filter on.
+        Args:
+            skit (SensorKit): The sensor kit type to be added to the request.
+            **kwargs (dict): If skit is None, the keyword arguments 'device_type', 'architecture', 'sensor_type',
+                             and 'version' are used to create the sensor kit type to be added.
 
         Returns:
-            The ReputationOverrideQuery with specified override_type.
-        """
-        if not isinstance(override_type, str) and override_type in ["SHA256", "CERT", "IT_TOOL"]:
-            raise ApiError("Invalid override_type must be one of SHA256, CERT, IT_TOOL")
-        self._criteria["override_type"] = override_type
+            SensorKitQuery: Reference to this object.
+        """
+        my_skit = skit
+        if my_skit is None:
+            my_skit = SensorKit.from_type(self._cb, kwargs.pop('device_type', None), kwargs.pop('architecture', None),
+                                          kwargs.pop('sensor_type', None), kwargs.pop('version', None))
+        self._update_criteria('sensor_types', [my_skit.sensor_type])
         return self
 
-    def sort_by(self, key, direction="ASC"):
+    def expires(self, expiration_date_time):
         """
-        Sets the sorting behavior on a query's results.
-
-        Example:
-            >>> cb.select(ReputationOverride).sort_by("create_time")
+        Sets the expiration date and time for the sensor kit query request.
 
         Args:
-            key (str): The key in the schema to sort by.
-            direction (str): The sort order, either "ASC" or "DESC".
+            expiration_date_time (str): The time at which the sensor download link will expire, expressed
+                                        as ISO 8601 UTC.
 
         Returns:
-            ReputationOverrideQuery: This instance.
-
-        Raises:
-            ApiError: If an invalid direction value is passed.
+            SensorKitQuery: Reference to this object.
         """
-        if direction not in ReputationOverrideQuery.VALID_DIRECTIONS:
-            raise ApiError("invalid sort direction specified")
-        self._sortcriteria = {"sort_field": key, "sort_order": direction}
+        self._expires = expiration_date_time
         return self
 
-    def _build_request(self, from_row, max_rows):
+    def config_params(self, params):
         """
-        Creates the request body for an API call.
+        Sets the configuration parameters for the sensor kit query request.
 
         Args:
-            from_row (int): The row to start the query at.
-            max_rows (int): The maximum number of rows to be returned.
+            params (str): The text of a config.ini file with a list of sensor properties to configure
+                          on installation.
 
         Returns:
-            dict: The complete request body.
+            SensorKitQuery: Reference to this object.
         """
-        request = {
-            "criteria": self._criteria,
-            "query": self._query_builder._collapse()
-        }
-        if from_row > 0:
-            request["start"] = from_row
-        if max_rows >= 0:
-            request["rows"] = max_rows
-        if self._sortcriteria != {}:
-            request.update(self._sortcriteria)
-        return request
+        self._config_params = params
+        return self
 
-    def _build_url(self, tail_end):
+    def _submit_query(self):
         """
-        Creates the URL to be used for an API call.
-
-        Args:
-            tail_end (str): String to be appended to the end of the generated URL.
+        Submits the current query to the server and returns the list of sensor kits.
 
         Returns:
-            str: The complete URL.
+            list: The list of sensor kits, each one expressed as a dict.
         """
-        url = self._doc_class.urlobject.format(self._cb.credentials.org_key) + tail_end
-        return url
+        url = "/lcm/v1/orgs/{0}/sensor/_download".format(self._cb.credentials.org_key)
+        request = {'sensor_types': self._criteria['sensor_types'], 'expires_at': self._expires}
+        resp = self._cb.post_multipart(url, _GET_SENSOR_KIT_TRANS_TABLE, sensor_url_request=json.dumps(request),
+                                       configParams=self._config_params)
+        result = resp.json()
+        return result.get('sensor_infos', [])
 
     def _count(self):
         """
         Returns the number of results from the run of this query.
 
         Returns:
             int: The number of results from the run of this query.
         """
         if self._count_valid:
             return self._total_results
 
-        url = self._build_url("/_search")
-        request = self._build_request(0, -1)
-        resp = self._cb.post_object(url, body=request)
-        result = resp.json()
-
-        self._total_results = result["num_found"]
+        self._total_results = len(self._submit_query())
         self._count_valid = True
 
         return self._total_results
 
     def _perform_query(self, from_row=0, max_rows=-1):
         """
         Performs the query and returns the results of the query in an iterable fashion.
 
         Args:
-            from_row (int): The row to start the query at (default 0).
-            max_rows (int): The maximum number of rows to be returned (default -1, meaning "all").
+            from_row (int): Not used; retained for compatibility.
+            max_rows (int): Not used; retained for compatibility.
 
         Returns:
             Iterable: The iterated query.
         """
-        url = self._build_url("/_search")
-        current = from_row
-        numrows = 0
-        still_querying = True
-        while still_querying:
-            request = self._build_request(current, max_rows)
-            resp = self._cb.post_object(url, body=request)
-            result = resp.json()
-
-            self._total_results = result["num_found"]
-            self._count_valid = True
-
-            results = result.get("results", [])
-            for item in results:
-                yield self._doc_class(self._cb, item["id"], item)
-                current += 1
-                numrows += 1
-
-                if max_rows > 0 and numrows == max_rows:
-                    still_querying = False
-                    break
-
-            if current >= self._total_results:
-                break
+        items_list = self._submit_query()
+        self._total_results = len(items_list)
+        self._count_valid = True
+        for item in items_list:
+            yield self._doc_class(self._cb, item)
 
     def _run_async_query(self, context):
         """
         Executed in the background to run an asynchronous query.
 
         Args:
             context (object): Not used, always None.
 
         Returns:
             list: Result of the async query, which is then returned by the future.
         """
-        url = self._build_url("/_search")
-        request = self._build_request(0, -1)
-        resp = self._cb.post_object(url, body=request)
-        result = resp.json()
-        self._total_results = result["num_found"]
+        items_list = self._submit_query()
+        self._total_results = len(items_list)
         self._count_valid = True
-        results = result.get("results", [])
-        return [self._doc_class(self._cb, item["id"], item) for item in results]
+        return [self._doc_class(self._cb, item) for item in items_list]
+
+
+def _do_sensor_install_request(cb, compute_resources, sensor_kits, config_file):
+    """
+    Internal helper function that performs a sensor installation request.
+
+    Not to be called directly by user code; use methods on the ComputeResource object to access this functionality.
+
+    Args:
+        cb (BaseAPI): Reference to API object used to communicate with the server.
+        compute_resources (list): A list of dicts containing the keys 'resource_manager_id' and 'compute_resource_id',
+                                  used to specify the compute resources to install on.
+        sensor_kits (list): A list of SensorKit objects used to specify sensor types to choose from in installation.
+        config_file (str): The text of a config.ini file with a list of sensor properties to configure on installation.
+
+    Returns:
+        dict: A dict with two members, 'type' and 'code', indicating the status of the installation.
+    """
+    request = {
+        'compute_resources': compute_resources,
+        'sensor_types': [kit.sensor_type for kit in sensor_kits]
+    }
+
+    url = "/lcm/v1/orgs/{0}/workloads/actions".format(cb.credentials.org_key)
+    return_data = cb.post_multipart(url,
+                                    _SENSOR_INSTALL_TRANS_TABLE,
+                                    action_type='INSTALL',
+                                    install_request=json.dumps(request),
+                                    file=config_file)
+    return return_data.json()
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/users.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             password has been set.
         """
         url = User.urlobject.format(cb.credentials.org_key)
         result = cb.post_object(url, user_data)
         resp = result.json()
         if resp['registration_status'] != 'SUCCESS':
             raise ServerError(500, f"registration return was unsuccessful: {resp['registration_status']} - "
-                                   f"{resp['message']}")
+                                   f"{resp['message']}", uri=url)
         # N.B.: new user is not "findable" until activated and initial password set
 
     def _refresh(self):
         """
         Rereads the user data from the server.
 
         Returns:
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/platform/vulnerability_assessment.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/platform/vulnerability_assessment.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/rest_api.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/rest_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,16 @@
         url = "/appservices/v6/orgs/{0}/device_actions".format(self.credentials.org_key)
         resp = self.post_object(url, body=request)
         if resp.status_code == 200:
             return resp.json()
         elif resp.status_code == 204:
             return None
         else:
-            raise ServerError(error_code=resp.status_code, message="Device action error: {0}".format(resp.content))
+            raise ServerError(error_code=resp.status_code, message="Device action error: {0}".format(resp.content),
+                              uri=url)
 
     def _device_action(self, device_ids, action_type, options=None):
         """
         Executes a device action on multiple device IDs.
 
         Args:
             device_ids (list): The list of device IDs to execute the action on.
@@ -505,9 +506,9 @@
 
         Raises:
             InvalidObjectError: If the rule configuration ID is not valid.
         """
         url = f"/policyservice/v1/orgs/{self.credentials.org_key}/rule_configs/{ruleconfig_id}/parameters/schema"
         try:
             return self.get_object(url)
-        except ServerError:
-            raise InvalidObjectError(f"invalid rule config ID {ruleconfig_id}")
+        except ServerError as e:
+            raise InvalidObjectError(f"invalid rule config ID {ruleconfig_id}", original_exception=e)
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/utils.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/winerror.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/winerror.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/computeResource.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/computeResource.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/deviceVulnerabilitySummary.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/deviceVulnerabilitySummary.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/sensorKit.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/sensorKit.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/vulnerability.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/vulnerability.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/vulnerabilityAssetView.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/vulnerabilityAssetView.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/models/vulnerabilityOrgSummary.yaml` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/models/vulnerabilityOrgSummary.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/nsx_remediation.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/nsx_remediation.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         request_body = {'device_ids': real_device_ids, 'action_type': 'NSX_REMEDIATION',
                         'options': {'toggle': 'ON' if set_tag else 'OFF', 'tag': tag}}
         url = "/applianceservice/v1/orgs/{}/device_actions".format(cb.credentials.org_key)
         response = cb.post_object(url, body=request_body)
         if response.status_code != 201:
             raise ServerError(response.status_code,
-                              f"could not start remediation request, error code {response.status_code}")
+                              f"could not start remediation request, error code {response.status_code}", uri=url)
         job_ids = response.json().get('job_ids', [])
         if job_ids:
             return NSXRemediationJob(cb, job_ids)
         raise NSXJobError("No jobs started")
 
     def _poll_status(self):
         """
```

### Comparing `carbon-black-cloud-sdk-1.4.2/src/cbc_sdk/workload/vm_workloads_search.py` & `carbon-black-cloud-sdk-1.4.3/src/cbc_sdk/workload/vm_workloads_search.py`

 * *Files identical despite different names*

