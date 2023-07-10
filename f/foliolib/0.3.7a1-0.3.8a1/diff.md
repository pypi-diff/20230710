# Comparing `tmp/foliolib-0.3.7a1.tar.gz` & `tmp/foliolib-0.3.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliolib-0.3.7a1.tar", last modified: Sun Jun 18 08:03:26 2023, max compression
+gzip compressed data, was "foliolib-0.3.8a1.tar", last modified: Mon Jul 10 17:46:11 2023, max compression
```

## Comparing `foliolib-0.3.7a1.tar` & `foliolib-0.3.8a1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-06-18 08:03:26.231989 foliolib-0.3.7a1/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.7a1/COPYING
--rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.7a1/MANIFEST.in
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2459 2023-06-18 08:03:26.231989 foliolib-0.3.7a1/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1719 2023-02-21 11:23:02.000000 foliolib-0.3.7a1/README.rst
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-06-18 08:03:26.219989 foliolib-0.3.7a1/foliolib/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.7a1/foliolib/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-06-18 08:03:23.000000 foliolib-0.3.7a1/foliolib/__version__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-06-18 08:03:26.223989 foliolib-0.3.7a1/foliolib/apiBuilder/
--rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.7a1/foliolib/apiBuilder/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.7a1/foliolib/apiBuilder/build_api.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.7a1/foliolib/apiBuilder/cli.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-06-18 08:03:26.223989 foliolib-0.3.7a1/foliolib/cli/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3820 2023-06-16 04:28:16.000000 foliolib-0.3.7a1/foliolib/cli/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-06-18 08:03:26.223989 foliolib-0.3.7a1/foliolib/cli/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.7a1/foliolib/cli/folio/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.7a1/foliolib/cli/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.7a1/foliolib/cli/main.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.7a1/foliolib/cli/main_err.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.7a1/foliolib/cli/main_noauth.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.7a1/foliolib/cli/module.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.7a1/foliolib/cli/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.7a1/foliolib/cli/orderedGroup.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3892 2023-05-29 05:12:42.000000 foliolib-0.3.7a1/foliolib/cli/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.7a1/foliolib/cli/server.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.7a1/foliolib/cli/tenant.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12652 2023-05-26 13:04:01.000000 foliolib-0.3.7a1/foliolib/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.7a1/foliolib/exceptions.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-06-18 08:03:26.223989 foliolib-0.3.7a1/foliolib/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.7a1/foliolib/folio/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-06-18 08:03:26.231989 foliolib-0.3.7a1/foliolib/folio/api/
--rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.7a1/foliolib/folio/api/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/audit.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2643 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/authtoken.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6783 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/bulkOperations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8152 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/calendar.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    40174 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/circulation.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/circulationStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/configuration.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10526 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/consortia.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/copycat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/courses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/dataExport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6349 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/dataExportSpring.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10066 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/dataExportWorker.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/dataImportConverterStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    41060 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/diConverterStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2213 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/ebsconet.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/email.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4984 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/entitiesLinks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/ermUsage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4482 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/ermUsageHarvester.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8498 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/eusageReports.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/eventConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-05-20 04:20:09.000000 foliolib-0.3.7a1/foliolib/folio/api/feesfines.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-05-20 04:20:10.000000 foliolib-0.3.7a1/foliolib/folio/api/finance.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-05-20 04:20:10.000000 foliolib-0.3.7a1/foliolib/folio/api/financeStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-05-20 04:20:10.000000 foliolib-0.3.7a1/foliolib/folio/api/fincConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6999 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/folioCustomFields.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1342 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/folioSpringBase.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1787 2023-05-20 04:20:08.000000 foliolib-0.3.7a1/foliolib/folio/api/folioVertxLib.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-05-20 04:20:10.000000 foliolib-0.3.7a1/foliolib/folio/api/gobi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7801 2023-05-20 04:20:10.000000 foliolib-0.3.7a1/foliolib/folio/api/idmConnect.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    74110 2023-05-20 04:20:28.000000 foliolib-0.3.7a1/foliolib/folio/api/innReach.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-05-20 04:20:28.000000 foliolib-0.3.7a1/foliolib/folio/api/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)   220610 2023-05-20 04:20:29.000000 foliolib-0.3.7a1/foliolib/folio/api/inventoryStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-05-20 04:20:29.000000 foliolib-0.3.7a1/foliolib/folio/api/inventoryUpdate.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-05-20 04:20:29.000000 foliolib-0.3.7a1/foliolib/folio/api/invoice.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-05-20 04:20:29.000000 foliolib-0.3.7a1/foliolib/folio/api/invoiceStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-05-20 04:20:29.000000 foliolib-0.3.7a1/foliolib/folio/api/kbEbscoJava.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-05-20 04:20:29.000000 foliolib-0.3.7a1/foliolib/folio/api/ldp.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-05-20 04:20:29.000000 foliolib-0.3.7a1/foliolib/folio/api/licenses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-05-20 04:20:29.000000 foliolib-0.3.7a1/foliolib/folio/api/login.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-05-20 04:20:29.000000 foliolib-0.3.7a1/foliolib/folio/api/loginSaml.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-05-20 04:20:29.000000 foliolib-0.3.7a1/foliolib/folio/api/marccat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    20533 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/metaStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8754 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/notes.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/notify.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12105 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/oaiPmh.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/orders.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/ordersStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/organizations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/organizationsStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3632 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/passwordValidator.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/patron.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/patronBlocks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/permissions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/pubsub.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4214 2023-05-20 04:20:30.000000 foliolib-0.3.7a1/foliolib/folio/api/quickMarc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17165 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/remoteStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    21731 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/reservoir.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/rtac.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17672 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/search.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/sender.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5419 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/settings.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11215 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/sharedIndex.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    23625 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/sourceRecordManager.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    28052 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/sourceRecordStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3187 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/tags.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/templateEngine.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/userImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24002 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/users.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-05-20 04:20:31.000000 foliolib-0.3.7a1/foliolib/folio/api/usersBl.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.7a1/foliolib/folio/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.7a1/foliolib/folio/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.7a1/foliolib/folio/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.7a1/foliolib/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24355 2023-05-09 16:17:52.000000 foliolib-0.3.7a1/foliolib/folio/inventoryReferenceData.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9397 2023-05-20 07:12:08.000000 foliolib-0.3.7a1/foliolib/folio/users.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-06-18 08:03:26.231989 foliolib-0.3.7a1/foliolib/helper/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1207 2023-04-21 05:23:46.000000 foliolib-0.3.7a1/foliolib/helper/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9311 2023-04-21 05:23:46.000000 foliolib-0.3.7a1/foliolib/helper/database.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.7a1/foliolib/helper/folio.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.7a1/foliolib/helper/modules.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.7a1/foliolib/helper/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6637 2023-05-27 07:21:39.000000 foliolib-0.3.7a1/foliolib/helper/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1517 2022-10-11 03:48:54.000000 foliolib-0.3.7a1/foliolib/helper/tenant.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-06-18 08:03:26.231989 foliolib-0.3.7a1/foliolib/okapi/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.7a1/foliolib/okapi/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.7a1/foliolib/okapi/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    16267 2023-04-21 05:23:46.000000 foliolib-0.3.7a1/foliolib/okapi/kubeClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.7a1/foliolib/okapi/misc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    39439 2023-06-16 08:13:58.000000 foliolib-0.3.7a1/foliolib/okapi/okapiClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.7a1/foliolib/okapi/okapiModule.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17123 2023-05-24 12:23:18.000000 foliolib-0.3.7a1/foliolib/okapi/okapiModuleKubernetes.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-06-18 08:03:26.223989 foliolib-0.3.7a1/foliolib.egg-info/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2459 2023-06-18 08:03:26.000000 foliolib-0.3.7a1/foliolib.egg-info/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3790 2023-06-18 08:03:26.000000 foliolib-0.3.7a1/foliolib.egg-info/SOURCES.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-06-18 08:03:26.000000 foliolib-0.3.7a1/foliolib.egg-info/dependency_links.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)       46 2023-06-18 08:03:26.000000 foliolib-0.3.7a1/foliolib.egg-info/entry_points.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-06-18 08:03:26.000000 foliolib-0.3.7a1/foliolib.egg-info/requires.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-06-18 08:03:26.000000 foliolib-0.3.7a1/foliolib.egg-info/top_level.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.7a1/requirements.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1182 2023-06-18 08:03:26.231989 foliolib-0.3.7a1/setup.cfg
--rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2023-05-29 06:44:32.000000 foliolib-0.3.7a1/setup.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.383590 foliolib-0.3.8a1/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.8a1/COPYING
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.8a1/MANIFEST.in
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2752 2023-07-10 17:46:11.383590 foliolib-0.3.8a1/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2012 2023-07-10 17:43:35.000000 foliolib-0.3.8a1/README.rst
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.371590 foliolib-0.3.8a1/foliolib/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.8a1/foliolib/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-07-10 17:46:09.000000 foliolib-0.3.8a1/foliolib/__version__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.371590 foliolib-0.3.8a1/foliolib/apiBuilder/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.8a1/foliolib/apiBuilder/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.8a1/foliolib/apiBuilder/build_api.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.8a1/foliolib/apiBuilder/cli.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.375590 foliolib-0.3.8a1/foliolib/cli/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3820 2023-06-16 04:28:16.000000 foliolib-0.3.8a1/foliolib/cli/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.375590 foliolib-0.3.8a1/foliolib/cli/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.8a1/foliolib/cli/folio/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.8a1/foliolib/cli/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.8a1/foliolib/cli/main.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.8a1/foliolib/cli/main_err.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.8a1/foliolib/cli/main_noauth.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.8a1/foliolib/cli/module.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.8a1/foliolib/cli/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.8a1/foliolib/cli/orderedGroup.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3892 2023-05-29 05:12:42.000000 foliolib-0.3.8a1/foliolib/cli/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.8a1/foliolib/cli/server.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.8a1/foliolib/cli/tenant.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12652 2023-05-26 13:04:01.000000 foliolib-0.3.8a1/foliolib/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.8a1/foliolib/exceptions.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.375590 foliolib-0.3.8a1/foliolib/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.8a1/foliolib/folio/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.379590 foliolib-0.3.8a1/foliolib/folio/api/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.8a1/foliolib/folio/api/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/audit.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2643 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/authtoken.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7100 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/bulkOperations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8152 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/calendar.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    40915 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/circulation.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/circulationStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/configuration.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    16302 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/consortia.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/copycat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/courses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/dataExport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6349 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/dataExportSpring.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10066 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/dataExportWorker.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/dataImportConverterStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    41060 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/diConverterStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2213 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/ebsconet.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/email.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5628 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/entitiesLinks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/ermUsage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5745 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/ermUsageHarvester.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8498 2023-07-10 17:25:43.000000 foliolib-0.3.8a1/foliolib/folio/api/eusageReports.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-07-10 17:25:43.000000 foliolib-0.3.8a1/foliolib/folio/api/eventConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-07-10 17:25:43.000000 foliolib-0.3.8a1/foliolib/folio/api/feesfines.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-07-10 17:25:43.000000 foliolib-0.3.8a1/foliolib/folio/api/finance.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-07-10 17:25:43.000000 foliolib-0.3.8a1/foliolib/folio/api/financeStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-07-10 17:25:44.000000 foliolib-0.3.8a1/foliolib/folio/api/fincConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6999 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/folioCustomFields.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1342 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/folioSpringBase.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1787 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/folioVertxLib.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-07-10 17:25:44.000000 foliolib-0.3.8a1/foliolib/folio/api/gobi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7801 2023-07-10 17:25:44.000000 foliolib-0.3.8a1/foliolib/folio/api/idmConnect.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    74110 2023-07-10 17:26:02.000000 foliolib-0.3.8a1/foliolib/folio/api/innReach.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-07-10 17:26:02.000000 foliolib-0.3.8a1/foliolib/folio/api/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)   220610 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/inventoryStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/inventoryUpdate.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/invoice.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/invoiceStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/kbEbscoJava.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/ldp.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/licenses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/login.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/loginSaml.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/marccat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    20533 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/metaStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8754 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/notes.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/notify.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12602 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/oaiPmh.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/orders.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/ordersStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/organizations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/organizationsStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3632 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/passwordValidator.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/patron.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/patronBlocks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/permissions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/pubsub.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4777 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/quickMarc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17165 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/remoteStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    21731 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/reservoir.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/rtac.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    18371 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/search.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/sender.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5419 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/settings.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11215 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/sharedIndex.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    23625 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/sourceRecordManager.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    29289 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/sourceRecordStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3187 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/tags.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/templateEngine.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/userImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24695 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/users.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/usersBl.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.8a1/foliolib/folio/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.8a1/foliolib/folio/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.8a1/foliolib/folio/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.8a1/foliolib/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24355 2023-05-09 16:17:52.000000 foliolib-0.3.8a1/foliolib/folio/inventoryReferenceData.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9397 2023-05-20 07:12:08.000000 foliolib-0.3.8a1/foliolib/folio/users.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.379590 foliolib-0.3.8a1/foliolib/helper/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1207 2023-04-21 05:23:46.000000 foliolib-0.3.8a1/foliolib/helper/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9311 2023-06-29 05:24:34.000000 foliolib-0.3.8a1/foliolib/helper/database.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.8a1/foliolib/helper/folio.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.8a1/foliolib/helper/modules.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.8a1/foliolib/helper/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6637 2023-05-27 07:21:39.000000 foliolib-0.3.8a1/foliolib/helper/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1518 2023-06-23 09:49:22.000000 foliolib-0.3.8a1/foliolib/helper/tenant.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.383590 foliolib-0.3.8a1/foliolib/okapi/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.8a1/foliolib/okapi/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.8a1/foliolib/okapi/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    16267 2023-04-21 05:23:46.000000 foliolib-0.3.8a1/foliolib/okapi/kubeClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.8a1/foliolib/okapi/misc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    39439 2023-06-16 08:13:58.000000 foliolib-0.3.8a1/foliolib/okapi/okapiClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.8a1/foliolib/okapi/okapiModule.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17123 2023-06-22 08:42:17.000000 foliolib-0.3.8a1/foliolib/okapi/okapiModuleKubernetes.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.371590 foliolib-0.3.8a1/foliolib.egg-info/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2752 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3790 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/SOURCES.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/dependency_links.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       46 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/entry_points.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/requires.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/top_level.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.8a1/requirements.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1182 2023-07-10 17:46:11.383590 foliolib-0.3.8a1/setup.cfg
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2023-05-29 06:44:32.000000 foliolib-0.3.8a1/setup.py
```

### Comparing `foliolib-0.3.7a1/COPYING` & `foliolib-0.3.8a1/COPYING`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/PKG-INFO` & `foliolib-0.3.8a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.7a1
+Version: 0.3.8a1
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: COPYING
 
 ========
 FolioLib
 ========
+
 |PyPI| |Pythons| |ReadTheDocs|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/foliolib.svg
    :alt: PyPI version
    :target: https://pypi.org/project/foliolib/
 
 .. |Pythons| image:: https://img.shields.io/pypi/pyversions/foliolib.svg
@@ -34,15 +35,20 @@
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/foliolib/badge/?version=latest
     :target: https://foliolib.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 FolioLib is an API-Client for `Folio <https://www.folio.org/>`_.
 The API is generated from the RAML and OAS files from the Folio-Modules.
 
