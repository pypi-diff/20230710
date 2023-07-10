# Comparing `tmp/domolibrary-0.1.95.tar.gz` & `tmp/domolibrary-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.95.tar", last modified: Fri Jul  7 21:12:44 2023, max compression
+gzip compressed data, was "domolibrary-0.1.96.tar", last modified: Mon Jul 10 13:06:06 2023, max compression
```

## Comparing `domolibrary-0.1.95.tar` & `domolibrary-0.1.96.tar`

### file list

```diff
@@ -1,154 +1,156 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.879287 domolibrary-0.1.95/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.775287 domolibrary-0.1.95/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.95/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-06-01 20:57:16.000000 domolibrary-0.1.95/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.783287 domolibrary-0.1.95/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.95/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.799287 domolibrary-0.1.95/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.95/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.819287 domolibrary-0.1.95/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.95/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-06-01 20:57:16.000000 domolibrary-0.1.95/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.823287 domolibrary-0.1.95/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.95/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-01 20:57:16.000000 domolibrary-0.1.95/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-06-01 20:57:16.000000 domolibrary-0.1.95/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-06-01 20:57:16.000000 domolibrary-0.1.95/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 21:12:44.875287 domolibrary-0.1.95/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-06-01 20:57:16.000000 domolibrary-0.1.95/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.823287 domolibrary-0.1.95/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   183314 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.839287 domolibrary-0.1.95/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24213 2023-07-07 21:11:59.000000 domolibrary-0.1.95/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-07-07 21:11:59.000000 domolibrary-0.1.95/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-07-07 21:11:59.000000 domolibrary-0.1.95/domolibrary/classes/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3477 2023-07-07 21:11:59.000000 domolibrary-0.1.95/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3962 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6722 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23039 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12268 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.839287 domolibrary-0.1.95/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12946 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12077 2023-07-07 21:11:59.000000 domolibrary-0.1.95/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.843287 domolibrary-0.1.95/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/integrations/Automation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.851287 domolibrary-0.1.95/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/application.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2369 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8439 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/job.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/stream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10314 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.855287 domolibrary-0.1.95/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-07-07 21:12:00.000000 domolibrary-0.1.95/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.827287 domolibrary-0.1.95/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 21:12:44.000000 domolibrary-0.1.95/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4141 2023-07-07 21:12:44.000000 domolibrary-0.1.95/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-07 21:12:44.000000 domolibrary-0.1.95/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-07-07 21:12:44.000000 domolibrary-0.1.95/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-01 20:57:34.000000 domolibrary-0.1.95/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-07-07 21:12:44.000000 domolibrary-0.1.95/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-07-07 21:12:44.000000 domolibrary-0.1.95/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-07-07 21:12:32.000000 domolibrary-0.1.95/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-07 21:12:44.879287 domolibrary-0.1.95/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-06-01 20:57:16.000000 domolibrary-0.1.95/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 21:12:44.867287 domolibrary-0.1.95/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-06-01 20:57:16.000000 domolibrary-0.1.95/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-06-01 20:57:16.000000 domolibrary-0.1.95/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-06-01 20:57:16.000000 domolibrary-0.1.95/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-06-01 20:57:16.000000 domolibrary-0.1.95/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-06-01 20:57:16.000000 domolibrary-0.1.95/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.95/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-06-01 20:57:16.000000 domolibrary-0.1.95/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-06-01 20:57:16.000000 domolibrary-0.1.95/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-06-01 20:57:16.000000 domolibrary-0.1.95/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-01 20:57:16.000000 domolibrary-0.1.95/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-06-01 20:57:16.000000 domolibrary-0.1.95/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:06.075770 domolibrary-0.1.96/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:05.923770 domolibrary-0.1.96/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 14:35:05.000000 domolibrary-0.1.96/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-04-26 14:35:05.000000 domolibrary-0.1.96/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:05.927770 domolibrary-0.1.96/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:05.959770 domolibrary-0.1.96/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-04-27 14:36:06.000000 domolibrary-0.1.96/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:05.983770 domolibrary-0.1.96/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-04-26 14:35:05.000000 domolibrary-0.1.96/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:05.983770 domolibrary-0.1.96/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 14:35:05.000000 domolibrary-0.1.96/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-04-26 14:35:05.000000 domolibrary-0.1.96/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-04-26 14:35:05.000000 domolibrary-0.1.96/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-04-26 14:35:05.000000 domolibrary-0.1.96/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-10 13:06:06.075770 domolibrary-0.1.96/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-05-25 07:22:11.000000 domolibrary-0.1.96/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:05.983770 domolibrary-0.1.96/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   186363 2023-07-10 13:04:36.000000 domolibrary-0.1.96/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:06.023770 domolibrary-0.1.96/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24213 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3477 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3962 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6722 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23039 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12268 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3427 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:06.027770 domolibrary-0.1.96/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12946 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12077 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:06.031770 domolibrary-0.1.96/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/integrations/Automation.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:06.063770 domolibrary-0.1.96/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/application.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2369 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8439 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/job.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2527 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/sandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/stream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10314 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:06.063770 domolibrary-0.1.96/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-07-10 13:04:35.000000 domolibrary-0.1.96/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:05.999770 domolibrary-0.1.96/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-10 13:06:05.000000 domolibrary-0.1.96/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4206 2023-07-10 13:06:05.000000 domolibrary-0.1.96/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-10 13:06:05.000000 domolibrary-0.1.96/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-07-10 13:06:05.000000 domolibrary-0.1.96/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-26 14:35:31.000000 domolibrary-0.1.96/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-07-10 13:06:05.000000 domolibrary-0.1.96/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-07-10 13:06:05.000000 domolibrary-0.1.96/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-07-10 13:05:36.000000 domolibrary-0.1.96/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-10 13:06:06.075770 domolibrary-0.1.96/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-04-26 14:35:05.000000 domolibrary-0.1.96/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 13:06:06.075770 domolibrary-0.1.96/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-04-26 14:35:05.000000 domolibrary-0.1.96/utils/upload_data.py
```

### Comparing `domolibrary-0.1.95/Automation/automation.py` & `domolibrary-0.1.96/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DataOcean/Transport.py` & `domolibrary-0.1.96/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.96/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.96/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DataOcean/cnfg_s3.py` & `domolibrary-0.1.96/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.96/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoAccount.py` & `domolibrary-0.1.96/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.96/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.96/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoApplication.py` & `domolibrary-0.1.96/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoAuth.py` & `domolibrary-0.1.96/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.96/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoCard.py` & `domolibrary-0.1.96/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoCertification.py` & `domolibrary-0.1.96/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.96/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.96/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoDataset.py` & `domolibrary-0.1.96/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoGrant.py` & `domolibrary-0.1.96/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoGroup.py` & `domolibrary-0.1.96/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.96/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoJob.py` & `domolibrary-0.1.96/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoLineage.py` & `domolibrary-0.1.96/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoPDP.py` & `domolibrary-0.1.96/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoPage.py` & `domolibrary-0.1.96/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoPublish.py` & `domolibrary-0.1.96/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoRole.py` & `domolibrary-0.1.96/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.96/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoStream.py` & `domolibrary-0.1.96/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoTag.py` & `domolibrary-0.1.96/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/DomoUser.py` & `domolibrary-0.1.96/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/get_data.py` & `domolibrary-0.1.96/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.96/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/LICENSE` & `domolibrary-0.1.96/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/PKG-INFO` & `domolibrary-0.1.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.95
+Version: 0.1.96
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary-0.1.95/README.md` & `domolibrary-0.1.96/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/_modidx.py` & `domolibrary-0.1.96/domolibrary/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,14 +569,30 @@
                                                                                                     'domolibrary/classes/DomoRole.py'),
                                               'domolibrary.classes.DomoRole.SearchRole_NotFound.__init__': ( 'classes/domorole.html#searchrole_notfound.__init__',
                                                                                                              'domolibrary/classes/DomoRole.py'),
                                               'domolibrary.classes.DomoRole.SetRoleGrants_MissingGrants': ( 'classes/domorole.html#setrolegrants_missinggrants',
                                                                                                             'domolibrary/classes/DomoRole.py'),
                                               'domolibrary.classes.DomoRole.SetRoleGrants_MissingGrants.__init__': ( 'classes/domorole.html#setrolegrants_missinggrants.__init__',
                                                                                                                      'domolibrary/classes/DomoRole.py')},
