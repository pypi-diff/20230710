# Comparing `tmp/seatsio-73.1.0.tar.gz` & `tmp/seatsio-74.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatsio-73.1.0.tar", last modified: Wed Jun 28 08:24:13 2023, max compression
+gzip compressed data, was "seatsio-74.0.0.tar", last modified: Mon Jul 10 11:13:35 2023, max compression
```

## Comparing `seatsio-73.1.0.tar` & `seatsio-74.0.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.753538 seatsio-73.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-28 08:24:06.000000 seatsio-73.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-28 08:24:06.000000 seatsio-73.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-28 08:24:13.753538 seatsio-73.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-06-28 08:24:06.000000 seatsio-73.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.749538 seatsio-73.1.0/seatsio/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.749538 seatsio-73.1.0/seatsio/charts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/charts/chartsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/charts/chartsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/charts/socialDistancingRulesetsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.749538 seatsio-73.1.0/seatsio/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/changeBestAvailableObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/changeObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/channelProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/channelsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/channelsRequests.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/createMultipleEventsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/createSingleEventRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/eventProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)    11476 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/eventsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/extraDataRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/forSaleRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/objectProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/events/statusChangeRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.749538 seatsio-73.1.0/seatsio/holdtokens/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/holdtokens/HoldTokenClient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/holdtokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/httpClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.749538 seatsio-73.1.0/seatsio/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/pagination/listableObjectsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/pagination/lister.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/pagination/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/pagination/pageFetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/pagination/pagedIterator.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.749538 seatsio-73.1.0/seatsio/reports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.749538 seatsio-73.1.0/seatsio/reports/charts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/reports/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/reports/charts/chartReports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.749538 seatsio-73.1.0/seatsio/reports/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/reports/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/reports/events/eventReports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.753538 seatsio-73.1.0/seatsio/reports/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/reports/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/reports/usage/usageReports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.753538 seatsio-73.1.0/seatsio/seasons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/seasons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/seasons/seasonsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.753538 seatsio-73.1.0/seatsio/subaccounts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/subaccounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/subaccounts/subaccountsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.753538 seatsio-73.1.0/seatsio/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/workspaces/UpdateWorkspaceRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/workspaces/createWorkspaceRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-28 08:24:06.000000 seatsio-73.1.0/seatsio/workspaces/workspacesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:24:13.749538 seatsio-73.1.0/seatsio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-28 08:24:13.000000 seatsio-73.1.0/seatsio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-28 08:24:13.000000 seatsio-73.1.0/seatsio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 08:24:13.000000 seatsio-73.1.0/seatsio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-28 08:24:13.000000 seatsio-73.1.0/seatsio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 08:24:13.000000 seatsio-73.1.0/seatsio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 08:24:13.753538 seatsio-73.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-28 08:24:10.000000 seatsio-73.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.691167 seatsio-74.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 11:13:28.000000 seatsio-74.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 11:13:28.000000 seatsio-74.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-10 11:13:35.691167 seatsio-74.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-07-10 11:13:28.000000 seatsio-74.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.683166 seatsio-74.0.0/seatsio/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.687167 seatsio-74.0.0/seatsio/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/charts/chartsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/charts/chartsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.687167 seatsio-74.0.0/seatsio/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/changeBestAvailableObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/changeObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/channelProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/channelsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/channelsRequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/createMultipleEventsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/createSingleEventRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/eventProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/eventsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/extraDataRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/forSaleRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/objectProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/events/statusChangeRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.687167 seatsio-74.0.0/seatsio/holdtokens/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/holdtokens/HoldTokenClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/holdtokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/httpClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.687167 seatsio-74.0.0/seatsio/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/pagination/listableObjectsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/pagination/lister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/pagination/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/pagination/pageFetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/pagination/pagedIterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.687167 seatsio-74.0.0/seatsio/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.687167 seatsio-74.0.0/seatsio/reports/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/reports/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/reports/charts/chartReports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.687167 seatsio-74.0.0/seatsio/reports/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/reports/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/reports/events/eventReports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.687167 seatsio-74.0.0/seatsio/reports/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/reports/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/reports/usage/usageReports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.687167 seatsio-74.0.0/seatsio/seasons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/seasons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/seasons/seasonsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.691167 seatsio-74.0.0/seatsio/subaccounts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/subaccounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/subaccounts/subaccountsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.691167 seatsio-74.0.0/seatsio/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/workspaces/UpdateWorkspaceRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/workspaces/createWorkspaceRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-10 11:13:28.000000 seatsio-74.0.0/seatsio/workspaces/workspacesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:13:35.687167 seatsio-74.0.0/seatsio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-10 11:13:35.000000 seatsio-74.0.0/seatsio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-10 11:13:35.000000 seatsio-74.0.0/seatsio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:13:35.000000 seatsio-74.0.0/seatsio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 11:13:35.000000 seatsio-74.0.0/seatsio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 11:13:35.000000 seatsio-74.0.0/seatsio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 11:13:35.691167 seatsio-74.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-10 11:13:32.000000 seatsio-74.0.0/setup.py
```

### Comparing `seatsio-73.1.0/LICENSE` & `seatsio-74.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/PKG-INFO` & `seatsio-74.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatsio
-Version: 73.1.0
+Version: 74.0.0
 Summary: The official Seats.io Python client library
 Home-page: https://github.com/seatsio/seatsio-python
 Author: The seats.io dev team
 Author-email: hello@seats.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `seatsio-73.1.0/README.md` & `seatsio-74.0.0/README.md`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/charts/chartsClient.py` & `seatsio-74.0.0/seatsio/charts/chartsClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 
 from munch import munchify
 
 from seatsio.reports.charts.chartReports import ChartReports
 from seatsio.charts.chartsRequest import ChartRequest
