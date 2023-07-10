# Comparing `tmp/inhandtest-0.0.59.tar.gz` & `tmp/inhandtest-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.59.tar", last modified: Wed Jul  5 03:14:22 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.60.tar", last modified: Mon Jul 10 05:54:06 2023, max compression
```

## Comparing `inhandtest-0.0.59.tar` & `inhandtest-0.0.60.tar`

### file list

```diff
@@ -1,61 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.59/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-07-05 03:14:22.000000 inhandtest-0.0.59/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.59/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.59/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.59/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.59/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.59/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.59/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    64382 2023-07-05 03:09:48.000000 inhandtest-0.0.59/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    26127 2023-07-05 03:02:01.000000 inhandtest-0.0.59/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.59/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3971 2023-06-16 00:48:06.000000 inhandtest-0.0.59/inhandtest/file.py
--rw-rw-rw-   0        0        0    10907 2023-06-15 06:06:07.000000 inhandtest-0.0.59/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.59/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.59/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    71861 2023-07-03 01:50:04.000000 inhandtest-0.0.59/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.59/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    14831 2023-07-03 08:50:33.000000 inhandtest-0.0.59/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.59/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.59/inhandtest/ip.py
--rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.59/inhandtest/log.py
--rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.59/inhandtest/mail.py
--rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.59/inhandtest/notice_email.html
-drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.59/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0    67491 2023-07-05 02:30:31.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0    71995 2023-07-05 02:31:02.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     3247 2023-07-05 03:12:45.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0    11890 2023-07-05 02:55:07.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86226 2023-07-05 01:05:03.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.59/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    34699 2023-06-20 09:30:58.000000 inhandtest-0.0.59/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    28122 2023-07-03 10:41:33.000000 inhandtest-0.0.59/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1656 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.59/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 03:14:22.000000 inhandtest-0.0.59/setup.cfg
--rw-rw-rw-   0        0        0     1615 2023-07-05 03:14:12.000000 inhandtest-0.0.59/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.60/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-07-10 05:54:06.000000 inhandtest-0.0.60/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.60/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.60/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.60/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.60/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.60/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.60/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    63306 2023-07-10 05:49:05.000000 inhandtest-0.0.60/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    26127 2023-07-05 03:02:01.000000 inhandtest-0.0.60/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.60/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3971 2023-06-16 00:48:06.000000 inhandtest-0.0.60/inhandtest/file.py
+-rw-rw-rw-   0        0        0    10907 2023-06-15 06:06:07.000000 inhandtest-0.0.60/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.60/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.60/inhandtest/inmqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/inrequest/
+-rw-rw-rw-   0        0        0      503 2023-07-10 05:21:05.000000 inhandtest-0.0.60/inhandtest/inrequest/__init__.py
+-rw-rw-rw-   0        0        0     8021 2023-07-06 09:44:41.000000 inhandtest-0.0.60/inhandtest/inrequest/console.py
+-rw-rw-rw-   0        0        0    26186 2023-07-05 05:25:12.000000 inhandtest-0.0.60/inhandtest/inrequest/dm.py
+-rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.60/inhandtest/inrequest/dn.py
+-rw-rw-rw-   0        0        0      183 2023-07-06 10:28:04.000000 inhandtest-0.0.60/inhandtest/inrequest/er_device.py
+-rw-rw-rw-   0        0        0     7352 2023-07-05 05:27:06.000000 inhandtest-0.0.60/inhandtest/inrequest/ics.py
+-rw-rw-rw-   0        0        0     9584 2023-07-06 10:16:13.000000 inhandtest-0.0.60/inhandtest/inrequest/inrequest.py
+-rw-rw-rw-   0        0        0    24111 2023-07-10 05:16:38.000000 inhandtest-0.0.60/inhandtest/inrequest/nezha.py
+-rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.60/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    16027 2023-07-06 07:21:54.000000 inhandtest-0.0.60/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.60/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.60/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.60/inhandtest/log.py
+-rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.60/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.60/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.60/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0    67724 2023-07-10 05:52:27.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0    72025 2023-07-05 08:11:13.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3247 2023-07-05 03:12:45.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0    11890 2023-07-05 02:55:07.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86226 2023-07-05 01:05:03.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.60/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    34823 2023-07-06 06:11:52.000000 inhandtest-0.0.60/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    30311 2023-07-10 05:36:50.000000 inhandtest-0.0.60/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1877 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.60/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 05:54:06.000000 inhandtest-0.0.60/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2023-07-10 05:53:53.000000 inhandtest-0.0.60/setup.py
```

### Comparing `inhandtest-0.0.59/PKG-INFO` & `inhandtest-0.0.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.59
+Version: 0.0.60
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.59/README.md` & `inhandtest-0.0.60/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.60/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.60/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.60/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/base_page/base_page.py` & `inhandtest-0.0.60/inhandtest/base_page/base_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -873,26 +873,30 @@
                     "param":{$key, $value}: 参数转换，如大小写转换{"ab":"AB"} {"wan":"Wan"}等.
                 :param action_dict: 要做操作的参数名称与对应的值{$param1: $value1, $param2: $value2}
                 :return:
                 """
         relations = []
 
         def operation(param, param_locator, value):
+
             if param_locator.get('type') == 'text':
                 self.fill(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'monaco':
                 self.monaco(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select':
-                value = replace_str(value, param_locator.get('param'))
+                if param_locator.get('param'):
+                    value = param_locator.get('param').get(value) if param_locator.get('param').get(value) else value
                 self.select_option(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select_more':
-                value = replace_str(value, param_locator.get('param'))
+                if param_locator.get('param'):
+                    value = param_locator.get('param').get(value) if param_locator.get('param').get(value) else value
                 self.select_more(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select_multi':
-                value = replace_str(value, param_locator.get('param'))
+                if param_locator.get('param'):
+                    value = param_locator.get('param').get(value) if param_locator.get('param').get(value) else value
                 self.select_multi(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'radio_select':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
                     value = param_locator.get('param').get(value)
                 self.radio_select(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'radio':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
@@ -1130,56 +1134,30 @@
                 return result.get(keys[0])
             else:
                 return result
         else:
             return None
 
     @allure.step("PC Ping")
-    @loop_inspector('PC Ping', timeout=120, interval=10)
     def pc_ping(self, host_or_ip: str or list or tuple = 'www.baidu.com', number: int = 4, src=None,
-                lost_packets=False, assert_result=True) -> bool:
+                lost_packets=False, assert_result=True, timeout=120, interval=10) -> None:
         """ 验证在PC机上ping某个地址是否丢包， 仅判断丢包
 
         :param lost_packets:
         :param src: 验证的源IP地址 '192.168.2.100'
         :param host_or_ip: 验证的目的IP地址, 可使用元组或列表接收多个地址
         :param number: 包数量
         :param lost_packets: True|False 如果为True判断会丢包，如果为False判断不丢包
         :param assert_result: True|False 是否对 lost_packets 的结果做判断
+        :param timeout: 超时时间
+        :param interval: 间隔时间
         :return:
         """
-        tag_result = True
-        if host_or_ip:
-            host_or_ip = [host_or_ip] if isinstance(host_or_ip, str) else host_or_ip
-            for host in host_or_ip:
-                command = f'ping {host} -n {number}' if src is None else f'ping -S {src} {host} -n {number}'
-                logging.debug(command)
-                if assert_result:
-                    result = os.popen(command).read()
-                    logging.debug(result)
-                    if lost_packets:  # 判断需要丢包
-                        send = re.findall(r'已发送 = (.*?)，', result, re.S)[0]
-                        accept = re.findall(r'已接收 = (.*?)，', result, re.S)[0]
-                        if send == accept:
-                            if '无法访问' not in result:
-                                logging.info(f'PC {src} ping {host} does not loss packet')
-                                tag_result = False
-                    else:  # 判断不丢包
-                        if '丢失 = 0' not in result:
-                            logging.info(f'PC {src} ping {host} loss packet')
-                            tag_result = False
-                        else:
-                            if '无法访问' in result:
-                                logging.info(f'PC {src} ping {host} loss packet')
-                                tag_result = False
-                else:
-                    os.popen(command)
-                if not tag_result:
-                    break
-        return tag_result
+        from inhandtest.tools import pc_ping
+        pc_ping(host_or_ip, number, src, lost_packets, assert_result, timeout, interval)
 
     def close(self) -> None:
         if self.__context and self.__browser and self.__playwright:
             self.__context.close()
             self.__browser.close()
             self.__playwright.stop()
             logging.info('close browser and playwright')
```

### Comparing `inhandtest-0.0.59/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.60/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/exception.py` & `inhandtest-0.0.60/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/file.py` & `inhandtest-0.0.60/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/inmodbus.py` & `inhandtest-0.0.60/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/inmongodb.py` & `inhandtest-0.0.60/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/inmqtt.py` & `inhandtest-0.0.60/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/inrequest.py` & `inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1403 +1,1228 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2023/3/3 9:23:56
+# @Time    : 2023/5/25 15:34:20
 # @Author  : Pane Li
-# @File    : inrequest.py
+# @File    : python_edge_computing.py
 """
-封装request， 使设备和平台都能来正常调用，统一入口，token过期时也能自动更新
+python_edge_computing
 
 """
-import base64
-import os
-import random
-import re
-import time
-from typing import List
-import urllib3
-import requests
-from inhandtest.exception import ParameterValueError, UsernameOrPasswordError, TimeOutError, UpgradeFailedError, \
-    ResourceNotFoundError
-from inhandtest.file import file_hash
-from inhandtest.tools import dict_in, dict_merge, replace_str, DotDict, loop_inspector, get_time_stamp, generate_string
 import logging
-
-
-class DnInterface:
-    def __init__(self, username, password, host='c.inhand.com.cn'):
+import random
+import allure
+import numpy as np
+from inhandtest.tools import loop_inspector
+from inhandtest.base_page.table_tr import IgTable
+from inhandtest.base_page.base_page import BasePage
+from inhandtest.pages.ingateway.locators import IgLocators
+
+
+class PythonEdgeComputing(BasePage, IgLocators):
+
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
+        IgLocators.__init__(self, page, locale)
+
+    @allure.step('断言Python Engine状态')
+    @loop_inspector('python_engine_status')
+    def assert_status(self, **kwargs):
         """
-        :param username  平台用户名
-        :param password  平台密码
-        :param host: 'c.inhand.com.cn'
-        """
-        self.host = host
-        self.username = username
-        self.api = InRequest(self.host, username, password, 'dn4')
-
-    def add_device(self, sn: str, mac: str, model: str) -> None:
-        """添加设备，
-
-        :param sn: 设备序列号
-        :param mac: 设备mac地址
-        :param model: 设备型号 IR6XX_EVDO  IR300
-        :return:
+        :param kwargs:
+               python_engine: enable,disable ex: python_engine='"${value}"=="enable"'
+               sdk_version: 1.4.3 ex: sdk_version='1.4.3'
+               python_version: Python3 ex: python_version='Python3'
+               username: adm ex: username='adm'
+               used_user_storage: 176MB/6GB3% ex: used_user_storage='"${value}".startswith("176MB")'
+               app: device_supervisor.*RUNNING   ex: app='device_supervisor.*RUNNING'  检测device_supervisor是否在运行
+        """
+        self.access_menu('edge computing.python edge computing')
+        if kwargs.get('app'):
+            if not IgTable([], self.edge_locators.app_status_table).exist(kwargs.get('app'), {}):
+                return False
+        return self.eval_locator_attribute(kwargs, self.edge_locators.python_engine_status_locator)
+
+    @allure.step('获取Python Engine状态')
+    def get_status(self, keys: str or list) -> str or dict or None:
         """
+        :param keys:
+               python_engine, sdk_version, python_version, username, used_user_storage, password
+        """
+        self.access_menu('edge computing.python edge computing')
+        return self.get_text(keys, self.edge_locators.python_engine_status_locator)
 
-        def get_model_id(model_name: str) -> str:
-            models = self.api.send_request('api/models', method='get', param={'limit': 0, 'verbose': 1}).json().get(
-                'result')
-            for model_ in models:
-                if model_.get('name').upper() == model_name.upper():
-                    return model_.get('_id')
-            else:
-                logging.exception(f"the model {model_name} not found")
-                raise ResourceNotFoundError(f"the model {model_name} not found")
-
-        for i in range(3):
-            response = self.api.send_request('api/devices', method='get',
-                                             param={"verbose": 100, "limit": 10, "cursor": 0,
-                                                    'serial_number': sn, 'plc_id': 0})
-            if response.json().get('total') == 0:
-                body = {"deviceConfig": {"maxHeartbeatLost": 6, "heartbeatInterval": 120, "heartbeatTimeout": 10,
-                                         "resendLogin": 60}, "siteName": "", "siteId": None, "name": sn,
-                        "businessState": "0", "modelId": get_model_id(model), "model": model.upper(),
-                        "serialNumber": sn, "mac": mac.upper(), "mobileNumber": "", "plcId": 0,
-                        "config": {"timeout": "300000", "ackTimeout": "120000", "ackRetries": "3", "sync": "2"}}
-                self.api.send_request('api/devices', 'post', param={"create_site": 0}, body=body)
-                logging.info(f"the {sn} device add success")
-            else:
-                break
-
-    @loop_inspector('device online')
-    def assert_device_online(self, sn: str, timeout=120, interval=5) -> int:
-        """ 校验设备基本状态
-
-        :param sn: 序列号
-        :param timeout: 校验信息，最大超时时间
-        :param interval: 校验信息，校验间隔时间
-        :return: True or False
-        """
-        response = self.api.send_request('api/devices', method='get',
-                                         param={"verbose": 100, "limit": 10, "cursor": 0,
-                                                'serial_number': sn, 'plc_id': 0})
-        if response.json().get('total') == 1:
-            device_id = response.json().get('result')[0].get('_id')
-            response = self.api.send_request(f'api/devices/{device_id}', method='get', param={"verbose": 100}).json()
-            return response.get('result').get('online')
-        else:
-            return 0
+    @allure.step('配置Python Edge Computing')
+    def config(self, **kwargs):
+        """
+        :param kwargs:
+               python_engine: enable,disable ex: python_engine='enable'
+               sdk_upgrade: file_path ex: sdk_upgrade='C:\\Users\\Administrator\\Downloads\\inhand-1.4.3.tar.gz'
+               sdk_upgrade_tip: dict sdk_upgrade_tip={'tip_messages': 'install_success', 'timeout': 100}
+               password: 123456 ex: password='123456'
+               start_all_app: True, False ex: app_all_start=True
+               stop_all_app: True, False ex: app_all_stop=True
+               restart_all_app: True, False ex: restart_all_app=True
+               app: [($action, **kwarg)] ex:
+                    [('enable', 'device_supervisor', True)],   # 启用 device_supervisor
+                    [('enable', 'device_supervisor', False)]   # 禁用 device_supervisor
+                    [('install', {'app_package': 'C:\\Users\\Administrator\\Downloads\\device_supervisor-1.0.0.tar.gz'})] # 添加 device_supervisor
+                    [('import_config', 'device_supervisor', 'C:\\Users\\Administrator\\Downloads\\device_supervisor-1.0.0.conf')] # 导入device_supervisor配置
+                    [('export_config', 'device_supervisor', {'file_path': 'C:\\Users\\Administrator\\Downloads', 'file_name': "device_supervisor-1.0.0.conf"})] # 导出device_supervisor配置， 文件名可以不传
+                    [('uninstall', 'device_supervisor')]   # 卸载 device_supervisor
+                    [('edit', 'device_supervisor', {'log_file_size': 1, 'number_of_log': 2, 'start_args': ''})]   # 编辑 device_supervisor
+                    [('download_log', 'device_supervisor', {'file_path': 'C:\\Users\\Administrator\\Downloads', 'file_name': "device_supervisor-1.0.0.log"})] # 导出device_supervisor日志， 文件名可以不传
+                    [('clear_log', 'device_supervisor')]   # 清除 device_supervisor 日志
+                    [('start', 'device_supervisor')]  # 启动 device_supervisor
+                    [('stop', 'device_supervisor')]   # 停止 device_supervisor
+                    [('restart', 'device_supervisor')]   # 重启 device_supervisor
+                    edit parameters:
+                        log_file_size: int
+                        number_of_log: int
+                        start_args: str  启动参数
+                        text_messages: str or list
+                        cancel: True, False
+               submit: True,False ex: submit=True  or submit={'tip_messages': 'APP start successful'}
+               text_messages: str ex: text_messages='ip_address_conflict'
+               tip_messages: ‘APP start successful’
+               reset: True, False ex: reset=True
+        """
+        self.access_menu('edge computing.python edge computing')
+        self.page.wait_for_load_state(state='networkidle')
+        self.page.wait_for_timeout(1 * 1000)
+        if kwargs.get('sdk_upgrade'):
+            kwargs.update({'sdk_upgrade_confirm': True})
+            if kwargs.get('sdk_upgrade_tip') is None:
+                kwargs.update({'sdk_upgrade_tip': {'tip_messages': 'install_success', 'timeout': 100}})
+        if kwargs.get('password'):
+            kwargs.update({'edit_password': True, 'submit_password': True})
+        if kwargs.get('app'):
+            app_list_action = []
+            app_status_action = []
+            for action in kwargs.pop('app'):
+                if action[0] in ('enable', 'install', 'import_config', 'export_config', 'uninstall', 'edit'):
+                    app_list_action.append(action)
+                else:
+                    app_status_action.append(action)
+            kwargs.update({'app_list': app_list_action, 'app_status': app_status_action})
+        self.agg_in(self.edge_locators.python_edge_computing_locator, kwargs)
 
-    def delete_device(self, sn):
-        response = self.api.send_request('api/devices', method='get',
-                                         param={"verbose": 100, "limit": 10, "cursor": 0,
-                                                'serial_number': sn, 'plc_id': 0}).json()
-        if response.get('total') == 1:
-            self.api.send_request(f'api/devices/{response.get("result")[0].get("_id")}', method='delete')
-            logging.info(f"the {sn} device delete success")
 
+class DockerManager(BasePage, IgLocators):
 
-class DmInterface:
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
+        IgLocators.__init__(self, page, locale)
 
-    def __init__(self, username, password, host='iot.inhand.com.cn'):
+    @allure.step('断言Docker Manager状态')
+    @loop_inspector('docker_manager_status')
+    def assert_status(self, **kwargs):
         """
