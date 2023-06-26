# Comparing `tmp/taegis-sdk-python-1.0.0a9.tar.gz` & `tmp/taegis-sdk-python-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis-sdk-python-1.0.0a9.tar", last modified: Thu May  4 18:48:20 2023, max compression
+gzip compressed data, was "taegis-sdk-python-1.0.0rc1.tar", last modified: Mon Jun 26 14:41:11 2023, max compression
```

## Comparing `taegis-sdk-python-1.0.0a9.tar` & `taegis-sdk-python-1.0.0rc1.tar`

### file list

```diff
@@ -1,196 +1,202 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.536567 taegis-sdk-python-1.0.0a9/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5757 2023-05-04 18:48:20.536567 taegis-sdk-python-1.0.0a9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5320 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/README.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 18:48:20.536567 taegis-sdk-python-1.0.0a9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.512569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8552 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10956 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.513569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    12477 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.514569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2370 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.515569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2560 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.516569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3851 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6644 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    78106 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.516569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6326 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14905 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.517569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9259 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    12852 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25353 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.518569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3040 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.519569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3843 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.520568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15774 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    22563 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    30929 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.520568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4105 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6219 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.521568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3145 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.522568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8546 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.523568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3949 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5436 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.524568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1769 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      851 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.524568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4228 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.525568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2726 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8988 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.526568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12950 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10408 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24248 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.527568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22054 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    27703 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    39186 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.528568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11536 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7165 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    38776 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.528568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9242 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.529568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.530568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6809 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2413 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.531568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5874 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5229 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    12489 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.531568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14158 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16048 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    22172 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.532568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.533568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11568 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5864 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    31540 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.534567 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3394 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    13732 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    53278 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.535567 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4086 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3856 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7946 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.535567 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11509 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6309 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25501 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     5811 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.513569 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5757 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7717 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.840248 taegis-sdk-python-1.0.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6231 2023-06-26 14:41:11.840248 taegis-sdk-python-1.0.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5793 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 14:41:11.840248 taegis-sdk-python-1.0.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.808248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8618 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10895 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.810248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    13384 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.811248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.812248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.813248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3900 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    78106 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.814248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6375 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14954 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.815248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12807 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25755 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.816248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10314 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.817248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.818248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15823 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    22760 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    30929 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.819248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4946 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.820248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.821248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8546 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.822248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7674 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.823248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.824248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.825248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9191 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.826248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12999 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10457 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24248 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.827248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22228 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    28008 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    37546 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.828248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12204 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7214 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    41182 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.829248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.830248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.831248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6858 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.832248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5923 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5961 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12949 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.833248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6660 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13046 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.834248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14207 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16097 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    22172 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.835248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.836248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11617 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5913 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    31658 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.837248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3443 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13781 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    53278 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.838248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7993 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.839248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11558 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7075 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25732 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     6493 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.810248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6231 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7969 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis-sdk-python-1.0.0a9/LICENSE` & `taegis-sdk-python-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/PKG-INFO` & `taegis-sdk-python-1.0.0rc1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: taegis-sdk-python
-Version: 1.0.0a9
-Summary: Taegis Python SDK
-Home-page: https://github.com/secureworks/taegis-sdk-python
-Author: Secureworks
-Author-email: sdks@secureworks.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Taegis SDK for Python
 
 The Taegis SDK is a Python library for interfacing with the GraphQL APIs in Taegis.
 
 ## Prerequisites
 
 - Python 3.8 or higher.
@@ -241,7 +227,19 @@
             suspended
             total
         }
     }
 """
 result = service.investigations.execute(gql_query)
 ```
+
+### Deprecation Warnings
+
+Deprecated input fields, output fields and endpoints are set to log a warning.  For more information, see the [docs](docs/deprecation.md).
+
+Example:
+
+```
+GraphQL Query `allInvestigations` is deprecated: 'replaced by investigationsSearch'
+Output field `activity_logs` is deprecated: 'Not Supported - Use audit logs', removing from default output...
+Output field `assignee` is deprecated: 'No longer supported', removing from default output...
+```
```

### Comparing `taegis-sdk-python-1.0.0a9/README.md` & `taegis-sdk-python-1.0.0rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: taegis-sdk-python
+Version: 1.0.0rc1
+Summary: Taegis Python SDK
+Home-page: https://github.com/secureworks/taegis-sdk-python
+Author: Secureworks
+Author-email: sdks@secureworks.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Taegis SDK for Python
 
 The Taegis SDK is a Python library for interfacing with the GraphQL APIs in Taegis.
 
 ## Prerequisites
 
 - Python 3.8 or higher.
@@ -227,7 +241,19 @@
             suspended
             total
         }
     }
 """
 result = service.investigations.execute(gql_query)
 ```
+
+### Deprecation Warnings
+
+Deprecated input fields, output fields and endpoints are set to log a warning.  For more information, see the [docs](docs/deprecation.md).
+
+Example:
+
+```
+GraphQL Query `allInvestigations` is deprecated: 'replaced by investigationsSearch'
+Output field `activity_logs` is deprecated: 'Not Supported - Use audit logs', removing from default output...
+Output field `assignee` is deprecated: 'No longer supported', removing from default output...
+```
```

### Comparing `taegis-sdk-python-1.0.0a9/setup.py` & `taegis-sdk-python-1.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/_consts.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/authentication.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,17 @@
             comments=["Check client_id and client_secret credentials"],
         )
 
     return access_token
 
 
 def get_token_by_password_grant(
-    request_url: str, username: str
+    request_url: str,
+    username: str,
+    password: Optional[str] = None,
 ) -> str:  # pragma: no cover
     """Get an access token by username/password with mfa.
 
     Parameters
     ----------
     request_url : str
         Endpoint URL for Taegis environment
@@ -197,15 +199,16 @@
     Raises
     ------
     requests.HTTPError
         Any issue with retrieving token via HTTP
     """
     auth_uri = "/auth/api/v2/auth/token"
 
-    password = getpass("Password: ")
+    if not password:
+        password = getpass("Password: ")
 
     response = post(
         f"{request_url}{auth_uri}",
         json={"username": username, "password": password, "grant_type": "password"},
         timeout=300,
     )
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/config.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/config.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/errors.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/service_core.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/service_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,15 @@
         ]
 
         if self.service.tenant_id:
             subprotocols.append(f"x-tenant-context-{self.service.tenant_id}")
 
         transport = WebsocketsTransport(
             f"{self.wss_url}{self.gateway}",
-            headers={
-                "User-Agent": f"taegis_sdk_python/{__version__}",
-            },
+            headers=self.service.headers,
             subprotocols=subprotocols,
             connect_args={"max_size": None},
         )
         client = Client(transport=transport, fetch_schema_from_transport=True)
         return client
 
     def get_sync_schema(self) -> GraphQLSchema:
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This needs to be a generated file.  Need to make jinja template.
 """
-from typing import Dict, Optional
+from typing import Dict, Optional, Any
 
 from taegis_sdk_python._consts import TAEGIS_ENVIRONMENT_URLS
 from taegis_sdk_python._version import __version__
 from taegis_sdk_python.authentication import get_token
 from taegis_sdk_python.config import write_to_config
 from taegis_sdk_python.service_core import ServiceCore
 from taegis_sdk_python.services.access_points import AccessPointsService
@@ -30,14 +30,15 @@
 from taegis_sdk_python.services.exports import ExportsService
 from taegis_sdk_python.services.investigations import InvestigationsService
 from taegis_sdk_python.services.investigations2 import Investigations2Service
 from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
 from taegis_sdk_python.services.notebooks import NotebooksService
 from taegis_sdk_python.services.notifications import NotificationsService
 from taegis_sdk_python.services.preferences import PreferencesService
+from taegis_sdk_python.services.roadrunner import RoadrunnerService
 from taegis_sdk_python.services.rules import RulesService
 from taegis_sdk_python.services.sharelinks import SharelinksService
 from taegis_sdk_python.services.tenants import TenantsService
 from taegis_sdk_python.services.threat import ThreatService
 from taegis_sdk_python.services.trip import TripService
 from taegis_sdk_python.services.users import UsersService
 
@@ -50,28 +51,31 @@
     def __init__(
         self,
         *,
         environment: Optional[str] = None,
         tenant_id: Optional[str] = None,
         environments: Optional[Dict[str, str]] = None,
         gateway: Optional[str] = None,
+        extra_headers: Optional[Dict[str, Any]] = None,
     ):
         """
         GraphQLService
 
         Parameters
         ----------
         environment : Optional[str], optional
             Taegis Cluster environment identifier.
         tenant_id : Optional[str], optional
             Tenant ID, by default None
         environments : Optional[Dict[str, str]], optional
             Environments dictionary {"identifier": "url"}
         gateway : Optional[str], optional
             Default Taegis Gateway, can be overwritten by service