-Documentation can be found `here <https://foliolib.readthedocs.io/>`_.
+Documentation can be found at `https://foliolib.readthedocs.io/ <https://foliolib.readthedocs.io/>`_.
+
+Python packages can be found at `https://pypi.org/project/foliolib/ <https://pypi.org/project/foliolib/>`_.
+
+Debian packages can be found at `https://github.com/tobi-weber/foliolib/releases/latest/ <https://github.com/tobi-weber/foliolib/releases/latest/>`_.
+
 
 Features:
 
 - Python Folio API
 - Commandline interface
 - Install and manage Folio
 - Install and manage Folio on Kubernetes
```

### Comparing `foliolib-0.3.7a1/README.rst` & `foliolib-0.3.8a1/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ========
 FolioLib
 ========
+
 |PyPI| |Pythons| |ReadTheDocs|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/foliolib.svg
    :alt: PyPI version
    :target: https://pypi.org/project/foliolib/
 
 .. |Pythons| image:: https://img.shields.io/pypi/pyversions/foliolib.svg
@@ -14,15 +15,20 @@
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/foliolib/badge/?version=latest
     :target: https://foliolib.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 FolioLib is an API-Client for `Folio <https://www.folio.org/>`_.
 The API is generated from the RAML and OAS files from the Folio-Modules.
 