-        :param username  平台用户名
-        :param password  平台密码
-        :param host: 'iot.inhand.com.cn'|'iot.inhandnetworks.com' 平台是哪个环境,
-        """
-        self.host = host
-        self.username = username
-        type_ = 'iot' if ('iot' in self.host) or ('elms' in self.host) else 'ics'
-        self.api = InRequest(self.host, username, password, type_)
-
-    def device_exist(self, sn: str, timeout=120, interval=5) -> None:
-        """检查设备在平台账号下存在，如果超时都不存在就抛异常
+        :param kwargs:
+               docker_manager: enable,disable ex: docker_manager='"${value}"=="enable"'
+               docker_version: 1.4.3 ex: docker_version='1.4.3'
+               portainer_manager: enable,disable ex: portainer_manager='"${value}"=="enable"'
+               username: adm ex: username='adm'
+               password: 123456 ex: password='123456'
+               port:  9000 ex: port='9000'
+        """
+        self.access_menu('edge computing.docker manager')
+        return self.eval_locator_attribute(kwargs, self.edge_locators.docker_manager_status_locator)
+
+    @allure.step('获取Docker Manager状态')
+    def get_status(self, keys: str or list) -> str or dict or None:
+        """
+        :param keys:
+               docker_manager, docker_version, portainer_manager, username, password, port
+        """
+        self.access_menu('edge computing.docker manager')
+        self.page.wait_for_timeout(1000)
+        return self.get_text(keys, self.edge_locators.docker_manager_status_locator)
 
-        :param sn:
-        :param timeout:
-        :param interval:
-        :return:
+    @allure.step('配置Docker Manager')
+    def config(self, **kwargs):
         """
-        for i in range(0, timeout, interval):
-            response = self.api.send_request('api/devices', method='get',
-                                             param={"verbose": 100, "limit": 10, "cursor": 0,
-                                                    'serial_number': sn})
-            if response.json().get('total') == 1:
-                logging.debug(f'check {sn} device exist')
+        :param kwargs:
+               docker_manager: enable,disable ex: docker_manager='enable'
+               docker_upgrade: file_path ex: docker_upgrade='C:\\Users\\Administrator\\Downloads\\inhand-1.4.3.tar.gz'
+               docker_upgrade_tip: 'install_failure', 'install_success', ex: docker_upgrade_tip='install_success'
+               submit_docker_manager: True, False ex: submit_docker_manager=True or submit_docker_manager={'tip_messages': 'submit_success'}
+               portainer_manager: enable,disable ex: portainer_manager='enable'
+               password: 123456 ex: password='123456'
+               port: 9000 ex: port='9000'
+               submit_portainer_manager: True, False ex: submit_portainer_manager=True or submit_portainer_manager={'tip_messages': 'submit_success'}
+               text_messages: str ex: text_messages='ip_address_conflict'
+               tip_messages: ‘submit_success’
+               reset: True, False ex: reset=True
+        """
+        self.access_menu('edge computing.docker manager')
+        self.page.wait_for_load_state(state='networkidle')
+        self.page.wait_for_timeout(1 * 1000)
+        if kwargs.get('docker_upgrade'):
+            kwargs.update({'docker_upgrade_confirm': True})
+            if kwargs.get('docker_upgrade_tip') is None:
+                kwargs.update({'docker_upgrade_tip': {'tip_messages': 'install_success', 'timeout': 100}})
+        self.agg_in(self.edge_locators.docker_manager_locator, kwargs)
+
+
+class MeasureMonitor(BasePage, IgLocators):
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
+        IgLocators.__init__(self, page, locale)
+
+    def __value_mapping(self, locator, value: tuple or list):
+        for i in range(0, locator.get('table').locator('//tbody/tr').count()):
+            self.click(locator.get('table').locator('//tbody/tr').nth(0).locator('//td[3]/a'))
+            self.click(locator.get('ok'))
+            self.page.wait_for_timeout(1000)
+        for i in range(0, len(value)):
+            self.click(locator.get('add'))
+            self.fill(locator.get('table').locator('//tbody/tr').nth(i).locator('//td[1]').locator('//input'),
+                      value[i][0])
+            self.fill(locator.get('table').locator('//tbody/tr').nth(i).locator('//td[2]').locator('//input'),
+                      value[i][1])
+            self.page.wait_for_timeout(500)
+
+    def __turn_page(self, name: str, type_='controller'):
+        """根据控制器/测点名称翻页
+
+        :param name: 控制器/测点名称
+        :param type_: 'controller' | 'measure' , 默认为 'controller'
+        :return:
+        """
+        page_number = 1
+        if type_ == 'controller':
+            locator = list(filter(lambda x: x[0] == 'select', self.edge_locators.controller_card(name)))[0][1].get(
+                'locator')
+        else:
+            locator = list(filter(lambda x: x[0] == 'name', self.edge_locators.measure_table(name)))[0][1].get(
+                'locator')
+        while True:
+            if locator.is_visible():
                 break
-            logging.info(f'check {sn} device is not exist, please wait for {interval}s')
-            time.sleep(interval)
-        else:
-            logging.exception(f'{self.host} {self.username} account not found device {sn}')
-            raise TimeOutError(f'{self.host} {self.username} account not found device {sn}')
-
-    def device_state(self, sn: list) -> List[dict]:
-        """根据sn 转换属性 属性值有：  online: 在线|离线   1|0
-                                       iccid:
-                                       imei:
-                                       imsi:
-                                       model: 设备型号
-                                       version: 固件版本
-                                       hwVersion: 硬件版本 'V1.0'
-                                       bootVersion:  Bootloader版本  '1.1.3.r4956'
-                                       sn: 序列号
-                                       address
-                                       id: 设备id
-                                       name: 设备名字
-                                       ip: 设备连接平台的ip地址
-                                       protocol: 设备连接平台的协议
-                                       config_sync: 设备配置同步状态
-        :param sn: 列表
-        :return: [{'sn': $sn, 'online': 1, 'iccid': '', 'imei'}]
-        """
-        result = []
-        for sn_ in sn:
-            response = self.api.send_request('api/devices', method='get',
-                                             param={"verbose": 100, "limit": 10, "cursor": 0,
-                                                    'serial_number': sn_}).json()
-            if response.get('total') == 1:
-                res = response.get('result')[0]
-                config_sync = res.get('config').get('sync') if res.get('config') else None
-                result.append(
-                    {'sn': sn_, 'online': res.get('online'), 'iccid': res.get('info').get('iccid'),
-                     'imei': res.get('info').get('imei'), 'imsi': res.get('info').get('imsi'),
-                     'version': res.get('info').get('swVersion'), 'hwVersion': res.get('info').get('hwVersion'),
-                     'bootVersion': res.get('info').get('bootVersion'), 'address': res.get('address'),
-                     'id': res.get('_id'), 'name': res.get('name'), 'ip': res.get('pubIp'),
-                     'protocol': res.get('protocol'), 'config_sync': config_sync, 'model': res.get('model')})
             else:
-                result.append(
-                    {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'version': None,
-                     'hwVersion': None, 'bootVersion': None, 'address': None, 'id': None, 'name': None, 'ip': None,
-                     'protocol': None, 'config_sync': None, 'model': None})
-        return result
-
-    def add_device(self, sn: str) -> None:
-        """添加设备，
-
-        :param sn: 设备序列号
-        :return:
-        """
-        for i in range(5):
-            response = self.api.send_request('api/devices', method='get',
-                                             param={"verbose": 100, "limit": 10, "cursor": 0,
-                                                    'serial_number': sn})
-            if response.json().get('total') == 0:
-                self.api.send_request('api/devices', 'post',
-                                      body={"name": sn + str(int(time.time())), "serialNumber": sn})
-                logging.info(f"the {sn} device add success")
-            else:
-                break
-
-    def assert_device_state(self, sn: str, state: dict, timeout=120, interval=5) -> None:
-        """校验设备基本状态
-
-        :param sn: 序列号
-        :param state:   支持表达式${value} ex: {'version': "'${value}' in 'V1.1.3.r4956'"}
-                        online: 在线|离线   1|0
-                        connected: true 只有ics 有该参数
-                        model: 设备型号
-                        iccid:
-                        imei:
-                        imsi:
-                        version: 固件版本
-                        hwVersion: 硬件版本 'V1.0'
-                        bootVersion:  Bootloader版本  '1.1.3.r4956'
-                        sn: 序列号
-                        address
-                        vip:  只能在ics里面使用
-                        ip: 设备连接平台的ip地址
-                        protocol: 设备连接平台的协议 ex: 'mqtt' or 'ovdp'
-                        config_sync: 设备配置同步状态 ex: 2  同成功
-        :param timeout: 校验信息，最大超时时间
-        :param interval: 校验信息，校验间隔时间
-        :return: True or False
-        """
-        if state:
-            import ipaddress
-            for i in range(0, timeout, interval):
-                result = self.device_state([sn])[0]
-                for key, value in state.items():
-                    if '${value}' in value:
-                        value = replace_str(value, {'${value}': result.get(key)})
-                        logging.debug(f'start assert {sn} state {key} {value}')
-                        try:
-                            if not eval(value, {'ipaddress': ipaddress}):
-                                logging.debug(f'the {sn} device {key} info eval {value} is false')
-                                break
-                        except Exception as e:
-                            logging.error(e)
-                            break
-                    else:
-                        logging.debug(f'start assert {sn} state {key} {value}')
-                        if result.get(key) != value:
-                            logging.debug(f'the {sn} device {key} info value is {result.get(key)} not {value}')
-                            break
+                if self.turn_page(self.edge_locators.page_father.get(type_), page_number):
+                    page_number = page_number + 1
+                else:  # 找不到就退出
+                    raise AssertionError(f'{name} is not exist')
+
+    def __controller(self, action: list = None):
+        """
+
+        :param action: [(action_type, value, ),]
+        :return:
+        """
+        for ac in action:
+            if ac[0] in ('add', 'apply_template'):
+                self.agg_in(self.edge_locators.controller_operation, {ac[0]: True})
+                self.agg_in(self.edge_locators.add_controller_all, ac[1])
+            elif ac[0] == 'delete_bulk':
+                all_controller = [ac[1]] if isinstance(ac[1], str) else ac[1]
+                self.__controller([('check', x, True) for x in all_controller])
+                self.agg_in(self.edge_locators.controller_operation, {'delete_bulk': True, 'delete_bulk_confirm': True})
+            else:
+                self.__turn_page(ac[1])
+                if ac[0] == 'edit':
+                    self.agg_in(self.edge_locators.controller_card(ac[1]), {'expand': True, 'edit': True})
+                    self.agg_in(self.edge_locators.add_controller_all, ac[2])
+                elif ac[0] == 'check':
+                    self.agg_in(self.edge_locators.controller_card(ac[1]), {'check': ac[2]})
+                elif ac[0] == 'select':
+                    self.agg_in(self.edge_locators.controller_card(ac[1]), {'select': True})
+                elif ac[0] == 'set_as_template':
+                    self.agg_in(self.edge_locators.controller_card(ac[1]), {'expand': True, 'set_as_template': True})
+                    self.agg_in(self.edge_locators.set_as_template, ac[2])
+                elif ac[0] == 'delete':
+                    self.agg_in(self.edge_locators.controller_card(ac[1]),
+                                {'expand': True, 'delete': True, 'delete_confirm': True})
+                elif ac[0] == 'enable':
+                    self.agg_in(self.edge_locators.controller_card(ac[1]), {'expand': True, 'enable': True})
+                elif ac[0] == 'disable':
+                    self.agg_in(self.edge_locators.controller_card(ac[1]), {'expand': True, 'disable': True})
+                elif ac[0] == 'realtime_communication_message':
+                    pass
+
+    def __measure(self, action: list = None):
+        """
+
+        :param action: [(action_type, value, ),]
+        :return:
+        """
+        for ac in action:
+            if ac[0] == 'add':
+                self.agg_in(self.edge_locators.measure_operation, {ac[0]: True})
+                self.agg_in(self.edge_locators.add_measure_all, ac[1])
+                if ac[1].get('value_mapping'):
+                    self.__value_mapping(self.edge_locators.value_mapping, ac[1].pop('value_mapping'))
+            elif ac[0] == 'edit':
+                self.__turn_page(ac[1], 'measure')
+                self.agg_in(self.edge_locators.measure_table(ac[1]), {ac[0]: True})
+                self.agg_in(self.edge_locators.add_measure_all, ac[2])
+                if ac[2].get('value_mapping'):
+                    self.__value_mapping(self.edge_locators.value_mapping, ac[2].pop('value_mapping'))
+            elif ac[0] == 'search':
+                self.agg_in(self.edge_locators.measure_operation, {"search_name": ac[1], 'search': True})
+            elif ac[0] in ('import', 'export'):
+                self.agg_in(self.edge_locators.measure_operation, {ac[0]: ac[1]})
+            elif ac[0] == 'check':
+                self.agg_in(self.edge_locators.measure_table(ac[1]), {'check': ac[2]})
+            elif ac[0] == 'check_all':
+                self.agg_in(self.edge_locators.measure_operation, {ac[0]: True})
+            elif ac[0] == 'delete_bulk':
+                self.agg_in(self.edge_locators.measure_operation, {'check_all': False})  # 先取消选择所有的
+                all_measure = [ac[1]] if isinstance(ac[1], str) else ac[1]
+                self.__measure([('check', x, True) for x in all_measure])
+                self.agg_in(self.edge_locators.measure_operation, {'delete_bulk': True, 'delete_bulk_confirm': True})
+            elif ac[0] == 'delete_all':
+                self.__measure([('check_all',)])
+                self.agg_in(self.edge_locators.measure_operation, {'delete_bulk': True, 'delete_bulk_confirm': True})
+            elif ac[0] == 'delete':
+                self.agg_in(self.edge_locators.measure_table(ac[1]), {'delete': True, 'delete_confirm': True})
+            elif ac[0] == 'value':
+                if isinstance(ac[2], str):
+                    value = {'value_edit': True, 'value': ac[2], 'submit': {"wait_for_time": 2 * 1000}}
+                else:
+                    value = {'value_edit': True}.update(ac[2])
+                self.agg_in(self.edge_locators.measure_table(ac[1]), value)
+            elif ac[0] == 'add_to_group':
+                if ac[1] == 'all':
+                    self.__measure([('check_all',)])
                 else:
-                    logging.info(f"check {sn} device all state success")
-                    break
-                logging.info(f"check {sn} device state failed, please wait for {interval}s")
-                time.sleep(interval)
+                    self.agg_in(self.edge_locators.measure_operation, {'check_all': False})  # 先取消选择所有的
+                    all_measure = [ac[1]] if isinstance(ac[1], str) else ac[1]
+                    self.__measure([('check', x, True) for x in all_measure])
+                self.agg_in(self.edge_locators.measure_operation, {"add_to_group": True})
+                self.agg_in(self.edge_locators.measure_add_to_group(ac[2]),
+                            {'group_name': True, "submit": {"wait_for_time": 3 * 1000}})
             else:
-                logging.exception(f"the {sn} state {state} check failed")
-                raise TimeOutError(f"the {sn} state {state} check failed")
-
-    def send_config_online(self, sn: str or list, config: str) -> List[str]:
-        """下发配置， 多台时仍然是一台一台下发的， 注意逻辑 设备必须是在线的才能下发
-
-        :param config: 配置命令，多个配置用'\n'隔开
-        :param sn: 一台设备或多台设备
-        :return: list 返回未成功下发配置的设备sn
-        """
-        body = {
-            "deviceType": 0,
-            "deviceContent": config,
-            "deviceDesc": 'set running config'
-        }
-        sn = [sn] if isinstance(sn, str) else sn
-        online_devices = list(filter(lambda x: x.get('online'), self.device_state(sn)))
-        offline_devices = list(filter(lambda x: not x.get('online'), self.device_state(sn)))
-        if online_devices:
-            for on_device in online_devices:
-                logging.info(f'the {on_device.get("sn")} device send config')
-                self.api.send_request(f'/api/devices/{on_device.get("id")}/config/set', 'post', param={'timeout': 30},
-                                      body=body)
-        else:
-            logging.warning(f"the {sn} all offline")
-        return [offline_.get('sn') for offline_ in offline_devices]
+                pass
 
-    def get_config_online(self, sn: str, config: str = None) -> None:
-        """平台获取配置 设备需要在线
-
-        :param sn: 序列号
-        :param config: 对获取到的配置做校验 多条配置使用'\n'隔开， 为None时仅获取
+    @allure.step('配置测点监控')
+    def config(self, **kwargs):
         """
-        response = self.api.send_request('api/devices', method='get',
-                                         param={"verbose": 100, "limit": 10, "cursor": 0,
-                                                'serial_number': sn})
-        if response.json().get('total') == 1 and response.json().get('result')[0].get('online') == 1:
-            device_id = response.json().get('result')[0].get('_id')
-            device_name = response.json().get('result')[0].get('name')
-            for i in range(0, 3):
-                try:
-                    task_state = self.api.send_request('api2/tasks/run', 'post',
-                                                       body={'name': "GET RUNNING CONFIG", 'objectId': device_id,
-                                                             'priority': 30, 'objectName': device_name,
-                                                             'timeout': 30000,
-                                                             'type': "4"}).json().get('result').get('state')
-                    assert task_state == 3, "GET RUNNING CONFIG task status error!"
-                    break
-                except Exception as e:
-                    logging.error(f'get running config task status reason is {e}, try {i + 2} again')
-            else:
-                logging.exception(f'device {sn} get running config task status failed')
-                raise Exception(f'device {sn} get running config task status failed')
-            config_content = self.api.send_request(f'api/devices/{device_id}/config', 'get').json().get('result').get(
-                'content')
-            if config:
-                assert set(config.split('\n')).issubset(set(config_content.split('\n'))), f'config {config} not exist'
-        else:
-            logging.exception(f'the {sn} device not exist or offline')
-            raise ResourceNotFoundError(f'the {sn} device not exist or offline')
 
-    def upgrade_firmware_online(self, sn: str, firmware: str, timeout=20 * 60, interval=10) -> None:
-        """ 升级固件， 保障升级成功不然就会报错
-
-        :param sn: 设备序列号
-        :param firmware: 升级的固件，本地全路径
-        :param timeout: 下发升级任务后，总体的升级超时时间， 单位秒 至少5分鐘， 10， 20， 30
-        :param interval: 升级任务检测间隔， 单位秒
-        :return None or TimeOutError， 升级失败就报TimeOutError
-        """
-
-        def model(name):
-            models = self.api.send_request('api/models', 'get',
-                                           {'gateway': True, 'verbose': 100, 'limit': 0}).json().get('result')
-            for model_ in models:
-                if len(re.findall(model_.get('firmwareNamePattern'), name)) == 1:
-                    return model_.get('name')
-
-        def version(name):
-            return 'V' + re.findall('V(.*).bin', name)[0]
-
-        online_devices = list(filter(lambda x: x.get('online'), self.device_state([sn])))
-        if online_devices:
-            device_id = online_devices[0].get('id')
-            device_name = online_devices[0].get('name')
-            file_name = os.path.basename(firmware)
-            if os.path.isfile(firmware):  # 只要升级文件存在就升级
-                get_firmware = self.api.send_request('api/firmware', 'get', {'name': file_name}).json()
-                if get_firmware.get('total') == 0:
-                    if os.path.exists(firmware):
-                        param = {'filename': firmware, 'oid': 'undefined'}
-                        upload_file = self.api.send_request('api/file/form', method='post', param=param,
-                                                            params_type='form', file_path=firmware).json().get('result')
-                        body = {'fid': upload_file['_id'], 'jobTimeout': int(timeout / 60), 'model': model(file_name),
-                                'name': file_name,
-                                'version': version(file_name), 'desc': 'auto test upload firmware'}
-                        firmware_id = self.api.send_request('api/firmware', 'post', body=body, ).json().get(
-                            'result').get(
-                            '_id')
-                    else:
-                        logging.exception(f'{firmware} not exist')
-                        raise FileNotFoundError(f'{firmware} not exist')
+        :param kwargs:
+               controller: [(action_type, value, ),]
+                           [('add', kwargs)]
+                            kwargs:
+                               name: 名称
+                               protocol: 'modbus.modbus tcp' | 'modbus.modbus rtu'| 'OPC.OPC-UA'|'Siemens Plc.ISO-on-TCP'
+                               servers_url: 服务器地址   OPC-UA
+                               ip_address: ip地址
+                               port: 端口号
+                               mode: 通讯方式 'Rack/Slot' | 'TSAP'    ISO-on-TCP
+                               rack: 机架号   ISO-on-TCP
+                               slot: 插槽号      ISO-on-TCP
+                               client_tsap:   ISO-on-TCP
+                               server_tsap:  ISO-on-TCP
+                               slave: 从站地址
+                               endpoint: 通讯方式 'RS485' | 'RS232'
+                               polling_interval: 轮询周期 1~864000 s
+                               multiple_polling_interval: enable | disable, 轮询周期是否可变
+                               polling_interval2: 轮询周期2 1~864000 s
+                               auth: anonymous | username_password| certificate_auth, OPC-UA 验证方式
+                               username: 用户名  OPC-UA
+                               password  : 密码 OPC-UA
+                               certificate: 证书路径 OPC-UA
+                               private_key: 私钥路径 OPC-UA
+                               security_policy: None|Automatic detection|Basic128Rsa15|Basic256|Basic256Sha256|Aes128Sha256RsaOaep 安全策略 OPC-UA
+                               security_mode: None|sign|sign_encrypt 安全模式 OPC-UA
+                               description: 描述
+                               advanced_settings: 展开高级设置 'expand' | 'close'
+                               byte_order_16int: 16位整数字节序 'AB' | 'BA'
+                               byte_order_32int: 32位整数字节序 'ABCD' | 'CDAB' | 'DCBA' | 'BADC'
+                               byte_order_32float: 32位浮点数字节序 'ABCD' | 'CDAB' | 'DCBA' | 'BADC'
+                               byte_order_64int: 同选择框的选项
+                               byte_order_64float: 同选择框的选项
+                               package_reporting： 是否启用包上报 'enable' | 'disable'
+                               packet_data_polling_interval: 包数据轮询周期 100~1000 ms
+                               mi_data_uploading: 毫秒数据上报（轮询几次后上报）
+                               continuous_collection: 是否启用批量采集 'enable' | 'disable'
+                               continuous_collection_address: 最大批量采集数 2~125
+                               timeout: 超时时间 2~60000 ms
+                               connect_timeout: 连接超时时间 2~60000 ms
+                               periodically_upload_onchange_data: 是否启用周期上报Onchange数据
+                               onchange_uploading_interval: Onchange数据上报间隔
+                               communication_interval_time: 通讯间隔时间 0~1000 ms
+                               coil_outputs_write_function_code: 线圈寄存器写入功能码 05 | 15
+                               holding_register_write_function_code: 保持寄存器写入功能码 06 | 16
+                               store_communication_message: 是否存储通讯信息 'enable' | 'disable'
+                               submit: 是否提交 'submit', submit=True or submit={'tip_messages': 'submit_success'}
+                               text_messages: 文本信息验证 str or list
+                               tip_messages: 提示信息验证 str or list or dict
+                               cancel: 是否取消  cancel=True
+                            [('edit', 'old_controller_name', kwargs)]  kwargs 同add
+                            [('apply_template', kwargs)] kwargs 同add, 多一个参数 template_name 模板名称
+                            [('check', name, is_check)]  # 选中或取消选中控制器
+                                name: str  控制器名称
+                                is_check: bool  是否选中 True | False
+                            [('delete_bulk', name)]  # 批量删除多个控制器
+                                name: str or list 一个或多个控制器名称
+                            [('select', name)]  # 点击选中控制器，方便操作对应的测点
+                                name: str  控制器名称
+                            [('delete', name)]  # 删除单个控制器
+                                name: str  控制器名称
+                            [('enable', name)]  # 启用单个控制器
+                                name: str  控制器名称
+                            [('disable', name)]  # 禁用单个控制器
+                                name: str  控制器名称
+                            [('set_as_template', name, kwargs)]
+                                name: str  控制器名称
+                                kwargs:
+                                    name: 模板名称
+                                    description: 模板描述
+                                    submit: 是否提交 'submit', submit=True or submit={'tip_messages': 'submit_success'}
+                                    text_messages: 文本信息验证 str or list
+                                    tip_messages: 提示信息验证 str or list or dict
+                                    cancel: 是否取消  cancel=True
+               measure: [(action_type, value, ),]
+                        [('add', kwargs)]
+                            kwargs:
+                                name: 名称
+                                namespace: 命名空间   OPC-UA
+                                address_type: String|Number   OPC-UA
+                                identifier: 标识符   OPC-UA
+                                register_type:   I|Q|M|DB    ISO-on-TCP
+                                register_address: 寄存器地址 list  ex: ['4X', '40001']
+                                data_type: 数据类型 bit,word,int,dword,dint,float,double,string,bcd16,ulong,long
+                                read_bit_data: enable | disable
+                                register_bit: 位寄存器
+                                data_register_bit: 数据寄存器
+                                negative_value: enable | disable
+                                storage_lwtsdb: enable | disable
+                                decimal_places: 小数位数
+                                size: 数据长度
+                                encoding_format: 编码格式 ascii, utf-8, utf-16, utf-16-big, gb2312
+                                is_array: enable | disable    OPC-UA
+                                read_write: 读写属性 read | write | read/write
+                                mode: periodic | onchange | never
+                                unit: 单位 str
+                                description: 描述
+                                group: 所属组
+                                polling_interval: polling_interval|polling_interval_2
+                                numerical_mapping: 数值映射 enable | disable
+                                data_calculation: 数据计算 no | ratio conversion | offset and zoom| bit truncation | pt/ct | value mapping
+                                trans_decimal: 数据运算小数位
+                                data_high_limit: 数据上限
+                                data_lower_limit: 数据下限
+                                high_limit_of_proportion: 比例上限
+                                lower_limit_of_proportion: 比例下限
+                                magnification: 放大倍数
+                                offset: 偏移量
+                                start_bit: 起始位
+                                end_bit: 结束位
+                                pt:
+                                ct:
+                                value_mapping: [(source, target),] 可以是多个， 代表的是最终结果
+                                package_reporting: enable | disable
+                                submit: 是否提交 'submit', submit=True or submit={'tip_messages': 'submit_success'}
+                                text_messages: 文本信息验证 str or list
+                                tip_messages: 提示信息验证 str or list or dict
+                                cancel: 是否取消  cancel=True
+                        [('edit', 'old_measure_name', kwargs)]  kwargs 同add
+                        [('check', name, is_check)]  # 选中或取消选中控制器
+                            name: str  测点名称
+                            is_check: bool  是否选中 True | False
+                        [('search', name)]  # 查询测点
+                            name: str  测点名称
+                        [('import', file_path)]  # 导入测点
+                            file_path: str 导入文件路径
+                        [('export', kwargs)]  # 导出测点
+                            kwargs: str, 就是导出文件的文件夹
+                            kwargs: dict,
+                            kwargs = {'file_path': './', 'file_name': None}
+                        [('delete_bulk', name)]  # 批量删除测点
+                            name: str or list 一个或多个测点名称
+                        [('delete_all', )]  # 删除全部测点
+                        [('delete', name)]  # 删除一个测点
+                            name: str  测点名称
+                        [('value', name, kwargs)]  # 编辑一个测点的值
+                            name: str  测点名称
+                            kwargs: str or dict
+                                str: 直接写更新的值
+                                dict: {'value': '1', 'submit': {'tip_messages': 'submit_success'}, 'cancel': False}
+                        [('add_to_group', measure_name, group_name)]  # 添加到分组
+                            measure_name: str  测点名称， 当为all 时表示添加全部测点
+                            group_name: str  分组名称
+               group: [('action_type', value, value1)]
+                    [('import', value, value1)]
+                        value: str  导入文件路径
+                        value1: 导入时的确认，默认为True， 也可以校验导入后的提示
+                    [('export', value,)]
+                        value: str  or dict   # 导出分组
+                        str: 导出文件夹
+                        dict: {"file_path": "./", "file_name": None}
+                    [('add', kwargs)]
+                        kwargs:
+                            is_exists: str, 可以填写分组相关连续的信息， 如果存在就不会添加了
+                            name: 名称
+                            reporting_interval: 上报间隔
+                            onchange_data: 是否上报变化数据 enable | disable
+                            onchange_uploading_interval: 变化数据上报间隔
+                            max_number:
+                            storage_policy: same_as_reporting_interval| independent_storage_interval
+                            storage_interval: 存储间隔
+                            storage_method: gateway|usb|sd_card
+                            storage_path: 存储路径
+                            save: 是否保存  save=True 没有该参数时自动保存
+                            cancel: 是否取消  cancel=True
+                            text_messages: str or list
+                            tip_messages: str or list
+                    [('edit', 'old_group_name', kwargs)]  kwargs 同add
+                    [('check', name, True)] or   [('check', name, False)] # 勾选或取消勾选分组
+                    [('delete', name)]  # 删除分组
+                    [('export_historical_data', kwargs})]
+                        kwargs: str or dict
+                            str: 导出文件夹
+                            dict: {"file_path": "./", "file_name": None}
+                    [('clear_historical_data', name)]  # 清除历史数据
+                    [('check_all', value,)]
+                        value: bool  勾选或取消勾选全部分组 True | False
+                    [('delete_bulk', name, value1)]  # 批量删除分组
+                        name: str or list 一个或多个分组名称
+                        value1: {'tip_messages': 'submit_success'} or None 提示信息
+              controller_template: [('action_type', value, value1)]
+                    [('import', value, value1)]
+                        value: str  导入文件路径
+                        value1: 导入时的确认，默认为True， 也可以校验导入后的提示
+                    [('export', value,)]
+                        value: str  or dict   # 导出分组
+                        str: 导出文件夹
+                        dict: {"file_path": "./", "file_name": None}
+                    [('edit', 'old_template_name', kwargs)]
+                        kwargs:
+                            name: 名称
+                            description: 描述
+                            save: 是否保存  save=True 没有该参数时自动保存
+                            cancel: 是否取消  cancel=True
+                            text_messages: str or list
+                            tip_messages: str or list
+                    [('check', name, True)] or   [('check', name, False)] # 勾选或取消勾选
+                    [('delete', name)]  # 删除
+                    [('check_all', value,)]
+                        value: bool  勾选或取消勾选全部分组 True | False
+                    [('delete_bulk', name, value1)]  # 批量删除分组
+                        name: str or list 一个或多个模板名称名称
+                        value1: {'tip_messages': 'submit_success'} or None 提示信息
+        :return:
+        """
+        self.access_menu('edge_computing.device_supervisor.measure_monitor.monitoring_list')
+        if kwargs.get('group') and isinstance(kwargs.get('group'), list):
+            self.access_menu('edge_computing.device_supervisor.measure_monitor.group')
+            for group in kwargs.get('group'):
+                if group[0] in ('add', 'edit', 'check', 'delete', 'export_historical_data', 'clear_historical_data'):
+                    self.agg_in(self.edge_locators.group_locator, {'table': [group]})
                 else:
-                    logging.debug(f'This file {firmware} already exists on the cloud {self.host} {self.username}')
-                    firmware_id = get_firmware.get('result')[0].get('_id')
-                # 已完成固件上传
-                job_id = self.api.send_request(f'api/device/{device_id}/upgrade', method='post',
-                                               body={'deviceName': device_name, 'firmwareId': firmware_id,
-                                                     'timeout': int(timeout / 60)}).json().get('result').get('_id')
-                for i in range(0, timeout, interval):
-                    time.sleep(interval)
-                    job_response = self.api.send_request(f'/api2/tasks', method='get',
-                                                         param={"verbose": 50, 'types': 6, 'object_id': device_id,
-                                                                'limit': 100, 'cursor': 0}).json().get('result')
-                    job = [job for job in job_response if job.get('_id') == job_id]
-                    if len(job) == 1:
-                        if job[0].get('_id') == job_id:
-                            if job[0].get('state') == 3:
-                                logging.info(f"upgrade to {file_name} success!")
-                                break
-                            elif job[0].get('state') == -1:
-                                logging.exception(f'upgrade to {file_name} failed!')
-                                raise UpgradeFailedError(f'upgrade to {file_name} failed!')
+                    if group[0] == 'import':
+                        import_confirm = True if group[2] is None else group[2]
+                        self.agg_in(self.edge_locators.group_locator,
+                                    {'import': group[1], 'import_confirm': import_confirm})
+                    elif group[0] == 'delete_bulk':
+                        try:
+                            delete_bulk_confirm = group[2]
+                        except IndexError:
+                            delete_bulk_confirm = True
+                        self.agg_in(self.edge_locators.group_locator, {'check_all': False})
+                        check_group = [group[1]] if isinstance(group[1], str) else group[1]
+                        for name in check_group:
+                            self.agg_in(self.edge_locators.group_locator, {'table': [('check', name, True)]})
+                        self.agg_in(self.edge_locators.group_locator,
+                                    {'delete_bulk': group[1], 'delete_bulk_confirm': delete_bulk_confirm})
                     else:
-                        logging.exception(f'upgrade to {file_name} failed!')
-                        raise UpgradeFailedError('create upgrade task failed!')
-                else:
-                    logging.exception(f'upgrade to {file_name} timeout!')
-                    raise TimeOutError('upgrade job check timeout')
-                self.assert_device_state(sn, state={'version': '"${value}" in ' + f'"{file_name}"'}, timeout=300)
-            else:
-                logging.debug(f'{firmware} not is file or version of same ')
-        else:
-            logging.exception(f'the device {sn} is offline or not exist')
-            raise Exception(f'the device {sn} is offline or not exist')
-
-    def upgrade_firmware(self, sn: str or list, firmware: str) -> None:
-        """ 升级固件，只管下发升级任务，不监督是否升级成功
-
-        :param sn: 设备序列号
-        :param firmware: 升级的固件，本地全路径
-        :return None
-        """
-
-        def model(name):
-            models = self.api.send_request('api/models', 'get',
-                                           {'gateway': True, 'verbose': 100, 'limit': 0}).json().get('result')
-            for model_ in models:
-                if len(re.findall(model_.get('firmwareNamePattern'), name)) == 1:
-                    return model_.get('name')
-
-        def version(name):
-            return 'V' + re.findall('V(.*).bin', name)[0]
-
-        sn = [sn] if isinstance(sn, str) else sn
-        devices = list(filter(lambda x: x.get('id'), self.device_state(sn)))
-        if os.path.isfile(firmware) and devices:
-            file_name = os.path.basename(firmware)
-            get_firmware = self.api.send_request('api/firmware', 'get', {'name': file_name}).json()
-            if get_firmware.get('total') == 0:
-                if os.path.exists(firmware):
-                    param = {'filename': firmware, 'oid': 'undefined'}
-                    upload_file = self.api.send_request('api/file/form', method='post', param=param,
-                                                        params_type='form', file_path=firmware).json().get('result')
-                    body = {'fid': upload_file['_id'], 'jobTimeout': 30, 'model': model(file_name),
-                            'name': file_name,
-                            'version': version(file_name), 'desc': 'auto test upload firmware'}
-                    firmware_id = self.api.send_request('api/firmware', 'post', body=body, ).json().get(
-                        'result').get(
-                        '_id')
+                        self.agg_in(self.edge_locators.group_locator, {group[0]: group[1]})
+            logging.info('group: {} success'.format(kwargs.get('group')))
+        if kwargs.get('controller'):
+            self.__controller(kwargs.get('controller'))
+            logging.info('controller: {} success'.format(kwargs.get('controller')))
+        if kwargs.get('measure'):
+            self.__measure(kwargs.get('measure'))
+            logging.info('measure: {} success'.format(kwargs.get('measure')))
+        if kwargs.get('controller_template') and isinstance(kwargs.get('controller_template'), list):
+            self.access_menu('edge_computing.device_supervisor.measure_monitor.controller_template')
+            for template in kwargs.get('controller_template'):
+                if template[0] in ('edit', 'check', 'delete'):
+                    self.agg_in(self.edge_locators.controller_template_locator, {'table': [template]})
                 else:
-                    logging.exception(f'{firmware} not exist')
-                    raise FileNotFoundError(f'{firmware} not exist')
-            else:
-                logging.debug(f'This file {firmware} already exists on the cloud {self.host} {self.username}')
-                firmware_id = get_firmware.get('result')[0].get('_id')
-            self.api.send_request(f'api/firmware/{firmware_id}/devices', method='post',
-                                  body={'deviceIds': [device.get('id') for device in devices], 'deviceGroupIds': [], })
-        else:
-            logging.debug(f'{firmware} not is file or device is not exist')
-
-    def web_remote_online(self, sn: str) -> str:
-        """封装远程web访问方法
+                    if template[0] == 'import':
+                        import_confirm = True if template[2] is None else template[2]
+                        self.agg_in(self.edge_locators.controller_template_locator,
+                                    {'import': template[1], 'import_confirm': import_confirm})
+                    elif template[0] == 'delete_bulk':
+                        try:
+                            delete_bulk_confirm = template[2]
+                        except IndexError:
+                            delete_bulk_confirm = True
+                        self.agg_in(self.edge_locators.controller_template_locator, {'check_all': False})
+                        check_group = [template[1]] if isinstance(template[1], str) else template[1]
+                        for name in check_group:
+                            self.agg_in(self.edge_locators.controller_template_locator,
+                                        {'table': [('check', name, True)]})
+                        self.agg_in(self.edge_locators.controller_template_locator,
+                                    {'delete_bulk': template[1], 'delete_bulk_confirm': delete_bulk_confirm})
+                    else:
+                        self.agg_in(self.edge_locators.controller_template_locator, {template[0]: template[1]})
+            logging.info('controller_template: {} success'.format(kwargs.get('controller_template')))
 
-        :param sn: str, 设备序列号
-        :return: 远程web管理链接
+    @allure.step('断言测点监控列表状态')
+    @loop_inspector('measure_monitor_status')
+    def assert_status(self, **kwargs):
         """
-        if self.host == 'iot.inhand.com.cn':
-            server = 'ngrok.iot.inhand.com.cn:4443'
-        elif self.host == 'iot.inhandnetworks.com':
-            server = 'iot.inhandnetworks.com:4443'
-        elif self.host == 'ics.inhandiot.com':
-            server = 'ics.inhandiot.com:4443'
-        else:
-            server = 'ngrok.ics.inhandnetworks.com:443'
-        response = self.api.send_request('api/devices', method='get',
-                                         param={"verbose": 100, "limit": 10, "cursor": 0,
-                                                'serial_number': sn})
-        if response.json().get('total') == 1 and response.json().get('result')[0].get('online') == 1:
-            device_id = response.json().get('result')[0].get('_id')
-            device_name = response.json().get('result')[0].get('name')
-            body = {"priority": 30, "timeout": 20000, "objectId": device_id, "objectName": device_name,
-                    "name": "ngrok connect", "type": "23", "data": {"server": server, "proto": 'http', "port": 80}}
-            for i in range(0, 3):
-                try:
-                    ngrok = self.api.send_request('api2/tasks/run', method='post', body=body).json()
-                    if ngrok["result"]["data"]["response"]:
-                        return ngrok["result"]["data"]["response"]
-                except Exception as e:
-                    logging.error(f"ngrok request failed reason is {e}, try {i + 2} again")
-            else:
-                logging.exception(f'Device {sn} get ngrok failed.')
-                raise Exception(f'Device {sn} get ngrok failed.')
-        else:
-            logging.exception(f'the device {sn} is offline or not exist')
-            raise ResourceNotFoundError(f'the {sn} is not exist or offline')
 
-    def reboot_online(self, sn: str) -> None:
-        """DM平台设备重启
+        :param kwargs:
+                controller: dict or list 校验一个或多个控制器状态
+                     name: str  控制器名称 必填
+                     online: bool  True | False
+                     status: str  enable | disable
+                     protocol: str
+                     address: str ex: '"10.5.23.84:502:1" in "${value}"'
+                     description: str ex: '"test" in "${value}"'
+                measure: dict or list 校验一个或多个测点状态
+                     name: str  测点名称 必填
+                     online: bool  True | False
+                     group: str  所属组
+                     datatype: str  数据类型
+                     address: str
+                     value: str ex: '"1" in "${value}"'
+                     unit:  str
+                     description: str
+                     time: str
+                timeout: int 超时时间
+                interval: int 轮询间隔
+        :return:
         """
-        response = self.api.send_request('api/devices', method='get',
-                                         param={"verbose": 100, "limit": 10, "cursor": 0,
-                                                'serial_number': sn})
-        if response.json().get('total') == 1 and response.json().get('result')[0].get('online') == 1:
-            device_id = response.json().get('result')[0].get('_id')
-            logging.debug(f'{self.host} send to {sn} reboot command')
-            status = self.api.send_request(f'api/device/{device_id}/methods', 'post',
-                                           body={'method': "reboot", 'timeout': 15000}).json().get('status')
-            assert status == 'succeeded', 'reboot error!'
-        else:
-            logging.exception(f'the device {sn} is offline or not exist')
-            raise ResourceNotFoundError(f'the {sn} is not exist or offline')
 
-    def remote_maintenance_online(self, sn: str, protocol='http', port=80, local_host='192.168.2.1',
-                                  action='connect') -> str or None:
-        """封装dm远程维护方法
-
-        :param sn，必须在线
-        :param protocol: str, 本地主机服务的协议, 'http'| 'https'| 'tcp'
-        :param port: 端口, 本地主机的端口
-        :param local_host: str, 本地主机的ip地址
-        :param action: str, 是否连接远程维护隧道, 'connect'| 'disconnect'| 'delete'| 当为connect 时如果隧道不存在则自动新增
-        :return: 当action='connect' 时返回远程维护连接
-        """
-        device = list(filter(lambda x: x.get('id'), self.device_state([sn])))
-
-        tunnel_des = f'{sn} tunnel {protocol}://{local_host}:{port} '
-
-        def find_tunnel(device_id_):
-            tunnels_ = self.api.send_request('/api/touch/tunnels', method='get',
-                                             param={'verbose': 100, 'device_id': device_id_}).json().get('result')
-            if tunnels_:
-                for tunnel_ in tunnels_:
-                    if tunnel_.get('proto') == protocol and tunnel_.get('localPort') == port and tunnel_.get(
-                            'localAddress'):
-                        return tunnel_.get('_id'), tunnel_.get('connected'), tunnel_.get('publicUrl')
-            return None, None, None
-
-        if device:
-            device_id = device[0].get('id')
-            add_tunnel_body = {'verbose': 100, 'proto': protocol, 'name': str(round(time.time() * 1000)),
-                               'localAddress': local_host, 'localPort': port, 'deviceId': device_id}
-            tunnel_id, tunnel_status, pub_url = find_tunnel(device_id)
-            if action == 'connect' and device[0].get('online'):
-                if not tunnel_id:
-                    result = self.api.send_request('/api/touch/tunnels', method='post', body=add_tunnel_body).json()
-                    tunnel_id = result.get('result').get('_id')
-                    tunnel_status = False
-                    logging.debug(f'Add {tunnel_des} success, tunnel name is {add_tunnel_body["name"]}')
-                if not tunnel_status:
-                    for i in range(0, 3):
-                        connect = self.api.send_request(f'/api/touch/tunnels/{tunnel_id}/connect', 'put').json()
-                        if connect.get('result').get('connected'):
-                            pub_url = connect.get('result').get('publicUrl')
-                            logging.info(f'tunnel {tunnel_des} connect success')
-                            break
-                    else:
-                        logging.exception(f'tunnel {tunnel_des} connect failed')
-                        raise ConnectionError(f'tunnel {tunnel_des} connect failed')
+        def controller(controller_info) -> bool:
+            controller_name = controller_info.get('name')
+            if controller_info.get('online') is not None:
+                if controller_info.get('online'):
+                    controller_info.update({'online_': '"default" not in "${value}"'})
                 else:
-                    logging.debug(f'tunnel {tunnel_des} already connect')
-                return pub_url
-            elif action == 'disconnect' and device[0].get('online'):
-                if tunnel_id and tunnel_status:
-                    self.api.send_request(f'/api/touch/tunnels/{tunnel_id}/disconnect', 'put')
-                    logging.info(f'tunnel {tunnel_des} disconnect success')
+                    controller_info.update({'online_': '"default" in "${value}"'})
+            if controller_info.get('status') is not None:
+                if controller_info.get('status') == 'enable':
+                    controller_info.update({'status_': '"enableCard" not in "${value}"'})
                 else:
-                    logging.debug(f'tunnel {tunnel_des} not exist or already disconnect')
-            elif action == 'delete':
-                if tunnel_id:
-                    self.api.send_request(f'/api/touch/tunnels/{tunnel_id}', 'delete')
-                    logging.info(f'tunnel {tunnel_des} delete success')
+                    controller_info.update({'status_': '"enableCard" in "${value}"'})
+            self.__turn_page(controller_name)
+            return self.eval_locator_attribute(controller_info,
+                                               self.edge_locators.controller_card_status(controller_name))
+
+        def measure(measure_info) -> bool:
+            measure_name = measure_info.get('name')
+            if measure_info.get('online') is not None:
+                if measure_info.get('online'):
+                    measure_info.update({'online_': '"default" not in "${value}"'})
                 else:
-                    logging.debug(f'tunnel {tunnel_des} not exist')
-        else:
-            logging.error(f'the device {sn} not exist')
-
-    def delete_device(self, sn: str or list) -> None:
-        """
-
-        :param sn: 设备序列号，一个或多个
-        :return:
-        """
-        sn = [sn] if isinstance(sn, str) else sn
-        device = list(filter(lambda x: x.get('id'), self.device_state(sn)))
-        if device:
-            for device_ in device:
-                self.api.send_request(f'api/devices/{device_.get("id")}', 'delete')
-                logging.info(f'the {device_.get("sn")} delete success')
-
-
-class IcsInterface(DmInterface):
-    __slots__ = ['remote_maintenance_online']
+                    measure_info.update({'online_': '"default" in "${value}"'})
+            self.__turn_page(measure_name, 'measure')
+            return self.eval_locator_attribute(measure_info, self.edge_locators.measure_card_status(measure_name))
+
+        if kwargs.get('controller'):
+            self.access_menu('edge_computing.device_supervisor.measure_monitor.monitoring_list')
+            if isinstance(kwargs.get('controller'), dict):
+                return controller(kwargs.get('controller'))
+            elif isinstance(kwargs.get('controller'), tuple) or isinstance(kwargs.get('controller'), list):
+                for controller_ in kwargs.get('controller'):
+                    if not controller(controller_):
+                        return False
+                else:
+                    return True
+        if kwargs.get('measure'):
+            self.access_menu('edge_computing.device_supervisor.measure_monitor.monitoring_list')
+            if isinstance(kwargs.get('measure'), dict):
+                return measure(kwargs.get('measure'))
+            elif isinstance(kwargs.get('measure'), tuple) or isinstance(kwargs.get('measure'), list):
+                for measure_ in kwargs.get('measure'):
+                    if not measure(measure_):
+                        return False
+                else:
+                    return True
 
-    def __init__(self, username, password, host='ics.inhandiot.com'):
-        """
-        :param username  平台用户名
-        :param password  平台密码
-        :param host: 'ics.inhandiot.com'|'ics.inhandnetworks.com' 平台是哪个环境
+    @allure.step('获取测点监控列表状态')
+    def get_status(self, measure_name: str or list or tuple, keys: str or list or tuple) -> str or dict or None:
         """
-        super().__init__(username, password, host)
-        self.oid = self.__oid()
-
-    def __oid(self) -> str:
-        return self.api.send_request('api/me', 'get', {'verbose': 100}).json().get('result').get('oid')
 