+            'domolibrary.classes.DomoSandbox': { 'domolibrary.classes.DomoSandbox.DomoRepository': ( 'classes/domosandbox.html#domorepository',
+                                                                                                     'domolibrary/classes/DomoSandbox.py'),
+                                                 'domolibrary.classes.DomoSandbox.DomoRepository.__post_init__': ( 'classes/domosandbox.html#domorepository.__post_init__',
+                                                                                                                   'domolibrary/classes/DomoSandbox.py'),
+                                                 'domolibrary.classes.DomoSandbox.DomoRepository._from_json': ( 'classes/domosandbox.html#domorepository._from_json',
+                                                                                                                'domolibrary/classes/DomoSandbox.py'),
+                                                 'domolibrary.classes.DomoSandbox.DomoRepository.convert_lineage_to_dataframe': ( 'classes/domosandbox.html#domorepository.convert_lineage_to_dataframe',
+                                                                                                                                  'domolibrary/classes/DomoSandbox.py'),
+                                                 'domolibrary.classes.DomoSandbox.DomoRepository.get_from_id': ( 'classes/domosandbox.html#domorepository.get_from_id',
+                                                                                                                 'domolibrary/classes/DomoSandbox.py'),
+                                                 'domolibrary.classes.DomoSandbox.DomoSandbox': ( 'classes/domosandbox.html#domosandbox',
+                                                                                                  'domolibrary/classes/DomoSandbox.py'),
+                                                 'domolibrary.classes.DomoSandbox.DomoSandbox.get_repositories': ( 'classes/domosandbox.html#domosandbox.get_repositories',
+                                                                                                                   'domolibrary/classes/DomoSandbox.py'),
+                                                 'domolibrary.classes.DomoSandbox.InvalidRepositoryError': ( 'classes/domosandbox.html#invalidrepositoryerror',
+                                                                                                             'domolibrary/classes/DomoSandbox.py')},
             'domolibrary.classes.DomoStream': { 'domolibrary.classes.DomoStream.DomoStream': ( 'classes/domostream.html#domostream',
                                                                                                'domolibrary/classes/DomoStream.py'),
                                                 'domolibrary.classes.DomoStream.DomoStream.create_stream': ( 'classes/domostream.html#domostream.create_stream',
                                                                                                              'domolibrary/classes/DomoStream.py'),
                                                 'domolibrary.classes.DomoStream.DomoStream.get_stream_by_id': ( 'classes/domostream.html#domostream.get_stream_by_id',
                                                                                                                 'domolibrary/classes/DomoStream.py'),
                                                 'domolibrary.classes.DomoStream.DomoStream.update_stream': ( 'classes/domostream.html#domostream.update_stream',
@@ -1124,14 +1140,18 @@
                                                                                                 'domolibrary/routes/role.py'),
                                          'domolibrary.routes.role.set_default_role': ( 'routes/role.html#set_default_role',
                                                                                        'domolibrary/routes/role.py'),
                                          'domolibrary.routes.role.set_role_grants': ( 'routes/role.html#set_role_grants',
                                                                                       'domolibrary/routes/role.py'),
                                          'domolibrary.routes.role.update_role_metadata': ( 'routes/role.html#update_role_metadata',
                                                                                            'domolibrary/routes/role.py')},