-from seatsio.charts.socialDistancingRulesetsRequest import SocialDistancingRulesetsRequest
 from seatsio.domain import Chart, ChartValidation, Category
 from seatsio.pagination.listableObjectsClient import ListableObjectsClient
 from seatsio.pagination.lister import Lister
 from seatsio.pagination.pageFetcher import PageFetcher
 
 
 class ChartsClient(ListableObjectsClient):
@@ -122,11 +121,7 @@
     def validate_published_version(self, key):
         response = self.http_client.url("/charts/{key}/version/published/actions/validate", key=key).post()
         return ChartValidation(json.loads(response.text))
 
     def validate_draft_version(self, key):
         response = self.http_client.url("/charts/{key}/version/draft/actions/validate", key=key).post()
         return ChartValidation(json.loads(response.text))
-
-    def save_social_distancing_rulesets(self, key, rulesets):
-        request = SocialDistancingRulesetsRequest(rulesets)
-        self.http_client.url("/charts/{key}/social-distancing-rulesets", key=key).post(request)
```

### Comparing `seatsio-73.1.0/seatsio/client.py` & `seatsio-74.0.0/seatsio/client.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/events/changeBestAvailableObjectStatusRequest.py` & `seatsio-74.0.0/seatsio/events/changeBestAvailableObjectStatusRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/events/changeObjectStatusRequest.py` & `seatsio-74.0.0/seatsio/events/changeObjectStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from past.builtins import basestring
 
 from seatsio.events.objectProperties import ObjectProperties
 
 
 class ChangeObjectStatusRequest:
-    def __init__(self, object_or_objects, status, hold_token, order_id, event_key_or_keys, keep_extra_data, ignore_channels, channel_keys, ignore_social_distancing=None, allowed_previous_statuses=None, rejected_previous_statuses=None):
+    def __init__(self, object_or_objects, status, hold_token, order_id, event_key_or_keys, keep_extra_data, ignore_channels, channel_keys, allowed_previous_statuses=None, rejected_previous_statuses=None):
         self.objects = self.__normalize_objects(object_or_objects)
         self.status = status
         if hold_token:
             self.holdToken = hold_token
         if order_id:
             self.orderId = order_id
         if isinstance(event_key_or_keys, basestring):