-    def add_device(self, sn_model: dict):
-        """添加设备，
-
-        :param sn_model: {$sn: 'IR302', $sn1: 'IR305'}
-                model: IR901|IR912|IG902|IR915-WiFi|IG902-WiFi|VG710|IR915|IR611|IR615|IR301|IR302|IR305|IG501|IG502|IG532|IG974|VG814,
-                    型号内容必须填写正确，不然添加的时候下发OpenVpn的配置会出问题，导致不能正常连接
-        :return:
-        """
-        if sn_model:
-            not_add = list(filter(lambda x: x.get('id') is None, self.device_state(list(sn_model.keys()))))
-            if not_add:
-                models = self.api.send_request('api/invpn/routers/models', 'get').json().get('result').get('models')
-                for not_a in not_add:
-                    sn = not_a.get('sn')
-                    model = sn_model.get(sn)
-                    for model_ in models:
-                        if model == model_.get('name'):
-                            lan_interface = model_.get('lanInterface')
-                            if len(re.findall(model_.get('serialNumberPattern'), sn)) == 1:
-                                subnet = self.api.send_request('api/invpn/router/subnet', 'get').json().get('result')
-                                body = {'serialNumber': sn, 'name': sn + str(int(time.time())),
-                                        'lanInterface': lan_interface,
-                                        'subnet': subnet}
-                                self.api.send_request('api/invpn/router', 'post', {'oid': self.oid}, body=body)
-                                logging.info(f'add device {sn} to cloud {self.host} successfully')
-                            break
+        :param measure_name: str or list or tuple 一个或多个测点名称
+        :param keys: str or list or tuple , value|time
+        :return: value or {'measure_name1': value}
+        """
+        if measure_name:
+            self.access_menu('edge_computing.device_supervisor.measure_monitor.monitoring_list')
+            if isinstance(measure_name, str):
+                return self.get_text(keys, self.edge_locators.measure_card_status(measure_name))
+            else:
+                measure_value = {}
+                for name in measure_name:
+                    measure_value.update({name: self.get_text(keys, self.edge_locators.measure_card_status(name))})
+                return measure_value
+
+
+class Cloud(BasePage, IgLocators):
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
+        IgLocators.__init__(self, page, locale)
+
+    def __measure_point(self, cloud_measure, mute_measure, close=False):
+        """
+
+        :param cloud_measure: [(action_type, value, ),]
+        :param mute_measure: [(action_type, value, ),]
+        :return:
+        """
+        if cloud_measure:
+            self.access_menu('edge_computing.device_supervisor.cloud.mqtt_cloud_service.cloud_measuring_setting.cloud')
+            for ac in cloud_measure:
+                if ac[0] == 'search':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {"search": ac[1], 'is_search': True})
+                elif ac[0] == 'page_number':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {"page_number": ac[1]})
+                elif ac[0] in ('import', 'export'):
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {ac[0]: ac[1]})
+                elif ac[0] == 'check':
+                    self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), {'check': ac[2]})
+                elif ac[0] == 'mute':
+                    self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), {'mute': True, 'confirm': True})
+                elif ac[0] == 'check_all':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {ac[0]: True})
+                elif ac[0] == 'mute_bulk':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {'check_all': False})  # 先取消选择所有的
+                    all_measure = [ac[1]] if isinstance(ac[1], str) else ac[1]
+                    self.__measure_point(cloud_measure=[('check', x, True) for x in all_measure], mute_measure=None)
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {'mute_bulk': True, 'bulk_confirm': True})
+                elif ac[0] == 'name':
+                    if isinstance(ac[2], str):
+                        value = {'name_edit': True, 'value': ac[2], 'submit': {"wait_for_time": 3 * 1000}}
                     else:
-                        logging.exception(f'the Serial number {sn} and model do not match ')
-                        raise Exception(f'the Serial number {sn} and model do not match ')
-
-    def device_state(self, sn: list) -> List[dict]:
-        """根据sn 转换属性 属性值有：  online: 在线|离线   1|0
-                                       connected: true | None
-                                       iccid:
-                                       imei:
-                                       imsi:
-                                       version: 固件版本
-                                       hwVersion: 硬件版本 'V1.0'
-                                       bootVersion:  Bootloader版本  '1.1.3.r4956'
-                                       sn: 序列号
-                                       id: 设备id
-                                       name: 设备名称
-                                       vip: 虚拟IP
-                                       ip: 设备连接平台的ip地址
-                                       protocol: 设备连接平台的协议
-                                       config_sync: 设备配置同步状态
-        :param sn: 列表
-        :return: [{'sn': $sn, 'online': 1, 'iccid': '', 'imei'}]
-        """
-        result = []
-        for sn_ in sn:
-            response = self.api.send_request('api/invpn/routers', method='get',
-                                             param={"limit": 10, "cursor": 0, 'verbose': 100,
-                                                    'serialNumber': sn_}).json()
-            if response.get('total') == 1:
-                logging.debug(f'the device {sn_} exist on {self.host}')
-                res = response.get('result')[0]
-                res_info = self.api.send_request(f'api/devices/{res.get("id")}', method='get',
-                                                 param={'verbose': 100}).json().get('result')
-                config_sync = res_info.get('config').get('sync') if res_info.get('config') else None
-                result.append(
-                    {'sn': sn_, 'online': res.get('online'), 'iccid': res.get('metadata').get('iccid'),
-                     'imei': res.get('metadata').get('imei'), 'imsi': res.get('metadata').get('imsi'),
-                     'version': res.get('metadata').get('swVersion'), 'hwVersion': res.get('metadata').get('hwVersion'),
-                     'bootVersion': res.get('metadata').get('bootVersion'), 'vip': res.get('vip'),
-                     'id': res.get('id'), 'connected': res.get('connected'), 'name': res.get('name'),
-                     'ip': res_info.get('pubIp'), 'protocol': res_info.get('protocol'), 'config_sync': config_sync})
-            else:
-                result.append(
-                    {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'version': None,
-                     'hwVersion': None, 'bootVersion': None, 'id': None, 'connected': None, 'name': None, 'ip': None,
-                     'protocol': None, 'config_sync': None, 'vip': None})
-        return result
-
-    def send_openvpn_config(self, sn: str) -> None:
-        """每次把设备添加到平台上线后，openvpn要连半天，可以主动推送下配置让openvpn连接的更快，
-           如果设备已经连接上了openvpn就不在下发了
-
-        :param sn: 单个sn
-        :return:
-        """
-        result = self.device_state([sn])[0]
-        if result.get('online') and not result.get('connected'):
-            self.api.send_request(f'api/invpn/router/{result.get("id")}/config/send', 'get', param={'oid': self.oid})
-        elif not result.get('id'):
-            logging.warning(f'the device {sn} not exist')
-        elif not result.get('online'):
-            logging.warning(f'the device {sn} offline')
-        elif result.get('connected'):
-            logging.warning(f'the device {sn} already connected')
-
-    def delete_device(self, sn: str or list) -> None:
-        """
-
-        :param sn: 设备序列号，一个或多个
-        :return:
-        """
-        sn = [sn] if isinstance(sn, str) else sn
-        device = list(filter(lambda x: x.get('id'), self.device_state(sn)))
-        if device:
-            for device_ in device:
-                self.api.send_request(f'api/invpn/router/{device_.get("id")}', 'delete', {'oid': self.oid})
-                logging.info(f'the {device_.get("sn")} delete success')
-
-    @loop_inspector('ics user connect openvpn')
-    def assert_user_openvpn_connect(self, email, timeout=60, interval=5):
-        response = self.api.send_request('/api/invpn/users', 'get', param={'verbose': 100, 'email': email}).json()
-        return response['result'][0]['connected']
-
-
-class StarInterface:
-
-    def __init__(self, username, password, host='star.inhandcloud.cn'):
-        """ 须确保用户关闭了多因素认证
-
-        :param username  平台用户名
-        :param password  平台密码
-        :param host: 'star.inhandcloud.cn'|'star.inhandcloud.cn'|'star.nezha.inhand.dev'|'star.nezha.inhand.design' 平台是哪个环境,
-        """
-        self.host = host
-        self.username = username
-        self.api = InRequest(self.host, username, password, 'star')
-        self.me = self.__get_me()
-
-    def __only_admin(function):
-        """只能当装饰器使用，只有admin用户才能使用
-
-        :param function:
-        :return:
-        """
-
-        def admin_user(self, *args, **kwargs):
-            if self.username != 'admin':
-                logging.exception('only admin user can use this function')
-                raise Exception('only admin user can use this function')
-            else:
-                res = function(self, *args, **kwargs)
-            return res
-
-        return admin_user
-
-    def __only_user(function):
-        """只能当装饰器使用，只有用户才能使用
-
-        :param function:
-        :return:
-        """
-
-        def _user(self, *args, **kwargs):
-            if self.username == 'admin':
-                logging.exception('only user can use this function')
-                raise Exception('only user can use this function')
-            else:
-                res = function(self, *args, **kwargs)
-            return res
-
-        return _user
-
-    def __get_me(self) -> DotDict:
-        """ 获取me的各种信息 包括oid
-
-        :return:
-        """
-        response = DotDict(
-            self.api.send_request('/api/v1/users/me', method='get', param={"expand": 'org'}).json().get('result'))
-        return response
-
-    @__only_user
-    def send_config(self, sn: str, payload: dict, commit=True) -> dict:
-        """下发设备配置
-
-        :param sn: 设备序列号
-        :param commit: 是否提交, 在云端可以保存配置，默认是提交
-        :param payload: 配置内容，当配置中的key是随机id时， 可使用$id，下发时会自动替换成随机id
-        :return:
-        """
-
-        def switch_config(in_payload: dict) -> dict:
-            """转换配置，当配置中的key是随机id时， 可使用$id, 然后该函数会自动替换成随机id并返回
-
-            :param in_payload: 需要修正的配置项，其中需要更新的key 使用$id来替换
-            :return:
-            """
-            local_time = str(hex(int(time.time())))[2:]
-            start = f'000{random.randint(1, 9)}{local_time}'
-            in_payload = str(in_payload)
-            for i in range(0, len(re.findall('\$id', in_payload))):
-                in_payload = in_payload.replace('$id',
-                                                f'{start}{generate_string(4, uppercase=False, special_chars=False)}', 1)
-            return eval(in_payload)
-
-        payload = switch_config(payload)
-        session_id = \
-            self.api.send_request('/api/v1/config/init', 'post',
-                                  param={'deviceId': self.device_state([sn])[0].get('id')},
-                                  ).json().get('result').get('_id')
-        header = {'x-session-id': session_id}
-        resp = self.api.send_request('/api/v1/config', 'put', body=payload, header=header).json()
-        assert resp == {'result': 'ok'}, 'save config failed'
-        if commit:
-            resp = self.api.send_request('/api/v1/config/commit', 'post', header=header).json()
-            assert resp == {'result': 'ok'}, 'commit config failed'
-            logging.info(f'the device {sn} config commit success')
-        return payload
-
-    @__only_user
-    def get_config(self, sn: str, expect: dict, type_='actual') -> dict or None:
-        """获取校验备配置
-
-        :param sn: 设备序列号
-        :param expect: 配置内容，完整的配置路径，如{'lan': {'type': 'dhcp'}}
-        :param type_: actual 实际设备上传的配置
-                      group 设备所在组的配置
-                      pending 正在下发的配置
-                      target 目标配置
-                      individual 个性化配置
-        :return: 如果 expect 为None 就返回设备当前实际的配置
-        """
-        expect = {'result': {type_: expect}}
-        if expect is not None:
-            self.api.send_request(f'/api/v1/devices/{self.device_state([sn])[0].get("id")}/config', 'get',
-                                  expect=expect)
-        else:
-            return self.api.send_request(f'/api/v1/devices/{self.device_state([sn])[0].get("id")}/config',
-                                         'get').json().get('result').get(type_)
-
-    @__only_user
-    def clear_config(self, sn: str):
-        """清除设备配置
-
-        :param sn:
-        :return:
-        """
-        self.api.send_request(f'/api/v1/config/layer/device/{self.device_state([sn])[0].get("id")}', 'delete', expect={
-            "result": 'ok'})
-        self.get_config(sn, expect={}, type_='individual')
-
-    @__only_user
-    def copy_config(self, source_sn: str, target_sns: list):
-        """清除设备配置
-
-        :param source_sn: 源设备sn
-        :param target_sns: 目标设备sn
-        :return:
-        """
-        body = {"sourceDeviceId": self.device_state([source_sn])[0].get("id"),
-                "targetDeviceIds": [device.get('id') for device in self.device_state(target_sns)]}
-        self.api.send_request(f'/api/v1/config/layer/bulk-copy', 'post', body=body, expect={"result": 'ok'})
-
-    @__only_user
-    def create_org(self, name: str, parent_name: str or None, level=2, email='', phone='', **kwargs) -> str:
-        """创建组织, 创建2级组织时，parent_name和parent_id可以不传
-
-        :param name: 组织名称 (在实现自动化时可让名称唯一，来实现创建组织的唯一性)
-        :param parent_name: 父组织名称，如果组织名称唯一，可以传入，如果不唯一就拿第一个创建
-        :param level: 组织层级，2 二级组织，3 三级组织 4 四级组织 5 五级组织
-        :param email: 组织邮箱
-        :param phone: 组织电话
-        :param kwargs: 组织信息
-               parent_id: 父组织id，唯一id，传入它时可以不用传入parent_name
-               description: 组织描述
-        :return: 组织id
-        """
-        if level in (2, 3, 4, 5):
-            parent_level = level - 1
-            orgs = self.api.send_request('/api/v1/orgs', 'get', param={'depth': 4, 'limit': 500}).json().get('result')
-            if parent_level == 1:
-                parent_id = [org.get('_id') for org in orgs if org.get('level') == 1][0]
-            else:
-                if kwargs.get('parent_id'):
-                    parent_id = kwargs.get('parent_id')
+                        value = {'name_edit': True}.update(ac[2])
+                    self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), value)
                 else:
-                    parent_id = [org.get('_id') for org in orgs if org.get('level') == parent_level and
-                                 org.get('name') == parent_name][0]
-            body = {'name': name, 'parent': parent_id, 'phone': phone, 'email': email,
-                    'description': kwargs.get('description')}
-            logging.info(f'create org {name} success')
-            return self.api.send_request('/api/v1/orgs', 'post', body=body).json().get('result').get('_id')
-        else:
-            raise ValueError('level must be in (2, 3, 4, 5)')
-
-    @__only_user
-    def delete_org(self, name: str or list or None, _id: str or list or None):
-        """删除组织, 不能删除一级组织
-
-        :param name: 组织名称, _id 为None时，使用名称删除，搜索到名称一致的组织就全部删除
-        :param _id: 组织id, 使用id删除，精确删除
-        :return:
-        """
-        if _id:
-            if isinstance(_id, str):
-                _id = [_id]
-        else:
-            if name:
-                if isinstance(name, str):
-                    name = [name]
-                orgs = self.api.send_request('/api/v1/orgs', 'get', param={'depth': 5, 'limit': 500}).json().get(
-                    'result')
-                _id = []
-                for name_ in name:
-                    [_id.append(org.get('_id')) for org in orgs if org.get('name') == name_]
-
-        if _id:
-            for __id in _id:
-                self.api.send_request(f'/api/v1/orgs/{__id}', 'delete')
-            logging.info(f'delete org success')
-
-    @__only_admin
-    def org_info_in_paas(self, org_email) -> DotDict:
-        """ 获取org info
-
-        :param org_email:
-        :return:   {name: "Admin_test_new", email: "liwei@inhand.com.cn", _id: "5fb24ef9f0393a4c4fd7c8b7"}
-        """
-        orgs = \
-            self.api.send_request('/api/v1/orgs', 'get',
-                                  param={'email': org_email, 'fields': '_id,name,email', 'limit': 100}).json().get(
-                'result')
-        if orgs:
-            for org in orgs:
-                if org.get('email') == org_email:
-                    return DotDict(org)
-            else:
-                logging.exception(f'the org {org_email} not exist')
-                raise Exception(f'the org {org_email} not exist')
-        else:
-            logging.exception(f'the org {org_email} not exist')
-            raise Exception(f'the org {org_email} not exist')
-
-    @__only_admin
-    def create_license_to_org(self, org_email: str, licenses: dict):
-        """ 创建license
-
-        :param org_email: 企业邮箱
-        :param licenses: license {'slug': 'star_pro', 'period': 'year', 'periodCount':1, 'number': 1}
-        """
-        license_prices = self.api.send_request(f'/api/v1/billing/license-types/{licenses.get("slug")}/prices', 'get',
-                                               param={'verbose': 100}).json().get('result')
-        org_info = self.org_info_in_paas(org_email)
-        try:
-            license_price = [i for i in license_prices if
-                             i['period'] == licenses.get('period') and i['periodCount'] == licenses.get('periodCount')][
-                0]
-            self.api.send_request('/api/v1/billing/licenses', 'post',
-                                  body={'type': licenses.get('slug'), 'active': True, 'count': licenses.get('number'),
-                                        'oid': org_info.get('_id'), 'priceId': license_price['_id']}, code=200)
-        except Exception:
-            logging.exception(f'licenses create fail, please check the licenses info')
-            raise
-
-    @__only_admin
-    def delete_user_in_paas(self, email):
-        """ 删除用户
-
-        :param email:
-        :return:
-        """
-        users = self.api.send_request('api/v1/users', 'get', param={'email': email, 'limit': 100}).json().get('result')
-        if users:
-            for user in users:
-                if email == user.get('email'):
-                    try:
-                        self.api.send_request(f'api/v1/users/{user.get("_id")}', 'delete',
-                                              param={'oid': user.get("oid")})
-                        logging.info(f'the {email} user delete success')
-                    except Exception:
-                        logging.exception(f'the email be used by org, can not delete')
-                    break
-            else:
-                logging.info(f'the {email} user not exist')
-
-    @__only_admin
-    def create_org_in_paas(self, org_info: dict):
-        """
+                    pass
+        if mute_measure:
+            self.access_menu('edge_computing.device_supervisor.cloud.mqtt_cloud_service.cloud_measuring_setting.mute')
+            for ac in mute_measure:
+                if ac[0] == 'search':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {"search": ac[1], 'is_search': True})
+                elif ac[0] == 'page_number':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {"page_number": ac[1]})
+                elif ac[0] in ('import', 'export'):
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {ac[0]: ac[1]})
+                elif ac[0] == 'check':
+                    self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), {'check': ac[2]})
+                elif ac[0] == 'add':
+                    self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), {'add': True, 'confirm': True})
+                elif ac[0] == 'check_all':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {ac[0]: True})
+                elif ac[0] == 'add_bulk':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {'check_all': False})  # 先取消选择所有的
+                    all_measure = [ac[1]] if isinstance(ac[1], str) else ac[1]
+                    self.__measure_point(cloud_measure=None, mute_measure=[('check', x, True) for x in all_measure])
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {'add_bulk': True, 'bulk_confirm': True})
+                else:
+                    pass
+        if (cloud_measure or mute_measure) and close:
+            self.agg_in(self.edge_locators.cloud_measuring_point, {'close': True})
 
-        :param org_info:  {'email': org_email, 'password': org_password} 必填
-        :return:
+    @allure.step('配置Device Supervisor Cloud')
+    def config(self, **kwargs):
         """
-        orgs = self.api.send_request('api/v1/orgs', 'get',
-                                     param={'email': org_info.get('email'), 'limit': 100}).json().get('result')
-        org_info.update(
-            {'name': org_info.get('email'), 'bizCategory': 'OILS_GAS_CONSUMABLE_FUELS', 'countryCode': 'AL'})
-        if orgs:
-            for org in orgs:
-                if org_info.get('email') == org.get('email'):
-                    self.update_user(org_info.get('email'), password=org_info.get('password'))  # 更新密码
-                    logging.debug(f'the {org_info.get("email")} org already exist')
-                    break
-            else:
-                self.api.send_request('api/v1/orgs', 'post', body=org_info)
-                logging.debug(f'admin create {org_info.get("email")} org success')
-        else:
-            self.api.send_request('api/v1/orgs', 'post', body=org_info)
-            logging.debug(f'admin create {org_info.get("email")} org success')
-
-    @__only_admin
-    def delete_org_in_paas(self, org_info: dict):
-        """ 删除企业
 