+        extra_headers: Optional[Dict[str, Any]], optional
+            Extra HTTP Headers to be included in API calls
 
         Raises
         ------
         ValueError
             environment must be charlie, delta, or echo
         """
         self._environments = environments or TAEGIS_ENVIRONMENT_URLS
@@ -79,14 +83,18 @@
 
         if self._environment not in self._environments:
             raise ValueError(f"environment must be in {self._environments.keys()}")
 
         self._tenant_id = tenant_id
         self._gateway = gateway or "/graphql"
         self._context_manager = {}
+        if not extra_headers:
+            self._extra_headers = {}
+        else:
+            self._extra_headers = extra_headers
 
         self._access_points = None
         self._agent = None
         self._alerts = None
         self._assets = None
         self._assets2 = None
         self._audits = None
@@ -102,14 +110,15 @@
         self._exports = None
         self._investigations = None
         self._investigations2 = None
         self._mitre_attack_info = None
         self._notebooks = None
         self._notifications = None
         self._preferences = None
+        self._roadrunner = None
         self._rules = None
         self._core = None
         self._sharelinks = None
         self._tenants = None
         self._threat = None
         self._trip = None
         self._users = None
@@ -163,28 +172,37 @@
 
     @property
     def output(self):
         """GraphQL Output."""
         return self._context_manager.get("output")
 
     @property
+    def extra_headers(self):
+        """Additional headers for API requests."""
+        extra_headers = self._extra_headers.copy()
+        extra_headers.update(self._context_manager.get("extra_headers", {}))
+        return extra_headers
+
+    @property
     def headers(self):
         """Taegis Headers."""
         headers = {
             "Accept": "application/json",
             "Authorization": f"Bearer {self.access_token}",
             "Content-Type": "application/json; charset=utf-8",
             "User-Agent": f"taegis_sdk_python/{__version__}",
             "apollographql-client-name": "taegis_sdk_python",
             "apollographql-client-version": __version__,
         }
 
         if self.tenant_id:
             headers["X-Tenant-Context"] = self.tenant_id
 
+        headers.update(self.extra_headers)
+
         return headers
 
     @property
     def access_points(self):
         """Access Points Service Endpoint."""
         if not self._access_points:
             self._access_points = AccessPointsService(self)
@@ -334,14 +352,21 @@
     def preferences(self):
         """Preferences Service Endpoint."""
         if not self._preferences:
             self._preferences = PreferencesService(self)
         return self._preferences
 
     @property
+    def roadrunner(self):
+        """Roadrunner Service Endpoint."""
+        if not self._roadrunner:
+            self._roadrunner = RoadrunnerService(self)
+        return self._roadrunner
+
+    @property
     def rules(self):
         """Rules Service Endpoint."""
         if not self._rules:
             self._rules = RulesService(self)
         return self._rules
 
     @property
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.access_points.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.access_points import AccessPointsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAccessPointsMutation:
     """Teagis Access_points Mutation operations."""
 
     def __init__(self, service: AccessPointsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.access_points.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.access_points import AccessPointsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAccessPointsQuery:
     """Teagis Access_points Query operations."""
 
     def __init__(self, service: AccessPointsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""AccessPoints Subscription."""
+"""Agent Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.access_points.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.agent.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.access_points import AccessPointsService
+    from taegis_sdk_python.services.agent import AgentService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKAccessPointsSubscription:
-    """Teagis Access_points Subscription operations."""
+class TaegisSDKAgentSubscription:
+    """Teagis Agent Subscription operations."""
 
-    def __init__(self, service: AccessPointsService):
+    def __init__(self, service: AgentService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/mutations.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.agent.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.agent import AgentService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAgentMutation:
     """Teagis Agent Mutation operations."""
 
     def __init__(self, service: AgentService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.agent.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.agent import AgentService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAgentQuery:
     """Teagis Agent Query operations."""
 
     def __init__(self, service: AgentService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Agent Subscription."""
+"""Trip Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.agent.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.trip.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.agent import AgentService
+    from taegis_sdk_python.services.trip import TripService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKAgentSubscription:
-    """Teagis Agent Subscription operations."""
+class TaegisSDKTripSubscription:
+    """Teagis Trip Subscription operations."""
 
-    def __init__(self, service: AgentService):
+    def __init__(self, service: TripService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.alerts.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.alerts import AlertsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAlertsMutation:
     """Teagis Alerts Mutation operations."""
 
     def __init__(self, service: AlertsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.alerts.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.alerts import AlertsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAlertsQuery:
     """Teagis Alerts Query operations."""
 
     def __init__(self, service: AlertsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.alerts.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.alerts import AlertsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAlertsSubscription:
     """Teagis Alerts Subscription operations."""
 
     def __init__(self, service: AlertsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.assets.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.assets import AssetsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAssetsMutation:
     """Teagis Assets Mutation operations."""
 
     def __init__(self, service: AssetsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.assets.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.assets import AssetsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAssetsQuery:
     """Teagis Assets Query operations."""
 
     def __init__(self, service: AssetsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Assets Subscription."""
+"""Assets2 Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.assets.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.assets2.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.assets import AssetsService
+    from taegis_sdk_python.services.assets2 import Assets2Service
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKAssetsSubscription:
-    """Teagis Assets Subscription operations."""
+class TaegisSDKAssets2Subscription:
+    """Teagis Assets2 Subscription operations."""
 
-    def __init__(self, service: AssetsService):
+    def __init__(self, service: Assets2Service):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.assets2.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.assets2 import Assets2Service
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAssets2Mutation:
     """Teagis Assets2 Mutation operations."""
 
     def __init__(self, service: Assets2Service):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.assets2.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.assets2 import Assets2Service
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAssets2Query:
     """Teagis Assets2 Query operations."""
 
     def __init__(self, service: Assets2Service):
         self.service = service
 
@@ -322,15 +324,11 @@
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for query assetDeadPeriod")
 
     def subject_can_isolate(self) -> CanIsolateResponse:
         """Returns whether a subject can isolate an asset for the current tenant context."""
         endpoint = "subjectCanIsolate"
 
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={},
-            output=build_output_string(CanIsolateResponse),
-        )
+        result = self.service.execute_query(endpoint=endpoint, variables={}, output="")
         if result.get(endpoint) is not None:
-            return CanIsolateResponse.from_dict(result.get(endpoint))
+            return CanIsolateResponse(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query subjectCanIsolate")
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Assets2 Subscription."""
+"""Tenants Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.assets2.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.tenants.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.assets2 import Assets2Service
+    from taegis_sdk_python.services.tenants import TenantsService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKAssets2Subscription:
-    """Teagis Assets2 Subscription operations."""
+class TaegisSDKTenantsSubscription:
+    """Teagis Tenants Subscription operations."""
 
-    def __init__(self, service: Assets2Service):
+    def __init__(self, service: TenantsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     SENSOR_VERSION_DESC = "sensor_version_desc"
     HOSTNAME_ASC = "hostname_asc"
     HOSTNAME_DESC = "hostname_desc"
     CONNECTION_STATUS_ASC = "connection_status_asc"
     CONNECTION_STATUS_DESC = "connection_status_desc"
     ISOLATION_STATUS_ASC = "isolation_status_asc"
     ISOLATION_STATUS_DESC = "isolation_status_desc"
+    DESIRED_ISOLATION_STATUS_ASC = "desired_isolation_status_asc"
+    DESIRED_ISOLATION_STATUS_DESC = "desired_isolation_status_desc"
     IP_ADDRESS_ASC = "ip_address_asc"
     IP_ADDRESS_DESC = "ip_address_desc"
     ENDPOINT_TYPE_ASC = "endpoint_type_asc"
     ENDPOINT_TYPE_DESC = "endpoint_type_desc"
     LAST_SEEN_ASC = "last_seen_asc"
     LAST_SEEN_DESC = "last_seen_desc"
     ETHERNET_ADDRESSES_ASC = "ethernet_addresses_asc"
@@ -410,14 +412,17 @@
     )
     created_at_gt: Optional[str] = field(
         default=None, metadata=config(field_name="createdAt_gt")
     )
     created_at_gte: Optional[str] = field(
         default=None, metadata=config(field_name="createdAt_gte")
     )
+    desired_isolation_status: Optional[str] = field(
+        default=None, metadata=config(field_name="desiredIsolationStatus")
+    )
     group_name: Optional[str] = field(
         default=None, metadata=config(field_name="groupName")
     )
     group_name_contains: Optional[str] = field(
         default=None, metadata=config(field_name="groupName_contains")
     )
     host_id: Optional[str] = field(default=None, metadata=config(field_name="hostId"))
@@ -598,14 +603,17 @@
     )
     connection_status: Optional[str] = field(
         default=None, metadata=config(field_name="connectionStatus")
     )
     isolation_status: Optional[str] = field(
         default=None, metadata=config(field_name="isolationStatus")
     )
+    desired_isolation_status: Optional[str] = field(
+        default=None, metadata=config(field_name="desiredIsolationStatus")
+    )
     model: Optional[str] = field(default=None, metadata=config(field_name="model"))
     cloud_provider_name: Optional[str] = field(
         default=None, metadata=config(field_name="cloudProviderName")
     )
     cloud_instance_id: Optional[str] = field(
         default=None, metadata=config(field_name="cloudInstanceId")
     )
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/mutations.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.audits.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.audits import AuditsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAuditsMutation:
     """Teagis Audits Mutation operations."""
 
     def __init__(self, service: AuditsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.audits.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.audits import AuditsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKAuditsQuery:
     """Teagis Audits Query operations."""
 
     def __init__(self, service: AuditsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/subscriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Audits Subscription."""