@@ -17,16 +17,14 @@
             self.events = event_key_or_keys
         if keep_extra_data is not None:
             self.keepExtraData = keep_extra_data
         if ignore_channels is not None:
             self.ignoreChannels = ignore_channels
         if channel_keys is not None:
             self.channelKeys = channel_keys
-        if ignore_social_distancing is not None:
-            self.ignoreSocialDistancing = ignore_social_distancing
         if allowed_previous_statuses is not None:
             self.allowedPreviousStatuses = allowed_previous_statuses
         if rejected_previous_statuses is not None:
             self.rejectedPreviousStatuses = rejected_previous_statuses
 
     def __normalize_objects(self, object_or_objects):
         if isinstance(object_or_objects, list):
```

### Comparing `seatsio-73.1.0/seatsio/events/channelsClient.py` & `seatsio-74.0.0/seatsio/events/channelsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/events/channelsRequests.py` & `seatsio-74.0.0/seatsio/events/channelsRequests.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/events/createSingleEventRequest.py` & `seatsio-74.0.0/seatsio/events/eventProperties.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-class CreateSingleEventRequest:
-    def __init__(self, chart_key, event_key=None, name=None, date=None, table_booking_config=None,
-                 social_distancing_ruleset_key=None, object_categories=None, categories=None):
-        if chart_key:
-            self.chartKey = chart_key
+class EventProperties:
+    def __init__(self, event_key=None, name=None, date=None, table_booking_config=None, object_categories=None, categories=None):
         if event_key:
             self.eventKey = event_key
         if name:
             self.name = name
         if date:
             self.date = date
         if table_booking_config is not None:
-            self.tableBookingConfig = table_booking_config.to_json()
-        if social_distancing_ruleset_key is not None:
-            self.socialDistancingRulesetKey = social_distancing_ruleset_key
+            self.tableBookingConfig = table_booking_config
         if object_categories is not None:
             self.objectCategories = object_categories
         if categories is not None:
             self.categories = categories
-
```

### Comparing `seatsio-73.1.0/seatsio/events/eventsClient.py` & `seatsio-74.0.0/seatsio/events/eventsClient.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,35 +19,32 @@
 class EventsClient(ListableObjectsClient):
 
     def __init__(self, http_client):
         ListableObjectsClient.__init__(self, http_client, event_from_json, "/events")
         self.reports = EventReports(self.http_client)
         self.channels = ChannelsClient(self.http_client)
 