-        :param org_info: 企业信息 {'email': org_email, 'password': org_password}
-        :return:
-        """
-        orgs = self.api.send_request('api/v1/orgs', 'get',
-                                     param={'email': org_info.get('email'), 'limit': 100}).json().get('result')
-        if orgs:
-            for org in orgs:
-                if org_info.get('email') == org.get('email'):
-                    org_user = StarInterface(org_info.get('email'), org_info.get('password'), self.host)
-                    org_user.delete_device('all')
-                    self.api.send_request(f'api/v1/orgs/{org.get("_id")}', 'delete')
-                    logging.info(f'admin delete {org_info.get("email")} org delete success')
-                    break
-            else:
-                logging.info(f'the {org_info.get("email")} org not exist')
-
-    @__only_user
-    def bind_license(self, sn: list, licenses: dict):
-        """ 绑定license
-
-        :param sn
-        :param licenses: {'slug': 'star_pro'}
-        """
-        licenses_ = []
-        org_license = self.api.send_request('/api/v1/billing/licenses', 'get',
-                                            param={'expand': 'org,device,type', 'limit': 200, 'page': 0},
-                                            code=200).json().get('result')
-        if org_license:
-            for org in org_license:
-                if org['status'] != 'expired' and org.get('device') is None and org['type']['slug'] == licenses.get(
-                        'slug'):
-                    licenses_.append(org['_id'])
-        if len(licenses_) < len(sn):
-            logging.error(f'licenses not enough, please check the licenses')
-        else:
-            device_ids = [device.get('id') for device in self.device_state(sn)]
-            for license_, _id in zip(licenses_, device_ids):
-                self.api.send_request(f'/api/v1/billing/licenses/{license_}/device', 'put', body={'deviceId': _id},
-                                      code=200)
-            logging.info(f'bind license success')
-
-    def device_state(self, sn: list) -> List[dict]:
-        """根据sn 转换属性 属性值有：  online: 在线|离线   True|False
-                                       iccid:
-                                       imei:
-                                       imsi:
-                                       version: 固件版本
-                                       licenseStatus: 'licensed'
-                                       sn: 序列号
-                                       address
-                                       id: 设备id
-                                       name: 设备名字
-                                       org:  {'_id': oid, 'name': 'org_name', 'email': 'org_email'}
-        :param sn: 列表
-        :return: [{'sn': $sn, 'online': 1, 'iccid': '', 'imei'}]
-        """
-        result = []
-        for sn_ in sn:
-            response = self.api.send_request('/api/v1/devices', method='get',
-                                             param={"expand": 'firmwareUpgradeStatus,compatibilities,org', "limit": 10,
-                                                    "compatibilities": 'nezha_device_config,nezha_device_webui',
-                                                    'serialNumber': sn_}).json()
-            if response.get('total') == 1:
-                res = response.get('result')[0]
-                state = res.get('state') if res.get('state') else None
-                result.append(
-                    {'sn': sn_, 'online': res.get('online'),
-                     'iccid': state.get('iccid') if state else None,
-                     'imei': state.get('imei') if state else None,
-                     'imsi': state.get('imsi') if state else None,
-                     'version': res.get('firmware'),
-                     'licenseStatus': res.get('licenseStatus'),
-                     'address': res.get('address'),
-                     'id': res.get('_id'), 'org': res.get('org'),
-                     'name': res.get('name')})
-            else:
-                result.append(
-                    {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'org': None,
-                     'version': None, 'licenseStatus': None, 'address': None, 'id': None, 'name': None})
-        return result
-
-    def add_device(self, sn: str, mac_or_imei: str) -> None:
-        """添加设备，
+        :param kwargs:
+                enable: bool True | False 是否启用
+                clear_offline_cache: bool True | False 是否清除离线缓存
+                import: str, 导入文件路径
+                import_confirm: bool True | False 是否确认导入, 或者可以写入 确认导入后的提示
+                export: str  or dict   # 导出
+                        str: 导出文件夹
+                        dict: {"file_path": "./", "file_name": None}
+                cloud_measure: [(action_type, value, ),]
+                    [('page_number', '100page')]  修改每页显示数量
+                    [('search', [$type, name]), ]  # 搜索
+                        type: point_name|controller_name|group_name
+                    [('check', 'test', True), ] or [('check', 'test', False), ]   # 选择与取消选择
+                    [('import', path), ]  # 导入
+                    [('export', path), ]  # 导出
+                    [('check_all', ), ]  # 选择所有
+                    [('mute', 'test',), ]  # 屏蔽
+                    [('mute_bulk', ['test','test1']), ]  # 批量屏蔽
+                    [('name', 'test', 'test1'), ]  # 修改名称
+                mute_measure: [(action_type, value, ),]
+                    [('page_number', '100page')]  修改每页显示数量
+                    [('search', [$type, name]), ]  # 搜索
+                        type: point_name|controller_name|group_name
+                    [('check', 'test', True), ] or [('check', 'test', False), ]   # 选择与取消选择
+                    [('import', path), ]  # 导入
+                    [('export', path), ]  # 导出
+                    [('add_all', ), ]  # 选择所有
+                    [('add', 'test',), ]  # 加入
+                    [('add_bulk', ['test','test1']), ]  # 批量屏蔽
+                cloud_type: mqtt|iSCADA Cloud|alibaba_cloud|AWS IoT|Azure IoT
+                mqtt_server: str
+                mqtt_client_id: str
+                mqtt_auth: True|False
+                mqtt_username: str
+                mqtt_password: str
+                mqtt_last_will: 'expand' | 'collapse'
+                mqtt_last_will_topic: str
+                mqtt_last_will_qos: 0|1|2
+                mqtt_last_will_retain: 'true'|'false'
+                mqtt_last_will_payload: str
+
+                ics_local_configuration: True|False
+                ics_server: str
+                ics_keepalive: int
+
+                alibaba_region_id: str
+                alibaba_auth_method: unique_certificate_per_device|unique_certificate_per_product
+                alibaba_product_key: str
+                alibaba_device_name: str
+                alibaba_device_secret: str
+                alibaba_tls_model: str, 文件路径
+
+                aws_endpoint: str
+                aws_client_id: str
+                aws_certificate: str, 文件路径
+                aws_private_key: str, 文件路径
+                aws_root_ca: str, 文件路径
+
+                azure_auth_method: Symmetric key|X.509 Self-Signed|X.509 CA-Signed
+                azure_connection_string: str
+                azure_hub_name: str
+                azure_device_id: str
+                azure_device_certificate: str, 文件路径
+                azure_device_key: str, 文件路径
+
+                advanced_settings: True|False
+                port: int
+                keep_alive: int
+                tls: 'enable'|'disable'
+                verify_method: verify_client_ca|verify_client_certificate_and_key
+                verify_server_certificate: True|False
+                root_ca: str, 文件路径
+                client_private_key: str, 文件路径
+                client_certificate: str, 文件路径
+                clean_session: no|yes
+                mqtt_version: v3.1 |v3.1.1
+
+                submit: bool or dict,
+
+                publish: [($action, **kwarg)]
+                 [('delete', 'test')]
+                 [('add', kwarg)]
+                     add parameter:
+                     is_exists: name, 如果存在就不添加
+                     name: str
+                     trigger: measuring_point|alarm_message
+                     label: list 多个选项
+                     topic: str
+                     qos: 0|1|2
+                     entry_function: main
+                     quick_function: str,  换行使用\n
+                     save: True|False
+                     text_messages: str or list
+                     tip_messages: str or list
+                     cancel: True, False
+                 [('edit', 'name', kwarg)]
+                 多个操作时使用列表 [('add',{}), ('add',{})]
+                 subscribe: [($action, **kwarg)]
+                 [('delete', 'test')]
+                 [('add', kwarg)]
+                     add parameter:
+                     is_exists: name, 如果存在就不添加
+                     name: str
+                     topic: str
+                     qos: 0|1|2
+                     entry_function: main
+                     payload_type: Plaintext|Base64|JSON|Hex
+                     quick_function: str,  换行使用\n
+                     save: True|False
+                     text_messages: str or list
+                     tip_messages: str or list
+                     cancel: True, False
+                 [('edit', 'name', kwarg)]
+                 多个操作时使用列表 [('add',{}), ('add',{})]
+        :return:
+        """
+        self.access_menu('edge_computing.device_supervisor.cloud')
+        if kwargs.get('cloud_measure') or kwargs.get('mute_measure'):
+            self.agg_in(self.edge_locators.cloud_locator, {'enable': True})
+            self.__measure_point(kwargs.get('cloud_measure'), kwargs.get('mute_measure'), True)
+        if kwargs.get('import') and kwargs.get('import_confirm') is None:
+            kwargs.update({'import_confirm': True})
+        if kwargs.get('clear_offline_cache'):
+            kwargs.update({'cache_confirm': True})
+        self.agg_in(self.edge_locators.cloud_locator, kwargs)
+
+
+class Alarm(BasePage, IgLocators):
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
+        IgLocators.__init__(self, page, locale)
 
-        :param sn: 设备序列号
-        :param mac_or_imei: 添加设备时需要依赖设备的mac地址或者IMEI号，去生产库查询该设备是否是映翰通设备
-        :return:
+    @allure.step('配置Device Supervisor告警')
+    def config(self, **kwargs):
         """
-        for i in range(5):
-            validated_field = self.api.send_request(f'api/v1/serialnumber/{sn}/validate', method='post').json().get(
-                'result').get('validatedField')
-            if not list(filter(lambda x: x.get('id'), self.device_state([sn]))):
-                self.api.send_request('api/v1/devices', 'post',
-                                      body={"name": sn + str(int(time.time())), "serialNumber": sn, 'oid': self.me.oid,
-                                            validated_field: mac_or_imei})
-                logging.info(f"the {sn} device add success")
-            else:
-                break
-
-    def assert_device_state(self, sn: str, state: dict, timeout=120, interval=5) -> None:
-        """校验设备基本状态
 
-        :param sn: 序列号
-        :param state:   支持表达式${value} ex: {'version': "'${value}' in 'V1.1.3.r4956'"}
-                        online: 在线|离线   True|False
-                        iccid:
-                        imei:
-                        imsi:
-                        version: 固件版本
-                        licenseStatus: 'licensed'
-                        sn: 序列号
-                        address
-        :param timeout: 校验信息，最大超时时间
-        :param interval: 校验信息，校验间隔时间
-        :return: True or False
-        """
-        if state:
-            for i in range(0, timeout, interval):
-                result = self.device_state([sn])[0]
-                for key, value in state.items():
-                    if '${value}' in value:
-                        value = replace_str(value, {'${value}': result.get(key)})
-                        logging.debug(f'start assert {sn} state {key} {value}')
+        :param kwargs:
+                realtime: dict
+                    page_number: 50page|30page|100page
+                rules: [('action_type', value, value1)]
+                    [('page_number', value, )]
+                        value: 50page|30page|100page
+                    [('import', value, value1)]
+                        value: str  导入文件路径
+                        value1: 导入时的确认，默认为True， 也可以校验导入后的提示
+                    [('export', value,)]
+                        value: str  or dict   # 导出
+                        str: 导出文件夹
+                        dict: {"file_path": "./", "file_name": None}
+                    [('add', kwargs)]
+                        kwargs:
+                            is_exists: str, 可以填写告警相关连续的信息， 如果存在就不会添加了
+                            name: 名称
+                            controller: 控制器名称
+                            measure: 测点名称
+                            level: remind|warning|secondary|important|serious
+                            condition: 告警条件， list，['=', '13', '&&', '>', '13'], 不需要的值可以写None
+                            content: 告警内容
+                            label: 标签
+                            save: 是否保存  save=True 没有该参数时自动保存
+                            cancel: 是否取消  cancel=True
+                            text_messages: str or list
+                            tip_messages: str or list
+                    [('edit', 'old_alarm_name', kwargs)]  kwargs 同add
+                    [('check', name, True)] or   [('check', name, False)] # 勾选或取消勾选分组
+                    [('delete', name)]  # 删除
+                    [('check_all', value,)]
+                        value: bool  勾选或取消勾选全部分组 True | False
+                    [('delete_bulk', name, value1)]  # 批量删除分组
+                        name: str or list 一个或多个告警名称
+                        value1: {'tip_messages': 'submit_success'} or None 提示信息
+                    [('add_to_label', name, label_name)]  # 添加到标签
+                        name: str or list 一个或多个告警名称
+                        label_name: str  标签名称
+                history: [('action_type', value, value1)]
+                    [('page_number', value, )]
+                        value: 50page|30page|100page
+                    [('search', **kwargs,)]
+                        name: str 搜索的名字
+                        start_time： 2023-05-29 16:38 開始時間
+                        end_time： 2023-05-29 16:38 結束時間
+                    [('check_all', value,)]
+                        value: bool  勾选或取消勾选全部分组 True | False
+                    [('check', name, True)] or   [('check', name, False)] # 勾选或取消勾选分组
+                    [('delete', name)]  # 删除
+                    [('delete_bulk', name, value1)]  # 批量删除分组
+                        name: str or list 一个或多个告警名称
+                        value1: {'tip_messages': 'submit_success'} or None 提示信息
+                label: [('action_type', value, value1)]
+                    [('page_number', value, )]
+                        value: 50page|30page|100page
+                    [('import', value, value1)]
+                        value: str  导入文件路径
+                        value1: 导入时的确认，默认为True， 也可以校验导入后的提示
+                    [('export', value,)]
+                        value: str  or dict   # 导出
+                        str: 导出文件夹
+                        dict: {"file_path": "./", "file_name": None}
+                    [('add', kwargs)]
+                            kwargs:
+                                is_exists: str, 可以填写告警相关连续的信息， 如果存在就不会添加了
+                                name: 名称
+                                save: 是否保存  save=True 没有该参数时自动保存
+                                cancel: 是否取消  cancel=True
+                                text_messages: str or list
+                                tip_messages: str or list
+                    [('check', name, True)] or   [('check', name, False)] # 勾选或取消勾选分组
+                    [('delete', name)]  # 删除
+                    [('check_all', value,)]
+                        value: bool  勾选或取消勾选全部 True | False
+                    [('delete_bulk', name, value1)]  # 批量删除
+                        name: str or list 一个或多个名称
+                        value1: {'tip_messages': 'submit_success'} or None 提示信息
+        :return:
+        """
+        if kwargs.get('label'):
+            self.access_menu('edge_computing.device_supervisor.alarm.alarm label')
+            for label in kwargs.get('label'):
+                if label[0] in ('add', 'check', 'delete'):
+                    self.agg_in(self.edge_locators.alarm_label_locator, {'table': [label]})
+                else:
+                    if label[0] == 'import':
+                        import_confirm = True if label[2] is None else label[2]
+                        self.agg_in(self.edge_locators.alarm_label_locator,
+                                    {'import': label[1], 'import_confirm': import_confirm})
+                    elif label[0] in ('delete_bulk',):
+                        self.agg_in(self.edge_locators.alarm_label_locator, {'check_all': False})
+                        check_group = [label[1]] if isinstance(label[1], str) else label[1]
+                        for name in check_group:
+                            self.agg_in(self.edge_locators.alarm_label_locator, {'table': [('check', name, True)]})
                         try:
-                            if not eval(value):
-                                logging.debug(f'the {sn} device {key} info eval {value} is false')
-                                break
-                        except Exception as e:
-                            logging.error(e)
-                            break
+                            delete_bulk_confirm = label[2]
+                        except IndexError:
+                            delete_bulk_confirm = True
+                        self.agg_in(self.edge_locators.alarm_label_locator,
+                                    {'delete_bulk': label[1], 'delete_bulk_confirm': delete_bulk_confirm})
                     else:
-                        logging.debug(f'start assert {sn} state {key} {value}')
-                        if result.get(key) != value:
-                            logging.debug(f'the {sn} device {key} info value is {result.get(key)} not {value}')
-                            break
-                else:
-                    logging.info(f"check {sn} device all state success")
-                    break
-                logging.info(f"check {sn} device state failed, please wait for {interval}s")
-                time.sleep(interval)
-            else:
-                logging.exception(f"the {sn} state {state} check failed")
-                raise TimeOutError(f"the {sn} state {state} check failed")
-
-    def delete_device(self, sn: str or list) -> None:
-        """
-
-        :param sn: 设备序列号，一个或多个, sn='all' 时，删除所有设备
-        :return:
-        """
-
-        def delete(ids: list):
-            if ids:
-                for _id in ids:
-                    self.api.send_request(f'api/v1/devices/{_id}', 'delete')
-                    logging.debug(f'{_id} device delete success')
-
-        if sn == 'all':
-            while True:
-                devices = self.api.send_request(f'api/v1/devices', 'get', {'limit': 100, 'page': 0}).json().get(
-                    'result')
-                if devices:
-                    delete([device.get('_id') for device in devices])
+                        self.agg_in(self.edge_locators.alarm_label_locator, {label[0]: label[1]})
+            logging.info('device supervisor alarm label: {} success'.format(kwargs.get('label')))
+        if kwargs.get('rules'):
+            self.access_menu('edge_computing.device_supervisor.alarm.alarm rules')
+            for rule in kwargs.get('rules'):
+                if rule[0] in ('add', 'edit', 'check', 'delete'):
+                    self.agg_in(self.edge_locators.alarm_rules_locator, {'table': [rule]})
                 else:
-                    break
-                logging.info(f'{self.username} user delete all device success')
-        else:
-            sn = [sn] if isinstance(sn, str) else sn
-            devices = list(filter(lambda x: x.get('id'), self.device_state(sn)))
-            delete([device.get('id') for device in devices])
-            logging.info(f'{self.username} user delete {sn} device success')
-
-    def update_user(self, email: str, **kwargs):
-        """更新用户
-
-        :param email: 用户邮箱
-        :param kwargs:
-               password: 密码
-        :return:
-        """
-        users = self.api.send_request('api/v1/users', 'get',
-                                      param={'email': email, 'limit': 20, 'expand': 'roles,mfa,org'}).json().get(
-            'result')
-        if users:
-            if kwargs.get('password'):
-                for user in users:
-                    if email == user.get('email'):
-                        self.api.send_request(f'api/v1/users/{user.get("_id")}/password', 'put',
-                                              body={'password': kwargs.get('password')})
-                        logging.info(f'the {email} user update password success')
-                        self.api = InRequest(self.host, email, kwargs.get('password'), 'star')  # 重新登录
-                        break
+                    if rule[0] == 'import':
+                        import_confirm = True if rule[2] is None else rule[2]
+                        self.agg_in(self.edge_locators.alarm_rules_locator,
+                                    {'import': rule[1], 'import_confirm': import_confirm})
+                    elif rule[0] in ('delete_bulk', 'add_to_label'):
+                        self.agg_in(self.edge_locators.alarm_rules_locator, {'check_all': False})
+                        check_group = [rule[1]] if isinstance(rule[1], str) else rule[1]
+                        for name in check_group:
+                            self.agg_in(self.edge_locators.alarm_rules_locator, {'table': [('check', name, True)]})
+                        if rule[0] == 'add_to_label':
+                            self.agg_in(self.edge_locators.alarm_add_to_label(rule[2]),
+                                        {'label_name': 'check', 'submit': True})
+                        else:
+                            try:
+                                delete_bulk_confirm = rule[2]
+                            except IndexError:
+                                delete_bulk_confirm = True
+                            self.agg_in(self.edge_locators.alarm_rules_locator,
+                                        {'delete_bulk': rule[1], 'delete_bulk_confirm': delete_bulk_confirm})
+                    else:
+                        self.agg_in(self.edge_locators.alarm_rules_locator, {rule[0]: rule[1]})
+            logging.info('device supervisor alarm rules: {} success'.format(kwargs.get('rules')))
+        if kwargs.get('realtime'):
+            self.access_menu('edge_computing.device_supervisor.alarm.realtime alarms')
+            self.agg_in(self.edge_locators.alarm_realtime_locator, kwargs.get('realtime'))
+        if kwargs.get('history'):
+            self.access_menu('edge_computing.device_supervisor.alarm.history alarms')
+            for history in kwargs.get('history'):
+                if history[0] in ('check', 'delete'):
+                    self.agg_in(self.edge_locators.alarm_history_locator, {'table': [history]})
                 else:
-                    logging.warning(f'the {email} user not exist')
-        else:
-            logging.warning(f'the {email} user not exist')
-
-    def assert_cellular_history(self, sn, state, delta_day=-1, data_interval=None):
-        """
+                    if history[0] == 'search':
+                        self.agg_in(self.edge_locators.alarm_history_locator, history[1].update({"search": True}))
+                    elif history[0] in ('delete_bulk',):
+                        self.agg_in(self.edge_locators.alarm_history_locator, {'check_all': False})
+                        check_group = [history[1]] if isinstance(history[1], str) else history[1]
+                        for name in check_group:
+                            self.agg_in(self.edge_locators.alarm_history_locator, {'table': [('check', name, True)]})
+                        try:
+                            delete_bulk_confirm = history[2]
+                        except IndexError:
+                            delete_bulk_confirm = True
+                        self.agg_in(self.edge_locators.alarm_history_locator,
+                                    {'delete_bulk': history[1], 'delete_bulk_confirm': delete_bulk_confirm})
+                    else:
+                        self.agg_in(self.edge_locators.alarm_history_locator, {history[0]: history[1]})
+            logging.info('device supervisor alarm history: {} success'.format(kwargs.get('history')))
 