+"""Users Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.audits.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.users.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.audits import AuditsService
+    from taegis_sdk_python.services.users import UsersService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKAuditsSubscription:
-    """Teagis Audits Subscription operations."""
+class TaegisSDKUsersSubscription:
+    """Teagis Users Subscription operations."""
 
-    def __init__(self, service: AuditsService):
+    def __init__(self, service: UsersService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,20 @@
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AllAuditsInput:
     """AllAuditsInput."""
 
+    tenant_ids: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="tenantIDs")
+    )
+    session_id: Optional[str] = field(
+        default=None, metadata=config(field_name="sessionID")
+    )
     offset: Optional[int] = field(default=None, metadata=config(field_name="offset"))
     limit: Optional[int] = field(default=None, metadata=config(field_name="limit"))
     before: Optional[str] = field(default=None, metadata=config(field_name="before"))
     after: Optional[str] = field(default=None, metadata=config(field_name="after"))
     sort_by: Optional[SortBy] = field(
         default=None, metadata=config(field_name="sortBy")
     )
@@ -211,14 +217,20 @@
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AuditSearchInput:
     """AuditSearchInput."""
 
+    tenant_ids: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="tenantIDs")
+    )
+    session_id: Optional[str] = field(
+        default=None, metadata=config(field_name="sessionID")
+    )
     offset: Optional[int] = field(default=None, metadata=config(field_name="offset"))
     limit: Optional[int] = field(default=None, metadata=config(field_name="limit"))
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     log_type: Optional[str] = field(default=None, metadata=config(field_name="logType"))
     application: Optional[str] = field(
         default=None, metadata=config(field_name="application")
     )
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.clients.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.clients import ClientsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKClientsMutation:
     """Teagis Clients Mutation operations."""
 
     def __init__(self, service: ClientsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.clients.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.clients import ClientsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKClientsQuery:
     """Teagis Clients Query operations."""
 
     def __init__(self, service: ClientsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/subscriptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Clients Subscription."""
+"""EntityProfile Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.clients.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.entity_profile.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.clients import ClientsService
+    from taegis_sdk_python.services.entity_profile import EntityProfileService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKClientsSubscription:
-    """Teagis Clients Subscription operations."""
+class TaegisSDKEntityProfileSubscription:
+    """Teagis Entity_profile Subscription operations."""
 
-    def __init__(self, service: ClientsService):
+    def __init__(self, service: EntityProfileService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/mutations.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.collector.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.collector import CollectorService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKCollectorMutation:
     """Teagis Collector Mutation operations."""
 
     def __init__(self, service: CollectorService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.collector.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.collector import CollectorService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKCollectorQuery:
     """Teagis Collector Query operations."""
 
     def __init__(self, service: CollectorService):
         self.service = service
 
@@ -132,14 +134,18 @@
         launch_console: Optional[bool] = None,
         aws_details: Optional[AWSDetails] = None,
         gcp_details: Optional[GCPDetails] = None,
     ) -> Image:
         """Deprecated, use `getClusterImageV2` instead for consolidated inputs.."""
         endpoint = "getClusterImage"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use `getClusterImageV2` instead for consolidated inputs.'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "clusterID": prepare_input(cluster_id),
                 "imageType": prepare_input(image_type),
                 "launchConsole": prepare_input(launch_console),
                 "awsDetails": prepare_input(aws_details),
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.collector.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.collector import CollectorService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKCollectorSubscription:
     """Teagis Collector Subscription operations."""
 
     def __init__(self, service: CollectorService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,122 +1,110 @@
-"""Comments Mutation."""
+"""EndpointManagementService Mutation."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.comments.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.endpoint_management_service.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.comments import CommentsService
+    from taegis_sdk_python.services.endpoint_management_service import (
+        EndpointManagementServiceService,
+    )
 
+log = logging.getLogger(__name__)
 
-class TaegisSDKCommentsMutation:
-    """Teagis Comments Mutation operations."""
 
-    def __init__(self, service: CommentsService):
+class TaegisSDKEndpointManagementServiceMutation:
+    """Teagis Endpoint_management_service Mutation operations."""
+
+    def __init__(self, service: EndpointManagementServiceService):
         self.service = service
 
-    def mark_comment_read(self, comment_id: str) -> Comment:
-        """None."""
-        endpoint = "markCommentRead"
+    def create_endpoint_group(self, input_: CreateEndpointGroupInput) -> EndpointGroup:
+        """Create new endpoint group for a tenant.."""
+        endpoint = "createEndpointGroup"
 
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
-                "comment_id": prepare_input(comment_id),
+                "input": prepare_input(input_),
             },
-            output=build_output_string(Comment),
+            output=build_output_string(EndpointGroup),
         )
         if result.get(endpoint) is not None:
-            return Comment.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for mutation markCommentRead")
+            return EndpointGroup.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for mutation createEndpointGroup")
 
-    def mark_parent_comments_read(self, parents: List[Parent]) -> List[Comment]:
-        """None."""
-        endpoint = "markParentCommentsRead"
+    def update_endpoint_group(self, input_: UpdateEndpointGroupInput) -> EndpointGroup:
+        """Update policy type of endpoint group for a tenant.."""
+        endpoint = "updateEndpointGroup"
 
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
-                "parents": prepare_input(parents),
+                "input": prepare_input(input_),
             },
-            output=build_output_string(Comment),
+            output=build_output_string(EndpointGroup),
         )
         if result.get(endpoint) is not None:
-            return Comment.schema().load(
-                [r or {} for r in result.get(endpoint)], many=True
-            )
-        raise GraphQLNoRowsInResultSetError("for mutation markParentCommentsRead")
-
-    def create_comment(self, comment: CommentInput) -> Comment:
-        """None."""
-        endpoint = "createComment"
+            return EndpointGroup.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for mutation updateEndpointGroup")
 
-        result = self.service.execute_mutation(
-            endpoint=endpoint,
-            variables={
-                "comment": prepare_input(comment),
-            },
-            output=build_output_string(Comment),
-        )
-        if result.get(endpoint) is not None:
-            return Comment.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for mutation createComment")
-
-    def update_comment(self, comment_id: str, comment: CommentUpdate) -> Comment:
-        """None."""
-        endpoint = "updateComment"
+    def delete_endpoint_group(self, input_: DeleteEndpointGrpInput) -> bool:
+        """Delete endpoint group for a tenant.."""
+        endpoint = "deleteEndpointGroup"
 
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
-                "comment_id": prepare_input(comment_id),
-                "comment": prepare_input(comment),
+                "input": prepare_input(input_),
             },
-            output=build_output_string(Comment),
+            output="",
         )
         if result.get(endpoint) is not None:
-            return Comment.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for mutation updateComment")
+            return result.get(endpoint)
+        raise GraphQLNoRowsInResultSetError("for mutation deleteEndpointGroup")
 
-    def delete_comment(self, comment_id: str) -> Comment:
-        """None."""
-        endpoint = "deleteComment"
+    def create_policy(self, input_: CreatePolicyInput) -> Policy:
+        """Create new policy. Used by administrator of the taegis."""
+        endpoint = "createPolicy"
 
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
-                "comment_id": prepare_input(comment_id),
+                "input": prepare_input(input_),
             },