-    def create(self, chart_key, event_key=None, name=None, date=None, table_booking_config=None, social_distancing_ruleset_key=None,
+    def create(self, chart_key, event_key=None, name=None, date=None, table_booking_config=None,
                object_categories=None, categories=None):
         response = self.http_client.url("/events").post(
-            CreateSingleEventRequest(chart_key, event_key, name, date, table_booking_config, social_distancing_ruleset_key,
+            CreateSingleEventRequest(chart_key, event_key, name, date, table_booking_config,
                                      object_categories, categories))
         return Event(response.json())
 
     def create_multiple(self, chart_key, events_properties):
         response = self.http_client.url("/events/actions/create-multiple").post(
             CreateMultipleEventsRequest(chart_key, events_properties))
         return Event.create_list(response.json().get("events"))
 
     def update(self, key, chart_key=None, event_key=None, name=None, date=None, table_booking_config=None,
-               social_distancing_ruleset_key=None, object_categories=None, categories=None):
+               object_categories=None, categories=None):
         self.http_client.url("/events/{key}", key=key).post(
-            CreateSingleEventRequest(chart_key, event_key, name, date, table_booking_config, social_distancing_ruleset_key,
+            CreateSingleEventRequest(chart_key, event_key, name, date, table_booking_config,
                                      object_categories, categories))
 
-    def remove_social_distancing_ruleset_key(self, key):
-        self.update(key, social_distancing_ruleset_key='')
-
     def remove_object_categories(self, key):
         self.update(key, object_categories={})
 
     def remove_categories(self, key):
         self.update(key, categories=[])
 
     def delete(self, key):
@@ -73,18 +70,17 @@
 
     def status_changes_for_object(self, key, object_id):
         url = "/events/{key}/objects/{objectId}/status-changes"
         page_fetcher = PageFetcher(StatusChange, self.http_client, url, key=key, objectId=object_id)
         return Lister(page_fetcher)
 
     def book(self, event_key_or_keys, object_or_objects, hold_token=None, order_id=None, keep_extra_data=None,
-             ignore_channels=None, channel_keys=None, ignore_social_distancing=None):
+             ignore_channels=None, channel_keys=None):
         return self.change_object_status(event_key_or_keys, object_or_objects, EventObjectInfo.BOOKED, hold_token,
-                                         order_id, keep_extra_data, ignore_channels, channel_keys,
-                                         ignore_social_distancing)
+                                         order_id, keep_extra_data, ignore_channels, channel_keys)
 
     def book_best_available(self, event_key, number, categories=None, hold_token=None, extra_data=None,
                             ticket_types=None, order_id=None, keep_extra_data=None, ignore_channels=None,
                             channel_keys=None, try_to_prevent_orphan_seats=None):
         return self.change_best_available_object_status(
             event_key,
             number,
@@ -127,25 +123,24 @@
 
     def release(self, event_key_or_keys, object_or_objects, hold_token=None, order_id=None, keep_extra_data=None,
                 ignore_channels=None, channel_keys=None):
         return self.change_object_status(event_key_or_keys, object_or_objects, EventObjectInfo.FREE, hold_token,
                                          order_id, keep_extra_data, ignore_channels, channel_keys)
 
     def hold(self, event_key_or_keys, object_or_objects, hold_token, order_id=None, keep_extra_data=None,
-             ignore_channels=None, channel_keys=None, ignore_social_distancing=None):
+             ignore_channels=None, channel_keys=None):
         return self.change_object_status(event_key_or_keys, object_or_objects, EventObjectInfo.HELD, hold_token,
-                                         order_id, keep_extra_data, ignore_channels, channel_keys,
-                                         ignore_social_distancing)
+                                         order_id, keep_extra_data, ignore_channels, channel_keys)
 
     def change_object_status(self, event_key_or_keys, object_or_objects, status, hold_token=None, order_id=None,
                              keep_extra_data=None, ignore_channels=None, channel_keys=None,
-                             ignore_social_distancing=None, allowed_previous_statuses=None,
+                             allowed_previous_statuses=None,
                              rejected_previous_statuses=None):
         request = ChangeObjectStatusRequest(object_or_objects, status, hold_token, order_id, event_key_or_keys,
-                                            keep_extra_data, ignore_channels, channel_keys, ignore_social_distancing,
+                                            keep_extra_data, ignore_channels, channel_keys,
                                             allowed_previous_statuses, rejected_previous_statuses)
         response = self.http_client.url("/events/groups/actions/change-object-status",
                                         query_params={"expand": "objects"}).post(request)
         return ChangeObjectStatusResult(response.json())
 
     def change_object_status_in_batch(self, status_change_requests):
         requests = list(
@@ -159,16 +154,15 @@
                                         query_params={"expand": "objects"}).post({"statusChanges": requests})
         return list(map(lambda r: ChangeObjectStatusResult(r), response.json().get("results")))
 
     def __change_object_status_in_batch_request(self, event_key, object_or_objects, status, hold_token, order_id,
                                                 keep_extra_data, ignore_channels, channel_keys,
                                                 allowed_previous_statuses, rejected_previous_statuses):
         request = ChangeObjectStatusRequest(object_or_objects, status, hold_token, order_id, "", keep_extra_data,
-                                            ignore_channels, channel_keys, None, allowed_previous_statuses,
-                                            rejected_previous_statuses)
+                                            ignore_channels, channel_keys, allowed_previous_statuses, rejected_previous_statuses)
         request.event = event_key
         delattr(request, "events")
         return request
 
     def retrieve_object_info(self, key, object_label):
         result = self.retrieve_object_infos(key, [object_label])
         return result[object_label]