-Documentation can be found `here <https://foliolib.readthedocs.io/>`_.
+Documentation can be found at `https://foliolib.readthedocs.io/ <https://foliolib.readthedocs.io/>`_.
+
+Python packages can be found at `https://pypi.org/project/foliolib/ <https://pypi.org/project/foliolib/>`_.
+
+Debian packages can be found at `https://github.com/tobi-weber/foliolib/releases/latest/ <https://github.com/tobi-weber/foliolib/releases/latest/>`_.
+
 
 Features:
 
 - Python Folio API
 - Commandline interface
 - Install and manage Folio
 - Install and manage Folio on Kubernetes
```

### Comparing `foliolib-0.3.7a1/foliolib/__init__.py` & `foliolib-0.3.8a1/foliolib/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/apiBuilder/build_api.py` & `foliolib-0.3.8a1/foliolib/apiBuilder/build_api.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/apiBuilder/cli.py` & `foliolib-0.3.8a1/foliolib/apiBuilder/cli.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/cli/__init__.py` & `foliolib-0.3.8a1/foliolib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/cli/folio/__init__.py` & `foliolib-0.3.8a1/foliolib/cli/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/cli/main.py` & `foliolib-0.3.8a1/foliolib/cli/main.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/cli/main_noauth.py` & `foliolib-0.3.8a1/foliolib/cli/main_noauth.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/cli/module.py` & `foliolib-0.3.8a1/foliolib/cli/module.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/cli/okapi.py` & `foliolib-0.3.8a1/foliolib/cli/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/cli/platform.py` & `foliolib-0.3.8a1/foliolib/cli/platform.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/cli/server.py` & `foliolib-0.3.8a1/foliolib/cli/server.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/cli/tenant.py` & `foliolib-0.3.8a1/foliolib/cli/tenant.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/config.py` & `foliolib-0.3.8a1/foliolib/config.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/exceptions.py` & `foliolib-0.3.8a1/foliolib/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/folio/__init__.py` & `foliolib-0.3.8a1/foliolib/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/audit.py` & `foliolib-0.3.8a1/foliolib/folio/api/audit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.audit")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/authtoken.py` & `foliolib-0.3.8a1/foliolib/folio/api/authtoken.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.authtoken")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/bulkOperations.py` & `foliolib-0.3.8a1/foliolib/folio/api/bulkOperations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.bulkOperations")
 