-            output=build_output_string(Comment),
+            output=build_output_string(Policy),
         )
         if result.get(endpoint) is not None:
-            return Comment.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for mutation deleteComment")
+            return Policy.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for mutation createPolicy")
 
-    def bulk_restore_comments(self, ids: List[str]) -> List[str]:
-        """None."""
-        endpoint = "bulkRestoreComments"
+    def assign_bulk_assets_to_group(
+        self, input_: Optional[BulkAssignRequestInput] = None
+    ) -> BulkAssignRequestOutput:
+        """Assign the assets to target group."""
+        endpoint = "assignBulkAssetsToGroup"
 
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
-                "ids": prepare_input(ids),
+                "input": prepare_input(input_),
             },
-            output="",
+            output=build_output_string(BulkAssignRequestOutput),
         )
         if result.get(endpoint) is not None:
-            return result.get(endpoint)
-        raise GraphQLNoRowsInResultSetError("for mutation bulkRestoreComments")
+            return BulkAssignRequestOutput.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for mutation assignBulkAssetsToGroup")
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/queries.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,39 +3,45 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.comments.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.comments import CommentsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKCommentsQuery:
     """Teagis Comments Query operations."""
 
     def __init__(self, service: CommentsService):
         self.service = service
 
     def comment(self, comment_id: str) -> Comment:
         """None."""
         endpoint = "comment"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'use investigation-v2 comments queries'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "comment_id": prepare_input(comment_id),
             },
             output=build_output_string(Comment),
         )
@@ -43,14 +49,18 @@
             return Comment.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query comment")
 
     def comments_by_parent(self, parent_type: str, parent_id: str) -> List[Comment]:
         """None."""
         endpoint = "commentsByParent"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'use investigation-v2 comments queries'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "parent_type": prepare_input(parent_type),
                 "parent_id": prepare_input(parent_id),
             },
             output=build_output_string(Comment),
@@ -63,14 +73,18 @@
 
     def comments_by_parent_section(
         self, parent_type: str, parent_id: str, section_type: str, section_id: str
     ) -> List[Comment]:
         """None."""
         endpoint = "commentsByParentSection"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'use investigation-v2 comments queries'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "parent_type": prepare_input(parent_type),
                 "parent_id": prepare_input(parent_id),
                 "section_type": prepare_input(section_type),
                 "section_id": prepare_input(section_id),
@@ -83,14 +97,18 @@
             )
         raise GraphQLNoRowsInResultSetError("for query commentsByParentSection")
 
     def comments_count_by_parent(self, parent_type: str, parent_id: str) -> ParentCount:
         """None."""
         endpoint = "commentsCountByParent"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'use investigation-v2 comments queries'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "parent_type": prepare_input(parent_type),
                 "parent_id": prepare_input(parent_id),
             },
             output=build_output_string(ParentCount),
@@ -99,14 +117,18 @@
             return ParentCount.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query commentsCountByParent")
 
     def comments_count_by_parent_type(self, parent_type: str) -> List[ParentCount]:
         """None."""
         endpoint = "commentsCountByParentType"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'use investigation-v2 comments queries'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "parent_type": prepare_input(parent_type),
             },
             output=build_output_string(ParentCount),
         )
@@ -116,14 +138,18 @@
             )
         raise GraphQLNoRowsInResultSetError("for query commentsCountByParentType")
 
     def unread_comments_by_parents(self, parents: List[Parent]) -> List[Comment]:
         """None."""
         endpoint = "unreadCommentsByParents"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'use investigation-v2 comments queries'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "parents": prepare_input(parents),
             },
             output=build_output_string(Comment),
         )
@@ -135,14 +161,18 @@
 
     def latest_bulk_comments_by_parent(
         self, parent_type: str, parent_ids: List[str]
     ) -> List[LatestComment]:
         """None."""
         endpoint = "latestBulkCommentsByParent"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'use investigation-v2 comments queries'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "parent_type": prepare_input(parent_type),
                 "parent_ids": prepare_input(parent_ids),
             },
             output=build_output_string(LatestComment),
