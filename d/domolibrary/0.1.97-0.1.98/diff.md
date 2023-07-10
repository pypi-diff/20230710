# Comparing `tmp/domolibrary-0.1.97.tar.gz` & `tmp/domolibrary-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.97.tar", last modified: Mon Jul 10 14:54:26 2023, max compression
+gzip compressed data, was "domolibrary-0.1.98.tar", last modified: Mon Jul 10 20:51:35 2023, max compression
```

## Comparing `domolibrary-0.1.97.tar` & `domolibrary-0.1.98.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.768854 domolibrary-0.1.97/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.712854 domolibrary-0.1.97/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.97/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-06-01 20:57:16.000000 domolibrary-0.1.97/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.712854 domolibrary-0.1.97/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.97/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.720854 domolibrary-0.1.97/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.97/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.736854 domolibrary-0.1.97/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.97/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-06-01 20:57:16.000000 domolibrary-0.1.97/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.736854 domolibrary-0.1.97/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.97/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-01 20:57:16.000000 domolibrary-0.1.97/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-06-01 20:57:16.000000 domolibrary-0.1.97/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-06-01 20:57:16.000000 domolibrary-0.1.97/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-10 14:54:26.768854 domolibrary-0.1.97/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-06-01 20:57:16.000000 domolibrary-0.1.97/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.736854 domolibrary-0.1.97/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   186363 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.752854 domolibrary-0.1.97/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24105 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3477 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3962 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6722 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23039 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12268 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3427 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.752854 domolibrary-0.1.97/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12946 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12077 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.756854 domolibrary-0.1.97/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/integrations/Automation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.760854 domolibrary-0.1.97/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/application.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2369 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8439 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/job.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2527 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/sandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/stream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10314 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.764854 domolibrary-0.1.97/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-07-10 14:54:17.000000 domolibrary-0.1.97/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.740854 domolibrary-0.1.97/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-10 14:54:26.000000 domolibrary-0.1.97/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4206 2023-07-10 14:54:26.000000 domolibrary-0.1.97/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-10 14:54:26.000000 domolibrary-0.1.97/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-07-10 14:54:26.000000 domolibrary-0.1.97/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-01 20:57:34.000000 domolibrary-0.1.97/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-07-10 14:54:26.000000 domolibrary-0.1.97/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-07-10 14:54:26.000000 domolibrary-0.1.97/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-07-10 14:53:58.000000 domolibrary-0.1.97/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-10 14:54:26.768854 domolibrary-0.1.97/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-06-01 20:57:16.000000 domolibrary-0.1.97/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 14:54:26.768854 domolibrary-0.1.97/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-06-01 20:57:16.000000 domolibrary-0.1.97/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-06-01 20:57:16.000000 domolibrary-0.1.97/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-06-01 20:57:16.000000 domolibrary-0.1.97/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-06-01 20:57:16.000000 domolibrary-0.1.97/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-06-01 20:57:16.000000 domolibrary-0.1.97/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.97/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-06-01 20:57:16.000000 domolibrary-0.1.97/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-06-01 20:57:16.000000 domolibrary-0.1.97/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-06-01 20:57:16.000000 domolibrary-0.1.97/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-01 20:57:16.000000 domolibrary-0.1.97/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-06-01 20:57:16.000000 domolibrary-0.1.97/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.099132 domolibrary-0.1.98/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.063132 domolibrary-0.1.98/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.98/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-06-01 20:57:16.000000 domolibrary-0.1.98/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.063132 domolibrary-0.1.98/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.98/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.071132 domolibrary-0.1.98/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.98/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.079132 domolibrary-0.1.98/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.98/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-06-01 20:57:16.000000 domolibrary-0.1.98/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.079132 domolibrary-0.1.98/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.98/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-01 20:57:16.000000 domolibrary-0.1.98/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-06-01 20:57:16.000000 domolibrary-0.1.98/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-06-01 20:57:16.000000 domolibrary-0.1.98/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-10 20:51:35.095132 domolibrary-0.1.98/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-06-01 20:57:16.000000 domolibrary-0.1.98/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.079132 domolibrary-0.1.98/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   186363 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.087132 domolibrary-0.1.98/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24126 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3477 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3962 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6722 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23039 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12268 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3427 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.087132 domolibrary-0.1.98/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12946 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12077 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.087132 domolibrary-0.1.98/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/integrations/Automation.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.091132 domolibrary-0.1.98/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/application.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2369 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8439 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/job.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2527 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/sandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/stream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10314 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.095132 domolibrary-0.1.98/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-07-10 20:51:22.000000 domolibrary-0.1.98/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.079132 domolibrary-0.1.98/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-10 20:51:34.000000 domolibrary-0.1.98/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4206 2023-07-10 20:51:34.000000 domolibrary-0.1.98/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-10 20:51:34.000000 domolibrary-0.1.98/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-07-10 20:51:34.000000 domolibrary-0.1.98/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-01 20:57:34.000000 domolibrary-0.1.98/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-07-10 20:51:34.000000 domolibrary-0.1.98/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-07-10 20:51:34.000000 domolibrary-0.1.98/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-07-10 20:51:07.000000 domolibrary-0.1.98/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-10 20:51:35.099132 domolibrary-0.1.98/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-06-01 20:57:16.000000 domolibrary-0.1.98/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-10 20:51:35.095132 domolibrary-0.1.98/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-06-01 20:57:16.000000 domolibrary-0.1.98/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-06-01 20:57:16.000000 domolibrary-0.1.98/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-06-01 20:57:16.000000 domolibrary-0.1.98/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-06-01 20:57:16.000000 domolibrary-0.1.98/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-06-01 20:57:16.000000 domolibrary-0.1.98/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.98/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-06-01 20:57:16.000000 domolibrary-0.1.98/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-06-01 20:57:16.000000 domolibrary-0.1.98/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-06-01 20:57:16.000000 domolibrary-0.1.98/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-01 20:57:16.000000 domolibrary-0.1.98/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-06-01 20:57:16.000000 domolibrary-0.1.98/utils/upload_data.py
```

### Comparing `domolibrary-0.1.97/Automation/automation.py` & `domolibrary-0.1.98/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DataOcean/Transport.py` & `domolibrary-0.1.98/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.98/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.98/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DataOcean/cnfg_s3.py` & `domolibrary-0.1.98/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.98/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoAccount.py` & `domolibrary-0.1.98/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.98/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.98/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoApplication.py` & `domolibrary-0.1.98/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoAuth.py` & `domolibrary-0.1.98/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.98/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoCard.py` & `domolibrary-0.1.98/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoCertification.py` & `domolibrary-0.1.98/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.98/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.98/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoDataset.py` & `domolibrary-0.1.98/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoGrant.py` & `domolibrary-0.1.98/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoGroup.py` & `domolibrary-0.1.98/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.98/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoJob.py` & `domolibrary-0.1.98/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoLineage.py` & `domolibrary-0.1.98/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoPDP.py` & `domolibrary-0.1.98/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoPage.py` & `domolibrary-0.1.98/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoPublish.py` & `domolibrary-0.1.98/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoRole.py` & `domolibrary-0.1.98/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.98/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoStream.py` & `domolibrary-0.1.98/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoTag.py` & `domolibrary-0.1.98/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/DomoUser.py` & `domolibrary-0.1.98/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/get_data.py` & `domolibrary-0.1.98/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.98/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/LICENSE` & `domolibrary-0.1.98/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/PKG-INFO` & `domolibrary-0.1.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.97
+Version: 0.1.98
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary-0.1.97/README.md` & `domolibrary-0.1.98/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/_modidx.py` & `domolibrary-0.1.98/domolibrary/_modidx.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.98/domolibrary/classes/DomoAccount.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
         """converts data_v1_accounts API response into an accounts class object"""
 
         dd = util_dd.DictDot(obj)
 
         return cls(
             id=dd.id or dd.databaseId,
             name=dd.displayName,
-            data_provider_type=dd.dataProviderType,
+            data_provider_type=dd.dataProviderId or dd.dataProviderType,
             created_dt=cd.convert_epoch_millisecond_to_datetime(dd.createdAt or dd.createDate),
             modified_dt=cd.convert_epoch_millisecond_to_datetime(dd.modifiedAt or dd.lastModified),
             auth=auth,
         )
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 21
 class DomoAccount_DataProviderType_ConfigNotDefined(de.DomoError):