@@ -205,7 +205,17 @@
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
             .. literalinclude:: ../files/Bulkoperations_getbulkoperationbyid_response.schema
         """
         return self.call("GET", f"/bulk-operations/{operationId}")
+
+    def cleanuplogfiles(self):
+        """Removed all files older than 30 days
+
+        ``POST /bulk-operations/clean-up-log-files``
+
+        Raises:
+            OkapiFatalError: Internal server errors, e.g. due to misconfiguration
+        """
+        return self.call("POST", "/bulk-operations/clean-up-log-files")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/calendar.py` & `foliolib-0.3.8a1/foliolib/folio/api/calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.calendar")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/circulation.py` & `foliolib-0.3.8a1/foliolib/folio/api/circulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.circulation")
 
@@ -144,14 +144,42 @@
 
         Raises:
             OkapiFatalError: Server Error
         """
         return self.call("POST", "/circulation/scheduled-age-to-lost-fee-charging")
 
 
+class AddInfo(FolioApi):
+    """API for adding patron or staff info
+
+    **Add info API**
+    """
+
+    def set_addInfo(self, loansId: str, addInfo: dict):
+        """
+
+        ``POST /circulation/loans/{loansId}/add-info``
+
+        Args:
+            loansId (str)
+            addInfo (dict): See Schema below
+
+        Raises:
+            OkapiRequestUnprocessableEntity: Unprocessable Entity
+            OkapiRequestNotFound: Not Found
+            OkapiFatalError: Server Error
+            OkapiRequestUnprocessableEntity: Unprocessable Entity
+
+        Schema:
+
+            .. literalinclude:: ../files/AddInfo_set_addInfo_request.schema
+        """
+        return self.call("POST", f"/circulation/loans/{loansId}/add-info", data=addInfo)
+
+
 class DeclareItemLost(FolioApi):
     """API for declaring loaned item lost
 
     **Declare item lost API**
     """
 
     def set_declareItemLost(self, loansId: str, declareItemLost: dict):
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/circulationStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/circulationStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.circulationStorage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/configuration.py` & `foliolib-0.3.8a1/foliolib/folio/api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.configuration")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/consortia.py` & `foliolib-0.3.8a1/foliolib/folio/api/consortia.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.consortia")
 
@@ -109,14 +109,101 @@
 
             .. literalinclude:: ../files/UserTenants_getusertenantbyassociationid_response.schema
         """
         return self.call("GET", f"/consortia/{consortiumId}/user-tenants/{associationId}")
 
 
 
+class SharingInstance(FolioApi):
+    """Sharing instance integration API
+
+    Sharing instance integration API
+    """
+
+    def getsharinginstances(self, consortiumId, **kwargs):
+        """Sharing instances
+
+        ``GET /consortia/{consortiumId}/sharing/instances``
+
+        Args:
+            consortiumId (str):
+
+        Keyword Args:
+            instanceIdentifier (str):
+            sourceTenantId (str): The ID of the source tenant
+            targetTenantId (str): The ID of the target tenant
+            status (str):
+            offset (int): Skip over a number of elements by specifying an offset value for the query (default: 0, minimum: 0, maximum: 2147483647)
+            limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0, maximum: 2147483647)
+
+        Returns:
+            dict: See Schema below.
+
+        Raises:
+            OkapiRequestError: Bad request
+            OkapiRequestNotFound: Resource not found
+            OkapiFatalError: Internal server error
+
+        Schema:
+
+            .. literalinclude:: ../files/SharingInstance_getsharinginstances_response.schema
+        """
+        return self.call("GET", f"/consortia/{consortiumId}/sharing/instances", query=kwargs)
+
+		
+    def start(self, consortiumId, sharingInstance):
+        """
+
+        ``POST /consortia/{consortiumId}/sharing/instances``
+
+        Args:
+            consortiumId (str):
+            sharingInstance (dict): See Schema below.
+
+        Returns:
+            dict: See Schema below.
+
+        Raises:
+            OkapiRequestError: Bad request
+            OkapiRequestNotFound: Resource not found
+            OkapiRequestConflict: Validation errors
+            OkapiRequestUnprocessableEntity: Validation errors
+            OkapiFatalError: Internal server error
+
+        Schema:
+
+            .. literalinclude:: ../files/SharingInstance_start_request.schema
+        """
+        return self.call("POST", f"/consortia/{consortiumId}/sharing/instances", sharingInstance)
+
+    def getsharinginstancebyid(self, consortiumId, actionId):
+        """
+
+        ``GET /consortia/{consortiumId}/sharing/instances/{actionId}``
+
+        Args:
+            consortiumId (str):
+            actionId (str):
+
+        Returns:
+            dict: See Schema below.
+
+        Raises:
+            OkapiRequestError: Bad request
+            OkapiRequestNotFound: Resource not found
+            OkapiFatalError: Internal server error
+
+        Schema:
+
+            .. literalinclude:: ../files/SharingInstance_getsharinginstancebyid_response.schema
+        """
+        return self.call("GET", f"/consortia/{consortiumId}/sharing/instances/{actionId}")
+
+
+
 class ConsortiaConfiguration(FolioApi):
     """Consortia Configuration integration API
 
     Consortia Configuration integration API
     """
 
     def getconfiguration(self):
@@ -191,38 +278,41 @@
         Schema:
 
             .. literalinclude:: ../files/Tenants_gettenants_response.schema
         """
         return self.call("GET", f"/consortia/{consortiumId}/tenants", query=kwargs)
 
 		
-    def savetenant(self, consortiumId, tenant):
+    def savetenant(self, consortiumId, tenant, **kwargs):
         """
 
         ``POST /consortia/{consortiumId}/tenants``
 
         Args:
             consortiumId (str):
             tenant (dict): See Schema below.
 
+        Keyword Args:
+            adminUserId (str):
+
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Resource not found
             OkapiRequestConflict: Validation errors
             OkapiRequestUnprocessableEntity: Validation errors
             OkapiFatalError: Internal server error
 
         Schema:
 
             .. literalinclude:: ../files/Tenants_savetenant_request.schema
         """