```

### Comparing `seatsio-73.1.0/seatsio/events/statusChangeRequest.py` & `seatsio-74.0.0/seatsio/events/statusChangeRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/exceptions.py` & `seatsio-74.0.0/seatsio/exceptions.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/holdtokens/HoldTokenClient.py` & `seatsio-74.0.0/seatsio/holdtokens/HoldTokenClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/httpClient.py` & `seatsio-74.0.0/seatsio/httpClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/pagination/listableObjectsClient.py` & `seatsio-74.0.0/seatsio/pagination/listableObjectsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/pagination/lister.py` & `seatsio-74.0.0/seatsio/pagination/lister.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/pagination/page.py` & `seatsio-74.0.0/seatsio/pagination/page.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/pagination/pageFetcher.py` & `seatsio-74.0.0/seatsio/pagination/pageFetcher.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/pagination/pagedIterator.py` & `seatsio-74.0.0/seatsio/pagination/pagedIterator.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/reports/charts/chartReports.py` & `seatsio-74.0.0/seatsio/reports/charts/chartReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/reports/events/eventReports.py` & `seatsio-74.0.0/seatsio/reports/events/eventReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/reports/usage/usageReports.py` & `seatsio-74.0.0/seatsio/reports/usage/usageReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/seasons/seasonsClient.py` & `seatsio-74.0.0/seatsio/seasons/seasonsClient.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 
 class SeasonsClient:
 
     def __init__(self, http_client, seatsio_client):
         self.http_client = http_client
         self.seatsio_client = seatsio_client
 
-    def create(self, chart_key, key=None, number_of_events=None, event_keys=None, table_booking_config=None,
-               social_distancing_ruleset_key=None):
+    def create(self, chart_key, key=None, number_of_events=None, event_keys=None, table_booking_config=None):
         request = {}
         if chart_key:
             request['chartKey'] = chart_key
         if key:
             request['key'] = key
         if number_of_events:
             request['numberOfEvents'] = number_of_events
         if event_keys:
             request['eventKeys'] = event_keys
         if table_booking_config is not None:
             request['tableBookingConfig'] = table_booking_config.to_json()
-        if social_distancing_ruleset_key is not None:
-            request['socialDistancingRulesetKey'] = social_distancing_ruleset_key
 
         response = self.http_client.url("/seasons").post(request)
         return Season(response.json())
 
     def create_partial_season(self, top_level_season_key, partial_season_key=None, event_keys=None):
         request = {}
         if partial_season_key:
```

### Comparing `seatsio-73.1.0/seatsio/subaccounts/subaccountsClient.py` & `seatsio-74.0.0/seatsio/subaccounts/subaccountsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio/workspaces/workspacesClient.py` & `seatsio-74.0.0/seatsio/workspaces/workspacesClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-73.1.0/seatsio.egg-info/PKG-INFO` & `seatsio-74.0.0/seatsio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatsio
-Version: 73.1.0
+Version: 74.0.0
 Summary: The official Seats.io Python client library
 Home-page: https://github.com/seatsio/seatsio-python
 Author: The seats.io dev team
 Author-email: hello@seats.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `seatsio-73.1.0/seatsio.egg-info/SOURCES.txt` & `seatsio-74.0.0/seatsio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 seatsio.egg-info/SOURCES.txt
 seatsio.egg-info/dependency_links.txt
 seatsio.egg-info/requires.txt
 seatsio.egg-info/top_level.txt
 seatsio/charts/__init__.py
 seatsio/charts/chartsClient.py
 seatsio/charts/chartsRequest.py
-seatsio/charts/socialDistancingRulesetsRequest.py
 seatsio/events/__init__.py
 seatsio/events/changeBestAvailableObjectStatusRequest.py
 seatsio/events/changeObjectStatusRequest.py
 seatsio/events/channelProperties.py
 seatsio/events/channelsClient.py
 seatsio/events/channelsRequests.py
 seatsio/events/createMultipleEventsRequest.py
```