+            'domolibrary.routes.sandbox': { 'domolibrary.routes.sandbox.get_repo_from_id': ( 'routes/sandbox.html#get_repo_from_id',
+                                                                                             'domolibrary/routes/sandbox.py'),
+                                            'domolibrary.routes.sandbox.get_shared_repos': ( 'routes/sandbox.html#get_shared_repos',
+                                                                                             'domolibrary/routes/sandbox.py')},
             'domolibrary.routes.stream': { 'domolibrary.routes.stream.create_stream': ( 'routes/stream.html#create_stream',
                                                                                         'domolibrary/routes/stream.py'),
                                            'domolibrary.routes.stream.execute_stream': ( 'routes/stream.html#execute_stream',
                                                                                          'domolibrary/routes/stream.py'),
                                            'domolibrary.routes.stream.get_stream_by_id': ( 'routes/stream.html#get_stream_by_id',
                                                                                            'domolibrary/routes/stream.py'),
                                            'domolibrary.routes.stream.update_stream': ( 'routes/stream.html#update_stream',
```

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.96/domolibrary/classes/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.96/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoApplication.py` & `domolibrary-0.1.96/domolibrary/classes/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.96/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoCard.py` & `domolibrary-0.1.96/domolibrary/classes/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.96/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.96/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.96/domolibrary/classes/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.96/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.96/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.96/domolibrary/classes/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoJob.py` & `domolibrary-0.1.96/domolibrary/classes/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoLineage.py` & `domolibrary-0.1.96/domolibrary/classes/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.96/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoPage.py` & `domolibrary-0.1.96/domolibrary/classes/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoPublish.py` & `domolibrary-0.1.96/domolibrary/classes/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.96/domolibrary/classes/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoStream.py` & `domolibrary-0.1.96/domolibrary/classes/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.96/domolibrary/classes/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.96/domolibrary/client/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/client/DomoError.py` & `domolibrary-0.1.96/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/client/Logger.py` & `domolibrary-0.1.96/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.96/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/client/get_data.py` & `domolibrary-0.1.96/domolibrary/client/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/integrations/Automation.py` & `domolibrary-0.1.96/domolibrary/integrations/Automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.96/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.96/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/account.py` & `domolibrary-0.1.96/domolibrary/routes/account.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/activity_log.py` & `domolibrary-0.1.96/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/application.py` & `domolibrary-0.1.96/domolibrary/routes/application.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.96/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/card.py` & `domolibrary-0.1.96/domolibrary/routes/card.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/datacenter.py` & `domolibrary-0.1.96/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/dataflow.py` & `domolibrary-0.1.96/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/dataset.py` & `domolibrary-0.1.96/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/grant.py` & `domolibrary-0.1.96/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/group.py` & `domolibrary-0.1.96/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/instance_config.py` & `domolibrary-0.1.96/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/job.py` & `domolibrary-0.1.96/domolibrary/routes/job.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/page.py` & `domolibrary-0.1.96/domolibrary/routes/page.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/pdp.py` & `domolibrary-0.1.96/domolibrary/routes/pdp.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/publish.py` & `domolibrary-0.1.96/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/role.py` & `domolibrary-0.1.96/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/stream.py` & `domolibrary-0.1.96/domolibrary/routes/stream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/routes/user.py` & `domolibrary-0.1.96/domolibrary/routes/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/utils/DictDot.py` & `domolibrary-0.1.96/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.96/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/utils/convert.py` & `domolibrary-0.1.96/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.96/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary/utils/upload_data.py` & `domolibrary-0.1.96/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.96/domolibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.95
+Version: 0.1.96
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary-0.1.95/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.96/domolibrary.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 domolibrary/classes/DomoInstanceConfig.py
 domolibrary/classes/DomoJob.py
 domolibrary/classes/DomoLineage.py
 domolibrary/classes/DomoPDP.py
 domolibrary/classes/DomoPage.py
 domolibrary/classes/DomoPublish.py
 domolibrary/classes/DomoRole.py
+domolibrary/classes/DomoSandbox.py
 domolibrary/classes/DomoStream.py
 domolibrary/classes/DomoUser.py
 domolibrary/classes/__init__.py
 domolibrary/client/DomoAuth.py
 domolibrary/client/DomoError.py
 domolibrary/client/Logger.py
 domolibrary/client/ResponseGetData.py
@@ -113,14 +114,15 @@
 domolibrary/routes/group.py
 domolibrary/routes/instance_config.py
 domolibrary/routes/job.py
 domolibrary/routes/page.py
 domolibrary/routes/pdp.py
 domolibrary/routes/publish.py
 domolibrary/routes/role.py
+domolibrary/routes/sandbox.py
 domolibrary/routes/stream.py
 domolibrary/routes/user.py
 domolibrary/utils/DictDot.py
 domolibrary/utils/__init__.py
 domolibrary/utils/chunk_execution.py
 domolibrary/utils/convert.py
 domolibrary/utils/read_creds_from_dotenv.py
```

### Comparing `domolibrary-0.1.95/settings.ini` & `domolibrary-0.1.96/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.95
+version = 0.1.96
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.95/setup.py` & `domolibrary-0.1.96/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/utils/Base.py` & `domolibrary-0.1.96/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/utils/DictDot.py` & `domolibrary-0.1.96/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/utils/Exceptions.py` & `domolibrary-0.1.96/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/utils/LoggerClass.py` & `domolibrary-0.1.96/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/utils/chunk_execution.py` & `domolibrary-0.1.96/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/utils/consol_get_creds.py` & `domolibrary-0.1.96/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/utils/convert.py` & `domolibrary-0.1.96/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.96/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.95/utils/upload_data.py` & `domolibrary-0.1.96/utils/upload_data.py`

 * *Files identical despite different names*

