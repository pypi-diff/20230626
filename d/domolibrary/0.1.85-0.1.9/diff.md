# Comparing `tmp/domolibrary-0.1.85.tar.gz` & `tmp/domolibrary-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.85.tar", last modified: Mon Jun 26 18:58:59 2023, max compression
+gzip compressed data, was "domolibrary-0.1.9.tar", last modified: Thu Apr 27 13:57:59 2023, max compression
```

## Comparing `domolibrary-0.1.85.tar` & `domolibrary-0.1.9.tar`

### file list

```diff
@@ -1,153 +1,146 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.659714 domolibrary-0.1.85/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.591714 domolibrary-0.1.85/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.85/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-06-01 20:57:16.000000 domolibrary-0.1.85/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.603714 domolibrary-0.1.85/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.85/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.623714 domolibrary-0.1.85/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.85/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.635714 domolibrary-0.1.85/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.85/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-06-01 20:57:16.000000 domolibrary-0.1.85/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.635714 domolibrary-0.1.85/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.85/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-01 20:57:16.000000 domolibrary-0.1.85/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-06-01 20:57:16.000000 domolibrary-0.1.85/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-06-01 20:57:16.000000 domolibrary-0.1.85/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-06-26 18:58:59.659714 domolibrary-0.1.85/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-06-01 20:57:16.000000 domolibrary-0.1.85/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.635714 domolibrary-0.1.85/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   178214 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.643715 domolibrary-0.1.85/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21687 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3001 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21366 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12330 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.643715 domolibrary-0.1.85/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12151 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.643715 domolibrary-0.1.85/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/integrations/Automation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.651714 domolibrary-0.1.85/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/application.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8368 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/job.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/stream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.651714 domolibrary-0.1.85/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-06-26 18:58:12.000000 domolibrary-0.1.85/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-06-26 18:58:13.000000 domolibrary-0.1.85/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.639714 domolibrary-0.1.85/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-06-26 18:58:59.000000 domolibrary-0.1.85/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4106 2023-06-26 18:58:59.000000 domolibrary-0.1.85/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-26 18:58:59.000000 domolibrary-0.1.85/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-06-26 18:58:59.000000 domolibrary-0.1.85/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-01 20:57:34.000000 domolibrary-0.1.85/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-06-26 18:58:59.000000 domolibrary-0.1.85/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-06-26 18:58:59.000000 domolibrary-0.1.85/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-06-26 18:58:31.000000 domolibrary-0.1.85/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-26 18:58:59.659714 domolibrary-0.1.85/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-06-01 20:57:16.000000 domolibrary-0.1.85/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 18:58:59.659714 domolibrary-0.1.85/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-06-01 20:57:16.000000 domolibrary-0.1.85/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-06-01 20:57:16.000000 domolibrary-0.1.85/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-06-01 20:57:16.000000 domolibrary-0.1.85/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-06-01 20:57:16.000000 domolibrary-0.1.85/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-06-01 20:57:16.000000 domolibrary-0.1.85/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.85/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-06-01 20:57:16.000000 domolibrary-0.1.85/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-06-01 20:57:16.000000 domolibrary-0.1.85/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-06-01 20:57:16.000000 domolibrary-0.1.85/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-01 20:57:16.000000 domolibrary-0.1.85/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-06-01 20:57:16.000000 domolibrary-0.1.85/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.375308 domolibrary-0.1.9/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.179308 domolibrary-0.1.9/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.9/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.187308 domolibrary-0.1.9/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.223308 domolibrary-0.1.9/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.9/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.9/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.9/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.9/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.9/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.9/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.9/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.243308 domolibrary-0.1.9/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.9/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.9/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.9/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.9/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.243308 domolibrary-0.1.9/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.9/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.9/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.9/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-27 13:57:59.371308 domolibrary-0.1.9/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.9/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.247308 domolibrary-0.1.9/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   151032 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.259308 domolibrary-0.1.9/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18323 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2076 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25143 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7045 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5045 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6984 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15704 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14378 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.263308 domolibrary-0.1.9/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12088 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.267308 domolibrary-0.1.9/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.303308 domolibrary-0.1.9/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8346 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4533 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3859 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.307308 domolibrary-0.1.9/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.251308 domolibrary-0.1.9/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3874 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.9/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-27 13:57:47.000000 domolibrary-0.1.9/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-27 13:57:59.375308 domolibrary-0.1.9/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.9/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.367308 domolibrary-0.1.9/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.9/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.9/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.9/utils/upload_data.py
```

### Comparing `domolibrary-0.1.85/Automation/automation.py` & `domolibrary-0.1.9/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DataOcean/Transport.py` & `domolibrary-0.1.9/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.9/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.9/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DataOcean/cnfg_s3.py` & `domolibrary-0.1.9/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.9/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoAccount.py` & `domolibrary-0.1.9/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.9/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.9/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoApplication.py` & `domolibrary-0.1.9/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoAuth.py` & `domolibrary-0.1.9/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.9/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoCard.py` & `domolibrary-0.1.9/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoCertification.py` & `domolibrary-0.1.9/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.9/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.9/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoDataset.py` & `domolibrary-0.1.9/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoGrant.py` & `domolibrary-0.1.9/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoGroup.py` & `domolibrary-0.1.9/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.9/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoJob.py` & `domolibrary-0.1.9/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoLineage.py` & `domolibrary-0.1.9/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoPDP.py` & `domolibrary-0.1.9/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoPage.py` & `domolibrary-0.1.9/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoPublish.py` & `domolibrary-0.1.9/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoRole.py` & `domolibrary-0.1.9/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.9/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoStream.py` & `domolibrary-0.1.9/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoTag.py` & `domolibrary-0.1.9/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/DomoUser.py` & `domolibrary-0.1.9/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/get_data.py` & `domolibrary-0.1.9/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/LICENSE` & `domolibrary-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/PKG-INFO` & `domolibrary-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.85
+Version: 0.1.9
+Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# domolibrary: a powerful pydomo alternative
+domolibrary: a powerful pydomo alternative
+================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Formatting
 
 use_snake_case for everything except class names is_bool - prefix any
 boolean parameters with is_bool