@@ -155,14 +185,18 @@
 
     def comments_count_by_parent_ids(
         self, parent_type: str, parent_ids: List[str]
     ) -> List[ParentCount]:
         """None."""
         endpoint = "commentsCountByParentIds"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'use investigation-v2 comments queries'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "parent_type": prepare_input(parent_type),
                 "parent_ids": prepare_input(parent_ids),
             },
             output=build_output_string(ParentCount),
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.comments.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.comments import CommentsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKCommentsSubscription:
     """Teagis Comments Subscription operations."""
 
     def __init__(self, service: CommentsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/mutations.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.detector_registry.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.detector_registry import DetectorRegistryService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKDetectorRegistryMutation:
     """Teagis Detector_registry Mutation operations."""
 
     def __init__(self, service: DetectorRegistryService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.detector_registry.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.detector_registry import DetectorRegistryService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKDetectorRegistryQuery:
     """Teagis Detector_registry Query operations."""
 
     def __init__(self, service: DetectorRegistryService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/subscriptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.detector_registry.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.detector_registry import DetectorRegistryService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKDetectorRegistrySubscription:
     """Teagis Detector_registry Subscription operations."""
 
     def __init__(self, service: DetectorRegistryService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from enum import Enum
 
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 
 
-class State(str, Enum):
-    """State."""
+class STATE(str, Enum):
+    """STATE."""
 
     DEPLOYED = "deployed"
     RESEARCH = "research"
     DISABLED = "disabled"
 
 
 @dataclass_json
@@ -82,8 +82,8 @@
     )
     created_at: Optional[str] = field(
         default=None, metadata=config(field_name="createdAt")
     )
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt")
     )
-    state: Optional[State] = field(default=None, metadata=config(field_name="state"))
+    state: Optional[STATE] = field(default=None, metadata=config(field_name="state"))
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.endpoint_command_manager.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.endpoint_command_manager import (
         EndpointCommandManagerService,
     )
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEndpointCommandManagerMutation:
     """Teagis Endpoint_command_manager Mutation operations."""
 
     def __init__(self, service: EndpointCommandManagerService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.endpoint_command_manager.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.endpoint_command_manager import (
         EndpointCommandManagerService,
     )
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEndpointCommandManagerQuery:
     """Teagis Endpoint_command_manager Query operations."""
 
     def __init__(self, service: EndpointCommandManagerService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.endpoint_command_manager.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.endpoint_command_manager import (
         EndpointCommandManagerService,
     )
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEndpointCommandManagerSubscription:
     """Teagis Endpoint_command_manager Subscription operations."""
 
     def __init__(self, service: EndpointCommandManagerService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.endpoint_management_service.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.endpoint_management_service import (
         EndpointManagementServiceService,
     )
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEndpointManagementServiceQuery:
     """Teagis Endpoint_management_service Query operations."""
 
     def __init__(self, service: EndpointManagementServiceService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.endpoint_management_service.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.endpoint_management_service import (
         EndpointManagementServiceService,
     )
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEndpointManagementServiceSubscription:
     """Teagis Endpoint_management_service Subscription operations."""
 
     def __init__(self, service: EndpointManagementServiceService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,20 @@
     )
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt")
     )
     skip_upgrade: Optional[bool] = field(
         default=None, metadata=config(field_name="skipUpgrade")
     )
+    archive_endpoint_after_days: Optional[int] = field(
+        default=None, metadata=config(field_name="ArchiveEndpointAfterDays")
+    )
+    is_archive_endpoint_enabled: Optional[bool] = field(
+        default=None, metadata=config(field_name="IsArchiveEndpointEnabled")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class DeleteEndpointGrpInput:
     """DeleteEndpointGrpInput."""
 
@@ -148,14 +154,17 @@
     desired_agent_version: Optional[str] = field(
         default=None, metadata=config(field_name="desiredAgentVersion")
     )
     is_default: Optional[bool] = field(
         default=None, metadata=config(field_name="isDefault")
     )
     channel: Optional[str] = field(default=None, metadata=config(field_name="channel"))
+    archive_endpoint_after_days: Optional[int] = field(
+        default=None, metadata=config(field_name="ArchiveEndpointAfterDays")
+    )
     policy_name: Optional[PolicyType] = field(
         default=None, metadata=config(field_name="policyName")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
@@ -167,14 +176,17 @@
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
     )
     desired_version: Optional[str] = field(
         default=None, metadata=config(field_name="desiredVersion")
     )
     channel: Optional[str] = field(default=None, metadata=config(field_name="channel"))
+    archive_endpoint_after_days: Optional[int] = field(
+        default=None, metadata=config(field_name="ArchiveEndpointAfterDays")
+    )
     policy_name: Optional[PolicyType] = field(
         default=None, metadata=config(field_name="policyName")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""EntityProfile Mutation."""
+"""Exports Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.entity_profile.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.exports.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.entity_profile import EntityProfileService
+    from taegis_sdk_python.services.exports import ExportsService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKEntityProfileMutation:
-    """Teagis Entity_profile Mutation operations."""
+class TaegisSDKExportsSubscription:
+    """Teagis Exports Subscription operations."""
 
-    def __init__(self, service: EntityProfileService):
+    def __init__(self, service: ExportsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.entity_profile.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.entity_profile import EntityProfileService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEntityProfileQuery:
     """Teagis Entity_profile Query operations."""
 
     def __init__(self, service: EntityProfileService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""EntityProfile Subscription."""
+"""Audits Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.entity_profile.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.audits.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.entity_profile import EntityProfileService
+    from taegis_sdk_python.services.audits import AuditsService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKEntityProfileSubscription:
-    """Teagis Entity_profile Subscription operations."""
+class TaegisSDKAuditsSubscription:
+    """Teagis Audits Subscription operations."""
 
-    def __init__(self, service: EntityProfileService):
+    def __init__(self, service: AuditsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/mutations.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.event_search.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.event_search import EventSearchService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEventSearchMutation:
     """Teagis Event_search Mutation operations."""
 
     def __init__(self, service: EventSearchService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.event_search.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.event_search import EventSearchService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEventSearchQuery:
     """Teagis Event_search Query operations."""
 
     def __init__(self, service: EventSearchService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.event_search.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.event_search import EventSearchService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEventSearchSubscription:
     """Teagis Event_search Subscription operations."""
 
     def __init__(self, service: EventSearchService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,22 @@
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AuxiliaryEventsByIDOptions:
     """AuxiliaryEventsByIDOptions."""
 
     search_events_api_first: Optional[bool] = field(
-        default=None, metadata=config(field_name="searchEventsAPIFirst")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "Obsolete. Events-API is now used automatically only if needed",
+            },
+            field_name="searchEventsAPIFirst",
+        ),
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AsynchronousEventsSearchPrepInputResponse:
     """AsynchronousEventsSearchPrepInputResponse."""
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/mutations.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.events.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.events import EventsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEventsMutation:
     """Teagis Events Mutation operations."""
 
     def __init__(self, service: EventsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.events.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.events import EventsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEventsQuery:
     """Teagis Events Query operations."""
 
     def __init__(self, service: EventsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/subscriptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.events.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.events import EventsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKEventsSubscription:
     """Teagis Events Subscription operations."""
 
     def __init__(self, service: EventsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,24 @@
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class EventUser:
     """EventUser."""
 
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
+    name: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "name is deprecated. Use `userID` instead.",
+            },
+            field_name="name",
+        ),
+    )
     role: Optional[str] = field(default=None, metadata=config(field_name="role"))
     email: Optional[str] = field(default=None, metadata=config(field_name="email"))
     user_id: Optional[str] = field(default=None, metadata=config(field_name="userID"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/mutations.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.exports.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.exports import ExportsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKExportsMutation:
     """Teagis Exports Mutation operations."""
 
     def __init__(self, service: ExportsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.exports.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.exports import ExportsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKExportsQuery:
     """Teagis Exports Query operations."""
 
     def __init__(self, service: ExportsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Exports Subscription."""
+"""Rules Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.exports.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.rules.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.exports import ExportsService
+    from taegis_sdk_python.services.rules import RulesService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKExportsSubscription:
-    """Teagis Exports Subscription operations."""
+class TaegisSDKRulesSubscription:
+    """Teagis Rules Subscription operations."""
 
-    def __init__(self, service: ExportsService):
+    def __init__(self, service: RulesService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.investigations.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.investigations import InvestigationsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKInvestigationsMutation:
     """Teagis Investigations Mutation operations."""
 
     def __init__(self, service: InvestigationsService):
         self.service = service
 
@@ -123,14 +125,18 @@
 
     def create_activity_log_for_investigation(
         self, investigation_id: str, activity_log: ActivityLogInput
     ) -> ActivityLog:
         """Create a new activity log for investigation."""
         endpoint = "createActivityLogForInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Not Supported - Use audit logs'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "activityLog": prepare_input(activity_log),
             },
             output=build_output_string(ActivityLog),
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.investigations.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.investigations import InvestigationsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKInvestigationsQuery:
     """Teagis Investigations Query operations."""
 
     def __init__(self, service: InvestigationsService):
         self.service = service
 
@@ -91,14 +93,18 @@
     ) -> List[Investigation]:
         """Get all investigations
         Max perPage Value is 100. If requesting over 100, only the first 100 will be returned.
         deprecated: Use `investigationsSearch` for better investigations query experience..
         """
         endpoint = "allInvestigations"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'replaced by investigationsSearch'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "status": prepare_input(status),
                 "page": prepare_input(page),
                 "perPage": prepare_input(per_page),
                 "createdAfter": prepare_input(created_after),
@@ -545,14 +551,18 @@
     ) -> List[Investigation]:
         """Get investigations by multi-tenant session
         DO NOT USE, this query is unsupported. Use investigationsSearch instead.
         Max perPage Value is 100. If requesting over 100, only the first 100 will be returned..
         """
         endpoint = "investigationsBySession"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Not Supported - use investigationsSearch'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "session_id": prepare_input(session_id),
                 "page": prepare_input(page),
                 "perPage": prepare_input(per_page),
             },
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.investigations.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.investigations import InvestigationsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKInvestigationsSubscription:
     """Teagis Investigations Subscription operations."""
 
     def __init__(self, service: InvestigationsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,82 +405,14 @@
         default=None, metadata=config(field_name="alerts")
     )
     tenant: Optional[str] = field(default=None, metadata=config(field_name="tenant"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class Hostname:
-    """Hostname."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="created_at")
-    )
-    updated_at: Optional[str] = field(
-        default=None, metadata=config(field_name="updated_at")
-    )
-    host_id: Optional[str] = field(default=None, metadata=config(field_name="host_id"))
-    hostname: Optional[str] = field(
-        default=None, metadata=config(field_name="hostname")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class EthernetAddress:
-    """EthernetAddress."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="created_at")
-    )
-    updated_at: Optional[str] = field(
-        default=None, metadata=config(field_name="updated_at")
-    )
-    host_id: Optional[str] = field(default=None, metadata=config(field_name="host_id"))
-    mac: Optional[str] = field(default=None, metadata=config(field_name="mac"))
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class IpAddress:
-    """IpAddress."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="created_at")
-    )
-    updated_at: Optional[str] = field(
-        default=None, metadata=config(field_name="updated_at")
-    )
-    ip: Optional[str] = field(default=None, metadata=config(field_name="ip"))
-    host_id: Optional[str] = field(default=None, metadata=config(field_name="host_id"))
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class User:
-    """User."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="created_at")
-    )
-    updated_at: Optional[str] = field(
-        default=None, metadata=config(field_name="updated_at")
-    )
-    host_id: Optional[str] = field(default=None, metadata=config(field_name="host_id"))
-    username: Optional[str] = field(
-        default=None, metadata=config(field_name="username")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class MitreAttackInfo:
     """MitreAttackInfo."""
 
     technique_id: Optional[str] = field(
         default=None, metadata=config(field_name="technique_id")
     )
     technique: Optional[str] = field(
@@ -824,18 +756,32 @@
     roles: Optional[List[str]] = field(
         default=None, metadata=config(field_name="roles")
     )
     status: Optional[str] = field(default=None, metadata=config(field_name="status"))
     user_id: Optional[str] = field(default=None, metadata=config(field_name="user_id"))
     email: Optional[str] = field(default=None, metadata=config(field_name="email"))
     email_verified: Optional[bool] = field(
-        default=None, metadata=config(field_name="email_verified")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "Do not use, is never available or true.",
+            },
+            field_name="email_verified",
+        ),
     )
     email_normalized: Optional[str] = field(
-        default=None, metadata=config(field_name="email_normalized")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "Do not use, is not available.",
+            },
+            field_name="email_normalized",
+        ),
     )
     family_name: Optional[str] = field(
         default=None, metadata=config(field_name="family_name")
     )
     given_name: Optional[str] = field(
         default=None, metadata=config(field_name="given_name")
     )
@@ -1029,27 +975,38 @@
     assets: Optional[List[Asset]] = field(
         default=None, metadata=config(field_name="assets")
     )
     search_queries: Optional[List[SearchQuery]] = field(
         default=None, metadata=config(field_name="search_queries")
     )
     activity_logs: Optional[List[ActivityLog]] = field(
-        default=None, metadata=config(field_name="activity_logs")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "Not Supported - Use audit logs",
+            },
+            field_name="activity_logs",
+        ),
     )
     created_by_user: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="created_by_user")
     )
     contributed_users: Optional[List[TDRUser]] = field(
         default=None, metadata=config(field_name="contributed_users")
     )
     assignee_user: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="assignee_user")
     )
     assignee: Optional[Assignee] = field(
-        default=None, metadata=config(field_name="assignee")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "No longer supported"},
+            field_name="assignee",
+        ),
     )
     access_vectors: Optional[List[AccessVector]] = field(
         default=None, metadata=config(field_name="access_vectors")
     )
     transition_state: Optional[TransitionState] = field(
         default=None, metadata=config(field_name="transition_state")
     )
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.investigations2.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.investigations2 import Investigations2Service
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKInvestigations2Mutation:
     """Teagis Investigations2 Mutation operations."""
 
     def __init__(self, service: Investigations2Service):
         self.service = service
 
@@ -289,7 +291,24 @@
                 "input": prepare_input(input_),
             },
             output=build_output_string(InvestigationV2),
         )
         if result.get(endpoint) is not None:
             return InvestigationV2.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation closeInvestigation")
+
+    def archive_investigation_v2(
+        self, input_: ArchiveInvestigationInput
+    ) -> InvestigationV2:
+        """Archive investigation."""
+        endpoint = "archiveInvestigationV2"
+
+        result = self.service.execute_mutation(
+            endpoint=endpoint,
+            variables={
+                "input": prepare_input(input_),
+            },
+            output=build_output_string(InvestigationV2),
+        )
+        if result.get(endpoint) is not None:
+            return InvestigationV2.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for mutation archiveInvestigationV2")
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.investigations2.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.investigations2 import Investigations2Service
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKInvestigations2Query:
     """Teagis Investigations2 Query operations."""
 
     def __init__(self, service: Investigations2Service):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/subscriptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.investigations2.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.investigations2 import Investigations2Service
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKInvestigations2Subscription:
     """Teagis Investigations2 Subscription operations."""
 
     def __init__(self, service: Investigations2Service):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     TEST = "TEST"
 
 
 class InvestigationStatus(str, Enum):
     """InvestigationStatus."""
 
     DRAFT = "DRAFT"
+    DRAFT_DISMISSED = "DRAFT_DISMISSED"
     OPEN = "OPEN"
     AWAITING_ACTION = "AWAITING_ACTION"
     ACTIVE = "ACTIVE"
     SUSPENDED = "SUSPENDED"
     CLOSED_CONFIRMED_SECURITY_INCIDENT = "CLOSED_CONFIRMED_SECURITY_INCIDENT"
     CLOSED_AUTHORIZED_ACTIVITY = "CLOSED_AUTHORIZED_ACTIVITY"
     CLOSED_THREAT_MITIGATED = "CLOSED_THREAT_MITIGATED"
@@ -150,14 +151,22 @@
     """DeleteInvestigationRuleInput."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class ArchiveInvestigationInput:
+    """ArchiveInvestigationInput."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class AddEvidenceToInvestigationResult:
     """AddEvidenceToInvestigationResult."""
 
     investigation_id: Optional[str] = field(
         default=None, metadata=config(field_name="investigationId")
     )
     alerts: Optional[List[str]] = field(
@@ -459,14 +468,22 @@
     """TDRUser."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class Client:
+    """Client."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class CreateInvestigationRuleInput:
     """CreateInvestigationRuleInput."""
 
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
     title: Optional[str] = field(default=None, metadata=config(field_name="title"))
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
@@ -567,16 +584,26 @@
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationsV2Arguments:
     """InvestigationsV2Arguments."""
 
     page: Optional[int] = field(default=None, metadata=config(field_name="page"))
     per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
     cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
+    search_children_tenants: Optional[bool] = field(
+        default=None, metadata=config(field_name="searchChildrenTenants")
+    )
     order_by: Optional[PaginationOrder] = field(
-        default=None, metadata=config(field_name="orderBy")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "does not do anything - sorting is done through cql",
+            },
+            field_name="orderBy",
+        ),
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class ExportInvestigationResourcesArgument:
     """ExportInvestigationResourcesArgument."""
@@ -669,14 +696,15 @@
     )
     events: Optional[List[str]] = field(
         default=None, metadata=config(field_name="events")
     )
     search_queries: Optional[List[str]] = field(
         default=None, metadata=config(field_name="searchQueries")
     )