-        return self.call("POST", f"/consortia/{consortiumId}/tenants", tenant)
+        return self.call("POST", f"/consortia/{consortiumId}/tenants", tenant, query=kwargs)
 
     def updatetenant(self, consortiumId, tenantId, tenant):
         """
 
         ``PUT /consortia/{consortiumId}/tenants/{tenantId}``
 
         Args:
@@ -257,14 +347,109 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Resource not found
             OkapiFatalError: Internal server error
         """
         return self.call("DELETE", f"/consortia/{consortiumId}/tenants/{tenantId}")
 
+    def syncprimaryaffiliations(self, consortiumId, tenantId):
+        """
+
+        ``POST /consortia/{consortiumId}/tenants/{tenantId}/sync-primary-affiliations``
+
+        Args:
+            consortiumId (str):
+            tenantId (str): The ID of the tenant
+
+        Raises:
+            OkapiRequestError: Bad request
+            OkapiRequestNotFound: Resource not found
+            OkapiRequestConflict: Validation errors
+            OkapiRequestUnprocessableEntity: Validation errors
+            OkapiFatalError: Internal server error
+        """
+        return self.call("POST", f"/consortia/{consortiumId}/tenants/{tenantId}/sync-primary-affiliations")
+
+    def createprimaryaffiliations(self, consortiumId, tenantId, syncPrimaryAffiliationBody):
+        """
+
+        ``POST /consortia/{consortiumId}/tenants/{tenantId}/create-primary-affiliations``
+
+        Args:
+            consortiumId (str):
+            tenantId (str): The ID of the tenant
+            syncPrimaryAffiliationBody (dict): See Schema below.
+
+        Raises:
+            OkapiRequestError: Bad request
+            OkapiRequestNotFound: Resource not found
+            OkapiRequestConflict: Validation errors
+            OkapiRequestUnprocessableEntity: Validation errors
+            OkapiFatalError: Internal server error
+
+        Schema:
+
+            .. literalinclude:: ../files/Tenants_createprimaryaffiliations_request.schema
+        """
+        return self.call("POST", f"/consortia/{consortiumId}/tenants/{tenantId}/create-primary-affiliations", syncPrimaryAffiliationBody)
+
+
+
+class Publications(FolioApi):
+    """Publish coordinator API
+
+    Publish coordinator API
+    """
+
+    def publishrequests(self, consortiumId, publicationRequest):
+        """
+
+        ``POST /consortia/{consortiumId}/publications``
+
+        Args:
+            consortiumId (str):
+            publicationRequest (dict): See Schema below.
+
+        Returns:
+            dict: See Schema below.
+
+        Raises:
+            OkapiRequestError: Bad request
+            OkapiRequestConflict: Validation errors
+            OkapiFatalError: Internal server error
+
+        Schema:
+
+            .. literalinclude:: ../files/Publications_publishrequests_request.schema
+            .. literalinclude:: ../files/Publications_publishrequests_request.schema_response.schema
+        """
+        return self.call("POST", f"/consortia/{consortiumId}/publications", publicationRequest)
+
+    def getpublicationdetails(self, consortiumId, publicationId):
+        """
+
+        ``GET /consortia/{consortiumId}/publications/{publicationId}``
+
+        Args:
+            consortiumId (str):
+            publicationId (str):
+
+        Returns:
+            dict: See Schema below.
+
+        Raises:
+            OkapiRequestError: Bad request
+            OkapiFatalError: Internal server error
+
+        Schema:
+
+            .. literalinclude:: ../files/Publications_getpublicationdetails_response.schema
+        """
+        return self.call("GET", f"/consortia/{consortiumId}/publications/{publicationId}")
+
 
 
 class Self(FolioApi):
     """Self integration API
 
     Self integration API
     """
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/copycat.py` & `foliolib-0.3.8a1/foliolib/folio/api/copycat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.copycat")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/courses.py` & `foliolib-0.3.8a1/foliolib/folio/api/courses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.courses")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/dataExport.py` & `foliolib-0.3.8a1/foliolib/folio/api/dataExport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.dataExport")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/dataExportSpring.py` & `foliolib-0.3.8a1/foliolib/folio/api/dataExportSpring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.dataExportSpring")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/dataExportWorker.py` & `foliolib-0.3.8a1/foliolib/folio/api/dataExportWorker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.dataExportWorker")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/dataImport.py` & `foliolib-0.3.8a1/foliolib/folio/api/dataImport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.dataImport")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/dataImportConverterStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/dataImportConverterStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.dataImportConverterStorage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/diConverterStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/diConverterStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.diConverterStorage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/ebsconet.py` & `foliolib-0.3.8a1/foliolib/folio/api/ebsconet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.ebsconet")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/email.py` & `foliolib-0.3.8a1/foliolib/folio/api/email.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.email")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/entitiesLinks.py` & `foliolib-0.3.8a1/foliolib/folio/api/entitiesLinks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.entitiesLinks")
 