-        :param sn:
-        :param state:
-        :param delta_day: 查询开始时间的起点， 默认晚一天时间
-        :param data_interval: 当查询的时间越长时，返回的数据会少，防止页面在渲染时卡顿，所以返回的数据间隔增大，可以对间隔做判断， 单位秒
-        :return:
+    @allure.step("断言Device Supervisor告警状态")
+    @loop_inspector('device_supervisor_alarm_status')
+    def assert_status(self, **kwargs):
         """
-        time.sleep(2)
-
-        def time_reduction(time_list, delta):
-            """
-            校验数据点时间差
-            :param time_list: list of timestamp
-            :param delta: int
-            :return:
-            """
-            tmp = []
-            for each in time_list:
-                each = time.strptime(each, "%Y-%m-%dT%H:%M:%SZ")
-                tmp.append(int(time.mktime(each)))
-            t0 = tmp[0]
-            for i in tmp[1:]:
-                assert abs(t0 - i) == delta
-                t0 = i
-
-        payload = {
-            "after": get_time_stamp(delta=delta_day, delta_type='d', time_format='%Y-%m-%dT16:00:00.000Z'),
-            "before": get_time_stamp(time_format='%Y-%m-%dT16:00:00.000Z')
-        }
-        resp = self.api.send_request(f'/api/v1/devices/{self.device_state([sn])[0].get("id")}/signal', 'get',
-                                     param=payload, code=200).json().get('result').get('series')
-        fields = resp[0]['fields']
-        cellular_state = []
-        if state:
-            for each_type in resp:
-                for data in each_type["data"]:
-                    temp = {"name": "signal", "tags": {"type": each_type["type"]}, "fields": {}}
-                    if data[1]:
-                        temp["timestamp"] = data[0]
-                        for i in range(1, len(data)):
-                            if data[i] != 0:
-                                if data[i]:
-                                    if i == 5:
-                                        temp["fields"]["level"] = data[i] - 1
-                                    temp["fields"][fields[i]] = data[i]
-                            elif data[i] == 0:
-                                temp["fields"][fields[i]] = 0
-                        temp["fields"].pop("strength")
-                        cellular_state.append(temp)
-                        assert temp in state, '查询结果不对'
-            assert len(cellular_state) == len(state), '查询结果不对'
-        if data_interval is not None:
-            cellular_type = []
-            for each_type in resp:
-                cellular_type.append(each_type['type'])
-                timestamp_ls = [i[0] for i in each_type['data']]
-                time_reduction(timestamp_ls, delta=data_interval)
-            assert len(cellular_type) == len(set(cellular_type)), '蜂窝历史返回数据不对'
-
-
-class InRequest:
-
-    def __init__(self, host: str, username: str, password: str, type_='device', protocol='https', port=443):
-        """支持设备，平台登录及操作API, 自动识别地址
-
-        :param host:  主机地址，如果是平台的就填写平台server，如果是设备就填写设备的地址
-        :param username:  用户名
-        :param password: 密码
-        :param type_: device|iot|ics|star|iscada|iwos|dn4  区分平台和设备
-        :param protocol: 协议，当前只支持http https
-        :param port: 端口
-        """
-        self.protocol = protocol
-        self.host = host
-        self.username = username
-        self.password = password
-        self.headers = {}
-        self.type_ = type_
-        self.port = port
-        self.__login()
 
-    def __url_pre(self, path: str):
-        """host+path
-
-        :param path:  请求路径
+        :param kwargs:
+            realtime:
+               str: 连续告警相关字段，需自己国际化， 这种是判断有
+               list: 连续告警相关字段，需自己国际化， 这种是判断有多个
+               dict: 当为字典时 key是连续告警相关字段， value是判断是否有告警，True是有告警，False是无告警
+                {'alarm_name': True or False}
         :return:
         """
-        if path.startswith('/'):
-            return self.protocol + '://' + self.host + ':' + str(self.port) + path
-        else:
-            return self.protocol + '://' + self.host + ':' + str(self.port) + '/' + path
 
-    def __login(self):
-        if self.type_ in ('iot', 'ics', 'iwos', 'dn4'):
-            self.headers = {"Content-Type": "application/x-www-form-urlencoded"}
-            param = {
-                'client_id': '17953450251798098136',
-                'client_secret': '08E9EC6793345759456CB8BAE52615F3',
-                'grant_type': 'password',
-                'type': 'account',
-                'autoLogin': 'true',
-                'password_type': 2,
-                'pwdType': 'pwd',
-                "username": self.username,
-                "password": file_hash(self.password)}
-            response = self.send_request('/oauth2/access_token', method='post', param=param).json()
-            self.headers = {'Authorization': 'Bearer ' + response['access_token']}
-        elif self.type_ in ('iscada', 'star'):
-            settings_url = '/api/v1/erlang/frontend/settings' if self.type_ == 'iscada' else '/api/v1/frontend/settings'
-            res_setting = self.send_request(settings_url, 'get', expect='result').json()
-            # erlang 登录地址不一样，需要重新指向
-            authority = res_setting['result']['authProvider']['authority']
-            protocol_re = self.protocol
-            host_re = self.host
-            self.protocol = authority.split('://')[0]
-            self.host = authority.split('://')[-1]
-            param = {
-                'client_id': res_setting['result']['authProvider']['clientId'],
-                'client_secret': res_setting['result']['authProvider']['clientSecret'],
-                'grant_type': 'password',
-                'scope': 'offline',
-                "username": self.username,
-                "password": self.password,
-                # "type": 'account'
-            }
-            response = self.send_request('/oauth2/token', method='post', param=param, params_type='form').json()
-            self.headers = {'Authorization': 'Bearer ' + response['access_token']}
-            self.protocol = protocol_re
-            self.host = host_re
-        elif self.type_ == 'device':
-            username_password = '%s:%s' % (self.username, self.password)
-            base_auth = base64.b64encode(username_password.encode()).decode()
-            self.headers = {'Authorization': 'Basic %s' % base_auth}
-            resp = self.send_request('v1/user/login', 'post').json()
-            self.headers['Authorization'] = 'Bearer ' + resp['results']['web_session']
-        logging.info(f'{self.username} login success')
-
-    def send_request(self, path, method, param=None, body=None, expect=None, file_path=None,
-                     params_type='json', header=None, code=200, auth=True):
-        """封装http请求，根据请求方式及参数类型自动判断使用哪些参数来发送请求
-
-        :param path: 请求路径
-        :param method: 请求方法
-        :param param: 请求中的参数,
-        :param body: post请求中的body，当消息体为json时使用
-        :param expect: 期望包含的结果
-        :param file_path: 文件路径，用于文件上传或者下载文件
-        :param params_type: 参数类型，用于post请求，参数值：form|json
-        :param header: 请求头 只支持字典
-        :param code: 验证返回code
-        :param auth: 是否认证， 默认需要的
-        :return:
-        """
-        header = dict_merge(self.headers, header) if auth else header
-        urllib3.disable_warnings()  # 去除https warnings提示
-        method = method.upper()
-        params_type = params_type.upper()
-        url = self.__url_pre(path)
-        if method == 'GET':
-            res = requests.get(url=url, params=param, headers=header, verify=False)
-            if file_path:
-                with open(file_path, 'w', encoding='UTF-8') as f:
-                    f.write(res.text)
-        elif method == 'POST':
-            if params_type == 'FORM':
-                if file_path:
-                    if self.type_ == 'device':
-                        files = {
-                            'file': (
-                                os.path.basename(file_path), open(file_path, 'rb'), 'application/octet-stream')}
-                        res = requests.post(url, params=param, files=files, headers=header, verify=False)
-                    else:
-                        with open(file_path, 'rb') as f:
-                            file_info = {"file": f}
-                            res = requests.post(url, data=param, files=file_info, headers=header, verify=False)
+        def _status(value_, type_):
+            if value_:
+                if type_ == 'realtime':
+                    self.access_menu('edge_computing.device_supervisor.alarm.realtime alarms')
+                    alarm = IgTable([], self.edge_locators.alarm_realtime_table)
                 else:
-                    res = requests.post(url=url, data=param, headers=header, verify=False)
-            elif params_type == 'JSON':
-                res = requests.post(url=url, params=param, json=body, headers=header, verify=False)
-            else:
-                res = requests.post(url=url, headers=header, verify=False)
-        elif method == 'DELETE':
-            if body:
-                if params_type == 'JSON':
-                    res = requests.delete(url, headers=header, json=body, verify=False)
+                    self.access_menu('edge_computing.device_supervisor.alarm.history alarms')
+                    alarm = IgTable([], self.edge_locators.alarm_history_table)
+                if isinstance(value_, str):
+                    realtime_expect = {value_: True}
+                elif isinstance(value_, list) or isinstance(value_, tuple):
+                    realtime_expect = {realtime: True for realtime in value_}
+                elif isinstance(value_, dict):
+                    realtime_expect = value_
                 else:
-                    res = requests.delete(url, headers=header, data=body, verify=False)
-            else:
-                res = requests.delete(url, params=param, headers=header, verify=False)
-        elif method == 'PUT':
-            if params_type == 'JSON':
-                res = requests.put(url, json=body, params=param, headers=header, verify=False)
+                    raise TypeError('realtime type error')
+                for key, value in realtime_expect.items():
+                    if value and not alarm.exist(key, locale={}):
+                        return False
+                    if not value and alarm.exist(key, locale={}):
+                        return False
+                else:
+                    return True
             else:
-                res = requests.put(url, data=param, headers=header, verify=False)
-        else:
-            logging.exception(f"requests method {method} not support")
-            raise ParameterValueError(f"requests method {method} not support")
-        # logging.debug(f'Requests Method:[{method}] Code: {res.status_code} URL: {url}, Param: {param}, Body: {body}')
-        if res.status_code != 401:
-            if self.type_ == 'device':
-                if res.status_code == 404:
-                    logging.exception(f"not support API login")
-                    raise Exception('not support API login')
-                if res.status_code == 200 and 'login' in path:
-                    if 'error' in res.json().keys():
-                        logging.exception(f"UsernameOrPasswordError")
-                        raise UsernameOrPasswordError
-            res.encoding = 'utf-8'  # 如返回内容有中文的需要编码正确
-            try:
-                logging.debug(f'Requests Response json is {res.json()}')
-            except Exception:
-                logging.warning(f'Requests Response json is None')
+                return True
+
+        if not _status(kwargs.get('realtime'), 'realtime'):
+            return False
+        if not _status(kwargs.get('history'), 'history'):
+            return False
         else:
-            # 当token过期时，统一重新登录后再次调API
-            self.__login()
-            res = self.send_request(path, method, param, body, expect, file_path, params_type, header, code)
-        if code:
-            assert res.status_code == code, res.text
-        if expect:
-            if isinstance(expect, list):
-                if len(expect) > 0:
-                    for i in expect:
-                        if isinstance(i, str) or isinstance(i, int):
-                            assert str(i) in res.text, f"Response text {res.text} Does not contain {i}"
-                        elif isinstance(i, dict):
-                            dict_in(res.json(), i)
-            elif isinstance(expect, dict):
-                dict_in(res.json(), expect)
-            elif isinstance(expect, str) or isinstance(expect, int):
-                assert str(expect) in res.text, f"Response text {res.text} Does not contain {expect}"
-            else:
-                logging.exception(f'expect param type error！')
-                raise ValueError('expect param type error！')
-        return res
+            return True
 
 
-if __name__ == "__main__":
-    from inhandtest.log import enable_log
+class ParameterSettings(BasePage, IgLocators):
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
+        IgLocators.__init__(self, page, locale)
 
-    enable_log(console_level='info')
-    # my.delete_org('test', None, )
+    @allure.step('配置Device Supervisor参数设置')
+    def config(self, **kwargs):
+        """
+
+        :param kwargs:
+               band_485: 300|1200|2400|4800|9600|19200|38400|57600|115200|230400
+               band_232: 300|1200|2400|4800|9600|19200|38400|57600|115200|230400
+               data_bits_485： 7|8
+               data_bits_232： 7|8
+               parity_485： none|odd|even
+               parity_232： none|odd|even
+               stop_bits_485: 1|2
+               stop_bits_232: 1|2
+               submit_serial: True or {'tip_message': 'submit_success'}
+               log_level: info|debug|warning|error
+               historical_alarm_max: int
+               cache_data_storage_method: usb|sd_card|gateway
+               cache_data_storage_path: str
+               cache_data_max: int
+               communication_storage_method: usb|sd_card|gateway
+               communication_storage_path: str
+               communication_max: int
+               submit_default_parameter: True or {'tip_message': 'submit_success'}
+               import: str , 上传文件路径
+               import_confirm: True or {'tip_message': 'submit_success'} 可以不传
+               export: str or dict, 导出文件路径
+               parameter: [(action, value)]
+                    [('add', kwargs)]
+                    kwargs:
+                        key: str
+                        value: str
+                    [('edit', 'old_name', kwargs)]  kwargs 同add
+                    [('delete', name)]  # 删除
+        :return:
+        """
+        self.access_menu('edge_computing.device_supervisor.parameter settings')
+        if kwargs.get('import') and kwargs.get('import_confirm') is None:
+            kwargs['import_confirm'] = {'wait_for_time': 3 * 1000}
+        self.agg_in(self.edge_locators.parameter_locator, kwargs)
+
+
+class DeviceSupervisor:
+
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        self.measure = MeasureMonitor(host, username, password, protocol, port, model, language, page, locale)
+        self.alarm = Alarm(host, username, password, protocol, port, model, language, page, locale)
+        self.cloud = Cloud(host, username, password, protocol, port, model, language, page, locale)
+        self.parameter = ParameterSettings(host, username, password, protocol, port, model, language, page, locale)
+
+    @allure.step("数据运算计算")
+    def data_calculation(self, transform_type, input_value, decimal=2, data_high_limit=0, data_lower_limit=0,
+                         high_limit_of_proportion=0, lower_limit_of_proportion=0, magnification=0, offset=0, pt=0, ct=0,
+                         start_bit=0, end_bit=0, reverse=False) -> int or float:
+        """数据运算计算测点值
+
+        :param transform_type: 1:比例换算 | 2:偏移及缩放 | 3:位截取 | 4:PT/CT
+        :param input_value: 输入值
+        :param decimal: 最后保留小数位
+        :param data_high_limit: 数据上限
+        :param data_lower_limit: 数据下限
+        :param high_limit_of_proportion: 比例上限
+        :param lower_limit_of_proportion: 比例下限
+        :param magnification: 倍率
+        :param offset: 偏移量
+        :param pt: PT
+        :param ct: CT
+        :param start_bit: 位截取起始位
+        :param end_bit: 位截取截止位
+        :param reverse: True | False
+        :return:
+        """
+        operator_value = operation_value = 0.0
+        if transform_type == 1:
+            if reverse:
+                operation_value = (input_value - lower_limit_of_proportion) * (data_high_limit - data_lower_limit) / \
+                                  (high_limit_of_proportion - lower_limit_of_proportion) + data_lower_limit
+            else:
+                operation_value = (high_limit_of_proportion - lower_limit_of_proportion) / \
+                                  (data_high_limit - data_lower_limit) * (input_value - data_lower_limit) + \
+                                  lower_limit_of_proportion
+        elif transform_type == 2:
+            if reverse:
+                operation_value = (input_value - offset) / magnification
+            else:
+                operation_value = input_value * magnification + offset
+        elif transform_type == 3:
+            if input_value >= 0:
+                bin_value = bin(input_value)
+            else:
+                bin_value = bin((1 << 64) + input_value)
+            operation_value = int(bin_value[::-1][start_bit:end_bit][::-1], 2)
+        elif transform_type == 4:
+            if reverse:
+                operator_value = (input_value / ct / pt - offset) / magnification
+            else:
+                operation_value = (input_value * magnification + offset) * pt * ct
+        else:
+            raise Exception('NonsupportTransformType')
+        if reverse:
+            return int(operator_value)
+        else:
+            return round(operation_value, decimal)
+
+    @allure.step("生成数据运算配置")
+    def generate_config_parameter(self, transform_type: int, datatype: str):
+        """
+
+        :param transform_type: 1:比例换算 | 2:偏移及缩放 | 3:位截取 | 4:PT/CT
+        :param datatype: 数据类型 BYTE| SINT| BCD| INT| WORD| DINT| DWORD| LONG| ULONG| FLOAT| DOUBLE
+        :return:
+        """
+        datatype_list = {'SINT': (-(2 ** 8 // 2), (2 ** 8 - 1) // 2), 'BYTE': (0, 2 ** 8 - 1), 'BCD': (0, 9999),
+                         'INT': (-(2 ** 16 // 2), (2 ** 16 - 1) // 2), 'WORD': (0, 2 ** 16 - 1),
+                         'DINT': (-(2 ** 32 // 2), (2 ** 32 - 1) // 2),
+                         'DWORD': (0, 2 ** 32 - 1), 'LONG': (-(2 ** 64 // 2), (2 ** 64 - 1) // 2),
+                         'ULONG': (0, 2 ** 64 - 1)}
+        digit_list = {'SINT': (0, 7), 'BYTE': (0, 7), 'BCD': (0, 15), 'INT': (0, 15), 'WORD': (0, 15), 'DINT': (0, 31),
+                      'DWORD': (0, 31), 'LONG': (0, 63), 'ULONG': (0, 63)}
+        type_ = datatype.upper()
+        if transform_type == 1:
+            if type_ in ['FLOAT', 'DOUBLE']:
+                value_range = sorted([random.uniform(-9999999999, 9999999999) for i in range(2)])
+            else:
+                value_range = sorted(list(np.random.randint(datatype_list[type_][0], datatype_list[type_][1], 2)))
+            print(value_range)
+            scale_range = sorted([random.uniform(-9999999999, 9999999999) for i in range(2)])
+            print(scale_range)
+            gain_value = value_range + scale_range
+            return gain_value
+        elif transform_type == 2:
+            zoom_range = [random.uniform(-9999999999, 9999999999) for i in range(2)]
+            return zoom_range
+        elif transform_type == 3:
+            bit_range = sorted([random.randint(digit_list[type_][0], digit_list[type_][1]) for i in range(2)])
+            return bit_range
+        else:
+            pt_range = [random.uniform(-9999999999, 9999999999) for i in range(4)]
+            return pt_range
+
+
+class EdgeComputing:
+
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        self.python_edge: PythonEdgeComputing = PythonEdgeComputing(host, username, password, protocol, port,
+                                                                    model, language, page, locale)
+        self.docker_manager: DockerManager = DockerManager(host, username, password, protocol, port, model, language,
+                                                           page, locale)
+        self.device_supervisor: DeviceSupervisor = DeviceSupervisor(host, username, password, protocol, port, model,
+                                                                    language, page, locale)
```

### Comparing `inhandtest-0.0.59/inhandtest/inserial.py` & `inhandtest-0.0.60/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/insocket.py` & `inhandtest-0.0.60/inhandtest/insocket.py`

 * *Files 8% similar despite different names*

```diff
@@ -159,60 +159,76 @@
             else:
                 logging.info(f'tcp client {client} recv content {recv_content} success')
         else:
             logging.exception(f'tcp client {client} not connected')
             raise AssertionError(f'tcp client {client} not connected')
 
 
-def udp_server_data(host, port, recv_content: str or list = None, connect_time=10, send_msg_to_client: dict = None):
+def udp_server_data(host, port, recv_content: str or list = None, connect_time=10, send_msg_to_client: dict = None,
+                    function=None, **kwargs):
     """ 开启udp_server, 并且接收数据，对数据做验证, udp 校验数据时未区分客户端，所以保证接入时只有一个客户端
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
 
     :param host:  server地址
     :param port:  server端口
     :param recv_content: 判断recv_content 在接收到的内容里面 也可以不做校验
     :param connect_time:  服务器和客户端建立连接后，需要连接的时间
     :param send_msg_to_client: 开启udp server后， 向客户端发送的内容{($host, $port): $msg}
                                总体内容为字典， key值为元组类型， 总共长度为2位，第一位是客户端的地址， 第二位是端口
                                字典的value为需要给对应客户端发送的内容，可以是str 或list，
                                如需要给客户端192.168.3.2:6541 发送两条内容 'hello', 'word', 可以这样写
                                {('192.168.3.2', 6541): ['hello', 'word']}