+    rule_id: Optional[str] = field(default=None, metadata=config(field_name="ruleId"))
     template_id: Optional[str] = field(
         default=None, metadata=config(field_name="templateId")
     )
     type: Optional[InvestigationType] = field(
         default=None, metadata=config(field_name="type")
     )
     status: Optional[InvestigationStatus] = field(
@@ -914,17 +942,27 @@
     )
     search_window: Optional[str] = field(
         default=None, metadata=config(field_name="searchWindow")
     )
     tenant_filter: Optional[str] = field(
         default=None, metadata=config(field_name="tenantFilter")
     )
-    comment: Optional[str] = field(default=None, metadata=config(field_name="comment"))
+    comment: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use appendComment"},
+            field_name="comment",
+        ),
+    )
     exclude_child_tenants: Optional[bool] = field(
-        default=None, metadata=config(field_name="excludeChildTenants")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use tenantFilter"},
+            field_name="excludeChildTenants",
+        ),
     )
     created_by: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="createdBy")
     )
     updated_by: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="updatedBy")
     )
@@ -944,28 +982,53 @@
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     short_id: Optional[str] = field(default=None, metadata=config(field_name="shortId"))
     title: Optional[str] = field(default=None, metadata=config(field_name="title"))
     key_findings: Optional[str] = field(
         default=None, metadata=config(field_name="keyFindings")
     )
     alerts: Optional[List[str]] = field(
-        default=None, metadata=config(field_name="alerts")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use alertsEvidence"},
+            field_name="alerts",
+        ),
     )
     assets: Optional[List[str]] = field(
-        default=None, metadata=config(field_name="assets")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use assetsEvidence"},
+            field_name="assets",
+        ),
     )
     events: Optional[List[str]] = field(
-        default=None, metadata=config(field_name="events")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use eventsEvidence"},
+            field_name="events",
+        ),
+    )
+    alerts_evidence_count: Optional[int] = field(
+        default=None, metadata=config(field_name="alertsEvidenceCount")
+    )
+    assets_evidence_count: Optional[int] = field(
+        default=None, metadata=config(field_name="assetsEvidenceCount")
+    )
+    events_evidence_count: Optional[int] = field(
+        default=None, metadata=config(field_name="eventsEvidenceCount")
     )
     search_queries: Optional[List[str]] = field(
         default=None, metadata=config(field_name="searchQueries")
     )
     tags: Optional[List[str]] = field(default=None, metadata=config(field_name="tags"))
     contributor_ids: Optional[List[str]] = field(
-        default=None, metadata=config(field_name="contributorIDs")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use contributorIds"},
+            field_name="contributorIDs",
+        ),
     )
     contributor_ids: Optional[List[str]] = field(
         default=None, metadata=config(field_name="contributorIds")
     )
     assignee_id: Optional[str] = field(
         default=None, metadata=config(field_name="assigneeId")
     )
@@ -989,14 +1052,15 @@
     )
     priority: Optional[int] = field(
         default=None, metadata=config(field_name="priority")
     )
     close_reason: Optional[str] = field(
         default=None, metadata=config(field_name="closeReason")
     )
+    rule_id: Optional[str] = field(default=None, metadata=config(field_name="ruleId"))
     alerts_evidence: Optional[List[AlertEvidence]] = field(
         default=None, metadata=config(field_name="alertsEvidence")
     )
     assets_evidence: Optional[List[AssetEvidence]] = field(
         default=None, metadata=config(field_name="assetsEvidence")
     )
     events_evidence: Optional[List[EventEvidence]] = field(
@@ -1007,20 +1071,29 @@
     )
     contributors: Optional[List[TDRUser]] = field(
         default=None, metadata=config(field_name="contributors")
     )
     assignee: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="assignee")
     )