@@ -105,14 +105,35 @@
 
         Schema:
 
             .. literalinclude:: ../files/Entitieslinks_getinstanceauthoritylinkingrulebyid_response.schema
         """
         return self.call("GET", f"/linking-rules/instance-authority/{ruleId}")
 
+    def suggestlinksformarcrecord(self, parsedRecordContentCollection):
+        """Retrieve links suggestions for marc records
+
+        ``POST /links-suggestions/marc``
+
+        Args:
+            parsedRecordContentCollection (dict): See Schema below.
+
+        Returns:
+            dict: See Schema below.
+
+        Raises:
+            OkapiRequestError: Validation errors.
+            OkapiFatalError: Internal server error.
+
+        Schema:
+
+            .. literalinclude:: ../files/Entitieslinks_suggestlinksformarcrecord_request.schema
+        """
+        return self.call("POST", f"/links-suggestions/marc", parsedRecordContentCollection)
+
     def getauthoritylinksstats(self, **kwargs):
         """Retrieve authority updates (related to links) statistics
 
         ``GET /links/stats/authority``
 
         Keyword Args:
             fromDate (str): Start date to seek from (format: date-time)
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/ermUsage.py` & `foliolib-0.3.8a1/foliolib/folio/api/ermUsage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ermUsage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/eusageReports.py` & `foliolib-0.3.8a1/foliolib/folio/api/eusageReports.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.eusageReports")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/eventConfig.py` & `foliolib-0.3.8a1/foliolib/folio/api/eventConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.eventConfig")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/feesfines.py` & `foliolib-0.3.8a1/foliolib/folio/api/feesfines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.feesfines")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/finance.py` & `foliolib-0.3.8a1/foliolib/folio/api/finance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.finance")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/financeStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/financeStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.financeStorage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/fincConfig.py` & `foliolib-0.3.8a1/foliolib/folio/api/fincConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.fincConfig")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/folioCustomFields.py` & `foliolib-0.3.8a1/foliolib/folio/api/folioCustomFields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.folioCustomFields")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/folioSpringBase.py` & `foliolib-0.3.8a1/foliolib/folio/api/folioSpringBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.folioSpringBase")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/folioVertxLib.py` & `foliolib-0.3.8a1/foliolib/folio/api/folioVertxLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.folioVertxLib")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/gobi.py` & `foliolib-0.3.8a1/foliolib/folio/api/gobi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.gobi")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/idmConnect.py` & `foliolib-0.3.8a1/foliolib/folio/api/idmConnect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.idmConnect")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/innReach.py` & `foliolib-0.3.8a1/foliolib/folio/api/innReach.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.innReach")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/inventory.py` & `foliolib-0.3.8a1/foliolib/folio/api/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.inventory")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/inventoryStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/inventoryStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.inventoryStorage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/inventoryUpdate.py` & `foliolib-0.3.8a1/foliolib/folio/api/inventoryUpdate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.inventoryUpdate")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/invoice.py` & `foliolib-0.3.8a1/foliolib/folio/api/invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.invoice")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/invoiceStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/invoiceStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.invoiceStorage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/kbEbscoJava.py` & `foliolib-0.3.8a1/foliolib/folio/api/kbEbscoJava.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.kbEbscoJava")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/ldp.py` & `foliolib-0.3.8a1/foliolib/folio/api/ldp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ldp")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/licenses.py` & `foliolib-0.3.8a1/foliolib/folio/api/licenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.licenses")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/login.py` & `foliolib-0.3.8a1/foliolib/folio/api/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.login")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/loginSaml.py` & `foliolib-0.3.8a1/foliolib/folio/api/loginSaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.loginSaml")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/marccat.py` & `foliolib-0.3.8a1/foliolib/folio/api/marccat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.marccat")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/metaStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/metaStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.metaStorage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/notes.py` & `foliolib-0.3.8a1/foliolib/folio/api/notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.notes")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/notify.py` & `foliolib-0.3.8a1/foliolib/folio/api/notify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.notify")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/oaiPmh.py` & `foliolib-0.3.8a1/foliolib/folio/api/oaiPmh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.oaiPmh")
 
@@ -270,14 +270,33 @@
         Schema:
 
             .. literalinclude:: ../files/FolioSetFilteringConditions_get_filteringConditions_return.schema 
         """
         return self.call("GET", "/oai-pmh/filtering-conditions")
 
 
+class CleanupErrorLogs(FolioApi):
+    """OAI-PMH Error Logs Cleaning API
+
+    provides endpoint for triggering clean up process of old error logs.
+    """
+
+    def set_cleanUpErrorLog(self):
+        """
+
+        ``POST /oai-pmh/clean-up-error-logs``
+
+        Raises:
+            OkapiRequestError: Bad Request
+            OkapiFatalError: Server Error
+            OkapiRequestUnprocessableEntity: Unprocessable Entity
+        """
+        return self.call("POST", "/oai-pmh/clean-up-error-logs")
+
+
 class FolioSet(FolioApi):
     """Set API
 
     API for managing sets and filtering conditions that is used as part of metadata harvesting protocol implementation
     """
 
     def get_sets(self, **kwargs):
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/orders.py` & `foliolib-0.3.8a1/foliolib/folio/api/orders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.orders")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/ordersStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/ordersStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ordersStorage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/organizations.py` & `foliolib-0.3.8a1/foliolib/folio/api/organizations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.organizations")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/organizationsStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/organizationsStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.organizationsStorage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/passwordValidator.py` & `foliolib-0.3.8a1/foliolib/folio/api/passwordValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.passwordValidator")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/patron.py` & `foliolib-0.3.8a1/foliolib/folio/api/patron.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.patron")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/patronBlocks.py` & `foliolib-0.3.8a1/foliolib/folio/api/patronBlocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.patronBlocks")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/permissions.py` & `foliolib-0.3.8a1/foliolib/folio/api/permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.permissions")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/pubsub.py` & `foliolib-0.3.8a1/foliolib/folio/api/pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.pubsub")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/quickMarc.py` & `foliolib-0.3.8a1/foliolib/folio/api/quickMarc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.quickMarc")
 
@@ -79,14 +79,35 @@
 
         Schema:
 
             .. literalinclude:: ../files/Recordseditor_getrecordcreationstatus_response.schema
         """
         return self.call("GET", "/records-editor/records/status", query=kwargs)
 
+    def suggestion(self, quickMarcView):
+        """
+
+        ``POST /records-editor/links/suggestion``
+
+        Args:
+            quickMarcView (dict): See Schema below.
+
+        Returns:
+            dict: See Schema below.
+
+        Raises:
+            OkapiRequestError: Bad Request
+            OkapiFatalError: Internal server error, e.g. due to misconfiguration
+
+        Schema:
+
+            .. literalinclude:: ../files/Recordseditor_suggestion_request.schema
+        """
+        return self.call("POST", f"/records-editor/links/suggestion", quickMarcView)
+
 
 
 class Recordseditorasync(FolioApi):
     """quickMARC Record Editor
 
     
     """
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/remoteStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/remoteStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.remoteStorage")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/reservoir.py` & `foliolib-0.3.8a1/foliolib/folio/api/reservoir.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.reservoir")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/rtac.py` & `foliolib-0.3.8a1/foliolib/folio/api/rtac.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.rtac")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/search.py` & `foliolib-0.3.8a1/foliolib/folio/api/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.search")
 
@@ -172,15 +172,15 @@
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
         """
         return self.call("GET", f"/search/resources/jobs/{jobId}/ids")
 
     def browseinstancesbycallnumber(self, **kwargs):
         """Provides list of instances for browsing by call number
 