@@ -232,7 +235,9 @@
 Consider
 [`query_dataset_private`](https://jaewilson07.github.io/domo_library/routes/dataset.html#query_dataset_private)
 from the `routes.dataset`.
 
 Inside this function we are using
 [`looper`](https://jaewilson07.github.io/domo_library/client/get_data.html#looper)
 from `client.get_data` to paginate over the API response.
+
+
```

### Comparing `domolibrary-0.1.85/README.md` & `domolibrary-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# domolibrary: a powerful pydomo alternative
+domolibrary: a powerful pydomo alternative
+================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Formatting
 
 use_snake_case for everything except class names is_bool - prefix any
 boolean parameters with is_bool
```

### Comparing `domolibrary-0.1.85/domolibrary/_modidx.py` & `domolibrary-0.1.9/domolibrary/_modidx.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,14 @@
                                                                                                                  'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.delete_account': ( 'classes/domoaccount.html#domoaccount.delete_account',
                                                                                                                  'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.generate_create_body': ( 'classes/domoaccount.html#domoaccount.generate_create_body',
                                                                                                                        'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.get_from_id': ( 'classes/domoaccount.html#domoaccount.get_from_id',
                                                                                                               'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount.share': ( 'classes/domoaccount.html#domoaccount.share',
-                                                                                                        'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.share_account': ( 'classes/domoaccount.html#domoaccount.share_account',
                                                                                                                 'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.update_config': ( 'classes/domoaccount.html#domoaccount.update_config',
                                                                                                                 'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount.update_name': ( 'classes/domoaccount.html#domoaccount.update_name',
                                                                                                               'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config': ( 'classes/domoaccount.html#domoaccount_config',
@@ -45,20 +43,14 @@
                                                                                                                                     'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AmazonS3': ( 'classes/domoaccount.html#domoaccount_config_amazons3',
                                                                                                                   'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AmazonS3._from_json': ( 'classes/domoaccount.html#domoaccount_config_amazons3._from_json',
                                                                                                                              'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AmazonS3.to_json': ( 'classes/domoaccount.html#domoaccount_config_amazons3.to_json',
                                                                                                                           'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_Config_AmazonS3Advanced': ( 'classes/domoaccount.html#domoaccount_config_amazons3advanced',
-                                                                                                                          'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_Config_AmazonS3Advanced._from_json': ( 'classes/domoaccount.html#domoaccount_config_amazons3advanced._from_json',
-                                                                                                                                     'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_Config_AmazonS3Advanced.to_json': ( 'classes/domoaccount.html#domoaccount_config_amazons3advanced.to_json',
-                                                                                                                                  'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AwsAthena': ( 'classes/domoaccount.html#domoaccount_config_awsathena',
                                                                                                                    'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AwsAthena._from_json': ( 'classes/domoaccount.html#domoaccount_config_awsathena._from_json',
                                                                                                                               'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AwsAthena.to_json': ( 'classes/domoaccount.html#domoaccount_config_awsathena.to_json',
                                                                                                                            'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_DatasetCopy': ( 'classes/domoaccount.html#domoaccount_config_datasetcopy',
@@ -103,26 +95,14 @@
                                                                                                                      'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog': ( 'classes/domoactivitylog.html#domoactivitylog',
                                                                                                               'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog._process_activity_log_row': ( 'classes/domoactivitylog.html#domoactivitylog._process_activity_log_row',
                                                                                                                                         'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog.get_activity_log': ( 'classes/domoactivitylog.html#domoactivitylog.get_activity_log',
                                                                                                                                'domolibrary/classes/DomoActivityLog.py')},
-            'domolibrary.classes.DomoApplication': { 'domolibrary.classes.DomoApplication.DomoApplication': ( 'classes/domoapplication.html#domoapplication',
-                                                                                                              'domolibrary/classes/DomoApplication.py'),
-                                                     'domolibrary.classes.DomoApplication.DomoApplication._from_json': ( 'classes/domoapplication.html#domoapplication._from_json',
-                                                                                                                         'domolibrary/classes/DomoApplication.py'),
-                                                     'domolibrary.classes.DomoApplication.DomoApplication.find_next_job_schedule': ( 'classes/domoapplication.html#domoapplication.find_next_job_schedule',
-                                                                                                                                     'domolibrary/classes/DomoApplication.py'),
-                                                     'domolibrary.classes.DomoApplication.DomoApplication.get_all_schedules': ( 'classes/domoapplication.html#domoapplication.get_all_schedules',
-                                                                                                                                'domolibrary/classes/DomoApplication.py'),
-                                                     'domolibrary.classes.DomoApplication.DomoApplication.get_from_id': ( 'classes/domoapplication.html#domoapplication.get_from_id',
-                                                                                                                          'domolibrary/classes/DomoApplication.py'),
-                                                     'domolibrary.classes.DomoApplication.DomoApplication.get_jobs': ( 'classes/domoapplication.html#domoapplication.get_jobs',
-                                                                                                                       'domolibrary/classes/DomoApplication.py')},
             'domolibrary.classes.DomoBootstrap': { 'domolibrary.classes.DomoBootstrap.DomoBootstrap': ( 'classes/domobootstrap.html#domobootstrap',
                                                                                                         'domolibrary/classes/DomoBootstrap.py'),
                                                    'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_all': ( 'classes/domobootstrap.html#domobootstrap.get_all',
                                                                                                                 'domolibrary/classes/DomoBootstrap.py'),
                                                    'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_features': ( 'classes/domobootstrap.html#domobootstrap.get_features',
                                                                                                                      'domolibrary/classes/DomoBootstrap.py'),
                                                    'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_pages': ( 'classes/domobootstrap.html#domobootstrap.get_pages',
@@ -134,31 +114,25 @@
             'domolibrary.classes.DomoCard': { 'domolibrary.classes.DomoCard.DomoCard': ( 'classes/domocard.html#domocard',
                                                                                          'domolibrary/classes/DomoCard.py'),
                                               'domolibrary.classes.DomoCard.DomoCard.__post_init__': ( 'classes/domocard.html#domocard.__post_init__',
                                                                                                        'domolibrary/classes/DomoCard.py'),
                                               'domolibrary.classes.DomoCard.DomoCard._from_json': ( 'classes/domocard.html#domocard._from_json',
                                                                                                     'domolibrary/classes/DomoCard.py'),
                                               'domolibrary.classes.DomoCard.DomoCard.display_url': ( 'classes/domocard.html#domocard.display_url',
-                                                                                                     'domolibrary/classes/DomoCard.py'),
-                                              'domolibrary.classes.DomoCard.DomoCard.get_by_id': ( 'classes/domocard.html#domocard.get_by_id',
-                                                                                                   'domolibrary/classes/DomoCard.py'),
-                                              'domolibrary.classes.DomoCard.DomoCard.share': ( 'classes/domocard.html#domocard.share',
-                                                                                               'domolibrary/classes/DomoCard.py')},
+                                                                                                     'domolibrary/classes/DomoCard.py')},
             'domolibrary.classes.DomoDatacenter': { 'domolibrary.classes.DomoDatacenter.DomoDatacenter': ( 'classes/domodatacenter.html#domodatacenter',
                                                                                                            'domolibrary/classes/DomoDatacenter.py'),
                                                     'domolibrary.classes.DomoDatacenter.DomoDatacenter.get_accounts': ( 'classes/domodatacenter.html#domodatacenter.get_accounts',
                                                                                                                         'domolibrary/classes/DomoDatacenter.py'),
                                                     'domolibrary.classes.DomoDatacenter.DomoDatacenter.search_datacenter': ( 'classes/domodatacenter.html#domodatacenter.search_datacenter',
                                                                                                                              'domolibrary/classes/DomoDatacenter.py'),
                                                     'domolibrary.classes.DomoDatacenter.DomoDatacenter.search_datasets': ( 'classes/domodatacenter.html#domodatacenter.search_datasets',
                                                                                                                            'domolibrary/classes/DomoDatacenter.py')},
             'domolibrary.classes.DomoDataflow': { 'domolibrary.classes.DomoDataflow.DomoDataflow': ( 'classes/domodataflow.html#domodataflow',
                                                                                                      'domolibrary/classes/DomoDataflow.py'),
-                                                  'domolibrary.classes.DomoDataflow.DomoDataflow.execute': ( 'classes/domodataflow.html#domodataflow.execute',
-                                                                                                             'domolibrary/classes/DomoDataflow.py'),
                                                   'domolibrary.classes.DomoDataflow.DomoDataflow.get_from_id': ( 'classes/domodataflow.html#domodataflow.get_from_id',
                                                                                                                  'domolibrary/classes/DomoDataflow.py'),
                                                   'domolibrary.classes.DomoDataflow.DomoDataflow_Action': ( 'classes/domodataflow.html#domodataflow_action',
                                                                                                             'domolibrary/classes/DomoDataflow.py'),
                                                   'domolibrary.classes.DomoDataflow.DomoDataflow_Action._from_obj': ( 'classes/domodataflow.html#domodataflow_action._from_obj',
                                                                                                                       'domolibrary/classes/DomoDataflow.py'),
                                                   'domolibrary.classes.DomoDataflow.DomoDataflow_Action_Type': ( 'classes/domodataflow.html#domodataflow_action_type',
@@ -173,28 +147,24 @@
                                                                                                   'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset.__post_init__': ( 'classes/domodataset.html#domodataset.__post_init__',
                                                                                                                 'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset.create': ( 'classes/domodataset.html#domodataset.create',
                                                                                                          'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset.delete': ( 'classes/domodataset.html#domodataset.delete',
                                                                                                          'domolibrary/classes/DomoDataset.py'),
-                                                 'domolibrary.classes.DomoDataset.DomoDataset.delete_partition': ( 'classes/domodataset.html#domodataset.delete_partition',
-                                                                                                                   'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset.display_url': ( 'classes/domodataset.html#domodataset.display_url',
                                                                                                               'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset.get_from_id': ( 'classes/domodataset.html#domodataset.get_from_id',
                                                                                                               'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset.index_dataset': ( 'classes/domodataset.html#domodataset.index_dataset',
                                                                                                                 'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset.list_partitions': ( 'classes/domodataset.html#domodataset.list_partitions',
                                                                                                                   'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset.query_dataset_private': ( 'classes/domodataset.html#domodataset.query_dataset_private',
                                                                                                                         'domolibrary/classes/DomoDataset.py'),
-                                                 'domolibrary.classes.DomoDataset.DomoDataset.share': ( 'classes/domodataset.html#domodataset.share',
-                                                                                                        'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset.upload_data': ( 'classes/domodataset.html#domodataset.upload_data',
                                                                                                               'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_CreateDataset_Error': ( 'classes/domodataset.html#domodataset_createdataset_error',
                                                                                                                       'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_CreateDataset_Error.__init__': ( 'classes/domodataset.html#domodataset_createdataset_error.__init__',
                                                                                                                                'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_DeleteDataset_Error': ( 'classes/domodataset.html#domodataset_deletedataset_error',
@@ -244,19 +214,15 @@
             'domolibrary.classes.DomoGrant': { 'domolibrary.classes.DomoGrant.DomoGrant': ( 'classes/domogrant.html#domogrant',
                                                                                             'domolibrary/classes/DomoGrant.py'),
                                                'domolibrary.classes.DomoGrant.DomoGrant.__eq__': ( 'classes/domogrant.html#domogrant.__eq__',
                                                                                                    'domolibrary/classes/DomoGrant.py'),
                                                'domolibrary.classes.DomoGrant.DomoGrant.__post_init__': ( 'classes/domogrant.html#domogrant.__post_init__',
                                                                                                           'domolibrary/classes/DomoGrant.py'),
                                                'domolibrary.classes.DomoGrant.DomoGrant._from_json': ( 'classes/domogrant.html#domogrant._from_json',
-                                                                                                       'domolibrary/classes/DomoGrant.py'),
-                                               'domolibrary.classes.DomoGrant.DomoGrants': ( 'classes/domogrant.html#domogrants',
-                                                                                             'domolibrary/classes/DomoGrant.py'),
-                                               'domolibrary.classes.DomoGrant.DomoGrants.get_grants': ( 'classes/domogrant.html#domogrants.get_grants',
-                                                                                                        'domolibrary/classes/DomoGrant.py')},
+                                                                                                       'domolibrary/classes/DomoGrant.py')},
             'domolibrary.classes.DomoGroup': { 'domolibrary.classes.DomoGroup.DomoGroup': ( 'classes/domogroup.html#domogroup',
                                                                                             'domolibrary/classes/DomoGroup.py'),
                                                'domolibrary.classes.DomoGroup.DomoGroup.__post_init__': ( 'classes/domogroup.html#domogroup.__post_init__',
                                                                                                           'domolibrary/classes/DomoGroup.py'),
                                                'domolibrary.classes.DomoGroup.DomoGroup._from_group_json': ( 'classes/domogroup.html#domogroup._from_group_json',
                                                                                                              'domolibrary/classes/DomoGroup.py'),
                                                'domolibrary.classes.DomoGroup.DomoGroup._from_grouplist_json': ( 'classes/domogroup.html#domogroup._from_grouplist_json',
@@ -319,72 +285,38 @@
                                                                                                         'domolibrary/classes/DomoGroup.py'),
                                                'domolibrary.classes.DomoGroup.UpdateGroupMembership.__init__': ( 'classes/domogroup.html#updategroupmembership.__init__',
                                                                                                                  'domolibrary/classes/DomoGroup.py')},
             'domolibrary.classes.DomoInstanceConfig': { 'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig': ( 'classes/domoinstanceconfig.html#domoinstanceconfig',
                                                                                                                        'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_allowlist': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_allowlist',
                                                                                                                                      'domolibrary/classes/DomoInstanceConfig.py'),
-                                                        'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_applications': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_applications',
-                                                                                                                                        'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_authorized_domains': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_authorized_domains',
                                                                                                                                               'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_grants': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_grants',
                                                                                                                                   'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_publications': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_publications',
                                                                                                                                         'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_roles': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_roles',
                                                                                                                                  'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.set_allowlist': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.set_allowlist',
                                                                                                                                      'domolibrary/classes/DomoInstanceConfig.py'),
-                                                        'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.set_authorized_domains': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.set_authorized_domains',
-                                                                                                                                              'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.upsert_allowlist': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.upsert_allowlist',
-                                                                                                                                        'domolibrary/classes/DomoInstanceConfig.py'),
-                                                        'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.upsert_authorized_domains': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.upsert_authorized_domains',
-                                                                                                                                                 'domolibrary/classes/DomoInstanceConfig.py')},
-            'domolibrary.classes.DomoJob': { 'domolibrary.classes.DomoJob.DomoJob': ( 'classes/domojob.html#domojob',
-                                                                                      'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoJob._from_json': ( 'classes/domojob.html#domojob._from_json',
-                                                                                                 'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoJob.create_domostats_job': ( 'classes/domojob.html#domojob.create_domostats_job',
-                                                                                                           'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoJob.create_watchdog_job': ( 'classes/domojob.html#domojob.create_watchdog_job',
-                                                                                                          'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoJob.generate_watchdog_body': ( 'classes/domojob.html#domojob.generate_watchdog_body',
-                                                                                                             'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoJob.get_body': ( 'classes/domojob.html#domojob.get_body',
-                                                                                               'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoJob.update_job': ( 'classes/domojob.html#domojob.update_job',
-                                                                                                 'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoTrigger': ( 'classes/domojob.html#domotrigger',
-                                                                                          'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoTrigger_Schedule': ( 'classes/domojob.html#domotrigger_schedule',
-                                                                                                   'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoTrigger_Schedule._from_str': ( 'classes/domojob.html#domotrigger_schedule._from_str',
-                                                                                                             'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoTrigger_Schedule.to_obj': ( 'classes/domojob.html#domotrigger_schedule.to_obj',
-                                                                                                          'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.DomoTrigger_Schedule.to_schedule_obj': ( 'classes/domojob.html#domotrigger_schedule.to_schedule_obj',
-                                                                                                                   'domolibrary/classes/DomoJob.py'),
-                                             'domolibrary.classes.DomoJob.WatchDogType': ( 'classes/domojob.html#watchdogtype',
-                                                                                           'domolibrary/classes/DomoJob.py')},
+                                                                                                                                        'domolibrary/classes/DomoInstanceConfig.py')},
             'domolibrary.classes.DomoPDP': { 'domolibrary.classes.DomoPDP.Dataset_PDP_Policies': ( 'classes/domopdp.html#dataset_pdp_policies',
                                                                                                    'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.__init__': ( 'classes/domopdp.html#dataset_pdp_policies.__init__',
                                                                                                             'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.get_policies': ( 'classes/domopdp.html#dataset_pdp_policies.get_policies',
                                                                                                                 'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.search_pdp_policies': ( 'classes/domopdp.html#dataset_pdp_policies.search_pdp_policies',
                                                                                                                        'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.toggle_dataset_pdp': ( 'classes/domopdp.html#dataset_pdp_policies.toggle_dataset_pdp',
                                                                                                                       'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.PDP_Parameter': ( 'classes/domopdp.html#pdp_parameter',
                                                                                             'domolibrary/classes/DomoPDP.py'),
-                                             'domolibrary.classes.DomoPDP.PDP_Parameter.generate_body_from_parameter': ( 'classes/domopdp.html#pdp_parameter.generate_body_from_parameter',
-                                                                                                                         'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.PDP_Parameter.generate_parameter_simple': ( 'classes/domopdp.html#pdp_parameter.generate_parameter_simple',
                                                                                                                       'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.PDP_Policy': ( 'classes/domopdp.html#pdp_policy',
                                                                                          'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.PDP_Policy._from_json': ( 'classes/domopdp.html#pdp_policy._from_json',
                                                                                                     'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.PDP_Policy.delete_policy': ( 'classes/domopdp.html#pdp_policy.delete_policy',
@@ -401,82 +333,26 @@
                                                                                          'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage._from_adminsummary': ( 'classes/domopage.html#domopage._from_adminsummary',
                                                                                                             'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage._from_bootstrap': ( 'classes/domopage.html#domopage._from_bootstrap',
                                                                                                          'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage._from_content_stacks_v3': ( 'classes/domopage.html#domopage._from_content_stacks_v3',
                                                                                                                  'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.DomoPage._get_domo_groups': ( 'classes/domopage.html#domopage._get_domo_groups',
-                                                                                                          'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.DomoPage._get_domo_owners_from_dd': ( 'classes/domopage.html#domopage._get_domo_owners_from_dd',
-                                                                                                                  'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.DomoPage._get_domo_users': ( 'classes/domopage.html#domopage._get_domo_users',
-                                                                                                         'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.display_url': ( 'classes/domopage.html#domopage.display_url',
                                                                                                      'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.get_accesslist': ( 'classes/domopage.html#domopage.get_accesslist',
                                                                                                         'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.get_by_id': ( 'classes/domopage.html#domopage.get_by_id',
-                                                                                                   'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.DomoPage.share': ( 'classes/domopage.html#domopage.share',
-                                                                                               'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.DomoPage.update_layout': ( 'classes/domopage.html#domopage.update_layout',
-                                                                                                       'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.DomoPages': ( 'classes/domopage.html#domopages',
-                                                                                          'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.DomoPages.get_pages': ( 'classes/domopage.html#domopages.get_pages',
-                                                                                                    'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayout': ( 'classes/domopage.html#pagelayout',
-                                                                                           'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayout._from_json': ( 'classes/domopage.html#pagelayout._from_json',
-                                                                                                      'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayout.generate_new_background_body': ( 'classes/domopage.html#pagelayout.generate_new_background_body',
-                                                                                                                        'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayout.get_body': ( 'classes/domopage.html#pagelayout.get_body',
-                                                                                                    'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutBackground': ( 'classes/domopage.html#pagelayoutbackground',
-                                                                                                     'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutBackground._from_json': ( 'classes/domopage.html#pagelayoutbackground._from_json',
-                                                                                                                'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutBackground.get_body': ( 'classes/domopage.html#pagelayoutbackground.get_body',
-                                                                                                              'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutCompact': ( 'classes/domopage.html#pagelayoutcompact',
-                                                                                                  'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutCompact._from_json': ( 'classes/domopage.html#pagelayoutcompact._from_json',
-                                                                                                             'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutContent': ( 'classes/domopage.html#pagelayoutcontent',
-                                                                                                  'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutContent._from_json': ( 'classes/domopage.html#pagelayoutcontent._from_json',
-                                                                                                             'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutContent.get_body': ( 'classes/domopage.html#pagelayoutcontent.get_body',
-                                                                                                           'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutStandard': ( 'classes/domopage.html#pagelayoutstandard',
-                                                                                                   'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutStandard._from_json': ( 'classes/domopage.html#pagelayoutstandard._from_json',
-                                                                                                              'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutTemplate': ( 'classes/domopage.html#pagelayouttemplate',
-                                                                                                   'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutTemplate._from_json': ( 'classes/domopage.html#pagelayouttemplate._from_json',
-                                                                                                              'domolibrary/classes/DomoPage.py'),
-                                              'domolibrary.classes.DomoPage.PageLayoutTemplate.get_body': ( 'classes/domopage.html#pagelayouttemplate.get_body',
-                                                                                                            'domolibrary/classes/DomoPage.py')},
+                                                                                                   'domolibrary/classes/DomoPage.py')},
             'domolibrary.classes.DomoPublish': { 'domolibrary.classes.DomoPublish.DomoPublication': ( 'classes/domopublish.html#domopublication',
                                                                                                       'domolibrary/classes/DomoPublish.py'),
                                                  'domolibrary.classes.DomoPublish.DomoPublication._from_json': ( 'classes/domopublish.html#domopublication._from_json',
                                                                                                                  'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication.accept_invite_by_id': ( 'classes/domopublish.html#domopublication.accept_invite_by_id',
-                                                                                                                          'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication.create_publication': ( 'classes/domopublish.html#domopublication.create_publication',
-                                                                                                                         'domolibrary/classes/DomoPublish.py'),
                                                  'domolibrary.classes.DomoPublish.DomoPublication.get_from_id': ( 'classes/domopublish.html#domopublication.get_from_id',
                                                                                                                   'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication.get_subscription_invites_list': ( 'classes/domopublish.html#domopublication.get_subscription_invites_list',
-                                                                                                                                    'domolibrary/classes/DomoPublish.py'),
-                                                 'domolibrary.classes.DomoPublish.DomoPublication.update_publication': ( 'classes/domopublish.html#domopublication.update_publication',
-                                                                                                                         'domolibrary/classes/DomoPublish.py'),
                                                  'domolibrary.classes.DomoPublish.DomoPublication_Content': ( 'classes/domopublish.html#domopublication_content',
                                                                                                               'domolibrary/classes/DomoPublish.py'),
                                                  'domolibrary.classes.DomoPublish.DomoPublication_Content._from_json': ( 'classes/domopublish.html#domopublication_content._from_json',
                                                                                                                          'domolibrary/classes/DomoPublish.py'),
                                                  'domolibrary.classes.DomoPublish.DomoPublication_Content.to_api_json': ( 'classes/domopublish.html#domopublication_content.to_api_json',
                                                                                                                           'domolibrary/classes/DomoPublish.py'),
                                                  'domolibrary.classes.DomoPublish.DomoPublication_Subscription': ( 'classes/domopublish.html#domopublication_subscription',
@@ -541,26 +417,14 @@
                                                                                                     'domolibrary/classes/DomoRole.py'),
                                               'domolibrary.classes.DomoRole.SearchRole_NotFound.__init__': ( 'classes/domorole.html#searchrole_notfound.__init__',
                                                                                                              'domolibrary/classes/DomoRole.py'),
                                               'domolibrary.classes.DomoRole.SetRoleGrants_MissingGrants': ( 'classes/domorole.html#setrolegrants_missinggrants',
                                                                                                             'domolibrary/classes/DomoRole.py'),
                                               'domolibrary.classes.DomoRole.SetRoleGrants_MissingGrants.__init__': ( 'classes/domorole.html#setrolegrants_missinggrants.__init__',
                                                                                                                      'domolibrary/classes/DomoRole.py')},
-            'domolibrary.classes.DomoStream': { 'domolibrary.classes.DomoStream.DomoStream': ( 'classes/domostream.html#domostream',
-                                                                                               'domolibrary/classes/DomoStream.py'),
-                                                'domolibrary.classes.DomoStream.DomoStream.create_stream': ( 'classes/domostream.html#domostream.create_stream',
-                                                                                                             'domolibrary/classes/DomoStream.py'),
-                                                'domolibrary.classes.DomoStream.DomoStream.get_stream_by_id': ( 'classes/domostream.html#domostream.get_stream_by_id',
-                                                                                                                'domolibrary/classes/DomoStream.py'),
-                                                'domolibrary.classes.DomoStream.DomoStream.update_stream': ( 'classes/domostream.html#domostream.update_stream',
-                                                                                                             'domolibrary/classes/DomoStream.py'),
-                                                'domolibrary.classes.DomoStream.DomoStream.upsert_connector': ( 'classes/domostream.html#domostream.upsert_connector',
-                                                                                                                'domolibrary/classes/DomoStream.py'),
-                                                'domolibrary.classes.DomoStream.StreamConfig': ( 'classes/domostream.html#streamconfig',
-                                                                                                 'domolibrary/classes/DomoStream.py')},
             'domolibrary.classes.DomoUser': { 'domolibrary.classes.DomoUser.CreateUser_MissingRole': ( 'classes/domouser.html#createuser_missingrole',
                                                                                                        'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.CreateUser_MissingRole.__init__': ( 'classes/domouser.html#createuser_missingrole.__init__',
                                                                                                                 'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser': ( 'classes/domouser.html#domouser',
                                                                                          'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser.__eq__': ( 'classes/domouser.html#domouser.__eq__',
@@ -741,16 +605,14 @@
                                                                                        'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.get_data_aiohttp': ( 'client/get_data.html#get_data_aiohttp',
                                                                                                'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.looper': ( 'client/get_data.html#looper',
                                                                                      'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.looper_aiohttp': ( 'client/get_data.html#looper_aiohttp',
                                                                                              'domolibrary/client/get_data.py')},
-            'domolibrary.integrations.Automation': { 'domolibrary.integrations.Automation.remove_partition_by_x_days': ( 'integrations/automation.html#remove_partition_by_x_days',
-                                                                                                                         'domolibrary/integrations/Automation.py')},
             'domolibrary.integrations.DomoJupyter': { 'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth',
                                                                                                                                 'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth.__post_init__': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth.__post_init__',
                                                                                                                                               'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth._clean_account_admin_accounts': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth._clean_account_admin_accounts',
                                                                                                                                                               'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.DomoJupyterAccount_InstanceAuth._generate_auth': ( 'integrations/domojupyter.html#domojupyteraccount_instanceauth._generate_auth',
@@ -771,20 +633,26 @@
                                                                                                                                      'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GenerateAuth_InvalidDomoInstanceList.__init__': ( 'integrations/domojupyter.html#generateauth_invaliddomoinstancelist.__init__',
                                                                                                                                               'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GetDomains_Query_AuthMatch_Error': ( 'integrations/domojupyter.html#getdomains_query_authmatch_error',
                                                                                                                                  'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GetDomains_Query_AuthMatch_Error.__init__': ( 'integrations/domojupyter.html#getdomains_query_authmatch_error.__init__',
                                                                                                                                           'domolibrary/integrations/DomoJupyter.py'),
+                                                      'domolibrary.integrations.DomoJupyter.GetDomains_Query_Exception_PW_Col_Error': ( 'integrations/domojupyter.html#getdomains_query_exception_pw_col_error',
+                                                                                                                                        'domolibrary/integrations/DomoJupyter.py'),
+                                                      'domolibrary.integrations.DomoJupyter.GetDomains_Query_Exception_PW_Col_Error.__init__': ( 'integrations/domojupyter.html#getdomains_query_exception_pw_col_error.__init__',
+                                                                                                                                                 'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GetInstanceConfig': ( 'integrations/domojupyter.html#getinstanceconfig',
                                                                                                                   'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GetInstanceConfig.__init__': ( 'integrations/domojupyter.html#getinstanceconfig.__init__',
                                                                                                                            'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GetInstanceConfig._retrieve_company_ds': ( 'integrations/domojupyter.html#getinstanceconfig._retrieve_company_ds',
                                                                                                                                        'domolibrary/integrations/DomoJupyter.py'),
+                                                      'domolibrary.integrations.DomoJupyter.GetInstanceConfig.get_domains_with_global_config_auth': ( 'integrations/domojupyter.html#getinstanceconfig.get_domains_with_global_config_auth',
+                                                                                                                                                      'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GetInstanceConfig.get_domains_with_instance_auth': ( 'integrations/domojupyter.html#getinstanceconfig.get_domains_with_instance_auth',
                                                                                                                                                  'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GetJupyter_ErrorRetrievingAccount': ( 'integrations/domojupyter.html#getjupyter_errorretrievingaccount',
                                                                                                                                   'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GetJupyter_ErrorRetrievingAccount.__init__': ( 'integrations/domojupyter.html#getjupyter_errorretrievingaccount.__init__',
                                                                                                                                            'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.GetJupyter_ErrorRetrievingAccountProperty': ( 'integrations/domojupyter.html#getjupyter_errorretrievingaccountproperty',
@@ -847,18 +715,14 @@
                                                                                                   'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.update_account_name': ( 'routes/account.html#update_account_name',
                                                                                                 'domolibrary/routes/account.py')},
             'domolibrary.routes.activity_log': { 'domolibrary.routes.activity_log.get_activity_log_object_types': ( 'routes/activity_log.html#get_activity_log_object_types',
                                                                                                                     'domolibrary/routes/activity_log.py'),
                                                  'domolibrary.routes.activity_log.search_activity_log': ( 'routes/activity_log.html#search_activity_log',
                                                                                                           'domolibrary/routes/activity_log.py')},
-            'domolibrary.routes.application': { 'domolibrary.routes.application.get_application_by_id': ( 'routes/application.html#get_application_by_id',
-                                                                                                          'domolibrary/routes/application.py'),
-                                                'domolibrary.routes.application.get_applications': ( 'routes/application.html#get_applications',
-                                                                                                     'domolibrary/routes/application.py')},
             'domolibrary.routes.bootstrap': { 'domolibrary.routes.bootstrap.get_bootstrap': ( 'routes/bootstrap.html#get_bootstrap',
                                                                                               'domolibrary/routes/bootstrap.py'),
                                               'domolibrary.routes.bootstrap.get_bootstrap_features': ( 'routes/bootstrap.html#get_bootstrap_features',
                                                                                                        'domolibrary/routes/bootstrap.py'),
                                               'domolibrary.routes.bootstrap.get_bootstrap_pages': ( 'routes/bootstrap.html#get_bootstrap_pages',
                                                                                                     'domolibrary/routes/bootstrap.py')},
             'domolibrary.routes.card': { 'domolibrary.routes.card.CardSearch_NotFoundError': ( 'routes/card.html#cardsearch_notfounderror',
@@ -879,66 +743,48 @@
                                                                                                                'domolibrary/routes/datacenter.py'),
                                                'domolibrary.routes.datacenter.Dataflow_Type_Filter_Enum': ( 'routes/datacenter.html#dataflow_type_filter_enum',
                                                                                                             'domolibrary/routes/datacenter.py'),
                                                'domolibrary.routes.datacenter.SearchDatacenter_NoResultsFound': ( 'routes/datacenter.html#searchdatacenter_noresultsfound',
                                                                                                                   'domolibrary/routes/datacenter.py'),
                                                'domolibrary.routes.datacenter.SearchDatacenter_NoResultsFound.__init__': ( 'routes/datacenter.html#searchdatacenter_noresultsfound.__init__',
                                                                                                                            'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.ShareResource_Enum': ( 'routes/datacenter.html#shareresource_enum',
-                                                                                                     'domolibrary/routes/datacenter.py'),
                                                'domolibrary.routes.datacenter.generate_search_datacenter_account_body': ( 'routes/datacenter.html#generate_search_datacenter_account_body',
                                                                                                                           'domolibrary/routes/datacenter.py'),
                                                'domolibrary.routes.datacenter.generate_search_datacenter_body': ( 'routes/datacenter.html#generate_search_datacenter_body',
                                                                                                                   'domolibrary/routes/datacenter.py'),
                                                'domolibrary.routes.datacenter.generate_search_datacenter_filter': ( 'routes/datacenter.html#generate_search_datacenter_filter',
                                                                                                                     'domolibrary/routes/datacenter.py'),
                                                'domolibrary.routes.datacenter.generate_search_datacenter_filter_search_term': ( 'routes/datacenter.html#generate_search_datacenter_filter_search_term',
                                                                                                                                 'domolibrary/routes/datacenter.py'),
                                                'domolibrary.routes.datacenter.get_lineage_upstream': ( 'routes/datacenter.html#get_lineage_upstream',
                                                                                                        'domolibrary/routes/datacenter.py'),
                                                'domolibrary.routes.datacenter.search_datacenter': ( 'routes/datacenter.html#search_datacenter',
-                                                                                                    'domolibrary/routes/datacenter.py'),
-                                               'domolibrary.routes.datacenter.share_resource': ( 'routes/datacenter.html#share_resource',
-                                                                                                 'domolibrary/routes/datacenter.py')},
-            'domolibrary.routes.dataflow': { 'domolibrary.routes.dataflow.execute_dataflow': ( 'routes/dataflow.html#execute_dataflow',
-                                                                                               'domolibrary/routes/dataflow.py'),
-                                             'domolibrary.routes.dataflow.get_dataflow_by_id': ( 'routes/dataflow.html#get_dataflow_by_id',
+                                                                                                    'domolibrary/routes/datacenter.py')},
+            'domolibrary.routes.dataflow': { 'domolibrary.routes.dataflow.get_dataflow_by_id': ( 'routes/dataflow.html#get_dataflow_by_id',
                                                                                                  'domolibrary/routes/dataflow.py')},
             'domolibrary.routes.dataset': { 'domolibrary.routes.dataset.DatasetNotFoundError': ( 'routes/dataset.html#datasetnotfounderror',
                                                                                                  'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.DatasetNotFoundError.__init__': ( 'routes/dataset.html#datasetnotfounderror.__init__',
                                                                                                           'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.QueryRequestError': ( 'routes/dataset.html#queryrequesterror',
                                                                                               'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.QueryRequestError.__init__': ( 'routes/dataset.html#queryrequesterror.__init__',
                                                                                                        'domolibrary/routes/dataset.py'),
-                                            'domolibrary.routes.dataset.ShareDataset_AccessLevelEnum': ( 'routes/dataset.html#sharedataset_accesslevelenum',
-                                                                                                         'domolibrary/routes/dataset.py'),
-                                            'domolibrary.routes.dataset.ShareDataset_Error': ( 'routes/dataset.html#sharedataset_error',
-                                                                                               'domolibrary/routes/dataset.py'),
-                                            'domolibrary.routes.dataset.ShareDataset_Error.__init__': ( 'routes/dataset.html#sharedataset_error.__init__',
-                                                                                                        'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.UploadDataError': ( 'routes/dataset.html#uploaddataerror',
                                                                                             'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.UploadDataError.__init__': ( 'routes/dataset.html#uploaddataerror.__init__',
                                                                                                      'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.create': ( 'routes/dataset.html#create',
                                                                                    'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.delete': ( 'routes/dataset.html#delete',
                                                                                    'domolibrary/routes/dataset.py'),
-                                            'domolibrary.routes.dataset.delete_partition_stage_1': ( 'routes/dataset.html#delete_partition_stage_1',
-                                                                                                     'domolibrary/routes/dataset.py'),
-                                            'domolibrary.routes.dataset.delete_partition_stage_2': ( 'routes/dataset.html#delete_partition_stage_2',
-                                                                                                     'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.generate_create_dataset_body': ( 'routes/dataset.html#generate_create_dataset_body',
                                                                                                          'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.generate_list_partitions_body': ( 'routes/dataset.html#generate_list_partitions_body',
                                                                                                           'domolibrary/routes/dataset.py'),
-                                            'domolibrary.routes.dataset.generate_share_dataset_payload': ( 'routes/dataset.html#generate_share_dataset_payload',
-                                                                                                           'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.get_dataset_by_id': ( 'routes/dataset.html#get_dataset_by_id',
                                                                                               'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.get_schema': ( 'routes/dataset.html#get_schema',
                                                                                        'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.index_dataset': ( 'routes/dataset.html#index_dataset',
                                                                                           'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.index_status': ( 'routes/dataset.html#index_status',
@@ -947,16 +793,14 @@
                                                                                             'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.query_dataset_private': ( 'routes/dataset.html#query_dataset_private',
                                                                                                   'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.query_dataset_public': ( 'routes/dataset.html#query_dataset_public',
                                                                                                  'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.set_dataset_tags': ( 'routes/dataset.html#set_dataset_tags',
                                                                                              'domolibrary/routes/dataset.py'),
-                                            'domolibrary.routes.dataset.share_dataset': ( 'routes/dataset.html#share_dataset',
-                                                                                          'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.upload_dataset_stage_1': ( 'routes/dataset.html#upload_dataset_stage_1',
                                                                                                    'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.upload_dataset_stage_2_df': ( 'routes/dataset.html#upload_dataset_stage_2_df',
                                                                                                       'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.upload_dataset_stage_2_file': ( 'routes/dataset.html#upload_dataset_stage_2_file',
                                                                                                         'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.upload_dataset_stage_3': ( 'routes/dataset.html#upload_dataset_stage_3',
@@ -1011,37 +855,22 @@
                                                                                                           'domolibrary/routes/instance_config.py'),
                                                     'domolibrary.routes.instance_config.get_authorized_domains': ( 'routes/instance_config.html#get_authorized_domains',
                                                                                                                    'domolibrary/routes/instance_config.py'),
                                                     'domolibrary.routes.instance_config.set_allowlist': ( 'routes/instance_config.html#set_allowlist',
                                                                                                           'domolibrary/routes/instance_config.py'),
                                                     'domolibrary.routes.instance_config.set_authorized_domains': ( 'routes/instance_config.html#set_authorized_domains',
                                                                                                                    'domolibrary/routes/instance_config.py')},
-            'domolibrary.routes.job': { 'domolibrary.routes.job.add_job': ('routes/job.html#add_job', 'domolibrary/routes/job.py'),
-                                        'domolibrary.routes.job.generate_body_remote_domostats': ( 'routes/job.html#generate_body_remote_domostats',
-                                                                                                   'domolibrary/routes/job.py'),
-                                        'domolibrary.routes.job.generate_body_watchdog_generic': ( 'routes/job.html#generate_body_watchdog_generic',
-                                                                                                   'domolibrary/routes/job.py'),
-                                        'domolibrary.routes.job.get_jobs': ('routes/job.html#get_jobs', 'domolibrary/routes/job.py'),
-                                        'domolibrary.routes.job.update_job': ('routes/job.html#update_job', 'domolibrary/routes/job.py'),
-                                        'domolibrary.routes.job.update_job_trigger': ( 'routes/job.html#update_job_trigger',
-                                                                                       'domolibrary/routes/job.py')},
-            'domolibrary.routes.page': { 'domolibrary.routes.page.delete_writelock': ( 'routes/page.html#delete_writelock',
-                                                                                       'domolibrary/routes/page.py'),
-                                         'domolibrary.routes.page.get_page_access_list': ( 'routes/page.html#get_page_access_list',
+            'domolibrary.routes.page': { 'domolibrary.routes.page.get_page_access_list': ( 'routes/page.html#get_page_access_list',
                                                                                            'domolibrary/routes/page.py'),
                                          'domolibrary.routes.page.get_page_by_id': ( 'routes/page.html#get_page_by_id',
                                                                                      'domolibrary/routes/page.py'),
                                          'domolibrary.routes.page.get_page_definition': ( 'routes/page.html#get_page_definition',
                                                                                           'domolibrary/routes/page.py'),
                                          'domolibrary.routes.page.get_pages_adminsummary': ( 'routes/page.html#get_pages_adminsummary',
-                                                                                             'domolibrary/routes/page.py'),
-                                         'domolibrary.routes.page.put_writelock': ( 'routes/page.html#put_writelock',
-                                                                                    'domolibrary/routes/page.py'),
-                                         'domolibrary.routes.page.update_page_layout': ( 'routes/page.html#update_page_layout',
-                                                                                         'domolibrary/routes/page.py')},
+                                                                                             'domolibrary/routes/page.py')},
             'domolibrary.routes.pdp': { 'domolibrary.routes.pdp.CreatePolicy_Error': ( 'routes/pdp.html#createpolicy_error',
                                                                                        'domolibrary/routes/pdp.py'),
                                         'domolibrary.routes.pdp.CreatePolicy_Error.__init__': ( 'routes/pdp.html#createpolicy_error.__init__',
                                                                                                 'domolibrary/routes/pdp.py'),
                                         'domolibrary.routes.pdp.PDP_NotRetrieved': ( 'routes/pdp.html#pdp_notretrieved',
                                                                                      'domolibrary/routes/pdp.py'),
                                         'domolibrary.routes.pdp.PDP_NotRetrieved.__init__': ( 'routes/pdp.html#pdp_notretrieved.__init__',
@@ -1057,30 +886,24 @@
                                         'domolibrary.routes.pdp.get_pdp_policies': ( 'routes/pdp.html#get_pdp_policies',
                                                                                      'domolibrary/routes/pdp.py'),
                                         'domolibrary.routes.pdp.toggle_pdp': ('routes/pdp.html#toggle_pdp', 'domolibrary/routes/pdp.py'),
                                         'domolibrary.routes.pdp.update_policy': ( 'routes/pdp.html#update_policy',
                                                                                   'domolibrary/routes/pdp.py')},
             'domolibrary.routes.publish': { 'domolibrary.routes.publish.accept_invite_by_id': ( 'routes/publish.html#accept_invite_by_id',
                                                                                                 'domolibrary/routes/publish.py'),
-                                            'domolibrary.routes.publish.create_publish_job': ( 'routes/publish.html#create_publish_job',
-                                                                                               'domolibrary/routes/publish.py'),
-                                            'domolibrary.routes.publish.generate_publish_body': ( 'routes/publish.html#generate_publish_body',
-                                                                                                  'domolibrary/routes/publish.py'),
                                             'domolibrary.routes.publish.get_publication_by_id': ( 'routes/publish.html#get_publication_by_id',
                                                                                                   'domolibrary/routes/publish.py'),
                                             'domolibrary.routes.publish.get_subscription_invititations': ( 'routes/publish.html#get_subscription_invititations',
                                                                                                            'domolibrary/routes/publish.py'),
                                             'domolibrary.routes.publish.get_subscription_summaries': ( 'routes/publish.html#get_subscription_summaries',
                                                                                                        'domolibrary/routes/publish.py'),
                                             'domolibrary.routes.publish.refresh_publish_jobs': ( 'routes/publish.html#refresh_publish_jobs',
                                                                                                  'domolibrary/routes/publish.py'),
                                             'domolibrary.routes.publish.search_publications': ( 'routes/publish.html#search_publications',
-                                                                                                'domolibrary/routes/publish.py'),
-                                            'domolibrary.routes.publish.udpate_publish_job': ( 'routes/publish.html#udpate_publish_job',
-                                                                                               'domolibrary/routes/publish.py')},
+                                                                                                'domolibrary/routes/publish.py')},
             'domolibrary.routes.role': { 'domolibrary.routes.role.Role_NotRetrieved': ( 'routes/role.html#role_notretrieved',
                                                                                         'domolibrary/routes/role.py'),
                                          'domolibrary.routes.role.Role_NotRetrieved.__init__': ( 'routes/role.html#role_notretrieved.__init__',
                                                                                                  'domolibrary/routes/role.py'),
                                          'domolibrary.routes.role.create_role': ( 'routes/role.html#create_role',
                                                                                   'domolibrary/routes/role.py'),
                                          'domolibrary.routes.role.delete_role': ( 'routes/role.html#delete_role',
@@ -1096,22 +919,14 @@
                                                                                                 'domolibrary/routes/role.py'),
                                          'domolibrary.routes.role.set_default_role': ( 'routes/role.html#set_default_role',
                                                                                        'domolibrary/routes/role.py'),
                                          'domolibrary.routes.role.set_role_grants': ( 'routes/role.html#set_role_grants',
                                                                                       'domolibrary/routes/role.py'),
                                          'domolibrary.routes.role.update_role_metadata': ( 'routes/role.html#update_role_metadata',
                                                                                            'domolibrary/routes/role.py')},
-            'domolibrary.routes.stream': { 'domolibrary.routes.stream.create_stream': ( 'routes/stream.html#create_stream',
-                                                                                        'domolibrary/routes/stream.py'),
-                                           'domolibrary.routes.stream.execute_stream': ( 'routes/stream.html#execute_stream',
-                                                                                         'domolibrary/routes/stream.py'),
-                                           'domolibrary.routes.stream.get_stream_by_id': ( 'routes/stream.html#get_stream_by_id',
-                                                                                           'domolibrary/routes/stream.py'),
-                                           'domolibrary.routes.stream.update_stream': ( 'routes/stream.html#update_stream',
-                                                                                        'domolibrary/routes/stream.py')},
             'domolibrary.routes.user': { 'domolibrary.routes.user.SearchUser_NoResults': ( 'routes/user.html#searchuser_noresults',
                                                                                            'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.SearchUser_NoResults.__init__': ( 'routes/user.html#searchuser_noresults.__init__',
                                                                                                     'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.UserProperty': ( 'routes/user.html#userproperty',
                                                                                    'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.UserProperty.__init__': ( 'routes/user.html#userproperty.__init__',
```

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.9/domolibrary/classes/DomoAccount.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoAccount.ipynb.
 
 # %% auto 0
 __all__ = ['DomoAccount_Config', 'DomoAccount_Config_AbstractCredential', 'DomoAccount_Config_DatasetCopy',
-           'DomoAccount_Config_Governance', 'DomoAccount_Config_AmazonS3', 'DomoAccount_Config_AmazonS3Advanced',
-           'DomoAccount_Config_AwsAthena', 'DomoAccount_Config_HighBandwidthConnector', 'AccountConfig', 'DomoAccount',
+           'DomoAccount_Config_Governance', 'DomoAccount_Config_AmazonS3', 'DomoAccount_Config_AwsAthena',
+           'DomoAccount_Config_HighBandwidthConnector', 'AccountConfig', 'DomoAccount',
            'DomoAccount_DataProviderType_ConfigNotDefined', 'DomoAccount_UpdateName_Error',
            'DomoAccount_CreateAccount_Error', 'DomoAccount_DeleteAccount_Error', 'DomoAccounts']
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 3
 from ..routes.account import ShareAccount_V1_AccessLevel, ShareAccount_V2_AccessLevel, ShareAccount
 
 
@@ -139,48 +139,14 @@
             "secretKey": self.secret_key,
             "bucket": bucket,
             "region": self.region,
         }
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 13
 @dataclass
-class DomoAccount_Config_AmazonS3Advanced(DomoAccount_Config):
-    access_key: str
-    secret_key: str = field(repr=False)
-    bucket: str
-    region: str = "us-west-2"
-    data_provider_type = "amazons3-advanced"
-
-    @classmethod
-    def _from_json(cls, obj):
-
-        dd = util_dd.DictDot(obj)
-
-        return cls(
-            access_key=dd.accessKey,
-            secret_key=dd.secretKey,
-            bucket=dd.bucket,
-            region=dd.region,
-        )
-
-    def to_json(self):
-        if self.bucket.lower().startswith("s3://"):
-            bucket = self.bucket[5:]
-            print(
-                f"🤦‍♀️- Domo bucket expects string without s3:// prefix. Trimming to '{bucket}' for the output")
-        return {
-            "accessKey": self.access_key,
-            "secretKey": self.secret_key,
-            "bucket": bucket,
-            "region": self.region,
-        }
-
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 14
-@dataclass
 class DomoAccount_Config_AwsAthena(DomoAccount_Config):
     aws_access_key: str
     aws_secret_key: str = field(repr=False)
     s3_staging_dir: str
     workgroup: str
 
     region: str = "us-west-2"
@@ -204,15 +170,15 @@
             "awsAccessKey": self.aws_access_key,
             "awsSecretKey": self.aws_secret_key,
             "s3StagingDir": self.s3_staging_dir,
             "region": self.region,
             "workgroup": self.workgroup,
         }
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 15
+# %% ../../nbs/classes/50_DomoAccount.ipynb 14
 @dataclass
 class DomoAccount_Config_HighBandwidthConnector(DomoAccount_Config):
     """ this connector is not enabled by default contact your CSM / AE"""
     
     aws_access_key: str
     aws_secret_key: str = field(repr=False)
     s3_staging_dir: str
@@ -237,34 +203,35 @@
             "awsAccessKey": self.aws_access_key,
             "awsSecretKey": self.aws_secret_key,
             "s3StagingDir": self.s3_staging_dir,
             "region": self.region,
         }
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 18
+# %% ../../nbs/classes/50_DomoAccount.ipynb 17
 class AccountConfig(Enum):
     """
     Enum provides appropriate spelling for data_provider_type and config object.
     The name of the enum should correspond with the data_provider_type with hyphens replaced with underscores.
     """
+
+    amazon_athena_high_bandwidth = DomoAccount_Config_HighBandwidthConnector
+
     abstract_credential_store = DomoAccount_Config_AbstractCredential
 
     dataset_copy = DomoAccount_Config_DatasetCopy
 
     domo_governance_d14c2fef_49a8_4898_8ddd_f64998005600 = DomoAccount_Config_Governance
 
     aws_athena = DomoAccount_Config_AwsAthena
-    amazon_athena_high_bandwidth = DomoAccount_Config_HighBandwidthConnector
 
     amazon_s3 = DomoAccount_Config_AmazonS3
-    amazons3_advanced = DomoAccount_Config_AmazonS3Advanced
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 20
+# %% ../../nbs/classes/50_DomoAccount.ipynb 19
 @dataclass
 class DomoAccount:
     name: str
     data_provider_type: str
 
     id: int = None
     created_dt: dt.datetime = None
@@ -284,15 +251,15 @@
             name=dd.displayName,
             data_provider_type=dd.dataProviderType,
             created_dt=cd.convert_epoch_millisecond_to_datetime(dd.createdAt),
             modified_dt=cd.convert_epoch_millisecond_to_datetime(dd.modifiedAt),
             auth=auth,
         )
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 21
+# %% ../../nbs/classes/50_DomoAccount.ipynb 20
 class DomoAccount_DataProviderType_ConfigNotDefined(de.DomoError):
     def __init__(
         self, account_id, data_provider_type, domo_instance, function_name="_get_config"
     ):
 
         message = f"🛑 data provider type {data_provider_type} for account_id {account_id} not defined yet.  Extend the AccountConfig class"
 
@@ -333,15 +300,15 @@
             function_name = '_get_config'
         )
 
     self.config = AccountConfig[enum_clean].value._from_json(res_config.response)
 
     return self.config
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 22
+# %% ../../nbs/classes/50_DomoAccount.ipynb 21
 @patch_to(DomoAccount, cls_method=True)
 async def get_from_id(
     cls,
     auth: dmda.DomoAuth,
     account_id: int,
     session: httpx.AsyncClient = None,
     return_raw: bool = False,
@@ -371,15 +338,15 @@
     
     except Exception as e:
         print(e)
 
     finally:
         return acc
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 26
+# %% ../../nbs/classes/50_DomoAccount.ipynb 25
 @patch_to(DomoAccount)
 async def update_config(
     self: DomoAccount,
     auth: dmda.DomoAuth = None,
     debug_api: bool = False,
     config: DomoAccount_Config = None,
     session: httpx.AsyncClient = None,
@@ -403,15 +370,15 @@
         return res
 
     await self._get_config(session=session, debug_api=debug_api)
 
     return self
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 29
+# %% ../../nbs/classes/50_DomoAccount.ipynb 28
 class DomoAccount_UpdateName_Error(de.DomoError):
     def __init__(
         self,
         domo_instance,
         status,
         message,
         entity_id,
@@ -460,15 +427,15 @@
             message=res.response,
         )
 
     self = await self.get_from_id(auth=auth, account_id=self.id)
 
     return self
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 33
+# %% ../../nbs/classes/50_DomoAccount.ipynb 32
 class DomoAccount_CreateAccount_Error(de.DomoError):
     def __init__(
         self,
         entity_id,
         domo_instance,
         status,
         message,
@@ -479,15 +446,15 @@
             function_name=function_name,
             entity_id=entity_id,
             domo_instance=domo_instance,
             status=status,
             message=message,
         )
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 34
+# %% ../../nbs/classes/50_DomoAccount.ipynb 33
 @patch_to(DomoAccount, cls_method=True)
 def generate_create_body(cls, account_name, config):
     return {
         "displayName": account_name,
         "dataProviderType": config.data_provider_type,
         "name": config.data_provider_type,
         "configurations": config.to_json(),
@@ -516,15 +483,15 @@
             domo_instance=auth.domo_instance,
             status=res.status,
             message=res.response,
         )
 
     return await cls.get_from_id(auth=auth, account_id=res.response.get("id"))
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 35
+# %% ../../nbs/classes/50_DomoAccount.ipynb 34
 class DomoAccount_DeleteAccount_Error(de.DomoError):
     def __init__(
         self,
         entity_id,
         domo_instance,
         status,
         message,
@@ -561,22 +528,21 @@
             domo_instance=auth.domo_instance,
             status=res.status,
             message=res.response,
         )
 
     return True
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 36
+# %% ../../nbs/classes/50_DomoAccount.ipynb 35
 @patch_to(DomoAccount)
-async def _is_group_ownership_beta(self, auth: dmda.DomoAuth):
+async def _is_group_ownership_beta(self, auth : dmda.DomoAuth):
 
     import domolibrary.classes.DomoBootstrap as dmbs
 
     domo_bsr = dmbs.DomoBootstrap(auth=auth or self.auth)
-    
     domo_feature_ls = await domo_bsr.get_features()
 
     match_accounts_v2 = next(
         (domo_feature for domo_feature in domo_feature_ls if domo_feature.name == 'accounts-v2'), None)
 
     return True if match_accounts_v2 else False
 
@@ -590,28 +556,29 @@
     access_level: ShareAccount = None,  # will default to Read
     debug_api: bool = False,
     debug_prn: bool = False,
     session: httpx.AsyncClient = None,
 ):
     auth = auth or self.auth
 
+    
     if isinstance(auth, dmda.DomoFullAuth) and is_v2 is None:
         is_v2 = await self._is_group_ownership_beta(auth)
 
     if debug_prn:
         print(
             f"ℹ️ - {auth.domo_instance} - {'is' if is_v2 else 'is not'} v2_group_ownership")
 
     if is_v2 is None:
         raise Exception(
             """🛑 ERROR must pass `is_v2` bool to share_accounts function IF NOT pass `dmda.DomoFullAuth`.
 the group management v2 API has a different body.  
 Alternatively pass a full auth object to auto check the bootstrap.
 """)
-
+    
     res = None
 
     if is_v2:
         share_payload = account_routes.generate_share_account_payload_v2(
             user_id=user_id, access_level=access_level or ShareAccount_V2_AccessLevel.CAN_VIEW
         )
 
@@ -641,93 +608,20 @@
 
     if res.status == 200:
         res.response = f"shared {self.id} - {self.name} with {user_id}"
 
     return res
 
 
-
-
 # %% ../../nbs/classes/50_DomoAccount.ipynb 38
-@patch_to(DomoAccount)
-async def share(
-    self: DomoAccount,
-    domo_user = None,
-    domo_group = None,
-    auth: dmda.DomoAuth = None,
-    is_v2: bool = None,
-    access_level: ShareAccount = None,  # will default to Read
-    debug_api: bool = False,
-    debug_prn: bool = False,
-    session: httpx.AsyncClient = None,
-):
-    auth = auth or self.auth
-
-    if isinstance(auth, dmda.DomoFullAuth) and is_v2 is None:
-        is_v2 = await self._is_group_ownership_beta(auth)
-
-    if debug_prn:
-        print(
-            f"ℹ️ - {auth.domo_instance} - {'is' if is_v2 else 'is not'} v2_group_ownership")
-
-    if is_v2 is None:
-        raise Exception(
-            """🛑 ERROR must pass `is_v2` bool to share_accounts function IF NOT passing `dmda.DomoFullAuth`.
-the group management v2 API has a different body.  
-Alternatively pass a full auth object to auto check the bootstrap.
-""")
-
-    res = None
-
-    if is_v2:
-        share_payload = account_routes.generate_share_account_payload_v2(
-            user_id=domo_user.id if domo_user else None, 
-            group_id =  domo_group.id if domo_group else None,
-            access_level=access_level or ShareAccount_V2_AccessLevel.CAN_VIEW
-        )
-
-        res = await account_routes.share_account_v2(
-            auth=auth,
-            account_id=self.id,
-            share_payload=share_payload,
-            debug_api=debug_api,
-            session=session,
-        )
-
-    else:
-        share_payload = account_routes.generate_share_account_payload_v1(
-            user_id=domo_user.id if domo_user else None,
-            group_id=domo_group.id if domo_group else None,
-            
-            access_level=access_level or ShareAccount_V1_AccessLevel.CAN_VIEW
-        )
-
-        res = await account_routes.share_account_v1(
-            auth=auth,
-            account_id=self.id,
-            share_payload=share_payload,
-            debug_api=debug_api,
-            session=session,
-        )
-
-    if res.status == 500 and res.response == 'Internal Server Error':
-        res.response = f'ℹ️ - {res.response + "| User may own account."}'
-
-    if res.status == 200:
-        domo_entity = domo_user or domo_group
-        res.response = f"shared {self.id} - {self.name} with {domo_entity.id}"
-
-    return res
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 41
 @dataclass
 class DomoAccounts:
     auth: dmda.DomoAuth
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 42
+# %% ../../nbs/classes/50_DomoAccount.ipynb 39
 @patch_to(DomoAccounts, cls_method=True)
 async def get_accounts(
     cls: DomoAccounts,
     auth: dmda.DomoAuth,
     account_name: str = None, # account string to search for, must be an exact match in spelling.  case insensitive
     account_type: AccountConfig = None, #to retrieve a specific account type
     debug_api: bool = False,
```

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.9/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.9/domolibrary/classes/DomoBootstrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # %% auto 0
 __all__ = ['DomoBootstrap_Feature', 'DomoBootstrap']
 
 # %% ../../nbs/classes/50_DomoBootstrap.ipynb 2
 from dataclasses import dataclass, field
 from fastcore.basics import patch_to
 import httpx
-import asyncio
 
 import domolibrary.classes.DomoPage as dmpg
 
 import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.Logger as lc
 import domolibrary.routes.bootstrap as bootstrap_routes
@@ -75,15 +74,15 @@
         return res.response
         
     if not res.is_success:
         return None
     
     page_ls = res.response
 
-    self.page_ls =  await asyncio.gather(*[dmpg.DomoPage._from_bootstrap(page_obj, auth = auth) for page_obj in page_ls])
+    self.page_ls =  [dmpg.DomoPage._from_bootstrap(page_obj, auth = auth) for page_obj in page_ls]
 
     return self.page_ls
 
 
 # %% ../../nbs/classes/50_DomoBootstrap.ipynb 11
 @patch_to(DomoBootstrap)
 async def get_features(self : DomoBootstrap,
```

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.9/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.9/domolibrary/classes/DomoDataflow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoDataflow.ipynb.
 
 # %% auto 0
 __all__ = ['DomoDataflow']
 
 # %% ../../nbs/classes/50_DomoDataflow.ipynb 2
+from fastcore.basics import patch_to
+
+# %% ../../nbs/classes/50_DomoDataflow.ipynb 3
 import httpx
 import asyncio
-from fastcore.basics import patch_to
 
 import pandas as pd
 import io
 
 import json
 from enum import Enum
 from dataclasses import dataclass, field
 
 import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.DomoError as de
 import domolibrary.routes.dataflow as dataflow_routes
 
 
-# %% ../../nbs/classes/50_DomoDataflow.ipynb 3
+# %% ../../nbs/classes/50_DomoDataflow.ipynb 4
 class DomoDataflow_Action_Type(Enum):
     LoadFromVault = 'LoadFromVault'
     PublishToVault = 'PublishToVault'
     GenerateTableAction = 'GenerateTableAction'
 
 @dataclass
 class DomoDataflow_Action:
@@ -50,28 +52,28 @@
             id = dd.id,
             name=dd.name or dd.targetTableName or dd.tableName or tbl_name,
             data_source_id = dd.dataSourceId or ds_id,
             sql=dd.selectStatement or dd.query
         )
 
 
-# %% ../../nbs/classes/50_DomoDataflow.ipynb 6
+# %% ../../nbs/classes/50_DomoDataflow.ipynb 7
 @dataclass
 class DomoDataflow:
     id: str
-    name: str = None
+    name: str
     auth : dmda.DomoAuth = field(default = None)
     owner: str = None
     description: str = None
     tags: list[str] = None
     actions: list[DomoDataflow_Action] = None
 
     action : list[DomoDataflow_Action] = field(default = None)
 
-# %% ../../nbs/classes/50_DomoDataflow.ipynb 7
+# %% ../../nbs/classes/50_DomoDataflow.ipynb 8
 @patch_to(DomoDataflow, cls_method = True)
 async def get_from_id(cls: DomoDataflow,
                       dataflow_id: int,
                         auth: dmda.DomoAuth = None,
                         debug_api: bool = False,
                         return_raw: bool = False):
 
@@ -95,17 +97,7 @@
     )
 
     if dd.actions:
         domo_dataflow.actions = [DomoDataflow_Action._from_obj(action) for action in dd.actions]
     
     return domo_dataflow
 
-
-# %% ../../nbs/classes/50_DomoDataflow.ipynb 10
-@patch_to(DomoDataflow)
-async def execute(self: DomoDataflow,
-                  auth: dmda.DomoAuth = None,
-                  debug_api: bool = False):
-
-    return await dataflow_routes.execute_dataflow(auth=auth or self.auth,
-                                                  dataflow_id=self.id, debug_api=debug_api)
-
```

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.9/domolibrary/classes/DomoDataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,14 @@
            'DomoDataset_UploadData_Error', 'DomoDataset_UploadData_DatasetUploadId_Error',
            'DomoDataset_UploadData_UploadData_Error', 'DomoDataset_UploadData_CommitDatasetUploadId_Error',
            'DomoDataset_CreateDataset_Error']
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 4
 from fastcore.basics import patch_to
 import pandas as pd
-from ..routes.dataset import ShareDataset_AccessLevelEnum
-
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 5
 from dataclasses import dataclass, field
 from typing import List, Optional
 from enum import Enum
 
 import json
@@ -277,21 +275,21 @@
     owner: dict = field(default_factory=dict)
     formula: dict = field(default_factory=dict)
 
     schema: DomoDataset_Schema = field(default=None)
     tags: DomoDataset_Tags = field(default=None)
 
     # certification: dmdc.DomoCertification = None
-    PDP: dmpdp.Dataset_PDP_Policies = None
+    PDPPolicies: dmpdp.Dataset_PDP_Policies = None
 
     def __post_init__(self):
         self.schema = DomoDataset_Schema(dataset=self)
         self.tags = DomoDataset_Tags(dataset=self)
 
-        self.PDP = dmpdp.Dataset_PDP_Policies(dataset=self)
+        self.PDPPolicies = dmpdp.Dataset_PDP_Policies(dataset=self)
 
     def display_url(self):
         return f"https://{self.auth.domo_instance }.domo.com/datasources/{self.id}/details/overview"
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 26
 @patch_to(DomoDataset, cls_method=True)
 async def get_from_id(
@@ -345,87 +343,61 @@
 class QueryExecutionError(de.DomoError):
     def __init__(self,
                  sql, dataset_id,
                  domo_instance,
                  status, message,
                  function_name=None ):
         
-        message = f"error executing {sql}: {message}"
+        self.message = f"error executing {sql}: {message}"
 
         super().__init__(entity_id=dataset_id,
                          function_name=function_name,
                          status=status,
                          message=message,
                          domo_instance=domo_instance)
 
 
 @patch_to(DomoDataset, cls_method=True)
 async def query_dataset_private(cls: DomoDataset,
                                 auth: dmda.DomoAuth,  # DomoFullAuth or DomoTokenAuth
                                 dataset_id: str,
                                 sql: str,
                                 session: Optional[httpx.AsyncClient] = None,
-                                filter_pdp_policy_id_ls : [int] = None, # filter by pdp policy
                                 loop_until_end: bool = False,  # retrieve all available rows
-                                
                                 limit=100,  # maximum rows to return per request.  refers to PAGINATION
                                 skip=0,
                                 maximum=100,  # equivalent to the LIMIT or TOP clause in SQL, the number of rows to return total
-                                
                                 debug_api: bool = False,
                                 debug_loop: bool = False,
-                                timeout = 10, # larger API requests may require a longer response time
-                                maximum_retry : int = 5
+                                timeout = 10 # larger API requests may require a longer response time
                                 ) -> pd.DataFrame:
-    
-    res = None
-    retry = 1
-
-    if filter_pdp_policy_id_ls and not isinstance(filter_pdp_policy_id_ls, list):
-        filter_pdp_policy_id_ls = [int(filter_pdp_policy_id_ls)]
 
-    while (not res or not res.is_success) and retry <= maximum_retry:
-        try:
-            res = await dataset_routes.query_dataset_private(auth=auth,
-                                                            dataset_id=dataset_id,
-                                                            sql=sql,
-                                                            maximum=maximum,
-                                                             filter_pdp_policy_id_ls=filter_pdp_policy_id_ls,
-                                                            skip=skip,
-                                                            limit=limit,
-                                                            loop_until_end=loop_until_end,
-                                                            session=session,
-                                                            debug_loop=debug_loop,
-                                                            debug_api=debug_api,
-                                                            timeout = timeout
-                                                            )
-        except dataset_routes.DatasetNotFoundError as e:
-            print(e)
-            return res
-
-        except dataset_routes.QueryRequestError as e:
-            print(e)
-            return res
-
-        except Exception as e:
-            if retry <= maximum_retry:
-                print(f"⚠️ Error.  Attempt {retry} / {maximum_retry} - {e} - while query dataset {dataset_id} in {auth.domo_instance} with {sql}" )
-            retry += 1
+    res = await dataset_routes.query_dataset_private(auth=auth,
+                                                     dataset_id=dataset_id,
+                                                     sql=sql,
+                                                     maximum=maximum,
+                                                     skip=skip,
+                                                     limit=limit,
+                                                     loop_until_end=loop_until_end,
+                                                     session=session,
+                                                     debug_loop=debug_loop,
+                                                     debug_api=debug_api,
+                                                     timeout = timeout
+                                                     )
 
-    if res and not res.is_success:
+    if not res.is_success:
         raise QueryExecutionError(
             status=res.status, message=res.response,
             function_name="query_dataset_private", 
             sql=sql, dataset_id=dataset_id, domo_instance=auth.domo_instance)
-    
 
     return pd.DataFrame(res.response)
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 32
+# %% ../../nbs/classes/50_DomoDataset.ipynb 31
 class DomoDataset_DeleteDataset_Error(de.DomoError):
     def __init__(self,
                  dataset_id,
                  status, reason,
                  domo_instance,
                  function_name
                  ):
@@ -459,44 +431,15 @@
             function_name="DomoDataset.delete",
             domo_instance=auth.domo_instance, 
             status=res.status, reason=res.response)
 
     return res
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 33
-@patch_to(DomoDataset)
-async def share(self: DomoDataset,
-                        member, # DomoUser or DomoGroup
-                        auth: dmda.DomoAuth = None,
-                        share_type: ShareDataset_AccessLevelEnum = ShareDataset_AccessLevelEnum.CAN_SHARE,
-                        is_send_email=False,
-                        debug_api: bool = False,
-                        debug_prn:bool = False,
-                        session: httpx.AsyncClient = None):
-
-    body = dataset_routes.generate_share_dataset_payload(entity_type='GROUP' if type(member).__name__ == 'DomoGroup' else 'USER',
-                                                      entity_id=int(member.id),
-                                                      access_level=share_type,
-                                                      is_send_email=is_send_email)
-    
-    if debug_prn:
-        print(access_list, auth.domo_instance)
-    
-
-    res = await dataset_routes.share_dataset(auth=auth or self.auth,
-                                       dataset_id=self.id,
-                                       body = body,
-                                       session=session,
-                                       debug_api=debug_api)
-    
-    return res
-
-
-# %% ../../nbs/classes/50_DomoDataset.ipynb 37
+# %% ../../nbs/classes/50_DomoDataset.ipynb 34
 class DomoDataset_UploadData_Error(Exception):
 
     def __init__(self,
                  message_error: str,
                  domo_instance: str,
                  dataset_id: str,
                  stage: int,
@@ -549,30 +492,30 @@
 
         super().__init__(message_error=message_error,
                             domo_instance=domo_instance, dataset_id=dataset_id,
                             stage=stage, status=status, reason=reason,
                             partition_key=partition_key)
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 38
+# %% ../../nbs/classes/50_DomoDataset.ipynb 35
 @patch_to(DomoDataset)
 async def index_dataset(self: DomoDataset,
                         auth: dmda.DomoAuth = None,
                         dataset_id: str = None,
                         debug_api: bool = False,
                         session: httpx.AsyncClient = None
                         ):
 
     auth = auth or self.auth
     dataset_id = dataset_id or self.id
     return await dataset_routes.index_dataset(auth=auth, dataset_id=dataset_id, debug_api=debug_api,
                                               session=session)
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 39
+# %% ../../nbs/classes/50_DomoDataset.ipynb 36
 @patch_to(DomoDataset)
 async def upload_data(self : DomoDataset,
                       upload_df: pd.DataFrame = None,
                       upload_df_ls: list[pd.DataFrame] = None,
                       upload_file: io.TextIOWrapper = None,
 
                       upload_method: str = 'REPLACE',  # APPEND or REPLACE
@@ -679,15 +622,15 @@
                                         dataset_id=dataset_id,
                                         debug_api=debug_api,
                                         session=session)
 
     return stage3_res
 
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 41
+# %% ../../nbs/classes/50_DomoDataset.ipynb 38
 @patch_to(DomoDataset)
 async def list_partitions(self : DomoDataset,
                             auth: dmda.DomoAuth = None,
                             dataset_id: str = None,
                             debug_api: bool = False,
                             session: httpx.AsyncClient = None
                             ):
@@ -698,15 +641,15 @@
     res = await dataset_routes.list_partitions(auth=auth, dataset_id=dataset_id, debug_api=debug_api,
                                                 session=session)
     if res.status != 200:
         return None
 
     return res.response
 
-# %% ../../nbs/classes/50_DomoDataset.ipynb 43
+# %% ../../nbs/classes/50_DomoDataset.ipynb 40
 class DomoDataset_CreateDataset_Error(Exception):
     def __init__(self, domo_instance: str, dataset_name: str, status: int, reason: str):
         message = f"Failure to create dataset {dataset_name} in {domo_instance} :: {status} - {reason}"
         super().__init__(message)
 
 
 @patch_to(DomoDataset, cls_method=True)
@@ -735,73 +678,7 @@
             domo_instance=auth.domo_instance, dataset_name=dataset_name, 
             status=res.status, reason=res.response)
 
     dataset_id = res.response.get('dataSource').get('dataSourceId')
 
     return await cls.get_from_id(dataset_id=dataset_id, auth=auth)
 
-
-# %% ../../nbs/classes/50_DomoDataset.ipynb 46
-@patch_to(DomoDataset)
-async def delete_partition(self: DomoDataset,
-                            dataset_partition_id: str,
-                            dataset_id: str = None,
-                            empty_df: pd.DataFrame = None,
-                            auth: dmda.DomoAuth = None,
-                            is_index: bool = True,
-                            debug_api: bool = False
-                            ):
-
-
-
-    auth = auth or self.auth
-    dataset_id = dataset_id or self.id
-
-    if empty_df is None:
-        empty_df = await self.query_dataset_private(auth=auth,
-                                               dataset_id=dataset_id,
-                                               sql="SELECT * from table limit 1",
-                                               debug_api=debug_api)
-
-    await self.upload_data(upload_df=empty_df.head(0),
-                              upload_method='REPLACE',
-                              is_index=is_index,
-                              partition_key=dataset_partition_id,
-                              debug_api=debug_api)
-    if debug_api:
-        print(f"\n\n🎭 starting Stage 1")
-
-    res = await dataset_routes.delete_partition_stage_1(auth=auth,
-                                                       dataset_id=dataset_id,
-                                                           dataset_partition_id=dataset_partition_id,
-                                                        debug_api=debug_api)
-    if debug_api:
-        print(f"\n\n🎭 Stage 1 response -- {res.status}")
-        print(res)
-    
-    stage_2_res = None
-    if debug_api:
-        print('starting Stage 2')
-    
-    stage_2_res = await dataset_routes.delete_partition_stage_2(auth=auth,
-                                                                   dataset_id=dataset_id,
-                                                                dataset_partition_id=dataset_partition_id,
-                                                                debug_api=debug_api)
-    if debug_api:
-        print(f"\n\n🎭 Stage 2 response -- {stage_2_res.status}")
-
-    stage_3_res = None
-    if debug_api:
-        print('starting Stage 3')
-    
-    stage_3_res = await dataset_routes.index_dataset(auth=auth,
-                                                dataset_id=dataset_id,
-                                                   debug_api=debug_api)
-    if debug_api:
-        print(f"\n\n🎭 Stage 3 response -- {stage_3_res.status}")
-
-
-    if debug_api:
-        print(stage_3_res)
-
-    if stage_3_res.status == 200:
-        return res.response
```

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.9/domolibrary/classes/DomoCard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,74 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoGrant.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoCard.ipynb.
 
 # %% auto 0
-__all__ = ['DomoGrant', 'DomoGrants']
+__all__ = ['DomoCard']
 
-# %% ../../nbs/classes/50_DomoGrant.ipynb 2
+# %% ../../nbs/classes/50_DomoCard.ipynb 2
 from dataclasses import dataclass, field
+
+import asyncio
 from fastcore.basics import patch_to
-import httpx
+
+import domolibrary.routes.card as card_routes
 
 import domolibrary.client.DomoAuth as dmda
+import domolibrary.client.DomoError as de
 import domolibrary.utils.DictDot as util_dd
-import domolibrary.routes.grant as grant_routes
-
 
-# %% ../../nbs/classes/50_DomoGrant.ipynb 3
+# %% ../../nbs/classes/50_DomoCard.ipynb 3
 @dataclass
-class DomoGrant:
+class DomoCard:
     id: str
-    display_group: str = None
+    auth: dmda.DomoAuth = field(repr=False)
     title: str = None
-    depends_on_ls: list[str] = None
     description: str = None
-    role_membership_ls: list[str] = field(default=None)
+    type: str = None
+    urn: str = None
+    chart_type: str = None
+    dataset_id: str = None
 
-    def __post_init__(self):
-        self.id = str(self.id)
-
-    def __eq__(self, other):
-        if not isinstance(other, DomoGrant):
-            return False
+    certification: field(default_factory=dict) = None
+    owners: field(default_factory=list) = None
 
-        return self.id == other.id
+    def __post_init__(self):
+        # self.Definition = CardDefinition(self)
+        pass
 
+    def display_url(self) -> str:
+        return f'https://{self.domo_instance}.domo.com/kpis/details/{self.id}'
 
     @classmethod
-    def _from_json(cls, obj):
-
-        dd = obj
-        if not isinstance(dd, util_dd.DictDot):
-            dd = util_dd.DictDot(obj)
-
-        return cls(id=dd.authority,
-                   display_group=dd.authorityUIGroup,
-                   depends_on_ls=dd.dependsOnAuthorities,
-                   title=dd.title,
-                   description=dd.description,
-                   role_membership_ls=[str(role) for role in dd.roleIds])
-
-
-# %% ../../nbs/classes/50_DomoGrant.ipynb 4
-@dataclass
-class DomoGrants:
-    pass
-
+    async def _from_json(cls,
+                  card_obj,
+                   auth: dmda.DomoAuth):
+
+        import domolibrary.classes.DomoUser as dmu
+        import domolibrary.classes.DomoGroup as dmg
+
+        dd = card_obj
+        if isinstance(card_obj, dict):
+            dd = util_dd.DictDot(card_obj)
+
+        card = cls(
+            auth=auth,
+            id=dd.id,
+            title=dd.title,
+            description=dd.description,
+            type=dd.type,
+            urn=dd.urn,
+            certification=dd.certification,
+            chart_type=dd.metadata.chartType,
+            dataset_id = dd.datasources[0].dataSourceId if dd.datasources else None
+        )
+
+        tasks = []
+        for user in dd.owners:
+            if user.type =='USER':
+                tasks.append(dmu.DomoUser.get_by_id(user_id=user.id, auth=auth))
+            if user.type == 'GROUP':
+                tasks.append(dmg.DomoGroup.get_by_id(group_id=group.get('id'), auth=auth))
 
+        card.owners = await asyncio.gather( *tasks)
 
-# %% ../../nbs/classes/50_DomoGrant.ipynb 5
-@patch_to(DomoGrants, cls_method=True)
-async def get_grants(cls: DomoGrants,
-                     auth: dmda.DomoAuth,
-                     session: httpx.AsyncClient = None, debug_api: bool = False, return_raw: bool = False,
-                     ):
-    res = await grant_routes.get_grants(auth=auth, debug_api = debug_api, session = session)
-
-    if return_raw or not res.is_success: 
-        return res
-    
-    return [DomoGrant._from_json(row) for index, row in enumerate(res.response)]
+        return card
```

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.9/domolibrary/classes/DomoGroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 f"➡️ adding {member.id}  of type {type(member).__name__} to {self.group.name}")
 
         if isinstance(member, dmu.DomoUser):
             list_to_update.append({'id': str(member.id), 'type': 'USER'})
 
             return list_to_update
 
-        if isinstance(member, DomoGroup):
+        if isinstance(member, DomoGroup) and not next((user_obj for user_obj in self._add_member_ls if user_obj.id == member.id), None):
             list_to_update.append({'id': str(member.id), 'type': 'GROUP'})
 
             return list_to_update
 
         member_name = getattr(member, 'name', None) or getattr(
             member, 'display_name', None) or "name not provided"
```

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.9/domolibrary/classes/DomoInstanceConfig.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,268 +10,191 @@
 from fastcore.basics import patch_to
 
 
 from dataclasses import dataclass, field
 from typing import List
 
 import domolibrary.client.DomoAuth as dmda
+import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoError as de
-
-
 import domolibrary.routes.instance_config as instance_config_routes
+import domolibrary.routes.grant as grant_routes
+import domolibrary.classes.DomoGrant as dmdg
+import domolibrary.classes.DomoRole as dmr
+import domolibrary.routes.role as role_routes
 import domolibrary.routes.publish as publish_routes
+import domolibrary.classes.DomoPublish as dmpb
 
 # import Library.utils.convert as cd
 # from .DomoApplication import DomoApplication
 
 # import domolibrary.utils.convert as cd
 # import domolibrary.utils.DictDot as util_dd
 # import domolibrary.client.DomoError as de
 
+
 # %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 4
 @dataclass
 class DomoInstanceConfig:
     """utility class that absorbs many of the domo instance configuration methods"""
-
+    
     auth: dmda.DomoAuth
-    allowlist: list[str] = field(default_factory=list)
+    allowlist : list[str] = field(default_factory = list)
 
     @classmethod
-    async def get_publications(
-        cls,
-        auth: dmda.DomoFullAuth,
-        debug_api: bool = False,
-        session: httpx.AsyncClient = None,
-        return_raw: bool = False,
-    ):
-        import domolibrary.classes.DomoPublish as dmpb
-
-
-        res = await publish_routes.search_publications(
-            auth=auth, debug_api=debug_api, session=session
-        )
+    async def get_publications(cls,
+                            auth: dmda.DomoFullAuth,
+                            debug_api: bool = False, session: httpx.AsyncClient = None, return_raw: bool = False):
+        
+        res = await publish_routes.search_publications(auth=auth,
+                                                       debug_api=debug_api,
+                                                       session=session)
         if debug_api:
-            print("Getting Publish jobs")
+            print('Getting Publish jobs')
 
         if res.status == 200 and not return_raw:
-            return await asyncio.gather(
-                *[
-                    dmpb.DomoPublication.get_from_id(
-                        publication_id=job.get("id"), auth=auth
-                    )
-                    for job in res.response
-                ]
-            )
+            return await asyncio.gather(*[dmpb.DomoPublication.get_from_id(publication_id=job.get('id'),
+                                                                           auth=auth) for job in res.response])
 
         if res.status == 200 and return_raw:
             return res.response
 
 # %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 7
 @patch_to(DomoInstanceConfig)
-async def get_allowlist(
-    self: DomoInstanceConfig,
-    auth: dmda.DomoFullAuth = None,  # get_allowlist requires full authentication
-    session: httpx.AsyncClient = None,
-    return_raw: bool = False,
-    debug_api: bool = False,
-) -> list[str]:
+async def get_allowlist(self: DomoInstanceConfig, 
+                        auth: dmda.DomoFullAuth = None, # get_allowlist requires full authentication
+                        session: httpx.AsyncClient = None, 
+                        return_raw : bool = False,
+                        debug_api: bool = False) -> list[str]:
     """retrieves the allowlist for an instance"""
 
     auth = auth or self.auth
-
+    
     res = None
     loop = 0
 
     while not res and loop <= 5:
         try:
-            res = await instance_config_routes.get_allowlist(
-                auth=auth, debug_api=debug_api, session=session
-            )
+            res =  await instance_config_routes.get_allowlist(auth=auth,  debug_api=debug_api, session = session)
         except Exception as e:
             print(e)
         finally:
             loop += 1
 
     if return_raw:
         return res
 
     if not res.is_success:
         return None
 
-    allowlist = res.response.get("addresses")
+    allowlist = res.response.get('addresses')
 
     self.allowlist = allowlist
 
     return allowlist
 
+
 # %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 11
 @patch_to(DomoInstanceConfig)
-async def set_allowlist(
-    self: DomoInstanceConfig,
-    ip_address_ls: list[str],
-    debug_api: bool = False,
-    auth: dmda.DomoFullAuth = None,
-    session: httpx.AsyncClient = None,
-):
+async def set_allowlist(self : DomoInstanceConfig,
+                        ip_address_ls: list[str],
+                        debug_api: bool = False,
+                        auth: dmda.DomoFullAuth = None,
+                        session: httpx.AsyncClient = None
+                        ):
+                        
     auth = auth or self.auth
 
-    await instance_config_routes.set_allowlist(
-        auth=auth, ip_address_ls=ip_address_ls, debug_api=debug_api, session=session
-    )
+    await instance_config_routes.set_allowlist(auth=auth,
+                                               ip_address_ls=ip_address_ls,
+                                               debug_api=debug_api, session=session)
 
     return await self.get_allowlist(auth=auth, debug_api=debug_api, session=session)
 
 
-@patch_to(
-    DomoInstanceConfig,
-)
-async def upsert_allowlist(
-    self: DomoInstanceConfig,
-    ip_address_ls: list[str],
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-    auth: dmda.DomoAuth = None,
-):
-    exist_ip_address_ls = await self.get_allowlist(
-        auth=auth, debug_api=debug_api, session=session
-    )
+@patch_to(DomoInstanceConfig, )
+async def upsert_allowlist(self : DomoInstanceConfig,
+                           ip_address_ls: list[str],
+                           debug_api: bool = False,
+                           session: httpx.AsyncClient = None,
+                           auth: dmda.DomoAuth = None,
+                           ):
+
+    exist_ip_address_ls = await self.get_allowlist(auth=auth, debug_api=debug_api, session=session)
     ip_address_ls += exist_ip_address_ls
 
-    return await self.set_allowlist(
-        auth=auth,
-        ip_address_ls=list(set(ip_address_ls)),
-        debug_api=debug_api,
-        session=session,
-    )
+    return await self.set_allowlist(auth=auth,
+                                   ip_address_ls=list(set(ip_address_ls)),
+                                   debug_api=debug_api, session=session)
+
 
 # %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 16
 @patch_to(DomoInstanceConfig)
-async def get_grants(
-    self: DomoInstanceConfig,
-    auth: dmda.DomoAuth = None,
-    debug_prn: bool = False,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-    return_raw: bool = False,
-):
-    import domolibrary.classes.DomoGrant as dmg
+async def get_grants(self: DomoInstanceConfig,
+                     auth: dmda.DomoAuth = None,
+                     debug_prn:bool = False,
+                     debug_api: bool = False,
+                     session: httpx.AsyncClient = None,
+                     return_raw: bool = False):
 
     auth = auth or self.auth
 
-    return await dmg.DomoGrants.get_grants(auth = auth, return_raw = return_raw, session = session, debug_api = debug_api)
+    res = await grant_routes.get_grants(auth=auth,
+                                        debug_api=debug_api,
+                                        session=session)
+
+    if debug_prn:
+        print(
+            f"ℹ️ - get_instance_grants: {len(res.response)} grants returned from {auth.domo_instance}")
     
 
-# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 19
-@patch_to(DomoInstanceConfig)
-async def get_roles(
-    self,
-    auth: dmda.DomoAuth = None,
-    debug_api: bool = False,
-    return_raw: bool = False,
-    session: httpx.AsyncClient = None,
-):
-    import domolibrary.classes.DomoRole as dmr
 
-    auth = auth or self.auth
+    if return_raw:
+        return res
 
-    return await dmr.DomoRoles.get_roles(auth=auth, debug_api=debug_api, return_raw = return_raw, session=session)
+    if res.status == 200:
+        json_list = res.response
+        return [dmdg.DomoGrant._from_json(obj) for obj in json_list]
 
-# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 23
+
+# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 19
 @patch_to(DomoInstanceConfig)
-async def get_authorized_domains(
-    self: DomoInstanceConfig,
-    auth: dmda.DomoAuth = None,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-    return_raw: bool = False,
-):
-    auth = auth or self.auth
+async def get_roles(self, auth: dmda.DomoAuth = None,
+                    debug_api: bool = False,
+                    return_raw: bool = False,
+                    session: httpx.AsyncClient = None):
 
-    res = await instance_config_routes.get_authorized_domains(
-        auth=auth, debug_api=debug_api, session=session, return_raw=return_raw
-    )
+    auth = auth or self.auth
 
+    res = await role_routes.get_roles(auth=auth,
+                                      debug_api=debug_api, session = session)
+    
     if return_raw:
         return res
 
-    return res.response
-
-# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 26
-@patch_to(DomoInstanceConfig, cls_method=True)
-async def set_authorized_domains(
-    cls: DomoInstanceConfig,
-    auth: dmda.DomoAuth,
-    authorized_domains: list[str],
-    debug_prn: bool = False,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-):
-    if debug_prn:
-        print(f'🌡️ setting authorized domain with {",".join(authorized_domains)}')
-
-    res = await instance_config_routes.set_authorized_domains(
-        auth=auth,
-        authorized_domain_ls=authorized_domains,
-        debug_api=debug_api,
-        session=session,
-    )
-
-    if res.status == 200 or res.status == 204:
-        dmdic = DomoInstanceConfig(auth=auth)
-        res.response = {
-            "authorized_domains": await dmdic.get_authorized_domains(debug_api=debug_api),
-            "status": 200,
-        }
-
-    return res
-
-
-@patch_to(DomoInstanceConfig, cls_method=True)
-async def upsert_authorized_domains(
-    cls: DomoInstanceConfig,
-    auth: dmda.DomoAuth,
-    authorized_domains: list[str],
-    debug_prn: bool = False,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-):
-    existing_domains = await cls.get_authorized_domains(
-        auth=auth, debug_api=debug_api
-    )
-
-    authorized_domains += existing_domains
+    if res.status == 200:
+        json_list = res.response
+        return [dmr.DomoRole._from_json(obj = obj, auth = auth
+                                   ) for obj in json_list]
 
-    if debug_prn:
-        print(f'🌡️ upsertting authorized domain to {",".join(authorized_domains)}')
 
-    return await cls.set_authorized_domains(
-        auth=auth,
-        authorized_domains=authorized_domains,
-        debug_api=debug_api,
-        session=session,
-    )
-
-# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 27
-@patch_to(DomoInstanceConfig, cls_method=True)
-async def get_applications(
-    cls,
-    auth: dmda.DomoAuth,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-    return_raw: bool = False):
-    
-    res = await application_routes.get_applications(
-        auth=auth,
-        debug=debug_api,
-        session=session
-    )
+# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 23
+@patch_to(DomoInstanceConfig)
+async def get_authorized_domains(self: DomoInstanceConfig,
+                                 auth: dmda.DomoAuth = None, 
+                                 debug_api: bool = False,
+                                 session: httpx.AsyncClient = None,
+                                 return_raw :bool = False
+                                 ):
+    auth = auth or self.auth
+                                 
+    res = await instance_config_routes.get_authorized_domains(auth=auth,
+                                                              debug_api=debug_api,
+                                                              session=session,
+                                                              return_raw = return_raw
+                                                              )
 
     if return_raw:
         return res
 
-    if res.status != 200:
-        return res
-    
-    return [DomoApplication._from_json(job) for job in res.response]
-
-
+    return res.response
```

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.9/domolibrary/classes/DomoPDP.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,28 @@
 from enum import Enum, auto
 
 from fastcore.basics import patch_to
 
 import httpx
 import pandas as pd
 
+#from ..utils.chunk_execution import chunk_list
+#from ..utils.DictDot import DictDot
 import domolibrary.utils.DictDot as util_dd
+#from . import DomoCertification as dmdc
+#from .DomoAuth import DomoDeveloperAuth, DomoFullAuth
 import domolibrary.client.DomoAuth as dmda
+#from .routes import pdp_routes
 import domolibrary.routes.pdp as pdp_routes
 import domolibrary.client.DomoError as de
-
-#from ..utils.chunk_execution import chunk_list
-#from . import DomoCertification as dmdc
+import domolibrary.classes.DomoDataset as dmd
 
 
 
 # %% ../../nbs/classes/50_DomoPDP.ipynb 4
-@dataclass
 class PDP_Parameter:
     column_name: str
     column_values_ls: list
     operator: str = 'EQUALS' or 'GREATER_THAN' or 'LESS_THAN' or 'GREATER_THAN_EQUAL' or 'LESS_THAN_EQUAL' or 'BETWEEN'
     ignore_case: bool = True
     type: str = 'COLUMN' or 'DYNAMIC' #column sets parameter on data vs dynamic creates on Domo Trusted Attribute
 
@@ -43,143 +45,119 @@
         return pdp_routes.generate_policy_parameter_simple(column_name=obj.name,
                                                            type=obj.type,
                                                            column_values_ls=obj.values,
                                                            operator=obj.operator,
                                                            ignore_case=obj.ignoreCase
                                                            )
 
-@patch_to(PDP_Parameter)
-def generate_body_from_parameter(self):
-
-        return pdp_routes.generate_policy_parameter_simple(column_name=self.column_name,
-                                                           type=self.type,
-                                                           column_values_ls=self.column_values_ls,
-                                                           operator=self.operator,
-                                                           ignore_case=self.ignore_case
-                                                           )
-
-# %% ../../nbs/classes/50_DomoPDP.ipynb 8
+# %% ../../nbs/classes/50_DomoPDP.ipynb 7
 @dataclass
 class PDP_Policy:
     dataset_id: str
     filter_group_id: str
     name: str
-    # resources: list
+    #resources: list
     parameters_ls: list[dict]
     user_ls: list[str]
     group_ls: list[str]
     virtual_user_ls: list[str]
 
     @classmethod
-    async def _from_json(cls, obj, auth: dmda.DomoAuth):
+    def _from_json(cls, obj):
         dd = util_dd.DictDot(obj)
 
-        import domolibrary.classes.DomoUser as dmu
-        import domolibrary.classes.DomoGroup as dmg
-
         return cls(dataset_id=dd.dataSourceId,
                    filter_group_id=dd.filterGroupId,
                    name=dd.name,
-                   # resources=dd.resources,
+                   #resources=dd.resources,
                    parameters_ls=dd.parameters,
-                   user_ls=await asyncio.gather(* [dmu.DomoUser.get_by_id(user_id=id, auth=auth) for id in dd.userIds]) if dd.userIds else None,
-                   group_ls=await asyncio.gather(*[dmg.DomoGroup.get_by_id(group_id=id, auth=auth) for id in dd.groupIds]) if dd.groupIds else None,
-                   
-                                                                                                                      
+                   user_ls=dd.userIds,
+                   group_ls=dd.groupIds,
                    virtual_user_ls=dd.virtualUserIds)
 
-    @ classmethod
-    async def upsert_policy(cls,
+    @classmethod
+    async def upsert_policy(cls, 
                             auth: dmda.DomoAuth,
                             dataset_id: str,
-                            # body sent to the API (uses camelCase instead of snake_case)
-                            policy_definition: dict,
-                            debug_api: bool=False,
-                            debug_prn: bool=False
+                            policy_definition: dict, # body sent to the API (uses camelCase instead of snake_case)
+                            debug_api: bool = False,
+                            debug_prn: bool = False
                             ):
-
-        # print(policy_definition)
-        policy_id=policy_definition.get('filterGroupId')
+        
+        #print(policy_definition)
+        policy_id = policy_definition.get('filterGroupId')
         if policy_id:
             if debug_prn:
-                print(f'Updating policy {policy_id} in {auth.domo_instance}')
-            res=await pdp_routes.update_policy(auth=auth,
+                print(f'Updating policy {policy_id} in {auth.domo_instance}')    
+            res = await pdp_routes.update_policy(auth=auth,
                                                  dataset_id=dataset_id,
                                                  policy_id=policy_id,
                                                  body=policy_definition,
                                                  debug_api=debug_api)
             return res
         else:
             if debug_prn:
-                print(
-                    f'Policy does not exist. Creating policy in {auth.domo_instance}')
-            res=await pdp_routes.create_policy(auth=auth,
+                print(f'Policy does not exist. Creating policy in {auth.domo_instance}')
+            res = await pdp_routes.create_policy(auth=auth,
                                                  dataset_id=dataset_id,
                                                  body=policy_definition,
                                                  debug_api=debug_api)
             return res
+    
 
-
-# %% ../../nbs/classes/50_DomoPDP.ipynb 10
+# %% ../../nbs/classes/50_DomoPDP.ipynb 9
 @patch_to(PDP_Policy)
 def generate_body_from_policy(
-        self: PDP_Policy
+        self: PDP_Policy, 
         #params: list[dict] = ''
         ):
-        if not self.parameters_ls:
-                raise Exception('generate_body_from_policy: no parameters')
-                
         self.parameters_ls = [PDP_Parameter.generate_parameter_simple(param) for param in self.parameters_ls]
-
-        
         return pdp_routes.generate_policy_body(policy_name=self.name,
                                                dataset_id=self.dataset_id,
                                                parameters_ls=self.parameters_ls,
                                                policy_id=self.filter_group_id,
                                                user_ids=self.user_ls,
                                                group_ids=self.group_ls,
                                                virtual_user_ids=self.virtual_user_ls)
 
-# %% ../../nbs/classes/50_DomoPDP.ipynb 12
+# %% ../../nbs/classes/50_DomoPDP.ipynb 11
 class Dataset_PDP_Policies:
 
-    dataset = None  # domo dataset class
-    policies: list[PDP_Policy] = None 
-    auth = None 
+    dataset: dmd.DomoDataset  # domo dataset class
+    policies: list[PDP_Policy] = None  
 
     def __init__(self, dataset):
         self.dataset = dataset
         self.policies = []
 
-# %% ../../nbs/classes/50_DomoPDP.ipynb 14
+# %% ../../nbs/classes/50_DomoPDP.ipynb 13
 @patch_to(Dataset_PDP_Policies)
 async def get_policies(
-        self: Dataset_PDP_Policies,
-        include_all_rows : bool = True, 
+        self: Dataset_PDP_Policies, 
         auth: dmda.DomoAuth = None, 
         dataset_id: str = None, 
         return_raw: bool = False,
         debug_api: bool = False
     ):
-        
+
         dataset_id = dataset_id or self.dataset.id
         auth = auth or self.dataset.auth
 
-        res = await pdp_routes.get_pdp_policies(auth=auth, dataset_id=dataset_id, debug_api=debug_api, include_all_rows=include_all_rows)
+        res = await pdp_routes.get_pdp_policies(auth=auth, dataset_id=dataset_id, debug_api=debug_api)
 
         if return_raw:
               return res
 
         if res.status == 200:
-            domo_policy = await asyncio.gather(*[PDP_Policy._from_json(
-                policy_obj, auth = auth) for policy_obj in res.response])
+            domo_policy = [PDP_Policy._from_json(
+                policy_obj) for policy_obj in res.response]
             self.policies = domo_policy
             return domo_policy
 
-# %% ../../nbs/classes/50_DomoPDP.ipynb 23
+# %% ../../nbs/classes/50_DomoPDP.ipynb 22
 class SearchPDP_NotFound(de.DomoError):
     def __init__(self, 
                  domo_instance,
                  dataset_id,
                  message='not found',
                  function_name='search_pdp'):
 
@@ -239,15 +217,15 @@
             message=f'There is no policy id "{search}" on dataset_id {dataset_id}',
             domo_instance=auth.domo_instance
         )  
           
     return policy_search    
     
 
-# %% ../../nbs/classes/50_DomoPDP.ipynb 27
+# %% ../../nbs/classes/50_DomoPDP.ipynb 26
 @patch_to(PDP_Policy)
 async def delete_policy(
     self: PDP_Policy, 
     auth: dmda.DomoAuth, 
     policy_id: str = None,
     dataset_id: str = None, 
     debug_api: bool = False
@@ -256,29 +234,27 @@
     dataset_id = dataset_id or self.dataset_id
     policy_id = policy_id or self.filter_group_id
 
     res = await pdp_routes.delete_policy(auth=auth, dataset_id=dataset_id, policy_id=policy_id, debug_api=debug_api)
     
     return res
 
-# %% ../../nbs/classes/50_DomoPDP.ipynb 31
+# %% ../../nbs/classes/50_DomoPDP.ipynb 30
 @patch_to(Dataset_PDP_Policies)
 async def toggle_dataset_pdp(
     self: Dataset_PDP_Policies,
-    auth: dmda.DomoAuth = None,
+    auth: dmda.DomoAuth,
     dataset_id: str = None,
     is_enable: bool = True, # True will enable pdp, False will disable pdp
     debug_api: bool = False,
     session: httpx.AsyncClient = None
 ):
-    auth = auth or self.dataset.auth
-
 
     return await pdp_routes.toggle_pdp(
-        auth=auth,
-        dataset_id=dataset_id or self.dataset.id,
+        auth=auth or self.auth,
+        dataset_id=dataset_id or self.dataset_id,
         is_enable=is_enable,
         debug_api=debug_api,
         session=session
     )
```

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.9/domolibrary/classes/DomoRole.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     # validate grants
     await asyncio.sleep(2)
 
     all_grants = await self.get_grants(auth=auth,
                                         debug_api=debug_api)
 
     missing_grants = [
-        grant.id for grant in domo_grants if grant not in all_grants]
+        grant.id for domo_grant in domo_grants if domo_grant not in all_grants]
 
     if missing_grants:
         raise SetRoleGrants_MissingGrants(
             role_id=role_id, missing_grants=missing_grants, domo_instance=auth.domo_instance)
 
     return domo_grants
```

### Comparing `domolibrary-0.1.85/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.9/domolibrary/classes/DomoUser.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         user_property_ls = property_ls,
         debug_api=debug_api,
         session = session
     )
     if return_raw:
         return res
 
-    self = await DomoUser.get_by_id(user_id = self.id, auth = auth)
+    self = await DomoUser.get_by_id(user_id =1681443709, auth = auth)
 
     return self
 
 # %% ../../nbs/classes/50_DomoUser.ipynb 17
 @dataclass
 class DomoUsers:
     """a class for searching for Users"""
```

### Comparing `domolibrary-0.1.85/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.9/domolibrary/client/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/client/DomoError.py` & `domolibrary-0.1.9/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/client/Logger.py` & `domolibrary-0.1.9/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.9/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/client/get_data.py` & `domolibrary-0.1.9/domolibrary/client/get_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     headers: Optional[dict] = None,
     body: Union[dict, str, None] = None,
     params: Optional[dict] = None,
     debug_api: bool = False,
     session: httpx.AsyncClient = None,
     return_raw: bool = False,
     is_follow_redirects: bool = False,
-    timeout = 10
+    timeout = 5
 ) -> rgd.ResponseGetData:
     """async wrapper for asyncio requests"""
 
     if debug_api:
         print("🐛 debugging get_data")
 
     if auth and not auth.token:
@@ -264,15 +264,14 @@
     allRows = []
     isLoop = True
 
     res = None
 
     if maximum < limit and not loop_until_end:
         limit = maximum
-    
 
     while isLoop:
         params = fixed_params or {}
 
         if offset_params_in_body:
             body[offset_params.get("offset")] = skip
             body[offset_params.get("limit")] = limit
@@ -305,46 +304,44 @@
             debug_api=debug_api,
             timeout = timeout
         )
 
         if not res.is_success:
             if is_close_session:
                 await session.aclose()
-                
             return res
 
         try:
             newRecords = arr_fn(res)
 
         except Exception as e:
             await session.aclose()
             raise LooperError(loop_stage="processing arr_fn", message=str(e)) from e
 
         allRows += newRecords
 
         if loop_until_end and len(newRecords) != 0:
             maximum = maximum + limit
-        
 
         if debug_loop:
             print({"all_rows": len(allRows), "new_records": len(newRecords)})
 
         if len(allRows) >= maximum or len(newRecords) == 0:
             if debug_loop:
                 print(
                     f"\n🎉 Success - {len(allRows)} records retrieved from {url} in query looper\n"
                 )
 
             break
 
         skip += len(newRecords)
 
-        if skip + limit > maximum and not loop_until_end:
+        if skip + limit > maximum:
             limit = maximum - len(allRows)
-        
+
         if debug_loop:
             print(f"skip: {skip}, limit: {limit}")
         
         time.sleep(wait_sleep)
 
     if is_close_session:
         await session.aclose()
```

### Comparing `domolibrary-0.1.85/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.9/domolibrary/integrations/DomoJupyter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/integrations/DomoJupyter.ipynb.
 
 # %% auto 0
 __all__ = ['GetJupyter_ErrorRetrievingAccount', 'GetJupyter_ErrorRetrievingAccountProperty', 'get_jupyter_account',
            'NoConfigCompanyError', 'GetInstanceConfig', 'InvalidAccountTypeError', 'DomoJupyterAccount_InstanceAuth',
            'GetDomains_Query_AuthMatch_Error', 'InvalidAccountNameError', 'GenerateAuth_InvalidDomoInstanceList',
-           'GenerateAuth_CredentialsNotProvided']
+           'GenerateAuth_CredentialsNotProvided', 'GetDomains_Query_Exception_PW_Col_Error']
 
 # %% ../../nbs/integrations/DomoJupyter.ipynb 2
 from dataclasses import dataclass, field
 from typing import Optional
 from enum import Enum
 
 
@@ -123,30 +123,29 @@
         )
 
         if debug_prn:
             print(message)
 
         self.logger.log_info(message, debug_log=debug_log)
 
-        config_df = await ds.query_dataset_private(
-            auth=config_auth, dataset_id=dataset_id, sql=sql, debug_api=debug_api,
-            loop_until_end = True
+        df = await ds.query_dataset_private(
+            auth=config_auth, dataset_id=dataset_id, sql=sql, debug_api=debug_api
         )
-        if len(config_df.index) == 0:
+        if len(df.index) == 0:
             raise NoConfigCompanyError(sql, domo_instance=config_auth.domo_instance)
 
-        self.config = config_df
+        self.config = df
 
-        message = f"\n⚙️ SUCCESS 🎉 Retrieved company list \nThere are {len(config_df.index)} companies to update"
+        message = f"\n⚙️ SUCCESS 🎉 Retrieved company list \nThere are {len(df.index)} companies to update"
 
         if debug_prn:
             print(message)
         self.logger.log_info(message, debug_log=debug_log)
 
-        return config_df
+        return df
 
 # %% ../../nbs/integrations/DomoJupyter.ipynb 8
 class InvalidAccountTypeError(Exception):
     """raised when account type is not expected type"""
 
     def __init__(self, account_name, account_type):
 
@@ -211,88 +210,77 @@
         )
         super().__init__(self.message)
 
 
 @patch_to(GetInstanceConfig, cls_method=True)
 async def get_domains_with_instance_auth(
     cls: GetInstanceConfig,
+    config_dataset_id: str,  # dataset_id to run config_sql query against
+    config_auth: dmda.DomoAuth,  # which instance to retrieve configuration data from
     default_auth: dmda.DomoAuth,  # default auth to use with each row
     auth_enum: Enum,  # Enum where enum_name should match to `auth_match_col` from config_sql query and enum_value is the appropriate DomoAuth or DomoJupyterAccount object
-    config_auth: dmda.DomoAuth = None,  # which instance to retrieve configuration data from
-    config_dataset_id: str = None,  # dataset_id to run config_sql query against
     config_sql: str = "select domain as domo_instance,concat(config_useprod, '-', project) as auth_match_col from table",
-    config_df: pd.DataFrame = None,
     debug_api: bool = False,
     debug_log: bool = False,
     debug_prn: bool = False,
     logger: lc.Logger = None,  # pass in Logger class
 ) -> pd.DataFrame:  # returns a dataframe with domo_instance, instance_auth, and binary column is_valid
     """uses a sql query to retrieve a list of domo_instances and map authentication object to each instance"""
 
     if not logger:
         logger = lc.Logger(app_name="get_domains_with_instance_auth")
 
     gic = cls(logger=logger)
 
-    config_df = config_df if isinstance(config_df, pd.DataFrame) else await gic._retrieve_company_ds(
+    df = await gic._retrieve_company_ds(
         config_auth=config_auth,
         dataset_id=config_dataset_id,
         sql=config_sql,
         debug_prn=debug_prn,
         debug_log=debug_log,
         debug_api=debug_api,
     )
 
-    if "auth_match_col" not in config_df.columns:
+    if "auth_match_col" not in df.columns:
         message = f"Query failed to return a column 'auth_match_col' sql = {config_sql} in {config_auth.domo_instance}"
         raise GetDomains_Query_AuthMatch_Error(message)
 
-    for index, instance in config_df.iterrows():
-        
-        domo_instance = instance["domo_instance"]  
-         
-        auth_match = instance["auth_match_col"]
-        creds = auth_enum[auth_match].value if auth_match in auth_enum._member_names_ else default_auth
-        
-        
-        if isinstance(creds, DomoJupyterAccount_InstanceAuth):
-            creds = creds._generate_auth(domo_instance=domo_instance)
-            creds.domo_instance = domo_instance
-        
-        config_df.at[index, "instance_auth"] = creds
+    for index, instance in df.iterrows():
 
-        if 'config_1' in auth_enum._member_names_  :
-            if debug_prn:
-                print("adding config_auth objects")
+        match_auth = next(
+            (
+                member.value
+                for member in auth_enum
+                if member.name == instance["auth_match_col"]
+            )
+        )
+
+        creds = match_auth or default_auth
 
-            if instance['config_exception_pw'] == 0:
-                auth  = auth_enum['config_1'].value
-            
-            elif instance['config_exception_pw'] == 1:
-                auth  = auth_enum['config_0'].value
-            
-            if isinstance(auth, DomoJupyterAccount_InstanceAuth):
-                auth = auth._generate_auth(domo_instance=domo_instance)
-                auth.domo_instance = domo_instance
-            
-            config_df.at[index, 'config_auth'] = auth
+        domo_instance = instance["domo_instance"]
+
+        creds.domo_instance = domo_instance
+
+        if isinstance(creds, DomoJupyterAccount_InstanceAuth):
+            creds = creds._generate_auth(domo_instance=domo_instance)
 
         try:
             await creds.get_auth_token(debug_api=debug_api)
-            config_df.at[index, "is_valid"] = 1
+            df.at[index, "is_valid"] = 1
 
         except dmda.InvalidCredentialsError as e:
             if debug_prn:
                 print(e)
 
             logger.log_error(str(e))
-            config_df.at[index, "is_valid"] = 0
+            df.at[index, "is_valid"] = 0
 
+        df.at[index, "instance_auth"] = creds
 
-    return config_df
+    return df
 
 # %% ../../nbs/integrations/DomoJupyter.ipynb 13
 class InvalidAccountNameError(Exception):
     """raised when account name does not follow format string"""
 
     def __init__(self, account_name=None, regex_pattern=None):
         account_str = f'"{account_name}" '
@@ -396,7 +384,76 @@
     self.auth_ls = []
     for domo_instance in self.domo_instance_ls:
         auth = self._generate_auth(domo_instance)
 
         self.auth_ls.append(auth)
 
     return self.auth_ls
+
+# %% ../../nbs/integrations/DomoJupyter.ipynb 20
+class GetDomains_Query_Exception_PW_Col_Error(Exception):
+    """raise if SQL query fails to return column named 'config_exception_pw'"""
+
+    def __init__(self, sql: str = None, domo_instance: str = None, message: str = None):
+        message = (
+            message
+            or f"Query failed to return a column 'config_exception_pw' sql = {sql} in {domo_instance}"
+        )
+        super().__init__(self, message)
+
+
+@patch_to(GetInstanceConfig, cls_method=True)
+async def get_domains_with_global_config_auth(
+    cls: GetInstanceConfig,
+    config_dataset_id: str,
+    config_auth: dmda.DomoAuth,  # which instance to retrieve configuration data from
+    global_auth: dmda.DomoAuth,  # global authentication credentials
+    global_exception_auth: dmda.DomoAuth,  # exception credentials (ex 24 char password)
+    # must return a column named domo_instance, if there is an exception_auth, must return a column 'config_exception_pw'
+    config_sql: str = "select domain as domo_instance, config_exception_pw from table",
+    debug_api: bool = False,
+    debug_log: bool = False,
+    debug_prn: bool = False,
+    logger: lc.Logger = None,
+) -> pd.DataFrame:
+    if not logger:
+        logger = lc.Logger(app_name="get_domains_with_global_config_auth")
+
+    gic = cls(logger=logger)
+
+    df = await gic._retrieve_company_ds(
+        config_auth=config_auth,
+        dataset_id=config_dataset_id,
+        sql=config_sql,
+        debug_prn=debug_prn,
+        debug_log=debug_log,
+        debug_api=debug_api,
+    )
+
+    if "config_exception_pw" not in df.columns:
+        message = f"Query failed to return a column 'config_exception_pw' sql = {config_sql} in {config_auth.domo_instance}"
+        gic.logger.log_error(message)
+        raise GetDomains_Query_Exception_PW_Col_Error(message=message)
+
+    for index, instance in df.iterrows():
+        creds = global_auth
+
+        if instance["config_exception_pw"] == 1:
+            creds = global_exception_auth
+
+        creds.domo_instance = instance["domo_instance"]
+
+        try:
+            await creds.get_auth_token()
+            df.at[index, "is_valid"] = 1
+
+        except dmda.InvalidCredentialsError as e:
+            if debug_prn:
+                print(e)
+
+            logger.log_error(str(e))
+            df.at[index, "is_valid"] = 0
+
+        finally:
+            df.at[index, "instance_auth"] = creds
+
+    return df
```

### Comparing `domolibrary-0.1.85/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.9/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/routes/account.py` & `domolibrary-0.1.9/domolibrary/routes/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -179,47 +179,34 @@
         session=session
     )
 
 # %% ../../nbs/routes/account.ipynb 19
 class ShareAccount():
     pass
 
-
 class ShareAccount_V1_AccessLevel(ShareAccount, Enum):
     CAN_VIEW = 'READ'
 
 
 class ShareAccount_V2_AccessLevel(ShareAccount, Enum):
     CAN_VIEW = 'CAN_VIEW'
     CAN_EDIT = 'CAN_EDIT'
     CAN_SHARE = 'CAN_SHARE'
 
 
-def generate_share_account_payload_v1(
-    access_level: ShareAccount,
-    user_id: int = None,
-    group_id: int = None
-):
-    if user_id:
-        return {"type": "USER", "id": int(user_id), "permissions": [access_level.value]}
-    if group_id:
-        return {"type": "GROUP", "id": int(group_id), "permissions": [access_level.value]}
-
-
-def generate_share_account_payload_v2(
-    access_level: ShareAccount,
-    user_id: int = None,
-    group_id: int = None
-):
+def generate_share_account_payload_v1(user_id: int,
+                                      access_level: ShareAccount):
+    return {"type": "USER", "id": int(user_id), "permissions": [access_level.value]}
+
 
-    if user_id:
-        return {"type": "USER", "id": int(user_id), "accessLevel": access_level.value}
+def generate_share_account_payload_v2(user_id: int,
+                                      access_level: ShareAccount
+                                      ):
 
-    if group_id:
-        return {"type": "GROUP", "id": int(group_id), "accessLevel": access_level.value}
+    return {"type": "USER", "id": int(user_id), "accessLevel": access_level.value}
 
 
 # %% ../../nbs/routes/account.ipynb 21
 async def share_account_v2(auth: dmda.DomoAuth,
                            account_id: str,
                            share_payload: dict,
                            debug_api: bool = False,
```

### Comparing `domolibrary-0.1.85/domolibrary/routes/activity_log.py` & `domolibrary-0.1.9/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.9/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/routes/card.py` & `domolibrary-0.1.9/domolibrary/routes/card.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,65 +26,59 @@
                   message = None,
                  ):
         super().__init__(status=status,
                          message=f"card {card_id} not found", domo_instance=domo_instance, function_name=function_name)
 
 
 # %% ../../nbs/routes/card.ipynb 4
-async def get_kpi_definition(auth: dmda.DomoAuth, card_id: str, debug_api: bool = False, session: httpx.AsyncClient = None) -> rgd.ResponseGetData:
+async def get_kpi_definition(auth: dmda.DomoAuth, card_id: str, debug_api: bool = False) -> rgd.ResponseGetData:
 
     url = f"https://{auth.domo_instance}.domo.com/api/content/v3/cards/kpi/definition"
 
     body = {"urn": card_id}
 
     res = await gd.get_data(
         auth=auth,
         url=url,
         method='PUT',
         body=body,
-        debug_api=False,
-        session = session
+        debug_api=False
     )
 
     if not res.is_success and res.response == 'Not Found':
         raise CardSearch_NotFoundError(card_id=card_id,
                                        status=res.status,
                                        domo_instance=auth.domo_instance, 
                                        function_name='get_kpi_definition')
 
     return res
 
 
 # %% ../../nbs/routes/card.ipynb 7
-async def get_card_metadata(auth: dmda.DomoAuth, card_id: str,
-                            debug_api: bool = False, 
-                            session: httpx.AsyncClient = None) -> rgd.ResponseGetData:
+async def get_card_metadata(auth: dmda.DomoAuth, card_id: str, debug_api: bool = False) -> rgd.ResponseGetData:
     optional_params = "metadata,certification,datasources,owners,problems"
-    
     url = f"https://{auth.domo_instance}.domo.com/api/content/v1/cards?urns={card_id}&parts={optional_params}"
 
     res = await gd.get_data(
         auth=auth,
         url=url,
         method='GET',
-        debug_api=debug_api,
-        session=session
+        debug_api=debug_api
     )
 
-    if res.is_success and len(res.response) == 0:
+    if res.is_success and len( res.response) == 0:
         raise CardSearch_NotFoundError(card_id=card_id,
                                        status=res.status,
                                        domo_instance=auth.domo_instance,
                                        function_name='get_kpi_definition')
 
     res.response = res.response[0]
 
     return res
 
-
 # %% ../../nbs/routes/card.ipynb 10
 def generate_body_search_cards_admin_summary(page_ids: [str] = None,
                                              searchPages: bool = True,
                                              cardSearchText: str = '',
                                              pageSearchText: str = '') -> dict:
     body = {
         "ascending": True,
```

### Comparing `domolibrary-0.1.85/domolibrary/routes/datacenter.py` & `domolibrary-0.1.9/domolibrary/routes/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,297 +1,324 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/datacenter.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/user.ipynb.
 
 # %% auto 0
-__all__ = ['Datacenter_Enum', 'Dataflow_Type_Filter_Enum', 'Datacenter_Filter_Field_Enum', 'generate_search_datacenter_filter',
-           'generate_search_datacenter_filter_search_term', 'generate_search_datacenter_body',
-           'generate_search_datacenter_account_body', 'SearchDatacenter_NoResultsFound', 'search_datacenter',
-           'get_lineage_upstream', 'ShareResource_Enum', 'share_resource']
+__all__ = ['get_all_users', 'get_by_id', 'generate_search_users_body_by_id', 'generate_search_users_body_by_email',
+           'process_v1_search_users', 'SearchUser_NoResults', 'search_users',
+           'search_virtual_user_by_subscriber_instance', 'create_user', 'set_user_landing_page', 'reset_password',
+           'request_password_reset', 'UserProperty_Type', 'UserProperty', 'generate_patch_user_property_body',
+           'update_user']
 
-# %% ../../nbs/routes/datacenter.ipynb 2
+# %% ../../nbs/routes/user.ipynb 3
 from enum import Enum
-from typing import Union
 import httpx
+import asyncio
 
+import utils.DictDot as dd
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
-import domolibrary.client.DomoError as de
 import domolibrary.client.DomoAuth as dmda
+import domolibrary.client.DomoError as de
 
-# %% ../../nbs/routes/datacenter.ipynb 3
-class Datacenter_Enum(Enum):
-    ACCOUNT = "ACCOUNT"
-    CARD = "CARD"
-    DATAFLOW = "DATAFLOW"
-    DATASET = "DATASET"
-    GROUP = "GROUP"
-    PAGE = "PAGE"
-    USER = "USER"
-
-
-class Dataflow_Type_Filter_Enum(Enum):
-    ADR = {
-        "filterType": "term",
-        "field": "data_flow_type",
-        "value": "ADR",
-        "name": "ADR",
-        "not": False,
-    }
+# %% ../../nbs/routes/user.ipynb 5
+async def get_all_users(
+    auth: dmda.DomoAuth, debug_api: bool = False
+) -> rgd.ResponseGetData:
 
-    MYSQL = {
-        "filterType": "term",
-        "field": "data_flow_type",
-        "value": "MYSQL",
-        "name": "MYSQL",
-        "not": False,
-    }
+    """retrieves all users from Domo"""
+    url = f"https://{ auth.domo_instance}.domo.com/api/content/v2/users"
 
-    REDSHIFT = {
-        "filterType": "term",
-        "field": "data_flow_type",
-        "value": "MYSQL",
-        "name": "MYSQL",
-        "not": False,
-    }
+    return await gd.get_data(url=url, method="GET", auth=auth, debug_api=debug_api)
 
-    MAGICV2 = {
-        "filterType": "term",
-        "field": "data_flow_type",
-        "value": "MAGIC",
-        "name": "Magic ETL v2",
-        "not": False,
-    }
 
-    MAGIC = {
-        "filterType": "term",
-        "field": "data_flow_type",
-        "value": "ETL",
-        "name": "Magic ETL",
-        "not": False,
-    }
+# %% ../../nbs/routes/user.ipynb 9
+async def get_by_id(user_id, auth: dmda.DomoAuth, debug_api: bool = False, session: httpx.AsyncClient = None):
+    v2_url = f'https://{auth.domo_instance}.domo.com/api/content/v2/users/{user_id}' # does not include role_id
 
-# %% ../../nbs/routes/datacenter.ipynb 4
-class Datacenter_Filter_Field_Enum(Enum):
-    DATAPROVIDER = "dataprovidername_facet"
+    v3_url = f'https://{auth.domo_instance}.domo.com/api/content/v3/users/{user_id}'
+    
+    params = {'includeDetails' :True}
 
+    
+    res_v2, res_v3 = await asyncio.gather(gd.get_data(url=v2_url, method="GET", auth=auth, debug_api=debug_api, session=session, params=params) , 
+    gd.get_data(url=v3_url, method="GET", auth=auth, debug_api=debug_api, session=session, params=params))
 
-def generate_search_datacenter_filter(
-    field,  # use Datacenter_Filter_Field_Enum
-    value,
-    is_not: bool = False,  # to handle exclusion
-):
-    return {
-        "filterType": "term",
-        "field": field,
-        "value": value,
-        "not": is_not,
-    }
+    res_v2.response.update({'roleId': res_v3.response.get('roleId')})
 
-# %% ../../nbs/routes/datacenter.ipynb 6
-def generate_search_datacenter_filter_search_term(search_term):
-    # if not "*" in search_term:
-    #     search_term = f"*{search_term}*"
-
-    return {"field": "name_sort", "filterType": "wildcard", "query": search_term}
-
-# %% ../../nbs/routes/datacenter.ipynb 9
-def generate_search_datacenter_body(
-    search_text: str = None,
-    entity_type: Union[
-        str, list
-    ] = "DATASET",  # can accept one entity_type or a list of entity_types
-    additional_filters_ls: list[dict] = None,
-    combineResults: bool = True,
-    limit: int = 100,
-    offset: int = 0,
-):
-    filters_ls = (
-        [generate_search_datacenter_filter_search_term(search_text)]
-        if search_text
-        else []
-    )
+    return res_v2
 
-    if not isinstance(entity_type, list):
-        entity_type = [entity_type]
 
-    if additional_filters_ls:
-        if not isinstance(additional_filters_ls, list):
-            additional_filters_ls = [additional_filters_ls]
 
-        filters_ls += additional_filters_ls
+# %% ../../nbs/routes/user.ipynb 11
+def generate_search_users_body_by_id(
+    user_ids: list[str],  # list of user ids to search
+) -> dict:  # dict to pass to search v1_users_search_api
+    """search v1_users_search_api"""
 
     return {
-        "entities": entity_type,
-        "filters": filters_ls or [],
-        "combineResults": combineResults,
-        "query": "*",
-        "count": limit,
-        "offset": offset,
+        # "showCount": true,
+        # "count": false,
+        "includeDeleted": False,
+        "includeSupport": False,
+        "filters": [
+            {"field": "id", "filterType": "value",
+                "values": user_ids, "operator": "EQ"}
+        ],
     }
 
-# %% ../../nbs/routes/datacenter.ipynb 12
-def generate_search_datacenter_account_body(
-    search_str: str, is_exact_match: bool = True
-):
+
+# %% ../../nbs/routes/user.ipynb 12
+def generate_search_users_body_by_email(
+    user_email_ls: list[
+        str
+    ],  # list of user emails to search.  Note:  search does not appear to be case sensitive
+) -> dict:  # dict to pass to search v1_users_search_api
+    """search v1_users_search_api"""
+
     return {
-        "count": 100,
+        # "showCount": true,
+        # "count": false,
+        "includeDeleted": False,
+        "includeSupport": False,
+        "limit": 200,
         "offset": 0,
-        "combineResults": False,
-        "query": search_str if is_exact_match else f"*{search_str}*",
-        "filters": [],
-        "facetValuesToInclude": [
-            "DATAPROVIDERNAME",
-            "OWNED_BY_ID",
-            "VALID",
-            "USED",
-            "LAST_MODIFIED_DATE",
+        "sort": {"field": "displayName", "order": "ASC"},
+        "filters": [
+            {
+                "filterType": "text",
+                "field": "emailAddress",
+                "text": " ".join(user_email_ls),
+            }
         ],
-        "queryProfile": "GLOBAL",
-        "entityList": [["account"]],
-        "sort": {"fieldSorts": [{"field": "display_name_sort", "sortOrder": "ASC"}]},
     }
 
-# %% ../../nbs/routes/datacenter.ipynb 13
-class SearchDatacenter_NoResultsFound(de.DomoError):
-    def __init__(self, body, domo_instance):
-        super().__init__(message=body, domo_instance=domo_instance)
+# %% ../../nbs/routes/user.ipynb 13
+def process_v1_search_users(
+    v1_user_ls: list[dict],  # list of users from v1_users_search API
+) -> list[dict]:  # sanitized list of users.
+    """sanitizes the response from v1_users_search API and removes unecessary attributes"""
 
+    clean_users = []
 
-async def search_datacenter(
-    auth: dmda.DomoAuth,
-    maximum: int = None,
-    body: dict = None,  # either pass a body or generate a body in the function using search_text, entity_type, and additional_filters parameters
-    search_text=None,
-    entity_type: Union[
-        str, list
-    ] = "dataset",  # can accept one value or a list of values
-    additional_filters_ls=None,
-    arr_fn: callable = None,
-    session: httpx.AsyncClient = None,
-    debug_api: bool = False,
-) -> rgd.ResponseGetData:
-    limit = 100  # api enforced limit
+    for obj_user in v1_user_ls:
 
-    if not body:
-        body = generate_search_datacenter_body(
-            entity_type=entity_type,
-            additional_filters_ls=additional_filters_ls,
-            search_text=search_text,
-            combineResults=False,
-            limit=limit,
+        dd_user = dd.DictDot(obj_user)
+
+        clean_users.append(
+            {
+                "id": dd_user.id,
+                "displayName": dd_user.displayName,
+                "roleId": dd_user.roleId,
+                "userName": dd_user.userName,
+                "emailAddress": dd_user.emailAddress,
+            }
         )
 
-    if not arr_fn:
+    return clean_users
 
-        def arr_fn(res):
-            return res.response.get("searchObjects")
+# %% ../../nbs/routes/user.ipynb 14
+class SearchUser_NoResults(de.DomoError):
+    def __init__(
+        self, domo_instance, function_name="search_users", search_criteria=None
+    ):
 
-    url = f"https://{auth.domo_instance}.domo.com/api/search/v1/query"
+        search_str = f"- {search_criteria}" if search_criteria else ""
 
-    res = await gd.looper(
-        auth=auth,
-        session=session,
+        print(search_str)
+
+        super().__init__(
+            message=f"query {search_str} returned no users", function_name=function_name
+        )
+
+# %% ../../nbs/routes/user.ipynb 15
+async def search_users(
+    auth: dmda.DomoAuth, body: dict, debug_api: bool = False, return_raw: bool = False
+) -> rgd.ResponseGetData:
+
+    url = f"https://{auth.domo_instance}.domo.com/api/identity/v1/users/search"
+
+    res = await gd.get_data(
         url=url,
-        body=body,
-        offset_params_in_body=True,
-        offset_params={"offset": "offset", "limit": "count"},
-        arr_fn=arr_fn,
         method="POST",
-        loop_until_end=True if not maximum else False,
-        maximum=maximum,
-        limit=limit,
+        auth=auth,
+        body=body,
         debug_api=debug_api,
     )
 
-    if res.is_success and len(res.response) == 0:
-        raise SearchDatacenter_NoResultsFound(
-            body=body, domo_instance=auth.domo_instance
-        )
+    if return_raw:
+        return res
+
+    if not res.is_success:
+        return res
 
+    if res.is_success and len(res.response.get("users")) == 0:
+        raise SearchUser_NoResults(domo_instance=auth.domo_instance)
+
+    res.response = process_v1_search_users(res.response.get("users"))
     return res
 
-# %% ../../nbs/routes/datacenter.ipynb 16
-async def get_lineage_upstream(
+# %% ../../nbs/routes/user.ipynb 19
+async def search_virtual_user_by_subscriber_instance(
+    auth: dmda.DomoAuth,  # domo auth object
+    subscriber_instance_ls: list[str],  # list of subscriber domo instances
+    debug_api: bool = False,  # debug API requests
+) -> rgd.ResponseGetData:  # list of virtual domo users
+    """retrieve virtual users for subscriber instances tied to one publisher"""
+
+    url = f"https://{auth.domo_instance}.domo.com/api/publish/v2/proxy_user/domain/"
+
+    body = {
+        "domains": [
+            f"{subscriber_instance}.domo.com"
+            for subscriber_instance in subscriber_instance_ls
+        ]
+    }
+
+    return await gd.get_data(
+        url=url,
+        method="POST",
+        auth=auth,
+        body=body,
+        debug_api=debug_api,
+    )
+
+# %% ../../nbs/routes/user.ipynb 23
+async def create_user(
     auth: dmda.DomoAuth,
-    entity_type: str,
-    entity_id: str,
-    session: httpx.AsyncClient = None,
+    display_name: str,
+    email_address: str,
+    role_id: int,
     debug_api: bool = False,
-):
-    url = f"https://{auth.domo_instance}.domo.com/api/data/v1/lineage/{entity_type}/{entity_id}"
+    session: httpx.AsyncClient = None,
+) -> rgd.ResponseGetData:
 
-    params = {"traverseDown": "false"}
+    url = f"https://{auth.domo_instance}.domo.com/api/content/v3/users"
+
+    body = {"displayName": display_name,
+            "detail": {
+                "email": email_address},
+            "roleId": role_id
+            }
 
     return await gd.get_data(
-        auth=auth,
-        method="GET",
         url=url,
-        params=params,
-        session=session,
-        debug_api=debug_api,
+        method="POST",
+        body=body,
+        auth=auth, debug_api=debug_api, session=session
     )
 
 
-# %% ../../nbs/routes/datacenter.ipynb 19
-class ShareResource_Enum(Enum):
-    PAGE = "page"
-    CARD = "badge"
+# %% ../../nbs/routes/user.ipynb 25
+async def set_user_landing_page(
+    auth: dmda.DomoAuth, user_id: str, page_id: str, debug_api: bool = False
+):
+
+    url = f"https://{auth.domo_instance}.domo.com/api/content/v1/landings/target/DESKTOP/entity/PAGE/id/{page_id}/{user_id}"
+
+    return await gd.get_data(
+        url=url,
+        method="PUT",
+        auth=auth,
+        # body = body,
+        debug_api=debug_api,
+    )
 
 
-async def share_resource(
+# %% ../../nbs/routes/user.ipynb 26
+async def reset_password(
     auth: dmda.DomoAuth,
-    resource_ids: list,
-    resource_type: ShareResource_Enum,
-    group_ids: list = None,
-    user_ids: list = None,
-    message: str = None,  # email to user
+    user_id: str,
+    new_password: str,
     debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-):
-    """shares page or card with users or groups
+) -> rgd.ResponseGetData:
 
-    body format:  {
-        "resources": [
-            {
-                "type": "page",
-                "id": {oage_id}
-            }
-        ],
-        "recipients": [
-            {
-                "type": "group",
-                "id": "{group_id}"
-            }
-        ],
-        "message": "I thought you might find this page interesting."
-    }"""
+    url = f"https://{auth.domo_instance}.domo.com/api/identity/v1/password"
 
-    resource_ids = resource_ids if isinstance(resource_ids, list) else [resource_ids]
-    if group_ids: group_ids = group_ids and group_ids if isinstance(group_ids, list) else [group_ids]
-    
-    if user_ids: user_ids = user_ids if isinstance(user_ids, list) else [user_ids]
+    body = {"domoUserId": user_id, "password": new_password}
+
+    return await gd.get_data(
+        url=url,
+        method="PUT",
+        auth=auth,
+        body=body,
+        debug_api=debug_api,
+    )
 
-    url = f"https://{auth.domo_instance}.domo.com/api/content/v1/share?sendEmail=false"
 
-    recipient_ls = []
+# %% ../../nbs/routes/user.ipynb 27
+async def request_password_reset(
+    domo_instance: str, 
+    email: str, locale="en-us", debug_api: bool = False,
+    session : httpx.AsyncClient = None
+):
+    url = f"https://{domo_instance}.domo.com/api/domoweb/auth/sendReset"
 
-    if group_ids:
-        [recipient_ls.append({"type": "group", "id": str(id)}) for id in group_ids]
+    params = {"email": email, "local": locale}
 
-    if user_ids:
-        [recipient_ls.append({"type": "user", "id": str(id)}) for id in user_ids]
+    return await gd.get_data(
+        url=url, method="GET", params=params, auth=None, debug_api=debug_api
+    )
 
-    resource_ls = [{"type": resource_type.value, "id": str(id)} for id in resource_ids]
 
-    body = {
-        "resources": resource_ls,
-        "recipients": recipient_ls,
-        "message": message,
+# %% ../../nbs/routes/user.ipynb 29
+class UserProperty_Type(Enum):
+    display_name = "displayName"
+    email_address = "emailAddress"
+    phone_number = "phoneNumber"
+    title = "title"
+    department = "department"
+    web_landing_page = "webLandingPage"
+    web_mobile_landing_page = "webMobileLandingPage"
+    role_id = "roleId"
+    employee_id = "employeeId"
+    employee_number = "employeeNumber"
+    hire_date = "hireDate"
+    reports_to = "reportsTo"
+
+
+class UserProperty:
+    property_type: UserProperty_Type
+    values: str
+
+    def __init__(self, property_type: UserProperty_Type, values):
+        self.property_type = property_type
+        self.values = self._valid_value(values)
+
+    @staticmethod
+    def _valid_value(values):
+        return values if isinstance(values, list) else [values]
+
+    def to_json(self):
+        return {
+            "key": self.property_type.value,
+            "values": self._valid_value(self.values),
+        }
+
+# %% ../../nbs/routes/user.ipynb 30
+def generate_patch_user_property_body(user_property_ls: [UserProperty]):
+    return {
+        "attributes": [user_property.to_json() for user_property in user_property_ls]
     }
 
-    res = await gd.get_data(
-        url, method="POST", auth=auth, body=body, session=session, debug_api=debug_api
+# %% ../../nbs/routes/user.ipynb 33
+async def update_user(
+    user_id: str,
+    user_property_ls: [UserProperty],
+    auth: dmda.DomoAuth = None,
+    debug_api: bool = False,
+    session: httpx.AsyncClient = None,
+):
+    url = f"https://{auth.domo_instance}.domo.com/api/identity/v1/users/{user_id}"
+
+    body = (
+        generate_patch_user_property_body(user_property_ls)
+        if isinstance(user_property_ls[0], UserProperty)
+        else user_property_ls
     )
 
-    if res.is_success:
-        res.response = f"{resource_type.value} {','.join([resource['id'] for resource in  resource_ls])} successfully shared with {', '.join([recipient['id'] for recipient in recipient_ls])}"
-    
-    return res
+    return await gd.get_data(
+        url=url,
+        method="Patch",
+        auth=auth,
+        body=body,
+        debug_api=debug_api,
+        session=session,
+    )
```

### Comparing `domolibrary-0.1.85/domolibrary/routes/dataflow.py` & `domolibrary-0.1.9/domolibrary/routes/dataflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/dataflow.ipynb.
 
 # %% auto 0
-__all__ = ['get_dataflow_by_id', 'execute_dataflow']
+__all__ = ['get_dataflow_by_id']
 
 # %% ../../nbs/routes/dataflow.ipynb 2
 import httpx
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
@@ -20,21 +20,7 @@
     domo_instance = auth.domo_instance
 
     url = f"https://{domo_instance}.domo.com/api/dataprocessing/v1/dataflows/{dataflow_id}"
 
     return await gd.get_data(
         auth=auth, url=url, method="GET", debug_api=debug_api, session=session
     )
-
-# %% ../../nbs/routes/dataflow.ipynb 6
-async def execute_dataflow(auth: dmda.DomoAuth,
-                          dataflow_id: int,
-                          debug_api: bool = False,
-                          session: httpx.AsyncClient = None,
-                          ) -> rgd.ResponseGetData:
-
-                    
-    url=f"https://{auth.domo_instance}.domo.com/api/dataprocessing/v1/dataflows/{dataflow_id}/executions"
-
-    return await gd.get_data( auth=auth, url=url, method="POST", debug_api=debug_api, session=session
-    )
-
```

### Comparing `domolibrary-0.1.85/domolibrary/routes/dataset.py` & `domolibrary-0.1.9/domolibrary/routes/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,41 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/dataset.ipynb.
 
 # %% auto 0
 __all__ = ['DatasetNotFoundError', 'QueryRequestError', 'query_dataset_public', 'query_dataset_private', 'get_dataset_by_id',
            'get_schema', 'set_dataset_tags', 'UploadDataError', 'upload_dataset_stage_1', 'upload_dataset_stage_2_file',
            'upload_dataset_stage_2_df', 'upload_dataset_stage_3', 'index_dataset', 'index_status',
-           'generate_list_partitions_body', 'list_partitions', 'generate_create_dataset_body', 'create',
-           'delete_partition_stage_1', 'delete_partition_stage_2', 'delete', 'ShareDataset_AccessLevelEnum',
-           'generate_share_dataset_payload', 'ShareDataset_Error', 'share_dataset']
+           'generate_list_partitions_body', 'list_partitions', 'generate_create_dataset_body', 'create', 'delete']
 
 # %% ../../nbs/routes/dataset.ipynb 3
 from typing import Optional
-from enum import Enum
 
 import io
 import pandas as pd
 
 import httpx
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
-import domolibrary.client.DomoError as de
 
 
 # %% ../../nbs/routes/dataset.ipynb 5
-class DatasetNotFoundError(de.DomoError):
-    def __init__(self, dataset_id, domo_instance, status = None):
-        message = f"dataset - {dataset_id} not found"
+class DatasetNotFoundError(Exception):
+    def __init__(self, dataset_id, domo_instance):
+        message = f"dataset - {dataset_id} not found in {domo_instance}"
 
-        super().__init__(message, status = status, domo_instance = domo_instance)
-        
+        super().__init__(message)
 
 # %% ../../nbs/routes/dataset.ipynb 6
-class QueryRequestError(de.DomoError):
-    def __init__(self, dataset_id, domo_instance, sql, status=None, message=''):
-        message = f"dataset - {dataset_id} received a bad request {message}.  Check your SQL \n {sql}"
-
-        super().__init__(message,
-                         status=status,
-                         domo_instance=domo_instance)
+class QueryRequestError(Exception):
+    def __init__(self, dataset_id, domo_instance, sql):
+        message = f"dataset - {dataset_id} in {domo_instance} received a bad request.  Check your SQL \n {sql}"
+
+        super().__init__(message)
 
 
 # typically do not use
 async def query_dataset_public(
     dev_auth: dmda.DomoDeveloperAuth,
     dataset_id: str,
     sql: str,
@@ -68,50 +61,32 @@
 
 async def query_dataset_private(
     auth: dmda.DomoAuth,  # DomoFullAuth or DomoTokenAuth
     dataset_id: str,
     sql: str,
     session: Optional[httpx.AsyncClient] = None,
     loop_until_end: bool = False,  # retrieve all available rows
-
     limit=100,  # maximum rows to return per request.  refers to PAGINATION
     skip=0,
     maximum=100,  # equivalent to the LIMIT or TOP clause in SQL, the number of rows to return total
-
-    filter_pdp_policy_id_ls: [int] = None,
-    
     debug_api: bool = False,
     debug_loop: bool = False,
-    timeout: int = 10
+    timeout :int = 10
 ):
     """execute SQL queries against private APIs, requires DomoFullAuth or DomoTokenAuth"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/query/v1/execute/{dataset_id}"
 
     offset_params = {
         "offset": "offset",
         "limit": "limit",
     }
 
-    # def body_fn(skip, limit):
-    #     return {"sql": f"{sql} limit {limit} offset {skip}"}
-
     def body_fn(skip, limit):
-        body = {"sql": f"{sql} limit {limit} offset {skip}"}
-
-        if filter_pdp_policy_id_ls:
-            body.update({"context": {
-                "dataControlContext": {
-                    "filterGroupIds": filter_pdp_policy_id_ls,
-                    "previewPdp": True
-                }
-
-            }})
-
-        return body
+        return {"sql": f"{sql} limit {limit} offset {skip}"}
 
     def arr_fn(res) -> pd.DataFrame:
         rows_ls = res.response.get("rows")
         columns_ls = res.response.get("columns")
         output = []
         for row in rows_ls:
             new_row = {}
@@ -131,35 +106,29 @@
         skip=skip,
         maximum=maximum,
         session=session,
         body_fn=body_fn,
         debug_api=debug_api,
         debug_loop=debug_loop,
         loop_until_end=loop_until_end,
-        timeout=timeout
+        timeout = timeout
     )
 
     if res.status == 404 and res.response == "Not Found":
         raise DatasetNotFoundError(
-            dataset_id=dataset_id, domo_instance=auth.domo_instance, status = res.status
+            dataset_id=dataset_id, domo_instance=auth.domo_instance
         )
 
     if res.status == 400 and res.response == "Bad Request":
         raise QueryRequestError(
-            dataset_id=dataset_id, domo_instance=auth.domo_instance,
-            sql=sql, status=res.status,
+            dataset_id=dataset_id, domo_instance=auth.domo_instance, sql=sql
         )
 
-    if not res.is_success:
-        raise QueryRequestError(dataset_id=dataset_id, domo_instance=auth.domo_instance,
-                                sql=sql, message=res.response, status=res.status)
-
     return res
 
-
 # %% ../../nbs/routes/dataset.ipynb 9
 async def get_dataset_by_id(
     dataset_id: str,  # dataset id from URL
     auth: Optional[dmda.DomoAuth] = None,  # requires full authentication
     debug_api: bool = False,  # for troubleshooting API request
     session: Optional[httpx.AsyncClient] = None,
 ) -> rgd.ResponseGetData:  # returns metadata about a dataset
@@ -169,15 +138,15 @@
 
     res = await gd.get_data(
         auth=auth, url=url, method="GET", debug_api=debug_api, session=session
     )
 
     if res.status == 404 and res.response == "Not Found":
         raise DatasetNotFoundError(
-            dataset_id=dataset_id, domo_instance=auth.domo_instance, status = res.status
+            dataset_id=dataset_id, domo_instance=auth.domo_instance
         )
 
     return res
 
 # %% ../../nbs/routes/dataset.ipynb 12
 async def get_schema(
     auth: dmda.DomoAuth, dataset_id: str, debug_api: bool = False
@@ -219,24 +188,20 @@
         res.set_response(
             response=f'Dataset {dataset_id} tags updated to [{ ", ".join(tag_ls) }]'
         )
 
     return res
 
 # %% ../../nbs/routes/dataset.ipynb 19
-class UploadDataError(de.DomoError):
+class UploadDataError(Exception):
     """raise if unable to upload data to Domo"""
 
-    def __init__(self, stage_num: int, dataset_id: str, status, message, domo_instance: str):
-
-        message = f"error uploading data during Stage { stage_num} - {message}"
-
-        super().__init__(entity_id=dataset_id, message=message,
-                         status=status, domo_instance=domo_instance)
-
+    def __init__(self, stage_num: int, dataset_id: str, domo_instance: str):
+        message = f"error uploading data to {dataset_id} during Stage { stage_num} in {domo_instance}"
+        super().__init__(message)
 
 # %% ../../nbs/routes/dataset.ipynb 20
 async def upload_dataset_stage_1(
     auth: dmda.DomoAuth,
     dataset_id: str,
     #  restate_data_tag: str = None, # deprecated
     partition_tag: str = None,  # synonymous with data_tag
@@ -266,18 +231,15 @@
         session=session,
         debug_api=debug_api,
         params=params,
     )
 
     if not res.is_success:
         raise UploadDataError(
-            stage_num=1, dataset_id=dataset_id, 
-            domo_instance=auth.domo_instance, 
-            status=res.status, 
-            message=res.response
+            stage_num=1, dataset_id=dataset_id, domo_instance=auth.domo_instance
         )
 
     return res
 
 # %% ../../nbs/routes/dataset.ipynb 21
 async def upload_dataset_stage_2_file(
     auth: dmda.DomoAuth,
@@ -301,24 +263,23 @@
         content_type="text/csv",
         body=body,
         session=session,
         debug_api=debug_api,
     )
     if not res.is_success:
         raise UploadDataError(
-            stage_num=2, dataset_id=dataset_id, domo_instance=auth.domo_instance, status=res.status, message=res.response
+            stage_num=2, dataset_id=dataset_id, domo_instance=auth.domo_instance
         )
 
     res.upload_id = upload_id
     res.dataset_id = dataset_id
     res.part_id = part_id
 
     return res
 
-
 # %% ../../nbs/routes/dataset.ipynb 22
 async def upload_dataset_stage_2_df(
     auth: dmda.DomoAuth,
     dataset_id: str,
     upload_id: str,  # must originate from  a stage_1 upload response
     upload_df: pd.DataFrame,
     session: Optional[httpx.AsyncClient] = None,
@@ -395,18 +356,17 @@
         body=body,
         session=session,
         debug_api=debug_api,
     )
 
     if not res.is_success:
         raise UploadDataError(
-            stage_num=3, dataset_id=dataset_id, domo_instance=auth.domo_instance, status=res.status, message=res.response
+            stage_num=3, dataset_id=dataset_id, domo_instance=auth.domo_instance
         )
 
-
     res.upload_id = upload_id
     res.dataset_id = dataset_id
 
     return res
 
 # %% ../../nbs/routes/dataset.ipynb 25
 async def index_dataset(
@@ -494,15 +454,15 @@
         session=session,
         debug_loop=debug_loop,
         debug_api=debug_api,
     )
 
     if res.status == 404 and res.response == "Not Found":
         raise DatasetNotFoundError(
-            dataset_id=dataset_id, domo_instance=auth.domo_instance, status = res.status
+            dataset_id=dataset_id, domo_instance=auth.domo_instance
         )
     return res
 
 # %% ../../nbs/routes/dataset.ipynb 30
 def generate_create_dataset_body(
     dataset_name: str, dataset_type: str = "API", schema: dict = None
 ):
@@ -540,108 +500,19 @@
         method="POST",
         url=url,
         body=body,
         session=session,
         debug_api=debug_api,
     )
 
-# %% ../../nbs/routes/dataset.ipynb 33
-async def delete_partition_stage_1(auth: dmda.DomoAuth,
-                                   dataset_id: str,
-                                    dataset_partition_id: str,
-                                    debug_api: bool = False):
-# Delete partition has 3 stages
-# Stage 1. This marks the data version associated with the partition tag as deleted.  It does not delete the partition tag or remove the association between the partition tag and data version.  There should be no need to upload an empty file – step #3 will remove the data from Adrenaline.
-# update on 9/9/2022 based on the conversation with Greg Swensen
-    url = f'https://{auth.domo_instance}.domo.com/api/query/v1/datasources/{dataset_id}/tag/{dataset_partition_id}/data'
-
-    return await gd.get_data(
-       auth=auth,
-       method="DELETE",
-       url=url,
-      debug_api=debug_api)
-# Stage 2. This will remove the partition association so that it doesn’t show up in the list call.  Technically, this is not required as a partition against a deleted data version will not count against the 400 partition limit, but as the current partitions api doesn’t make that clear, cleaning these up will make it much easier for you to manage.
-
-
-# %% ../../nbs/routes/dataset.ipynb 34
-async def delete_partition_stage_2(auth: dmda.DomoAuth,
-                                   dataset_id: str,
-                                   dataset_partition_id: str,
-                                   debug_api: bool = False):
-    url = f'https://{auth.domo_instance}.domo.com/api/query/v1/datasources/{dataset_id}/partition/{dataset_partition_id}'
-
-    return await gd.get_data(
-        auth=auth,
-        method="DELETE",
-        url=url,
-
-       debug_api=debug_api
-    )
-
-
 # %% ../../nbs/routes/dataset.ipynb 35
 async def delete(
     auth: dmda.DomoAuth,
     dataset_id: str,
     session: httpx.AsyncClient = None,
     debug_api: bool = False,
 ):
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}?deleteMethod=hard"
 
     return await gd.get_data(
         auth=auth, method="DELETE", url=url, session=session, debug_api=debug_api
     )
-
-# %% ../../nbs/routes/dataset.ipynb 36
-class ShareDataset_AccessLevelEnum(Enum):
-    CO_OWNER = 'CO_OWNER'
-    CAN_EDIT = 'CAN_EDIT'
-    CAN_SHARE = 'CAN_SHARE'
-
-
-def generate_share_dataset_payload(entity_type,  # USER or GROUP
-                                   entity_id,
-                                   access_level: ShareDataset_AccessLevelEnum = ShareDataset_AccessLevelEnum.CAN_SHARE,
-                                   is_send_email : bool = False
-
-                                   ):
-
-    return {
-        "permissions": [
-            {
-                "type": entity_type,
-                "id": entity_id,
-                "accessLevel": access_level.value
-            }
-        ],
-        "sendEmail": is_send_email
-    }
-
-
-# %% ../../nbs/routes/dataset.ipynb 37
-class ShareDataset_Error(de.DomoError):
-    def __init__(self, dataset_id, status, response, domo_instance):
-
-        message = f"error sharing dataset {dataset_id} - {response}"
-        
-        super().__init__(status = status, domo_instance = domo_instance, message = message)
-
-async def share_dataset(auth: dmda.DomoAuth,
-                        dataset_id: str, 
-                        body: dict,
-                        session: httpx.AsyncClient = None,
-                        debug_api=False):
-
-    url = f'https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}/share'
-
-    res = await gd.get_data(
-        auth=auth, method="POST", url=url, body = body, session=session, debug_api=debug_api
-    )
-
-    if not res.is_success:
-        raise ShareDataset_Error(dataset_id = dataset_id, status = res.status, response = res.response, domo_instance = auth.domo_instance)
-    
-    update_user_ls = [f"{user['type']} - {user['id']}"for user in body['permissions']]
-
-    res.response = f"updated access list { ', '.join(update_user_ls)} added to {dataset_id}"
-    return res
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `domolibrary-0.1.85/domolibrary/routes/grant.py` & `domolibrary-0.1.9/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/routes/group.py` & `domolibrary-0.1.9/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/routes/instance_config.py` & `domolibrary-0.1.9/domolibrary/routes/instance_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,24 +99,22 @@
     auth: dmda.DomoAuth,
     authorized_domain_ls: [str],
     debug_api: bool = False,
     session: httpx.AsyncClient = None,
 ):
     url = f"https://{auth.domo_instance}.domo.com/api/content/v1/customer-states/authorized-domains"
 
-    body = {
-        "name": "authorized-domains",
-        "value": ",".join(authorized_domain_ls)
-    }
-    
+    body = {"name": "authorized-domains", "value": authorized_domain_ls}
+
     res = await gd.get_data(
         auth=auth,
         url=url,
         method="PUT",
         body=body,
+        log_results=log_results,
         debug_api=debug_api,
         session=session,
     )
 
     return res
```

### Comparing `domolibrary-0.1.85/domolibrary/routes/page.py` & `domolibrary-0.1.9/domolibrary/routes/page.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,175 +1,111 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/page.ipynb.
 
 # %% auto 0
-__all__ = ['get_page_by_id', 'get_page_definition', 'get_page_access_list', 'get_pages_adminsummary', 'update_page_layout',
-           'put_writelock', 'delete_writelock']
+__all__ = ['get_page_by_id', 'get_page_definition', 'get_page_access_list', 'get_pages_adminsummary']
 
 # %% ../../nbs/routes/page.ipynb 2
 import httpx
 import pandas as pd
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
 
-# %% ../../nbs/routes/page.ipynb 3
-async def get_page_by_id(
-    auth: dmda.DomoAuth,
-    page_id: str,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-    include_layout: bool = False,
-) -> rgd.ResponseGetData:
-    url = f"https://{auth.domo_instance}.domo.com/api/content/v3/stacks/{page_id}/cards"
 
+# %% ../../nbs/routes/page.ipynb 3
+async def get_page_by_id(auth: dmda.DomoAuth, page_id: str,
+                         debug_api: bool = False, 
+                         session: httpx.AsyncClient = None,
+                         include_layout: bool = False
+                         ) -> rgd.ResponseGetData:
+    url = f'https://{auth.domo_instance}.domo.com/api/content/v3/stacks/{page_id}/cards'
+    
     if include_layout:
-        url += "?includeV4PageLayouts=true"
-
+        url+='?includeV4PageLayouts=true'
+    
     res = await gd.get_data(
         auth=auth,
         url=url,
-        method="GET",
+        method='GET',
         debug_api=debug_api,
-        session=session,
+        session = session,
     )
 
     res.response
 
+
     return res
 
 # %% ../../nbs/routes/page.ipynb 6
-async def get_page_definition(
-    auth, page_id, debug_api: bool = False, session: httpx.AsyncClient = None
-):
+async def get_page_definition(auth, page_id, debug_api: bool = False, session: httpx.AsyncClient = None):
+
     url = f"https://{auth.domo_instance}.domo.com/api/content/v3/stacks/{page_id}/cards"
 
-    params = {
-        "includeV4PageLayouts": "true",
-        "parts": "metadata,datasources,library,drillPathURNs,certification,owners,dateInfo,subscriptions,slicers",
-    }
+    params = {"includeV4PageLayouts": "true",
+              "parts": "metadata,datasources,library,drillPathURNs,certification,owners,dateInfo,subscriptions,slicers"}
 
-    res = await gd.get_data(
-        url,
-        method="GET",
-        auth=auth,
-        session=session,
-        params=params,
-        debug_api=debug_api,
-    )
+    res = await gd.get_data(url,
+                            method='GET',
+                            auth=auth,
+                            session=session,
+                            params=params, debug_api=debug_api)
 
     return res
 
+
 # %% ../../nbs/routes/page.ipynb 9
-async def get_page_access_list(
-    auth,
-    page_id,
-    is_expand_users: bool = True,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-):
+async def get_page_access_list(auth,
+                              page_id,
+                              is_expand_users: bool = True,
+                              debug_api: bool = False, session: httpx.AsyncClient = None):
     """retrieves accesslist, which users and groups a page is shared with"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/content/v1/share/accesslist/page/{page_id}?expandUsers={is_expand_users}"
 
-    res = await gd.get_data(
-        url, method="GET", auth=auth, session=session, debug_api=debug_api
-    )
+    res = await gd.get_data(url,
+                            method='GET',
+                            auth=auth,
+                            session=session, debug_api=debug_api)
 
     # add group members to users response
     if is_expand_users:
-        group_users = [
-            user for group in res.response.get("groups") for user in group.get("users")
-        ]
-        users = res.response.get("users") + group_users
-        res.response.update({"users": users})
+        group_users = [user for group in res.response.get(
+            'groups') for user in group.get('users')]
+        users = res.response.get('users') + group_users
+        res.response.update({'users': users})
 
     return res
 
+
 # %% ../../nbs/routes/page.ipynb 12
-async def get_pages_adminsummary(
-    auth: dmda.DomoAuth,
-    debug_loop: bool = False,
-    debug_api: bool = False,
-    limit=35,
-    session: httpx.AsyncClient = None,
-):
+async def get_pages_adminsummary(auth: dmda.DomoAuth,
+                                 debug_loop: bool = False,
+                                 debug_api : bool = False,
+                                 limit = 35,
+                                 session: httpx.AsyncClient = None):
     """retrieves all pages in instance user is able to see (but may not have been explicitly shared)"""
 
-    url = f"https://{auth.domo_instance}.domo.com/api/content/v1/pages/adminsummary"
+    url = f'https://{auth.domo_instance}.domo.com/api/content/v1/pages/adminsummary'
 
     offset_params = {
-        "offset": "skip",
-        "limit": "limit",
+        'offset': 'skip',
+        'limit': 'limit',
     }
 
     body = {"orderBy": "pageTitle", "ascending": True}
 
     def arr_fn(res) -> list[dict]:
-        return res.response.get("pageAdminSummaries")
-
-    res = await gd.looper(
-        auth=auth,
-        method="POST",
-        url=url,
-        arr_fn=arr_fn,
-        offset_params=offset_params,
-        session=session,
-        loop_until_end=True,
-        body=body,
-        limit=limit,
-        debug_loop=debug_loop,
-        debug_api=debug_api,
-    )
-    return res
-
-# %% ../../nbs/routes/page.ipynb 14
-async def update_page_layout(
-    auth: dmda.DomoAuth, layout_id: str, body: dict, debug_api: bool = False
-):
-    url = f"https://{auth.domo_instance}.domo.com/api/content/v4/pages/layouts/{layout_id}"
-
-    res = await gd.get_data(
-        auth=auth, url=url, body=body, method="PUT", debug_api=debug_api
-    )
-
-    if debug_api:
-        print(res)
-
-    return res
-
-
-async def put_writelock(
-    auth: dmda.DomoAuth,
-    layout_id: str,
-    user_id: str,
-    epoch_time: int,
-    debug_api: bool = False,
-):
-    url = f"https://{auth.domo_instance}.domo.com/api/content/v4/pages/layouts/{layout_id}/writelock"
-    body = {
-        "layoutId": layout_id,
-        "lockHeartbeat": epoch_time,
-        "lockTimestamp": epoch_time,
-        "userId": user_id,
-    }
-
-    res = await gd.get_data(
-        auth=auth, url=url, body=body, method="PUT", debug_api=debug_api
-    )
-
-    if debug_api:
-        print(res)
+        return res.response.get('pageAdminSummaries')
 
-    return res
-
-
-async def delete_writelock(
-    auth: dmda.DomoAuth, layout_id: str, debug_api: bool = False
-):
-    url = f"https://{auth.domo_instance}.domo.com/api/content/v4/pages/layouts/{layout_id}/writelock"
-    res = await gd.get_data(auth=auth, url=url, method="DELETE", debug_api=debug_api)
+    res = await gd.looper(auth=auth,
+                          method='POST',
+                          url=url,
+                          arr_fn=arr_fn,
+                          offset_params=offset_params,
+                          session=session,
+                          loop_until_end=True,
+                          body = body,
+                          limit = limit, 
+                          debug_loop=debug_loop, debug_api= debug_api)
+    return res.response
 
-    if debug_api:
-        print(res)
-
-    return res
```

### Comparing `domolibrary-0.1.85/domolibrary/routes/pdp.py` & `domolibrary-0.1.9/domolibrary/routes/pdp.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,21 +34,17 @@
         )
 
 # %% ../../nbs/routes/pdp.ipynb 4
 async def get_pdp_policies(
     auth: dmda.DomoAuth,
     dataset_id: str,
     debug_api: bool = False,
-    include_all_rows: bool = True
 ) -> rgd.ResponseGetData:
     url = f"http://{auth.domo_instance}.domo.com/api/query/v1/data-control/{dataset_id}/filter-groups/"
 
-    if include_all_rows:
-        url+="?options=load_associations,load_filters,include_open_policy"
-        
     if debug_api:
         print(url)
 
     res = await gd.get_data(
         auth=auth, 
         url=url, 
         method="GET",
```

### Comparing `domolibrary-0.1.85/domolibrary/routes/role.py` & `domolibrary-0.1.9/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/utils/DictDot.py` & `domolibrary-0.1.9/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.9/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/utils/convert.py` & `domolibrary-0.1.9/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.9/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/domolibrary/utils/upload_data.py` & `domolibrary-0.1.9/domolibrary/utils/upload_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,44 +29,41 @@
 ):
     base_msg = f"{partition_key} in {consol_ds.auth.domo_instance}" if partition_key else f"in {consol_ds.auth.domo_instance}"
 
     if debug_fn:
         print(
             f"starting upload of {len(upload_df)} rows to {base_msg} with {max_retry} attempts")
 
-    retry_attempt = 1
+    retry_attempt = 0
     
     res = None
 
-    while retry_attempt <= max_retry and not res:
+    while retry_attempt <= max_retry:
         try:
-            if debug_fn:
-                print(f"attempt {retry_attempt}/{max_retry} for {base_msg}")
+            retry_attempt += 1
 
+            if debug_fn:
+                print(f"attempt {retry_attempt} for {base_msg}")
 
             res = await consol_ds.upload_data(
                 upload_df=upload_df,
                 upload_method="REPLACE" if partition_key else upload_method,
                 partition_key=partition_key,
                 is_index=is_index,
                 debug_api=debug_api,
                 debug_prn=debug_prn,
             )
 
         except Exception as e:
-            retry_attempt += 1
+            message = f"⚠️ upload_data : unexpected error: {e} in {partition_key} during retry_attempt {retry_attempt}"
 
-            message = f"⚠️ upload_data : unexpected error: {e} in {partition_key} during retry_attempt {retry_attempt}/{max_retry}"
             logger.log_warning(message)
             if debug_fn :
                 print(message)
     
-    if not res:
-        raise Exception(f"💣 failed to upload data {len(upload_df)} rows to {base_msg} - {retry_attempt}/{max_retry} retries reached")
-    
     return res
 
 # %% ../../nbs/utils/upload_data.ipynb 4
 async def upload_data(
     # instance where the data_fn function will execute against
     data_fn,  # data function to execute
     instance_auth: dmda.DomoAuth,  # instance to run the data function against
```

### Comparing `domolibrary-0.1.85/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.9/domolibrary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.85
+Version: 0.1.9
+Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# domolibrary: a powerful pydomo alternative
+domolibrary: a powerful pydomo alternative
+================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Formatting
 
 use_snake_case for everything except class names is_bool - prefix any
 boolean parameters with is_bool
@@ -232,7 +235,9 @@
 Consider
 [`query_dataset_private`](https://jaewilson07.github.io/domo_library/routes/dataset.html#query_dataset_private)
 from the `routes.dataset`.
 
 Inside this function we are using
 [`looper`](https://jaewilson07.github.io/domo_library/client/get_data.html#looper)
 from `client.get_data` to paginate over the API response.
+
+
```

### Comparing `domolibrary-0.1.85/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.9/domolibrary.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,59 +68,52 @@
 domolibrary.egg-info/dependency_links.txt
 domolibrary.egg-info/entry_points.txt
 domolibrary.egg-info/not-zip-safe
 domolibrary.egg-info/requires.txt
 domolibrary.egg-info/top_level.txt
 domolibrary/classes/DomoAccount.py
 domolibrary/classes/DomoActivityLog.py
-domolibrary/classes/DomoApplication.py
 domolibrary/classes/DomoBootstrap.py
 domolibrary/classes/DomoCard.py
 domolibrary/classes/DomoDatacenter.py
 domolibrary/classes/DomoDataflow.py
 domolibrary/classes/DomoDataset.py
 domolibrary/classes/DomoGrant.py
 domolibrary/classes/DomoGroup.py
 domolibrary/classes/DomoInstanceConfig.py
-domolibrary/classes/DomoJob.py
 domolibrary/classes/DomoPDP.py
 domolibrary/classes/DomoPage.py
 domolibrary/classes/DomoPublish.py
 domolibrary/classes/DomoRole.py
-domolibrary/classes/DomoStream.py
 domolibrary/classes/DomoUser.py
 domolibrary/classes/__init__.py
 domolibrary/client/DomoAuth.py
 domolibrary/client/DomoError.py
 domolibrary/client/Logger.py
 domolibrary/client/ResponseGetData.py
 domolibrary/client/__init__.py
 domolibrary/client/get_data.py
-domolibrary/integrations/Automation.py
 domolibrary/integrations/DomoJupyter.py
 domolibrary/integrations/RoleHierarchy.py
 domolibrary/integrations/__init__.py
 domolibrary/routes/__init__.py
 domolibrary/routes/account.py
 domolibrary/routes/activity_log.py
-domolibrary/routes/application.py
 domolibrary/routes/bootstrap.py
 domolibrary/routes/card.py
 domolibrary/routes/datacenter.py
 domolibrary/routes/dataflow.py
 domolibrary/routes/dataset.py
 domolibrary/routes/grant.py
 domolibrary/routes/group.py
 domolibrary/routes/instance_config.py
-domolibrary/routes/job.py
 domolibrary/routes/page.py
 domolibrary/routes/pdp.py
 domolibrary/routes/publish.py
 domolibrary/routes/role.py
-domolibrary/routes/stream.py
 domolibrary/routes/user.py
 domolibrary/utils/DictDot.py
 domolibrary/utils/__init__.py
 domolibrary/utils/chunk_execution.py
 domolibrary/utils/convert.py
 domolibrary/utils/read_creds_from_dotenv.py
 domolibrary/utils/upload_data.py
```

### Comparing `domolibrary-0.1.85/settings.ini` & `domolibrary-0.1.9/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.85
+version = 0.1.09
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.85/setup.py` & `domolibrary-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/utils/Base.py` & `domolibrary-0.1.9/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/utils/DictDot.py` & `domolibrary-0.1.9/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/utils/Exceptions.py` & `domolibrary-0.1.9/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/utils/LoggerClass.py` & `domolibrary-0.1.9/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/utils/chunk_execution.py` & `domolibrary-0.1.9/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/utils/consol_get_creds.py` & `domolibrary-0.1.9/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/utils/convert.py` & `domolibrary-0.1.9/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.9/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.85/utils/upload_data.py` & `domolibrary-0.1.9/utils/upload_data.py`

 * *Files identical despite different names*