-                                确保对端服务和端口正常开启，不然要出问题
+                               端口可以为None, 但是地址必须要有， 也就是说，如果需要给客户端
+                               确保对端服务和端口正常开启，不然要出问题
+    :param function: 当客户端 连接上后做的操作
     :return: AssertionError or None
     """
+    own_port_client = None
+    not_port_client = None
+    if send_msg_to_client is not None:
+        own_port_client = {key: value for key, value in send_msg_to_client.items() if key[1] is not None}
+        not_port_client = {key[0]: value for key, value in send_msg_to_client.items() if key[1] is None}
 
     def server_send_msg_to_client(server, msg: dict):
         if msg:
             for key, value in msg.items():
-                msg = [value] if isinstance(value, str) else [value_ for value_ in value]
+                msg = [value] if isinstance(value, str) else value
                 for msg_ in msg:
                     server.sendto(msg_.encode('utf-8'), key)
                     logging.info(f'udp server {host}: {port} send msg {msg_} to client {key}')
 
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:  # 使用with， 不用担心没有关闭server
         s.bind((host, port))  # 绑定服务器IP地址和端口号
         logging.debug(f'udp server {host}:{port} enable')
-        threading.Thread(target=server_send_msg_to_client, args=(s, send_msg_to_client)).start()
+        send_msg_thread = threading.Thread(target=server_send_msg_to_client, args=(s, own_port_client))
+        send_msg_thread.start()
+        if function is not None:
+            threading.Thread(target=function, kwargs=kwargs).start()
         datas = b''
         now_time = int(time.time())
-        while int(time.time()) <= now_time + connect_time:
-            # 接收客户端数据
-            data, addr = s.recvfrom(5024)
-            logging.debug(f'udp server {host}:{port} recv data from {addr}: {data}')
-            datas = datas + data
-            if recv_content is not None:
+        if not_port_client or recv_content:  # 始终要去接收客户端
+            send_client = {}
+            while int(time.time()) <= now_time + connect_time:
+                # 接收客户端数据
+                data, addr = s.recvfrom(5024)
+                logging.debug(f'udp server {host}:{port} recv data from {addr}: {data}')
+                if addr not in send_client.keys() and addr[0] in not_port_client.keys():
+                    msg = [not_port_client.get(addr[0])] if isinstance(not_port_client.get(addr[0]),
+                                                                       str) else not_port_client.get(addr[0])
+                    for msg_ in msg:
+                        s.sendto(msg_.encode('utf-8'), addr)
+                        logging.info(f'udp server {host}: {port} send msg {msg_} to client {addr}')
+                datas = datas + data
+            if recv_content:
                 contents = [recv_content.encode()] if isinstance(recv_content, str) else [c_.encode() for c_ in
                                                                                           recv_content]
                 # 校验数据内容
-                if not list(filter(lambda x: x not in datas, contents)):
-                    break
-        else:
-            if recv_content is not None:
-                logging.exception(f'recv all data is {datas}')
-                raise AssertionError('recv data error')
+                if list(filter(lambda x: x not in datas, contents)):
+                    logging.exception(f'recv all data is {datas}')
+                    raise AssertionError('recv data error')
 
 
 def udp_client_data(server: tuple, client: tuple = None, recv_content: str or list = None, connect_time=10,
                     send_msg_to_server: str or list = None):
     """ 开启udp_client, 并且接收数据，对数据做验证
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
 
@@ -252,8 +268,9 @@
             if recv_content is not None:
                 logging.exception(f'recv all data is {datas}')
                 raise AssertionError('recv data error')
 
 
 if __name__ == '__main__':
     import sys
+
     pass
```

### Comparing `inhandtest-0.0.59/inhandtest/inssh.py` & `inhandtest-0.0.60/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/ip.py` & `inhandtest-0.0.60/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/log.py` & `inhandtest-0.0.60/inhandtest/log.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/mail.py` & `inhandtest-0.0.60/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,16 @@
 
     @property
     def add_controller_all(self) -> list:
         return [('template_name',
                  {'locator': self.pop_up.locator('.ant-select.ant-select-enabled').first, 'type': 'select'}),
                 ('name', {'locator': self.page.locator('#name'), 'type': 'text'}),
                 ('protocol', {'locator': self.pop_up.locator('.ant-cascader-picker'), 'type': 'select_multi',
-                              'param': {'modbus.modbus tcp': 'Modbus.Modbus Tcp', 'Siemens PLC': self.locale.siemens_plc,
+                              'param': {'modbus.modbus tcp': 'Modbus.Modbus Tcp',
+                                        'Siemens PLC': self.locale.siemens_plc,
                                         'modbus.modbus rtu': 'Modbus.Modbus Rtu'}}),
                 # opc ua
                 ('servers_url', {'locator': self.pop_up.locator('#endpoint'), 'type': 'text'}),
 
                 # modbus tcp or rtu
                 ('ip_address', {'locator': self.page.locator('#point\.ip'), 'type': 'text'}),
                 ('port', {'locator': self.page.locator('#point\.port'), 'type': 'text'}),
@@ -256,19 +257,22 @@
                 ('onchange_uploading_interval',
                  {'locator': self.page.locator('#onchangePeriod'), 'type': 'text',
                   'relation': [('advanced_settings', 'expand'), ('periodically_upload_onchange_data', 'enable')]}),
                 ('communication_interval_time',
                  {'locator': self.page.locator('#args\.communicationInterval'), 'type': 'text',
                   'relation': [('advanced_settings', 'expand')]}),
                 ('coil_outputs_write_function_code',
-                 {'locator': self.page.locator('#args\.writeCoilFunction'), 'type': 'select'}),
+                 {'locator': self.page.locator('#args\.writeCoilFunction'), 'type': 'select',
+                  'relation': [('advanced_settings', 'expand')]}),
                 ('holding_register_write_function_code',
-                 {'locator': self.page.locator('#args\.writeRegisterFunction'), 'type': 'select'}),
+                 {'locator': self.page.locator('#args\.writeRegisterFunction'), 'type': 'select',
+                  'relation': [('advanced_settings', 'expand')]}),
                 ('store_communication_message',
-                 {'locator': self.pop_up.locator('#enableDebug'), 'type': 'switch_button'}),
+                 {'locator': self.pop_up.locator('#enableDebug'), 'type': 'switch_button',
+                  'relation': [('advanced_settings', 'expand')]}),
                 ('submit', {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'),
                             'type': 'button'}),
                 ('text_messages', {'type': 'text_messages'}),
                 ('tip_messages', {'type': 'tip_messages'}),
                 ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
                             'type': 'button'}),
                 ]
@@ -429,16 +433,16 @@
                 ('mode', {'locator': self.pop_up.locator('#uploadType'), 'type': 'select',
                           'param': {'periodic': 'Periodic', 'onchange': 'Onchange', 'never': 'Never'}}),
                 ('unit', {'locator': self.pop_up.locator('#unit'), 'type': 'text'}),
                 ('description', {'locator': self.pop_up.locator('#desc'), 'type': 'text'}),
                 ('group', {'locator': self.pop_up.locator('#group'), 'type': 'select'}),
                 ('storage_lwtsdb', {'locator': self.pop_up.locator('#storageLwTSDB'), 'type': 'switch_button'}),
                 ('polling_interval', {'locator': self.pop_up.locator('#pollCycle'), 'type': 'select',
-                                      'relation': {'polling_interval': self.locale.polling_interval,
-                                                   'polling_interval_2': self.locale.polling_interval_2}}),
+                                      'param': {'polling_interval': self.locale.polling_interval,
+                                                'polling_interval_2': self.locale.polling_interval_2}}),
                 ('numerical_mapping', {'locator': self.pop_up.locator('#bitMap'), 'type': 'switch_button'}),
                 ('data_calculation', {'locator': self.pop_up.locator('#transformType'), 'type': 'select',
                                       'param': {'no': self.locale.get('no'),
                                                 'ratio conversion': self.locale.get('ratio_conversion'),
                                                 'offset and zoom': self.locale.get('offset_and_zoom'),
                                                 'bit truncation': self.locale.get('bit_truncation'),
                                                 'pt/ct': self.locale.get('pt/ct'),
```

### Comparing `inhandtest-0.0.59/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.60/inhandtest/pages/ingateway/ingateway.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.60/inhandtest/pages/ingateway/locale.yml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.60/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.60/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.60/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.60/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.60/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.60/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.60/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/pytest_email.html` & `inhandtest-0.0.60/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.59/inhandtest/telnet.py` & `inhandtest-0.0.60/inhandtest/telnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,27 +435,28 @@
                 if expect:
                     if 'expect' in key_replace_type:
                         expect = replace_str(expect, key_replace)
                     if 'expect' in interface_replace_type:
                         expect = replace_str(expect, self.interface_replace)
                     logging.debug(f'start assert cli expect {expect}')
                     if isinstance(expect, str):
-                        if not len(re.findall(expect, result)):
+                        if not ((expect in result) or len(re.findall(expect, result))):
                             check_ = False
                     elif isinstance(expect, list):
-                        if [expect_ for expect_ in expect if not len(re.findall(expect_, result))]:
+                        if [expect_ for expect_ in expect if
+                                not ((expect_ in result) or len(re.findall(expect_, result)))]:
                             check_ = False
                     elif isinstance(expect, dict):
                         for k, v in expect.items():
                             if v:
-                                if not len(re.findall(k, result)):
+                                if not ((k in result) or len(re.findall(k, result))):
                                     check_ = False
                                     break
                             else:
-                                if len(re.findall(k, result)):
+                                if (k in result) or len(re.findall(k, result)):
                                     check_ = False
                                     break
                     else:
                         logging.exception(f'parameter expect type error, expect {expect}')
                         raise Exception('parameter expect is error')
                 if check_:
                     break
@@ -531,15 +532,15 @@
             elif isinstance(expect, list) or isinstance(expect, tuple):
                 expect_ = expect
             else:
                 logging.exception('parameter expect type error')
                 raise Exception('parameter expect type error')
             if expect_:
                 try:
-                    _result = self.send_cli(command, expect_, timeout=timeout, type_='super', key_replace=key_replace,
+                    _result = self.send_cli(command, [expect_], timeout=timeout, type_='super', key_replace=key_replace,
                                             key_replace_type='cli')
                     logging.debug('find the exception in tcpdump result.')
                     self.tn.write(("\003" + "\r").encode("cp936"))
                     if not_expect_:
                         if [not_expect for not_expect in not_expect_ if not_expect in _result]:
                             result = False
                 except:
@@ -670,11 +671,10 @@
         """
         self.tn.close()
         logging.info("Telnet 【%s:%s】 close connect session" % (self.host, self.port))
 
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
-
-    enable_log('./log.log', 'DEBUG')
-    a = Telnet('IG902', '10.5.24.96', 'inhand', '64391099@inhand')
-    a.assert_cli('ifconfig', 'fe80::67f:eff:fe01:92be/64')
+    # enable_log('./log.log', 'DEBUG')
+    # a = Telnet('IG902', '10.5.24.96', 'inhand', '64391099@inhand')
+    # a.assert_cli('ifconfig', 'fe80::67f:eff:fe01:92be/64')
```

### Comparing `inhandtest-0.0.59/inhandtest/tools.py` & `inhandtest-0.0.60/inhandtest/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -620,14 +620,60 @@
         except:
             pass
     else:
         logging.exception(f'all installed software is {all_installed}')
         raise ResourceNotFoundError(f'Not found the software {name}')
 
 
+@loop_inspector('PC Ping',)
+def pc_ping(host_or_ip: str or list or tuple = 'www.baidu.com', number: int = 4, src=None,
+            lost_packets=False, assert_result=True, timeout=120, interval=10) -> bool:
+    """ 验证在PC机上ping某个地址是否丢包， 仅判断丢包
+
+    :param lost_packets:
+    :param src: 验证的源IP地址 '192.168.2.100'
+    :param host_or_ip: 验证的目的IP地址, 可使用元组或列表接收多个地址
+    :param number: 包数量
+    :param lost_packets: True|False 如果为True判断会丢包，如果为False判断不丢包
+    :param assert_result: True|False 是否对 lost_packets 的结果做判断
+    :param timeout: 超时时间
+    :param interval: 间隔时间
+    :return:
+    """
+    tag_result = True
+    if host_or_ip:
+        host_or_ip = [host_or_ip] if isinstance(host_or_ip, str) else host_or_ip
+        for host in host_or_ip:
+            command = f'ping {host} -n {number}' if src is None else f'ping -S {src} {host} -n {number}'
+            logging.debug(command)
+            if assert_result:
+                result = os.popen(command).read()
+                logging.debug(result)
+                if lost_packets:  # 判断需要丢包
+                    send = re.findall(r'已发送 = (.*?)，', result, re.S)[0]
+                    accept = re.findall(r'已接收 = (.*?)，', result, re.S)[0]
+                    if send == accept:
+                        if '无法访问' not in result:
+                            logging.info(f'PC {src} ping {host} does not loss packet')
+                            tag_result = False
+                else:  # 判断不丢包
+                    if '丢失 = 0' not in result:
+                        logging.info(f'PC {src} ping {host} loss packet')
+                        tag_result = False
+                    else:
+                        if '无法访问' in result:
+                            logging.info(f'PC {src} ping {host} loss packet')
+                            tag_result = False
+            else:
+                os.popen(command)
+            if not tag_result:
+                break
+    return tag_result
+
+
 class DotDict(dict):
     """使用点号深度获取字典key的值
 
     """
 
     def __getattr__(self, key):
         try:
```

### Comparing `inhandtest-0.0.59/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.60/inhandtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.59
+Version: 0.0.60
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.59/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.60/inhandtest.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 setup.py
 inhandtest/__init__.py
 inhandtest/exception.py
 inhandtest/file.py
 inhandtest/inmodbus.py
 inhandtest/inmongodb.py
 inhandtest/inmqtt.py
-inhandtest/inrequest.py
 inhandtest/inserial.py
 inhandtest/insocket.py
 inhandtest/inssh.py
 inhandtest/ip.py
 inhandtest/log.py
 inhandtest/mail.py
 inhandtest/notice_email.html
@@ -26,14 +25,22 @@
 inhandtest.egg-info/top_level.txt
 inhandtest/base_page/__init__.py
 inhandtest/base_page/_ig_contents_locators.py
 inhandtest/base_page/_ir3XX_contents_locators.py
 inhandtest/base_page/_vg710_contents_locators.py
 inhandtest/base_page/base_page.py
 inhandtest/base_page/table_tr.py
+inhandtest/inrequest/__init__.py
+inhandtest/inrequest/console.py
+inhandtest/inrequest/dm.py
+inhandtest/inrequest/dn.py
+inhandtest/inrequest/er_device.py
+inhandtest/inrequest/ics.py
+inhandtest/inrequest/inrequest.py
+inhandtest/inrequest/nezha.py
 inhandtest/pages/__init__.py
 inhandtest/pages/ingateway/__init__.py
 inhandtest/pages/ingateway/ingateway.py
 inhandtest/pages/ingateway/locale.yml
 inhandtest/pages/ingateway/locators.py
 inhandtest/pages/ingateway/edge_computing/__init__.py
 inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
```

### Comparing `inhandtest-0.0.59/setup.py` & `inhandtest-0.0.60/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.59',
+    version='0.0.60',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