-        ``GET /search/browse/call-numbers/instances``
+        ``GET /browse/call-numbers/instances``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
             limit (int): Limit the number of elements returned in the browse response. (minimum: 0, maximum: 100, default: 100)
             expandAll (bool): Whether to return only basic properties or entire instance. (default: False)
             highlightMatch (bool): Whether to highlight matched resource by query input or not. (default: True)
             precedingRecordsCount (int): Number of preceding records for browsing around and around-including options (minimum: 1, maximum: 100)
@@ -193,20 +193,20 @@
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
             .. literalinclude:: ../files/Search_browseinstancesbycallnumber_response.schema
         """
-        return self.call("GET", "/search/browse/call-numbers/instances", query=kwargs)
+        return self.call("GET", "/browse/call-numbers/instances", query=kwargs)
 
     def browseinstancesbysubject(self, **kwargs):
         """Provides list of instances for browsing by subject
 
-        ``GET /search/browse/subjects/instances``
+        ``GET /browse/subjects/instances``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
             limit (int): Limit the number of elements returned in the response. (minimum: 0, maximum: 500, default: 100)
             highlightMatch (bool): Whether to highlight matched resource by query input or not. (default: True)
             precedingRecordsCount (int): Number of preceding records for browsing around and around-including options (minimum: 1, maximum: 100)
 
@@ -217,20 +217,20 @@
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
             .. literalinclude:: ../files/Search_browseinstancesbysubject_response.schema
         """
-        return self.call("GET", "/search/browse/subjects/instances", query=kwargs)
+        return self.call("GET", "/browse/subjects/instances", query=kwargs)
 
     def browseinstancesbycontributor(self, **kwargs):
         """Provides list of instances for browsing by contributor
 
-        ``GET /search/browse/contributors/instances``
+        ``GET /browse/contributors/instances``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
             limit (int): Limit the number of elements returned in the response. (minimum: 0, maximum: 500, default: 100)
             highlightMatch (bool): Whether to highlight matched resource by query input or not. (default: True)
             precedingRecordsCount (int): Number of preceding records for browsing around and around-including options (minimum: 1, maximum: 100)
 
@@ -241,20 +241,20 @@
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
             .. literalinclude:: ../files/Search_browseinstancesbycontributor_response.schema
         """
-        return self.call("GET", "/search/browse/contributors/instances", query=kwargs)
+        return self.call("GET", "/browse/contributors/instances", query=kwargs)
 
     def browseauthorities(self, **kwargs):
         """Provides list of authorities by headingRef
 
-        ``GET /search/browse/authorities``
+        ``GET /browse/authorities``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
             limit (int): Limit the number of elements returned in the response. (minimum: 0, maximum: 500, default: 100)
             expandAll (bool): Whether to return only basic properties or entire instance. (default: False)
             highlightMatch (bool): Whether to highlight matched resource by query input or not. (default: True)
             precedingRecordsCount (int): Number of preceding records for browsing around and around-including options (minimum: 1, maximum: 100)
@@ -266,15 +266,15 @@
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
             .. literalinclude:: ../files/Search_browseauthorities_response.schema
         """
-        return self.call("GET", "/search/browse/authorities", query=kwargs)
+        return self.call("GET", "/browse/authorities", query=kwargs)
 
     def createindices(self, createIndexRequest):
         """Creates indices for passed resource name and tenant id in request header.
 
         ``POST /search/index/indices``
 
         Args:
@@ -311,14 +311,35 @@
         Schema:
 
             .. literalinclude:: ../files/Search_updatemappings_request.schema
             .. literalinclude:: ../files/Search_updatemappings_request.schema_response.schema
         """
         return self.call("POST", f"/search/index/mappings", updateMappingsRequest)
 
+    def updateindexdynamicsettings(self, updateIndexDynamicSettingsRequest):
+        """Update Index Dynamic Settings data.
+
+        ``PUT /search/index/settings``
+
+        Args:
+            updateIndexDynamicSettingsRequest (dict): See Schema below.
+
+        Returns:
+            dict: See Schema below.
+
+        Raises:
+            OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
+
+        Schema:
+
+            .. literalinclude:: ../files/Search_updateindexdynamicsettings_request.schema
+            .. literalinclude:: ../files/Search_updateindexdynamicsettings_request.schema_response.schema
+        """
+        return self.call("PUT", f"/search/index/settings", updateIndexDynamicSettingsRequest)
+
     def reindexinventoryrecords(self, reindexRequest):
         """Initiates reindex for the inventory records
 
         ``POST /search/index/inventory/reindex``
 
         Args:
             reindexRequest (dict): See Schema below.
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/sender.py` & `foliolib-0.3.8a1/foliolib/folio/api/sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.sender")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/settings.py` & `foliolib-0.3.8a1/foliolib/folio/api/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.settings")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/sharedIndex.py` & `foliolib-0.3.8a1/foliolib/folio/api/sharedIndex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.sharedIndex")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/sourceRecordManager.py` & `foliolib-0.3.8a1/foliolib/folio/api/sourceRecordManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.sourceRecordManager")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/sourceRecordStorage.py` & `foliolib-0.3.8a1/foliolib/folio/api/sourceRecordStorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.sourceRecordStorage")
 