+    assignee_client: Optional[Client] = field(
+        default=None, metadata=config(field_name="assigneeClient")
+    )
     created_by: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="createdBy")
     )
+    created_by_client: Optional[Client] = field(
+        default=None, metadata=config(field_name="createdByClient")
+    )
     updated_by: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="updatedBy")
     )
+    updated_by_client: Optional[Client] = field(
+        default=None, metadata=config(field_name="updatedByClient")
+    )
     type: Optional[InvestigationType] = field(
         default=None, metadata=config(field_name="type")
     )
     processing_status: Optional[InvestigationProcessingStatus] = field(
         default=None, metadata=config(field_name="processingStatus")
     )
     comments_count: Optional[InvestigationCommentsCount] = field(
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.mitre_attack_info.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKMitreAttackInfoMutation:
     """Teagis Mitre_attack_info Mutation operations."""
 
     def __init__(self, service: MitreAttackInfoService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.mitre_attack_info.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKMitreAttackInfoQuery:
     """Teagis Mitre_attack_info Query operations."""
 
     def __init__(self, service: MitreAttackInfoService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.mitre_attack_info.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKMitreAttackInfoSubscription:
     """Teagis Mitre_attack_info Subscription operations."""
 
     def __init__(self, service: MitreAttackInfoService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.notebooks.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.notebooks import NotebooksService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKNotebooksMutation:
     """Teagis Notebooks Mutation operations."""
 
     def __init__(self, service: NotebooksService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/queries.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.notebooks.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.notebooks import NotebooksService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKNotebooksQuery:
     """Teagis Notebooks Query operations."""
 
     def __init__(self, service: NotebooksService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Notebooks Subscription."""
+"""Notifications Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.notebooks.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.notifications.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.notebooks import NotebooksService
+    from taegis_sdk_python.services.notifications import NotificationsService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKNotebooksSubscription:
-    """Teagis Notebooks Subscription operations."""
+class TaegisSDKNotificationsSubscription:
+    """Teagis Notifications Subscription operations."""
 
-    def __init__(self, service: NotebooksService):
+    def __init__(self, service: NotificationsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/mutations.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.notifications.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.notifications import NotificationsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKNotificationsMutation:
     """Teagis Notifications Mutation operations."""
 
     def __init__(self, service: NotificationsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.notifications.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.notifications import NotificationsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKNotificationsQuery:
     """Teagis Notifications Query operations."""
 
     def __init__(self, service: NotificationsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.preferences.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.preferences import PreferencesService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKPreferencesMutation:
     """Teagis Preferences Mutation operations."""
 
     def __init__(self, service: PreferencesService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.preferences.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.preferences import PreferencesService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKPreferencesQuery:
     """Teagis Preferences Query operations."""
 
     def __init__(self, service: PreferencesService):
         self.service = service
 
@@ -116,14 +118,33 @@
         )
         if result.get(endpoint) is not None:
             return TenantPreference.schema().load(
                 [r or {} for r in result.get(endpoint)], many=True
             )
         raise GraphQLNoRowsInResultSetError("for query listTenantPreferencesByKey")
 
+    def list_all_tenant_preferences(
+        self, filter_: listAllTenantPreferencesInput
+    ) -> List[TenantPreference]:
+        """None."""
+        endpoint = "listAllTenantPreferences"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "filter": prepare_input(filter_),
+            },
+            output=build_output_string(TenantPreference),
+        )
+        if result.get(endpoint) is not None:
+            return TenantPreference.schema().load(
+                [r or {} for r in result.get(endpoint)], many=True
+            )
+        raise GraphQLNoRowsInResultSetError("for query listAllTenantPreferences")
+
     def ticketing_settings(self) -> List[TicketingSettings]:
         """None."""
         endpoint = "ticketingSettings"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={},
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/subscriptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.preferences.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.preferences import PreferencesService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKPreferencesSubscription:
     """Teagis Preferences Subscription operations."""
 
     def __init__(self, service: PreferencesService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,28 @@
     token_placeholder: Optional[str] = field(
         default=None, metadata=config(field_name="tokenPlaceholder")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class listAllTenantPreferencesInput:
+    """listAllTenantPreferencesInput."""
+
+    keys: Optional[List[str]] = field(default=None, metadata=config(field_name="keys"))
+    tenant_ids: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="tenant_IDs")
+    )
+    environment: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="environment")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class PartnerPreference:
     """PartnerPreference."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     tenant_id: Optional[str] = field(
         default=None, metadata=config(field_name="tenantID")
     )
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.rules.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.rules import RulesService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKRulesMutation:
     """Teagis Rules Mutation operations."""
 
     def __init__(self, service: RulesService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.rules.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.rules import RulesService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKRulesQuery:
     """Teagis Rules Query operations."""
 
     def __init__(self, service: RulesService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Rules Subscription."""
+"""Notebooks Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.rules.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.notebooks.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.rules import RulesService
+    from taegis_sdk_python.services.notebooks import NotebooksService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKRulesSubscription:
-    """Teagis Rules Subscription operations."""
+class TaegisSDKNotebooksSubscription:
+    """Teagis Notebooks Subscription operations."""
 
-    def __init__(self, service: RulesService):
+    def __init__(self, service: NotebooksService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.sharelinks.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.sharelinks import SharelinksService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKSharelinksMutation:
     """Teagis Sharelinks Mutation operations."""
 
     def __init__(self, service: SharelinksService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.sharelinks.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.sharelinks import SharelinksService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKSharelinksQuery:
     """Teagis Sharelinks Query operations."""
 
     def __init__(self, service: SharelinksService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.sharelinks.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.sharelinks import SharelinksService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKSharelinksSubscription:
     """Teagis Sharelinks Subscription operations."""
 
     def __init__(self, service: SharelinksService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.tenants.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.tenants import TenantsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKTenantsMutation:
     """Teagis Tenants Mutation operations."""
 
     def __init__(self, service: TenantsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.tenants.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.tenants import TenantsService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKTenantsQuery:
     """Teagis Tenants Query operations."""
 
     def __init__(self, service: TenantsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Tenants Subscription."""
+"""Threat Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.tenants.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.threat.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.tenants import TenantsService
+    from taegis_sdk_python.services.threat import ThreatService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKTenantsSubscription:
-    """Teagis Tenants Subscription operations."""
+class TaegisSDKThreatSubscription:
+    """Teagis Threat Subscription operations."""
 
-    def __init__(self, service: TenantsService):
+    def __init__(self, service: ThreatService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,17 @@
     action: Optional[str] = field(default=None, metadata=config(field_name="action"))
     who: Optional[str] = field(default=None, metadata=config(field_name="who"))
     event_name: Optional[str] = field(
         default=None, metadata=config(field_name="event_name")
     )
     before: Optional[str] = field(default=None, metadata=config(field_name="before"))
     after: Optional[str] = field(default=None, metadata=config(field_name="after"))
+    owner_tenant_id: Optional[str] = field(
+        default=None, metadata=config(field_name="owner_tenant_id")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class Environment:
     """Environment."""
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/mutations.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.threat.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.threat import ThreatService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKThreatMutation:
     """Teagis Threat Mutation operations."""
 
     def __init__(self, service: ThreatService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.threat.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.threat import ThreatService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKThreatQuery:
     """Teagis Threat Query operations."""
 
     def __init__(self, service: ThreatService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/subscriptions.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Threat Subscription."""
+"""Assets Subscription."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
-from taegis_sdk_python.services.threat.types import *
-
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
+from taegis_sdk_python.services.assets.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.threat import ThreatService
+    from taegis_sdk_python.services.assets import AssetsService
+
+log = logging.getLogger(__name__)
 
 
-class TaegisSDKThreatSubscription:
-    """Teagis Threat Subscription operations."""
+class TaegisSDKAssetsSubscription:
+    """Teagis Assets Subscription operations."""
 
-    def __init__(self, service: ThreatService):
+    def __init__(self, service: AssetsService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.trip.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.trip import TripService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKTripMutation:
     """Teagis Trip Mutation operations."""
 
     def __init__(self, service: TripService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.trip.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.trip import TripService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKTripQuery:
     """Teagis Trip Query operations."""
 
     def __init__(self, service: TripService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 class ApiIntegrationHealthStatus(str, Enum):
     """ApiIntegrationHealthStatus."""
 
     PENDING = "Pending"
     HEALTHY = "Healthy"
     UNHEALTHY = "Unhealthy"
+    PROVISIONING_FAILED = "ProvisioningFailed"
 
 
 class ApiIntegrationHistoryStatus(str, Enum):
     """ApiIntegrationHistoryStatus."""
 
     RUNNING = "Running"
     SUCCESS = "Success"
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/__init__.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/mutations.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/mutations.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.users.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.users import UsersService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKUsersMutation:
     """Teagis Users Mutation operations."""
 
     def __init__(self, service: UsersService):
         self.service = service
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/queries.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Dict, Optional, Tuple, Union
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
-    prepare_input,
     parse_union_result,
+    prepare_input,
 )
 from taegis_sdk_python.services.users.types import *
 
-from taegis_sdk_python import GraphQLNoRowsInResultSetError
-
 if TYPE_CHECKING:  # pragma: no cover
     from taegis_sdk_python.services.users import UsersService
 
+log = logging.getLogger(__name__)
+
 
 class TaegisSDKUsersQuery:
     """Teagis Users Query operations."""
 
     def __init__(self, service: UsersService):
         self.service = service
 
@@ -135,14 +137,31 @@
             variables={},
             output=build_output_string(TDRUserSupportPin),
         )
         if result.get(endpoint) is not None:
             return TDRUserSupportPin.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query getSupportPin")
 
+    def get_support_pin_verification(self, support_pin: str) -> List[SupportPinDetails]:
+        """Get a list of details associated with the given support pin.."""
+        endpoint = "getSupportPinVerification"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "supportPin": prepare_input(support_pin),
+            },
+            output=build_output_string(SupportPinDetails),
+        )
+        if result.get(endpoint) is not None:
+            return SupportPinDetails.schema().load(
+                [r or {} for r in result.get(endpoint)], many=True
+            )
+        raise GraphQLNoRowsInResultSetError("for query getSupportPinVerification")
+
     def tdr_users_search(
         self, filters: Optional[TDRUsersSearchInput] = None
     ) -> TDRUsersSearchResults:
         """Fast Search Users."""
         endpoint = "tdrUsersSearch"
 
         result = self.service.execute_query(
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/types.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,24 @@
     expires_at: Optional[str] = field(
         default=None, metadata=config(field_name="expires_at")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class SupportPinDetails:
+    """SupportPinDetails."""
+
+    email_address: Optional[str] = field(
+        default=None, metadata=config(field_name="emailAddress")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class ForgotPasswordResponse:
     """ForgotPasswordResponse."""
 
     message: Optional[str] = field(default=None, metadata=config(field_name="message"))
 
 
 @dataclass_json
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/tokens.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python/utils.py` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,82 @@
 """utils.py
 
 Taegis SDK Python General Utilities"""
 import asyncio
 import concurrent
+import logging
+from dataclasses import fields as dc_fields
 from dataclasses import is_dataclass
 from enum import Enum
 from typing import Any, Callable, Dict, Optional, Union
 
-from graphql.type import (
-    is_union_type as is_gql_union_type,
-    is_wrapping_type,
-    is_scalar_type,
-    is_object_type,
-)
-
+from graphql.type import is_object_type, is_scalar_type
+from graphql.type import is_union_type as is_gql_union_type
+from graphql.type import is_wrapping_type
 from typing_inspect import get_args, is_union_type
 
+log = logging.getLogger(__name__)
+
 
-def build_output_string(dataclass) -> str:
+def build_output_string(cls) -> str:
     """
     Generate GraphQL output string from defined Dataclass.
 
     Parameters
     ----------
     dataclass : dataclass
         Dataclass class reference
 
     Returns
     -------
     str
         GraphQL Output
     """
-    if is_union_type(dataclass):
+    if is_union_type(cls):
         fragments = ["__typename"]
-        for item in get_args(dataclass):
+        for item in get_args(cls):
             output_string = _build_dataclass_string(item)
             fragments.append(f"... on {item.__name__} {{{output_string}}}")
         return "\n".join(fragments)
 
-    return _build_dataclass_string(dataclass)
+    return _build_dataclass_string(cls)
 
 
-def _build_dataclass_string(dataclass) -> str:
+def _build_dataclass_string(cls) -> str:
     """Build output string from a Dataclass."""
 
-    def get_nested_field(dataclass) -> str:
-        fields = []
-        for _, field in dataclass.fields.items():
-            fields.append(field.data_key)
-            if hasattr(field, "nested"):
-                fields.append(f"{{ {get_nested_field(field.nested)} }}")
-            if hasattr(field, "inner") and hasattr(field.inner, "nested"):
-                fields.append(f"{{ {get_nested_field(field.inner.nested)} }}")
-        return " ".join(fields)
+    output_fields = []
+    for field in dc_fields(cls):
+        letter_case = field.metadata.get("dataclasses_json", {}).get("letter_case")
+        if letter_case:
+            field_name = letter_case(...)
+        else:
+            field_name = field.name
+
+        if field.metadata.get("deprecated"):
+            log.warning(
+                f"Output field `{field_name}` is deprecated: "
+                f"'{field.metadata.get('deprecation_reason')}', "
+                "removing from default output..."
+            )
+            continue
 
-    fields = []
-    for _, field in dataclass.schema().declared_fields.items():
-        fields.append(field.data_key)
-        if hasattr(field, "nested"):
-            fields.append(f"{{ {get_nested_field(field.nested)} }}")
-        if hasattr(field, "inner") and hasattr(field.inner, "nested"):
-            fields.append(f"{{ {get_nested_field(field.inner.nested)} }}")
-    return " ".join(fields)
+        output_fields.append(field_name)
+
+        # unwrap the field type
+        # example: Optional[List[List[Event]]]
+        # should submit Event for recursive iteration
+        type_ = field.type
+        while args := get_args(type_):
+            type_ = args[0]
+
+        if is_dataclass(type_):
+            output_fields.append(f"{{ {_build_dataclass_string(type_)} }}")
+
+    return " ".join(output_fields)
 
 
 def graphql_unwrap_field(field: Any) -> Any:
     """
     Unwrap GraphQL objects to the internal scalar/object.
 
     Parameters
@@ -156,14 +167,27 @@
 
     Returns
     -------
     Any
         _description_
     """
     if is_dataclass(value):
+        for field in dc_fields(value):
+            letter_case = field.metadata.get("dataclasses_json", {}).get("letter_case")
+            if letter_case:
+                field_name = letter_case(...)
+            else:
+                field_name = field.name
+
+            if field.metadata.get("deprecated"):
+                log.warning(
+                    f"Input field `{field_name}` is deprecated: "
+                    f"'{field.metadata.get('deprecation_reason')}'"
+                )
+
         # return Dict[str. Any] where Any is not None
         return {
             key: value
             for key, value in value.to_dict(encode_json=True).items()
             if value is not None
         }
     # return value of Enum instead of the object
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/PKG-INFO` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.0a9
+Version: 1.0.0rc1
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -241,7 +241,19 @@
             suspended
             total
         }
     }
 """
 result = service.investigations.execute(gql_query)
 ```
+
+### Deprecation Warnings
+
+Deprecated input fields, output fields and endpoints are set to log a warning.  For more information, see the [docs](docs/deprecation.md).
+
+Example:
+
+```
+GraphQL Query `allInvestigations` is deprecated: 'replaced by investigationsSearch'
+Output field `activity_logs` is deprecated: 'Not Supported - Use audit logs', removing from default output...
+Output field `assignee` is deprecated: 'No longer supported', removing from default output...
+```
```

### Comparing `taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,19 @@
 taegis_sdk_python/services/notifications/subscriptions.py
 taegis_sdk_python/services/notifications/types.py
 taegis_sdk_python/services/preferences/__init__.py
 taegis_sdk_python/services/preferences/mutations.py
 taegis_sdk_python/services/preferences/queries.py
 taegis_sdk_python/services/preferences/subscriptions.py
 taegis_sdk_python/services/preferences/types.py
+taegis_sdk_python/services/roadrunner/__init__.py
+taegis_sdk_python/services/roadrunner/mutations.py
+taegis_sdk_python/services/roadrunner/queries.py
+taegis_sdk_python/services/roadrunner/subscriptions.py
+taegis_sdk_python/services/roadrunner/types.py
 taegis_sdk_python/services/rules/__init__.py
 taegis_sdk_python/services/rules/mutations.py
 taegis_sdk_python/services/rules/queries.py
 taegis_sdk_python/services/rules/subscriptions.py
 taegis_sdk_python/services/rules/types.py
 taegis_sdk_python/services/sharelinks/__init__.py
 taegis_sdk_python/services/sharelinks/mutations.py
```