```

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.98/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoApplication.py` & `domolibrary-0.1.98/domolibrary/classes/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.98/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoCard.py` & `domolibrary-0.1.98/domolibrary/classes/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.98/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.98/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.98/domolibrary/classes/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.98/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.98/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.98/domolibrary/classes/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoJob.py` & `domolibrary-0.1.98/domolibrary/classes/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoLineage.py` & `domolibrary-0.1.98/domolibrary/classes/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.98/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoPage.py` & `domolibrary-0.1.98/domolibrary/classes/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoPublish.py` & `domolibrary-0.1.98/domolibrary/classes/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.98/domolibrary/classes/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoSandbox.py` & `domolibrary-0.1.98/domolibrary/classes/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoStream.py` & `domolibrary-0.1.98/domolibrary/classes/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.98/domolibrary/classes/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.98/domolibrary/client/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/client/DomoError.py` & `domolibrary-0.1.98/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/client/Logger.py` & `domolibrary-0.1.98/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.98/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/client/get_data.py` & `domolibrary-0.1.98/domolibrary/client/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/integrations/Automation.py` & `domolibrary-0.1.98/domolibrary/integrations/Automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.98/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.98/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/account.py` & `domolibrary-0.1.98/domolibrary/routes/account.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/activity_log.py` & `domolibrary-0.1.98/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/application.py` & `domolibrary-0.1.98/domolibrary/routes/application.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.98/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/card.py` & `domolibrary-0.1.98/domolibrary/routes/card.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/datacenter.py` & `domolibrary-0.1.98/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/dataflow.py` & `domolibrary-0.1.98/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/dataset.py` & `domolibrary-0.1.98/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/grant.py` & `domolibrary-0.1.98/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/group.py` & `domolibrary-0.1.98/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/instance_config.py` & `domolibrary-0.1.98/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/job.py` & `domolibrary-0.1.98/domolibrary/routes/job.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/page.py` & `domolibrary-0.1.98/domolibrary/routes/page.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/pdp.py` & `domolibrary-0.1.98/domolibrary/routes/pdp.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/publish.py` & `domolibrary-0.1.98/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/role.py` & `domolibrary-0.1.98/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/sandbox.py` & `domolibrary-0.1.98/domolibrary/routes/sandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/stream.py` & `domolibrary-0.1.98/domolibrary/routes/stream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/routes/user.py` & `domolibrary-0.1.98/domolibrary/routes/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/utils/DictDot.py` & `domolibrary-0.1.98/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.98/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/utils/convert.py` & `domolibrary-0.1.98/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.98/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary/utils/upload_data.py` & `domolibrary-0.1.98/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.98/domolibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.97
+Version: 0.1.98
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary-0.1.97/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.98/domolibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/settings.ini` & `domolibrary-0.1.98/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.97
+version = 0.1.98
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.97/setup.py` & `domolibrary-0.1.98/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/utils/Base.py` & `domolibrary-0.1.98/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/utils/DictDot.py` & `domolibrary-0.1.98/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/utils/Exceptions.py` & `domolibrary-0.1.98/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/utils/LoggerClass.py` & `domolibrary-0.1.98/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/utils/chunk_execution.py` & `domolibrary-0.1.98/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/utils/consol_get_creds.py` & `domolibrary-0.1.98/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/utils/convert.py` & `domolibrary-0.1.98/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.98/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.97/utils/upload_data.py` & `domolibrary-0.1.98/utils/upload_data.py`

 * *Files identical despite different names*