@@ -681,14 +681,62 @@
             OkapiRequestError: Bad Request
             OkapiRequestUnprocessableEntity: Unprocessable Entity
             OkapiFatalError: Server Error
         """
         return self.call("PUT", f"/source-storage/records/{recordsId}/suppress-from-discovery", query=kwargs)
 
 
+class SourceRecordStorageMigrationsJobs(FolioApi):
+    """Source Record Storage Migration Jobs API
+
+    API for managing asynchronous migration jobs
+    """
+
+    def set_job(self, job: dict):
+        """Initiate a migration job
+
+        ``POST /source-storage/migrations/jobs``
+
+        Args:
+            job (dict): See Schema below
+
+        Returns:
+            dict: See Schema below
+
+        Raises:
+            OkapiFatalError: Server Error
+
+        Schema:
+
+            .. literalinclude:: ../files/SourceRecordStorageMigrationsJobs_set_job_request.schema
+            .. literalinclude:: ../files/SourceRecordStorageMigrationsJobs_set_job_return.schema 
+        """
+        return self.call("POST", "/source-storage/migrations/jobs", data=job)
+
+    def get_job(self, jobsId: str):
+        """Get a migration job
+
+        ``GET /source-storage/migrations/jobs/{jobsId}``
+
+        Args:
+            jobsId (str)
+
+        Returns:
+            dict: See Schema below
+
+        Raises:
+            OkapiRequestNotFound: Not Found
+
+        Schema:
+
+            .. literalinclude:: ../files/SourceRecordStorageMigrationsJobs_get_job_return.schema 
+        """
+        return self.call("GET", f"/source-storage/migrations/jobs/{jobsId}")
+
+
 class SourceRecordStorageSnapshots(FolioApi):
     """Source Record Storage Snapshot API
 
     API for managing snapshots
     """
 
     def get_snapshots(self, **kwargs):
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/tags.py` & `foliolib-0.3.8a1/foliolib/folio/api/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.tags")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/templateEngine.py` & `foliolib-0.3.8a1/foliolib/folio/api/templateEngine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.templateEngine")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/userImport.py` & `foliolib-0.3.8a1/foliolib/folio/api/userImport.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.userImport")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/users.py` & `foliolib-0.3.8a1/foliolib/folio/api/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.users")
 
@@ -735,23 +735,46 @@
 
         Returns:
             dict: See Schema below
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiRequestUnauthorized: Authentication is required
-            OkapiRequestNotFound: Not Found
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/UserTenants_get_userTenants_return.schema 
         """
         return self.call("GET", "/user-tenants", query=kwargs)
 
+    def set_userTenant(self, userTenant: dict):
+        """Create a user-tenant
+
+        ``POST /user-tenants``
+
+        Args:
+            userTenant (dict): See Schema below
+
+        Raises:
+            OkapiRequestError: Bad Request
+            OkapiRequestUnauthorized: Authentication is required
+            OkapiFatalError: Server Error
+            OkapiRequestUnprocessableEntity: Unprocessable Entity
+            OkapiRequestUnprocessableEntity: Unprocessable Entity
+
+        Headers:
+            - **Location** - URI to the created userTenant item
+
+        Schema:
+
+            .. literalinclude:: ../files/UserTenants_set_userTenant_request.schema
+        """
+        return self.call("POST", "/user-tenants", data=userTenant)
+
 
 class Patronpin(FolioApi):
     """patron-pins API
 
     This documents the API calls that can be made to set and verify patron pins
     """
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/api/usersBl.py` & `foliolib-0.3.8a1/foliolib/folio/api/usersBl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-05-20
+# Generated at 2023-07-10
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.usersBl")
```

### Comparing `foliolib-0.3.7a1/foliolib/folio/config.py` & `foliolib-0.3.8a1/foliolib/folio/config.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/folio/dataImport.py` & `foliolib-0.3.8a1/foliolib/folio/dataImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/folio/inventory.py` & `foliolib-0.3.8a1/foliolib/folio/inventory.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/folio/inventoryReferenceData.py` & `foliolib-0.3.8a1/foliolib/folio/inventoryReferenceData.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/folio/users.py` & `foliolib-0.3.8a1/foliolib/folio/users.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/helper/__init__.py` & `foliolib-0.3.8a1/foliolib/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/helper/database.py` & `foliolib-0.3.8a1/foliolib/helper/database.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/helper/folio.py` & `foliolib-0.3.8a1/foliolib/helper/folio.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/helper/modules.py` & `foliolib-0.3.8a1/foliolib/helper/modules.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/helper/okapi.py` & `foliolib-0.3.8a1/foliolib/helper/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/helper/platform.py` & `foliolib-0.3.8a1/foliolib/helper/platform.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/helper/tenant.py` & `foliolib-0.3.8a1/foliolib/helper/tenant.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,9 +38,9 @@
                 _kwargs = kwargs.copy()
                 del _kwargs["purge"]
                 msg = okapi.disable_module(modId, tenantid, **_kwargs)
                 log.debug(json.dumps(msg, indent=2))
             else:
                 raise
 
-    print("Remove tenat %s." % tenantid)
+    print("Remove tenant %s." % tenantid)
     OkapiClient().remove_tenant(tenantid)
```

### Comparing `foliolib-0.3.7a1/foliolib/okapi/__init__.py` & `foliolib-0.3.8a1/foliolib/okapi/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/okapi/exceptions.py` & `foliolib-0.3.8a1/foliolib/okapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/okapi/kubeClient.py` & `foliolib-0.3.8a1/foliolib/okapi/kubeClient.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/okapi/misc.py` & `foliolib-0.3.8a1/foliolib/okapi/misc.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/okapi/okapiClient.py` & `foliolib-0.3.8a1/foliolib/okapi/okapiClient.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/okapi/okapiModule.py` & `foliolib-0.3.8a1/foliolib/okapi/okapiModule.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib/okapi/okapiModuleKubernetes.py` & `foliolib-0.3.8a1/foliolib/okapi/okapiModuleKubernetes.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/foliolib.egg-info/PKG-INFO` & `foliolib-0.3.8a1/foliolib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.7a1
+Version: 0.3.8a1
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: COPYING
 
 ========
 FolioLib
 ========
+
 |PyPI| |Pythons| |ReadTheDocs|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/foliolib.svg
    :alt: PyPI version
    :target: https://pypi.org/project/foliolib/
 
 .. |Pythons| image:: https://img.shields.io/pypi/pyversions/foliolib.svg
@@ -34,15 +35,20 @@
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/foliolib/badge/?version=latest
     :target: https://foliolib.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 FolioLib is an API-Client for `Folio <https://www.folio.org/>`_.
 The API is generated from the RAML and OAS files from the Folio-Modules.
 
-Documentation can be found `here <https://foliolib.readthedocs.io/>`_.
+Documentation can be found at `https://foliolib.readthedocs.io/ <https://foliolib.readthedocs.io/>`_.
+
+Python packages can be found at `https://pypi.org/project/foliolib/ <https://pypi.org/project/foliolib/>`_.
+
+Debian packages can be found at `https://github.com/tobi-weber/foliolib/releases/latest/ <https://github.com/tobi-weber/foliolib/releases/latest/>`_.
+
 
 Features:
 
 - Python Folio API
 - Commandline interface
 - Install and manage Folio
 - Install and manage Folio on Kubernetes
```

### Comparing `foliolib-0.3.7a1/foliolib.egg-info/SOURCES.txt` & `foliolib-0.3.8a1/foliolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.7a1/setup.cfg` & `foliolib-0.3.8a1/setup.cfg`

 * *Files identical despite different names*

