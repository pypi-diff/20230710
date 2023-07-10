# Comparing `tmp/testbench2robotframework-0.5.2.tar.gz` & `tmp/testbench2robotframework-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\testbench2robotframework-0.5.2.tar", last modified: Sun Apr  2 19:04:47 2023, max compression
+gzip compressed data, was "testbench2robotframework-0.6.0.tar", last modified: Mon Jul 10 17:12:25 2023, max compression
```

## Comparing `testbench2robotframework-0.5.2.tar` & `testbench2robotframework-0.6.0.tar`

### file list

```diff
@@ -1,81 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 19:04:47.061045 testbench2robotframework-0.5.2/
--rwxrwxrwx   0        0        0      133 2023-02-22 15:56:30.000000 testbench2robotframework-0.5.2/CreatePiPWheel.bat
--rw-rw-rw-   0        0        0      139 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/CreatePiPWheel.sh
--rw-rw-rw-   0        0        0     2614 2023-02-24 15:19:12.000000 testbench2robotframework-0.5.2/DEVELOPMENT.md
--rw-rw-rw-   0        0        0    11558 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/LICENSE
--rw-rw-rw-   0        0        0      288 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0    17951 2023-04-02 19:04:47.063029 testbench2robotframework-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    15210 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/README.md
--rw-rw-rw-   0        0        0     1252 2023-03-20 07:05:49.000000 testbench2robotframework-0.5.2/config.json
-drwxrwxrwx   0        0        0        0 2023-04-02 19:04:46.815220 testbench2robotframework-0.5.2/images/
--rw-rw-rw-   0        0        0     5625 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/images/LibrarySubdivision.PNG
--rw-rw-rw-   0        0        0      167 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/images/Unbenannt.PNG
--rw-rw-rw-   0        0        0    29769 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/images/generated.png
--rw-rw-rw-   0        0        0     5625 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/images/libraries.PNG
--rw-rw-rw-   0        0        0     5627 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/images/resources.PNG
--rw-rw-rw-   0        0        0     6384 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/images/rfLibraryRootsTestBench.PNG
--rw-rw-rw-   0        0        0     5407 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/images/testbench_rfLibraryRegex.PNG
--rw-rw-rw-   0        0        0     4944 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/images/testbench_rfResourceRegex.PNG
--rw-rw-rw-   0        0        0    13816 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/images/testthemen.PNG
--rw-rw-rw-   0        0        0     1676 2023-02-24 10:19:19.000000 testbench2robotframework-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0     1705 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/requirements.txt
--rw-rw-rw-   0        0        0      969 2023-04-02 19:04:47.067029 testbench2robotframework-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 19:04:46.881567 testbench2robotframework-0.5.2/testbench2robotframework/
--rw-rw-rw-   0        0        0      695 2023-04-01 09:06:43.000000 testbench2robotframework-0.5.2/testbench2robotframework/__init__.py
--rw-rw-rw-   0        0        0     1710 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/testbench2robotframework/__main__.py
--rw-rw-rw-   0        0        0     6071 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/testbench2robotframework/config.py
--rw-rw-rw-   0        0        0     5352 2023-02-24 10:19:19.000000 testbench2robotframework-0.5.2/testbench2robotframework/json_reader.py
--rw-rw-rw-   0        0        0     1167 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/testbench2robotframework/json_writer.py
--rw-rw-rw-   0        0        0      903 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/testbench2robotframework/log.py
--rw-rw-rw-   0        0        0    24382 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/testbench2robotframework/model.py
--rw-rw-rw-   0        0        0    29331 2023-04-01 09:06:43.000000 testbench2robotframework-0.5.2/testbench2robotframework/result_writer.py
--rw-rw-rw-   0        0        0      954 2023-02-21 09:15:38.000000 testbench2robotframework-0.5.2/testbench2robotframework/robotframework2testbench.py
--rw-rw-rw-   0        0        0    29008 2023-04-01 13:41:54.000000 testbench2robotframework-0.5.2/testbench2robotframework/testbench2rf.py
--rw-rw-rw-   0        0        0     1196 2023-02-21 12:18:27.000000 testbench2robotframework-0.5.2/testbench2robotframework/testbench2robotframework.py
--rw-rw-rw-   0        0        0     1858 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/testbench2robotframework/testsuite_write.py
--rw-rw-rw-   0        0        0     7121 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/testbench2robotframework/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-02 19:04:46.914694 testbench2robotframework-0.5.2/testbench2robotframework.egg-info/
--rw-rw-rw-   0        0        0    17951 2023-04-02 19:04:46.000000 testbench2robotframework-0.5.2/testbench2robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2023-04-02 19:04:46.000000 testbench2robotframework-0.5.2/testbench2robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 19:04:46.000000 testbench2robotframework-0.5.2/testbench2robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-04-02 19:04:46.000000 testbench2robotframework-0.5.2/testbench2robotframework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-18 16:06:06.000000 testbench2robotframework-0.5.2/testbench2robotframework.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      120 2023-04-02 19:04:46.000000 testbench2robotframework-0.5.2/testbench2robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-02 19:04:46.000000 testbench2robotframework-0.5.2/testbench2robotframework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-02 19:04:46.926748 testbench2robotframework-0.5.2/tests/
-drwxrwxrwx   0        0        0        0 2023-04-02 19:04:46.682128 testbench2robotframework-0.5.2/tests/test_data/
-drwxrwxrwx   0        0        0        0 2023-04-02 19:04:46.936200 testbench2robotframework-0.5.2/tests/test_data/configurations/
--rw-rw-rw-   0        0        0     1196 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/tests/test_data/configurations/invalid_config.json
--rw-rw-rw-   0        0        0     1173 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/tests/test_data/configurations/valid_config.json
--rw-rw-rw-   0        0        0      236 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/tests/test_missing_files.py
--rw-rw-rw-   0        0        0      426 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/tests/test_robot_files_should_not_contain_invalid_characters.py
-drwxrwxrwx   0        0        0        0 2023-04-02 19:04:46.942221 testbench2robotframework-0.5.2/tests/test_setup/
-drwxrwxrwx   0        0        0        0 2023-04-02 19:04:46.948206 testbench2robotframework-0.5.2/tests/test_setup/test_data/
--rw-rw-rw-   0        0        0      642 2023-02-27 12:42:27.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/config.json
-drwxrwxrwx   0        0        0        0 2023-04-02 19:04:47.056674 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/
--rw-rw-rw-   0        0        0     6538 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/TestThemeTree.json
--rw-rw-rw-   0        0        0    23984 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2184-PC-21637.json
--rw-rw-rw-   0        0        0     1038 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2184.json
--rw-rw-rw-   0        0        0    24699 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2185-PC-21639.json
--rw-rw-rw-   0        0        0     1041 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2185.json
--rw-rw-rw-   0        0        0    24918 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2231-PC-21643.json
--rw-rw-rw-   0        0        0     1210 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2231.json
--rw-rw-rw-   0        0        0    24754 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2232-PC-21645.json
--rw-rw-rw-   0        0        0     1044 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2232.json
--rw-rw-rw-   0        0        0     8682 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2233-PC-21647.json
--rw-rw-rw-   0        0        0     8677 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2233-PC-21649.json
--rw-rw-rw-   0        0        0     1439 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2233.json
--rw-rw-rw-   0        0        0    14003 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2241-PC-21667.json
--rw-rw-rw-   0        0        0    13993 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2241-PC-21668.json
--rw-rw-rw-   0        0        0     1459 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2241.json
--rw-rw-rw-   0        0        0    12223 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2242-PC-21671.json
--rw-rw-rw-   0        0        0     1052 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2242.json
--rw-rw-rw-   0        0        0     2318 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2243-PC-21673.json
--rw-rw-rw-   0        0        0     1042 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2243.json
--rw-rw-rw-   0        0        0     3155 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2244-PC-21675.json
--rw-rw-rw-   0        0        0     1056 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2244.json
--rw-rw-rw-   0        0        0     4795 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2261-PC-21683.json
--rw-rw-rw-   0        0        0     1086 2023-02-27 14:12:05.000000 testbench2robotframework-0.5.2/tests/test_setup/test_data/json-report/itba-TC-2261.json
--rw-rw-rw-   0        0        0     2337 2023-02-27 16:41:38.000000 testbench2robotframework-0.5.2/tests/test_setup/test_setup_name.py
--rw-rw-rw-   0        0        0      957 2023-02-10 14:36:22.000000 testbench2robotframework-0.5.2/tests/test_zip_file_generation.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.598090 testbench2robotframework-0.6.0/
+-rwxr-xr-x   0 rener      (502) wheel        (0)      133 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/CreatePiPWheel.bat
+-rwxr-xr-x   0 rener      (502) wheel        (0)      133 2023-02-02 12:59:06.000000 testbench2robotframework-0.6.0/CreatePiPWheel.sh
+-rw-r--r--   0 rener      (502) wheel        (0)     2511 2023-07-10 10:03:03.000000 testbench2robotframework-0.6.0/DEVELOPMENT.md
+-rw-r--r--   0 rener      (502) wheel        (0)    11357 2023-02-02 13:01:04.000000 testbench2robotframework-0.6.0/LICENSE
+-rw-r--r--   0 rener      (502) wheel        (0)      275 2022-11-28 14:39:21.000000 testbench2robotframework-0.6.0/MANIFEST.in
+-rw-r--r--   0 rener      (502) wheel        (0)    15345 2023-07-10 17:12:25.598207 testbench2robotframework-0.6.0/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)    14921 2023-02-02 12:59:35.000000 testbench2robotframework-0.6.0/README.md
+-rw-r--r--   0 rener      (502) wheel        (0)     1028 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/config.json
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.591794 testbench2robotframework-0.6.0/images/
+-rw-r--r--   0 rener      (502) wheel        (0)     5625 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/LibrarySubdivision.PNG
+-rw-r--r--   0 rener      (502) wheel        (0)      167 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/Unbenannt.PNG
+-rw-r--r--   0 rener      (502) wheel        (0)    29769 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/generated.png
+-rw-r--r--   0 rener      (502) wheel        (0)     5625 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/libraries.PNG
+-rw-r--r--   0 rener      (502) wheel        (0)     5627 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/resources.PNG
+-rw-r--r--   0 rener      (502) wheel        (0)     6384 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/rfLibraryRootsTestBench.PNG
+-rw-r--r--   0 rener      (502) wheel        (0)     5407 2022-11-03 23:53:27.000000 testbench2robotframework-0.6.0/images/testbench_rfLibraryRegex.PNG
+-rw-r--r--   0 rener      (502) wheel        (0)     4944 2022-11-03 23:53:27.000000 testbench2robotframework-0.6.0/images/testbench_rfResourceRegex.PNG
+-rw-r--r--   0 rener      (502) wheel        (0)    13816 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/testthemen.PNG
+-rw-r--r--   0 rener      (502) wheel        (0)     2392 2023-07-10 17:07:51.000000 testbench2robotframework-0.6.0/pyproject.toml
+-rw-r--r--   0 rener      (502) wheel        (0)     1623 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/requirements.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      923 2023-07-10 17:12:25.598585 testbench2robotframework-0.6.0/setup.cfg
+-rw-r--r--   0 rener      (502) wheel        (0)       69 2022-10-26 13:43:50.000000 testbench2robotframework-0.6.0/setup.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.595711 testbench2robotframework-0.6.0/testbench2robotframework/
+-rw-r--r--   0 rener      (502) wheel        (0)      678 2023-07-10 15:51:18.000000 testbench2robotframework-0.6.0/testbench2robotframework/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1679 2023-07-10 13:09:41.000000 testbench2robotframework-0.6.0/testbench2robotframework/__main__.py
+-rw-r--r--   0 rener      (502) wheel        (0)     5888 2023-02-03 13:47:35.000000 testbench2robotframework-0.6.0/testbench2robotframework/config.py
+-rw-r--r--   0 rener      (502) wheel        (0)     5226 2023-07-10 16:55:23.000000 testbench2robotframework-0.6.0/testbench2robotframework/json_reader.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1144 2023-07-10 13:24:22.000000 testbench2robotframework-0.6.0/testbench2robotframework/json_writer.py
+-rw-r--r--   0 rener      (502) wheel        (0)      878 2023-02-03 13:47:35.000000 testbench2robotframework-0.6.0/testbench2robotframework/log.py
+-rw-r--r--   0 rener      (502) wheel        (0)    23595 2023-07-10 10:40:18.000000 testbench2robotframework-0.6.0/testbench2robotframework/model.py
+-rw-r--r--   0 rener      (502) wheel        (0)    28537 2023-07-10 15:28:36.000000 testbench2robotframework-0.6.0/testbench2robotframework/result_writer.py
+-rw-r--r--   0 rener      (502) wheel        (0)      968 2023-07-10 14:57:23.000000 testbench2robotframework-0.6.0/testbench2robotframework/robotframework2testbench.py
+-rw-r--r--   0 rener      (502) wheel        (0)    28269 2023-07-10 17:10:29.000000 testbench2robotframework-0.6.0/testbench2robotframework/testbench2rf.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1164 2023-02-03 13:47:35.000000 testbench2robotframework-0.6.0/testbench2robotframework/testbench2robotframework.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1789 2023-07-10 15:29:48.000000 testbench2robotframework-0.6.0/testbench2robotframework/testsuite_write.py
+-rw-r--r--   0 rener      (502) wheel        (0)     6979 2023-07-10 15:48:25.000000 testbench2robotframework-0.6.0/testbench2robotframework/utils.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.596856 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/
+-rw-r--r--   0 rener      (502) wheel        (0)    15345 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)     1473 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      132 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/entry_points.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2023-02-03 13:42:07.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/not-zip-safe
+-rw-r--r--   0 rener      (502) wheel        (0)      120 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/requires.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       25 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.597569 testbench2robotframework-0.6.0/tests/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.587396 testbench2robotframework-0.6.0/tests/test_data/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.597944 testbench2robotframework-0.6.0/tests/test_data/configurations/
+-rw-r--r--   0 rener      (502) wheel        (0)     1150 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/tests/test_data/configurations/invalid_config.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1128 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/tests/test_data/configurations/valid_config.json
+-rw-r--r--   0 rener      (502) wheel        (0)      227 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/tests/test_missing_files.py
+-rw-r--r--   0 rener      (502) wheel        (0)      415 2022-10-26 13:44:46.000000 testbench2robotframework-0.6.0/tests/test_robot_files_should_not_contain_invalid_characters.py
+-rw-r--r--   0 rener      (502) wheel        (0)      928 2022-11-01 23:24:18.000000 testbench2robotframework-0.6.0/tests/test_zip_file_generation.py
```

### Comparing `testbench2robotframework-0.5.2/DEVELOPMENT.md` & `testbench2robotframework-0.6.0/DEVELOPMENT.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-# Contributing
-
-## Development Environment Setup
-
-1. Install Python 3.8 and VS Code
-
-2. Open a terminal in this repository
-
-3. Create the virtual environment .venv
-
-    > /path/to/python38/python -m venv .venv
-
-4. Activate the virtual environment
-
-    > .venv/scripts/activate
-
-4. Install the dependencies
-
-    > pip install -r requirements.txt
-
-5. [Install Pandoc](https://pandoc.org/installing.html)
-
-
-## Generate documentation in Word format
-
-```shell
-pandoc -s README.md -M title="imbus TestBench - Robot Code Generator" -M subtitle=Benutzerhandbuch -M toc-title=Inhaltsverzeichnis --toc -o Benutzerhandbuch.docx
-```
-
-
-## Build, Install and Run
-
-The package is built using setuptools. The build configuration is defined in `setup.cfg`.
-
-- Build and install the package
-    > pip install -e .
-
-- Run the application
-    > tb2robot
-
-- Build a pure-Python wheel
-    > pip install wheel
-    > python setup.py bdist_wheel
-
-- Build a pure-Python wheel and publish new version to pypi
-    > pip install wheel
-    > pip install twine
-    > CreatePipWheel.bat oder CreatePipWheel.sh
-
-
-## Adding New Dependencies
-1. Install pip-tools (to pin dependencies)
-
-    > python -m pip install pip-tools
-
-
-2. In `setup.cfg` add a package to the corresponding section
-
-    - Development dependencies: `dev` extra under `options.extras_require`
-
-    - Runtime dependencies: `install-requires`
-
-3. Update `requirements.txt`
-    - Development dependencies
-        > pip-compile --extra dev setup.cfg
-
-    - Runtime dependencies
-        > pip-compile setup.cfg
-
-4. Create a commit with `setup.cfg`, `requirements.txt`, `pyproject.toml` explaining why the dependency was added.
-
-
-## Static Analysis and Code Formatting
-
-Static analysis and code formatting tools are configured in `pyproject.toml`.
-
-### Static Analysis
-
-- `mypy`: static type checker
-    * [The mypy configuration file](https://mypy.readthedocs.io/en/stable/config_file.html)
-
-- `pylint`: syntax and code quality checks
-
-    * [Pylint Global options and switches](https://pylint.pycqa.org/en/latest/technical_reference/features.html)
-
-    * [Overview of all Pylint messages](https://pylint.pycqa.org/en/latest/messages/messages_list.html)
-
-    * [Naming Styles](https://pylint.pycqa.org/en/latest/user_guide/options.html)
-
-
-### Code Formatting
-
-- `black`: Format the code according to a subset of PEP 8
-    > black .
-
-- `isort`: Sort the package imports following PEP 8
-    > isort .
-
-
-## Testing
-
-- `pytest` is configured in `pyproject.toml`
-    > python -m pytest
+# Contributing
+
+## Development Environment Setup
+
+1. Install Python 3.8 and VS Code
+
+2. Open a terminal in this repository
+
+3. Create the virtual environment .venv
+
+    > /path/to/python38/python -m venv .venv
+
+4. Activate the virtual environment
+
+    > .venv/scripts/activate
+
+4. Install the dependencies
+
+    > pip install -r requirements.txt
+
+5. [Install Pandoc](https://pandoc.org/installing.html)
+
+
+## Generate documentation in Word format
+
+```shell
+pandoc -s README.md -M title="imbus TestBench - Robot Code Generator" -M subtitle=Benutzerhandbuch -M toc-title=Inhaltsverzeichnis --toc -o Benutzerhandbuch.docx
+```
+
+
+## Build, Install and Run
+
+The package is built using setuptools. The build configuration is defined in `setup.cfg`.
+
+- Build and install the package
+    > pip install -e .
+
+- Run the application
+    > tb2robot
+
+- Build a pure-Python wheel
+    > pip install wheel
+    > python setup.py bdist_wheel
+
+- Build a pure-Python wheel and publish new version to pypi
+    > pip install wheel
+    > pip install twine
+    > CreatePipWheel.bat oder CreatePipWheel.sh
+
+
+## Adding New Dependencies
+1. Install pip-tools (to pin dependencies)
+
+    > python -m pip install pip-tools
+
+
+2. In `setup.cfg` add a package to the corresponding section
+
+    - Development dependencies: `dev` extra under `options.extras_require`
+
+    - Runtime dependencies: `install-requires`
+
+3. Update `requirements.txt`
+    - Development dependencies
+        > pip-compile --extra dev setup.cfg
+
+    - Runtime dependencies
+        > pip-compile setup.cfg
+
+4. Create a commit with `setup.cfg`, `requirements.txt`, `pyproject.toml` explaining why the dependency was added.
+
+
+## Static Analysis and Code Formatting
+
+Static analysis and code formatting tools are configured in `pyproject.toml`.
+
+### Static Analysis
+
+- `mypy`: static type checker
+    * [The mypy configuration file](https://mypy.readthedocs.io/en/stable/config_file.html)
+
+- `pylint`: syntax and code quality checks
+
+    * [Pylint Global options and switches](https://pylint.pycqa.org/en/latest/technical_reference/features.html)
+
+    * [Overview of all Pylint messages](https://pylint.pycqa.org/en/latest/messages/messages_list.html)
+
+    * [Naming Styles](https://pylint.pycqa.org/en/latest/user_guide/options.html)
+
+
+### Code Formatting
+
+- `black`: Format the code according to a subset of PEP 8
+    > black .
+
+- `isort`: Sort the package imports following PEP 8
+    > isort .
+
+
+## Testing
+
+- `pytest` is configured in `pyproject.toml`
+    > python -m pytest
```

### Comparing `testbench2robotframework-0.5.2/LICENSE` & `testbench2robotframework-0.6.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `testbench2robotframework-0.5.2/PKG-INFO` & `testbench2robotframework-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,302 +1,303 @@
-Metadata-Version: 2.1
-Name: testbench2robotframework
-Version: 0.5.2
-Summary: Robot Framework Code Generator from Keyword-Driven Tests in imbus TestBench 3.0 and newer
-Home-page: https://github.com/imbus/testbench2robotframework
-Author: imbus AG
-Author-email: support@imbus.de
-License: Apache 2.0 License
-Description: # Installation des Robot Code Generators
-        
-        Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
-        
-        ```powershell
-        python --version
-        ```
-        
-        Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
-        Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
-        
-        ```powershell
-        python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
-        ```
-        
-        Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
-        ```powershell
-        pip install testbench2robotframework
-        ```
-        
-        Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
-        
-        ```powershell
-        tb2robot --version
-        ```
-        
-        # Verwendung des Robot Code Generators
-        Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
-        
-        Der Befehl ``tb2robot --help
-        `` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
-        
-        Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
-        
-        (@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
-        
-        (@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-        
-        Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
-        ```powershell
-        tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
-        ```
-        Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
-        
-        ![](./images/testthemen.PNG)
-        ![](./images/generated.PNG)
-        
-        Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
-        
-        Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
-        Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
-        
-        (@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
-        
-        (@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
-        
-        (@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-        
-        Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
-        ```powershell
-        tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
-        ```
-        
-        # Konfiguration der Ergebnisse
-        Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
-        
-        ## rfLibraryRegex
-        Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
-        Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
-        Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
-        
-        ![](./images/testbench_rfLibraryRegex.PNG)
-        
-        ```python
-        *** Settings ***
-        Library    Browser
-        Library    BuiltIn
-        ```
-        In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-        ```json
-        "rfLibraryRegex": [
-            "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
-          ]
-        ```
-        
-        ## rfResourceRegex
-        Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
-        Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
-        Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
-        
-        ![](./images/testbench_rfResourceRegex.PNG)
-        
-        ```python
-        *** Settings ***
-        Resource    keywords.resource
-        ```
-        In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-        ```json
-        "rfResourceRegex": [
-            "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
-          ]
-        ```
-        ## rfLibraryRoots
-        Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
-        Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
-        
-        Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
-        
-        Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
-        
-        ```json
-        "rfLibraryRoots": ["RobotLibraries"]
-        ```
-        
-        ![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
-        
-        Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
-        
-        ```python
-        *** Settings ***
-        Library    BuiltIn
-        Library    OperatingSystem
-        # UNKNOWN    Process
-        ```
-        
-        ## rfResourceRoots
-        Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
-        
-        Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
-        
-        ```json
-        "rfResourceRoots": ["RF-Resources"]
-        ```
-        
-        ![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
-        
-        Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
-        
-        ```python
-        *** Settings ***
-        Resource    keywords.resource
-        # UNKNOWN    unknownKeywords
-        ```
-        
-        ## fullyQualified
-        Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
-        
-        Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
-        
-        ```python
-        SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
-        ```
-        Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
-        
-        ```python
-        Open Browser      https://robotframework.org/    firefox
-        ```
-        
-        ## resourceDirectory
-        Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
-        Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
-        
-        ```json
-        "resourceDirectory": "{root}/Resources",
-        ```
-        
-        ```robotframework
-        *** Settings ***
-        Resource    ../Resources/myKeywords.resource
-        ```
-        
-        ## generationDirectory
-        Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
-        ```json
-        "generationDirectory": "{root}/generatedRobotFiles"
-        ```
-        
-        ## createOutputZip
-        Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
-        
-        ## logSuiteNumbering
-        Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
-        
-        ```json
-        "logSuiteNumbering": true
-        ```
-        ## clearGenerationDirectory
-        Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
-        
-        ```json
-        "clearGenerationDirectory": true,
-        ```
-        
-        ## logCompoundInteractions
-        Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
-        
-        ```json
-        "logCompoundInteractions": true,
-        ```
-        
-        ## subdivisionsMapping
-        Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
-        
-        ```json
-        "subdivisionsMapping": {
-            "libraries": {
-              "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
-              "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
-            },
-            "resources": {
-              "MyKeywords": "{root}/../MyKeywords.resource",
-              "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
-            }
-          }
-        ```
-        
-        
-        ## forcedImport
-        Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
-        
-        ```json
-        "forcedImport": {
-            "libraries": [
-              "SeleniumLibrary"
-            ],
-            "resources":
-            [
-              "technical_keywords.resource"
-            ],
-            "variables": [
-              "myVars.py"
-            ]
-          }
-        ```
-        
-        ## loggingConfiguration
-        Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
-        Gültige Optionen sind:
-        
-        * "CRITICAL"
-        
-        * "FATAL"
-        
-        * "ERROR"
-        
-        * "WARNING"
-        
-        * "WARN"
-        
-        * "INFO"
-        
-        * "DEBUG"
-        
-        * "NOTSET"
-        
-        Das Default Log-Level ist ``INFO``.
-        ```json
-        "loggingConfiguration": {
-          "console": {
-            "logLevel": "info"
-          }
-        }
-        ```
-        
-        ## referenceBehaviour
-        Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
-        Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
-        Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
-        
-        ```json
-        "referenceBehaviour": "ATTACHMENT"
-        ```
-        
-        ## attachmentConflictBehaviour
-        Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
-        Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
-        
-        Die möglichen Werte haben dabei die folgende Bedeutung:
-        - ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
-        - USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
-        - USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
-        - RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
-        ```json
-        "attachmentConflictBehaviour": "USE_EXISTING"
-        ```
-        
-        ## testCaseSplitPathRegEx
-        Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
-        
-        
-Platform: any
-Requires-Python: >= 3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+Metadata-Version: 2.1
+Name: testbench2robotframework
+Version: 0.6.0
+Summary: Robot Framework Code Generator from Keyword-Driven Tests in imbus TestBench 3.0 and newer
+Home-page: https://github.com/imbus/testbench2robotframework
+Author: imbus AG
+Author-email: support@imbus.de
+License: Apache 2.0 License
+Platform: any
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Installation des Robot Code Generators
+
+Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
+
+```powershell
+python --version
+```
+
+Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
+Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
+
+```powershell
+python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
+```
+
+Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
+```powershell
+pip install testbench2robotframework
+```
+
+Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
+
+```powershell
+tb2robot --version
+```
+
+# Verwendung des Robot Code Generators
+Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
+
+Der Befehl ``tb2robot --help
+`` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
+
+Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
+
+(@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
+
+(@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+
+Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
+```powershell
+tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
+```
+Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
+
+![](./images/testthemen.PNG)
+![](./images/generated.PNG)
+
+Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
+
+Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
+Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
+
+(@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
+
+(@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
+
+(@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+
+Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
+```powershell
+tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
+```
+
+# Konfiguration der Ergebnisse
+Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
+
+## rfLibraryRegex
+Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
+Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
+Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
+
+![](./images/testbench_rfLibraryRegex.PNG)
+
+```python
+*** Settings ***
+Library    Browser
+Library    BuiltIn
+```
+In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+```json
+"rfLibraryRegex": [
+    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
+  ]
+```
+
+## rfResourceRegex
+Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
+Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
+Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
+
+![](./images/testbench_rfResourceRegex.PNG)
+
+```python
+*** Settings ***
+Resource    keywords.resource
+```
+In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+```json
+"rfResourceRegex": [
+    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
+  ]
+```
+## rfLibraryRoots
+Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
+Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
+
+Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
+
+Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
+
+```json
+"rfLibraryRoots": ["RobotLibraries"]
+```
+
+![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
+
+Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
+
+```python
+*** Settings ***
+Library    BuiltIn
+Library    OperatingSystem
+# UNKNOWN    Process
+```
+
+## rfResourceRoots
+Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
+
+Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
+
+```json
+"rfResourceRoots": ["RF-Resources"]
+```
+
+![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
+
+Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
+
+```python
+*** Settings ***
+Resource    keywords.resource
+# UNKNOWN    unknownKeywords
+```
+
+## fullyQualified
+Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
+
+Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
+
+```python
+SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
+```
+Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
+
+```python
+Open Browser      https://robotframework.org/    firefox
+```
+
+## resourceDirectory
+Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
+Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
+
+```json
+"resourceDirectory": "{root}/Resources",
+```
+
+```robotframework
+*** Settings ***
+Resource    ../Resources/myKeywords.resource
+```
+
+## generationDirectory
+Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
+```json
+"generationDirectory": "{root}/generatedRobotFiles"
+```
+
+## createOutputZip
+Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
+
+## logSuiteNumbering
+Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
+
+```json
+"logSuiteNumbering": true
+```
+## clearGenerationDirectory
+Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
+
+```json
+"clearGenerationDirectory": true,
+```
+
+## logCompoundInteractions
+Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
+
+```json
+"logCompoundInteractions": true,
+```
+
+## subdivisionsMapping
+Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
+
+```json
+"subdivisionsMapping": {
+    "libraries": {
+      "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
+      "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
+    },
+    "resources": {
+      "MyKeywords": "{root}/../MyKeywords.resource",
+      "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
+    }
+  }
+```
+
+
+## forcedImport
+Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
+
+```json
+"forcedImport": {
+    "libraries": [
+      "SeleniumLibrary"
+    ],
+    "resources":
+    [
+      "technical_keywords.resource"
+    ],
+    "variables": [
+      "myVars.py"
+    ]
+  }
+```
+
+## loggingConfiguration
+Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
+Gültige Optionen sind:
+
+* "CRITICAL"
+
+* "FATAL"
+
+* "ERROR"
+
+* "WARNING"
+
+* "WARN"
+
+* "INFO"
+
+* "DEBUG"
+
+* "NOTSET"
+
+Das Default Log-Level ist ``INFO``.
+```json
+"loggingConfiguration": {
+  "console": {
+    "logLevel": "info"
+  }
+}
+```
+
+## referenceBehaviour
+Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
+Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
+Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
+
+```json
+"referenceBehaviour": "ATTACHMENT"
+```
+
+## attachmentConflictBehaviour
+Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
+Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
+
+Die möglichen Werte haben dabei die folgende Bedeutung:
+- ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
+- USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
+- USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
+- RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
+```json
+"attachmentConflictBehaviour": "USE_EXISTING"
+```
+
+## testCaseSplitPathRegEx
+Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
+
```

### Comparing `testbench2robotframework-0.5.2/README.md` & `testbench2robotframework-0.6.0/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,289 +1,289 @@
-# Installation des Robot Code Generators
-
-Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
-
-```powershell
-python --version
-```
-
-Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
-Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
-
-```powershell
-python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
-```
-
-Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
-```powershell
-pip install testbench2robotframework
-```
-
-Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
-
-```powershell
-tb2robot --version
-```
-
-# Verwendung des Robot Code Generators
-Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
-
-Der Befehl ``tb2robot --help
-`` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
-
-Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
-
-(@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
-
-(@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-
-Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
-```powershell
-tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
-```
-Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
-
-![](./images/testthemen.PNG)
-![](./images/generated.PNG)
-
-Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
-
-Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
-Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
-
-(@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
-
-(@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
-
-(@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-
-Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
-```powershell
-tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
-```
-
-# Konfiguration der Ergebnisse
-Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
-
-## rfLibraryRegex
-Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
-Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
-Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
-
-![](./images/testbench_rfLibraryRegex.PNG)
-
-```python
-*** Settings ***
-Library    Browser
-Library    BuiltIn
-```
-In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-```json
-"rfLibraryRegex": [
-    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
-  ]
-```
-
-## rfResourceRegex
-Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
-Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
-Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
-
-![](./images/testbench_rfResourceRegex.PNG)
-
-```python
-*** Settings ***
-Resource    keywords.resource
-```
-In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-```json
-"rfResourceRegex": [
-    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
-  ]
-```
-## rfLibraryRoots
-Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
-Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
-
-Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
-
-Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
-
-```json
-"rfLibraryRoots": ["RobotLibraries"]
-```
-
-![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
-
-Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
-
-```python
-*** Settings ***
-Library    BuiltIn
-Library    OperatingSystem
-# UNKNOWN    Process
-```
-
-## rfResourceRoots
-Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
-
-Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
-
-```json
-"rfResourceRoots": ["RF-Resources"]
-```
-
-![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
-
-Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
-
-```python
-*** Settings ***
-Resource    keywords.resource
-# UNKNOWN    unknownKeywords
-```
-
-## fullyQualified
-Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
-
-Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
-
-```python
-SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
-```
-Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
-
-```python
-Open Browser      https://robotframework.org/    firefox
-```
-
-## resourceDirectory
-Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
-Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
-
-```json
-"resourceDirectory": "{root}/Resources",
-```
-
-```robotframework
-*** Settings ***
-Resource    ../Resources/myKeywords.resource
-```
-
-## generationDirectory
-Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
-```json
-"generationDirectory": "{root}/generatedRobotFiles"
-```
-
-## createOutputZip
-Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
-
-## logSuiteNumbering
-Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
-
-```json
-"logSuiteNumbering": true
-```
-## clearGenerationDirectory
-Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
-
-```json
-"clearGenerationDirectory": true,
-```
-
-## logCompoundInteractions
-Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
-
-```json
-"logCompoundInteractions": true,
-```
-
-## subdivisionsMapping
-Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
-
-```json
-"subdivisionsMapping": {
-    "libraries": {
-      "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
-      "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
-    },
-    "resources": {
-      "MyKeywords": "{root}/../MyKeywords.resource",
-      "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
-    }
-  }
-```
-
-
-## forcedImport
-Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
-
-```json
-"forcedImport": {
-    "libraries": [
-      "SeleniumLibrary"
-    ],
-    "resources":
-    [
-      "technical_keywords.resource"
-    ],
-    "variables": [
-      "myVars.py"
-    ]
-  }
-```
-
-## loggingConfiguration
-Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
-Gültige Optionen sind:
-
-* "CRITICAL"
-
-* "FATAL"
-
-* "ERROR"
-
-* "WARNING"
-
-* "WARN"
-
-* "INFO"
-
-* "DEBUG"
-
-* "NOTSET"
-
-Das Default Log-Level ist ``INFO``.
-```json
-"loggingConfiguration": {
-  "console": {
-    "logLevel": "info"
-  }
-}
-```
-
-## referenceBehaviour
-Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
-Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
-Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
-
-```json
-"referenceBehaviour": "ATTACHMENT"
-```
-
-## attachmentConflictBehaviour
-Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
-Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
-
-Die möglichen Werte haben dabei die folgende Bedeutung:
-- ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
-- USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
-- USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
-- RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
-```json
-"attachmentConflictBehaviour": "USE_EXISTING"
-```
-
-## testCaseSplitPathRegEx
-Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
-
+# Installation des Robot Code Generators
+
+Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
+
+```powershell
+python --version
+```
+
+Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
+Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
+
+```powershell
+python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
+```
+
+Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
+```powershell
+pip install testbench2robotframework
+```
+
+Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
+
+```powershell
+tb2robot --version
+```
+
+# Verwendung des Robot Code Generators
+Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
+
+Der Befehl ``tb2robot --help
+`` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
+
+Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
+
+(@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
+
+(@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+
+Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
+```powershell
+tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
+```
+Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
+
+![](./images/testthemen.PNG)
+![](./images/generated.PNG)
+
+Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
+
+Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
+Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
+
+(@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
+
+(@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
+
+(@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+
+Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
+```powershell
+tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
+```
+
+# Konfiguration der Ergebnisse
+Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
+
+## rfLibraryRegex
+Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
+Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
+Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
+
+![](./images/testbench_rfLibraryRegex.PNG)
+
+```python
+*** Settings ***
+Library    Browser
+Library    BuiltIn
+```
+In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+```json
+"rfLibraryRegex": [
+    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
+  ]
+```
+
+## rfResourceRegex
+Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
+Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
+Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
+
+![](./images/testbench_rfResourceRegex.PNG)
+
+```python
+*** Settings ***
+Resource    keywords.resource
+```
+In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+```json
+"rfResourceRegex": [
+    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
+  ]
+```
+## rfLibraryRoots
+Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
+Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
+
+Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
+
+Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
+
+```json
+"rfLibraryRoots": ["RobotLibraries"]
+```
+
+![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
+
+Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
+
+```python
+*** Settings ***
+Library    BuiltIn
+Library    OperatingSystem
+# UNKNOWN    Process
+```
+
+## rfResourceRoots
+Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
+
+Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
+
+```json
+"rfResourceRoots": ["RF-Resources"]
+```
+
+![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
+
+Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
+
+```python
+*** Settings ***
+Resource    keywords.resource
+# UNKNOWN    unknownKeywords
+```
+
+## fullyQualified
+Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
+
+Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
+
+```python
+SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
+```
+Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
+
+```python
+Open Browser      https://robotframework.org/    firefox
+```
+
+## resourceDirectory
+Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
+Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
+
+```json
+"resourceDirectory": "{root}/Resources",
+```
+
+```robotframework
+*** Settings ***
+Resource    ../Resources/myKeywords.resource
+```
+
+## generationDirectory
+Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
+```json
+"generationDirectory": "{root}/generatedRobotFiles"
+```
+
+## createOutputZip
+Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
+
+## logSuiteNumbering
+Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
+
+```json
+"logSuiteNumbering": true
+```
+## clearGenerationDirectory
+Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
+
+```json
+"clearGenerationDirectory": true,
+```
+
+## logCompoundInteractions
+Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
+
+```json
+"logCompoundInteractions": true,
+```
+
+## subdivisionsMapping
+Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
+
+```json
+"subdivisionsMapping": {
+    "libraries": {
+      "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
+      "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
+    },
+    "resources": {
+      "MyKeywords": "{root}/../MyKeywords.resource",
+      "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
+    }
+  }
+```
+
+
+## forcedImport
+Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
+
+```json
+"forcedImport": {
+    "libraries": [
+      "SeleniumLibrary"
+    ],
+    "resources":
+    [
+      "technical_keywords.resource"
+    ],
+    "variables": [
+      "myVars.py"
+    ]
+  }
+```
+
+## loggingConfiguration
+Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
+Gültige Optionen sind:
+
+* "CRITICAL"
+
+* "FATAL"
+
+* "ERROR"
+
+* "WARNING"
+
+* "WARN"
+
+* "INFO"
+
+* "DEBUG"
+
+* "NOTSET"
+
+Das Default Log-Level ist ``INFO``.
+```json
+"loggingConfiguration": {
+  "console": {
+    "logLevel": "info"
+  }
+}
+```
+
+## referenceBehaviour
+Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
+Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
+Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
+
+```json
+"referenceBehaviour": "ATTACHMENT"
+```
+
+## attachmentConflictBehaviour
+Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
+Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
+
+Die möglichen Werte haben dabei die folgende Bedeutung:
+- ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
+- USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
+- USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
+- RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
+```json
+"attachmentConflictBehaviour": "USE_EXISTING"
+```
+
+## testCaseSplitPathRegEx
+Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
+
```

### Comparing `testbench2robotframework-0.5.2/images/LibrarySubdivision.PNG` & `testbench2robotframework-0.6.0/images/LibrarySubdivision.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.5.2/images/generated.png` & `testbench2robotframework-0.6.0/images/generated.png`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.5.2/images/libraries.PNG` & `testbench2robotframework-0.6.0/images/libraries.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.5.2/images/resources.PNG` & `testbench2robotframework-0.6.0/images/resources.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.5.2/images/rfLibraryRootsTestBench.PNG` & `testbench2robotframework-0.6.0/images/rfLibraryRootsTestBench.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.5.2/images/testbench_rfLibraryRegex.PNG` & `testbench2robotframework-0.6.0/images/testbench_rfLibraryRegex.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.5.2/images/testbench_rfResourceRegex.PNG` & `testbench2robotframework-0.6.0/images/testbench_rfResourceRegex.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.5.2/images/testthemen.PNG` & `testbench2robotframework-0.6.0/images/testthemen.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.5.2/pyproject.toml` & `testbench2robotframework-0.6.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,123 @@
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[tool.pylint.FORMAT]
-max-line-length = 100
-max-module-lines = 1000
-
-[tool.pylint.MASTER]
-ignore = "tests"
-
-[tool.pylint.BASIC]
-argument-naming-style = 'snake_case'
-attr-naming-style = 'snake_case'
-class-naming-style = 'PascalCase'
-const-naming-style = 'UPPER_CASE'
-function-naming-style = 'snake_case'
-method-naming-style = 'snake_case'
-module-naming-style = 'snake_case'
-variable-naming-style = 'snake_case'
-
-[tool.pylint.DESIGN]
-# Maximum number of arguments for function / method.
-max-args = 5
-# Maximum number of statements in function / method body.
-max-statements = 50
-
-[tool.pylint."MESSAGES CONTROL"]
-disable = '''
-    logging-fstring-interpolation,
-    fixme,
-    import-error,
-    missing-module-docstring,
-    missing-class-docstring,
-    missing-function-docstring,
-    too-many-instance-attributes,
-    too-few-public-methods,
-'''
-
-[tool.pylint.REFACTORING]
-# Maximum number of nested blocks for function / method body
-max-nested-blocks = 3
-
-[tool.mypy]
-python_version = "3.8"
-ignore_missing_imports = true
-no_implicit_optional = true
-strict_optional = true
-warn_return_any = true
-warn_no_return = true
-warn_unreachable = true
-pretty = true
-
-[tool.black]
-target-version = ['py38']
-line-length = 100
-include_trailing_comma = false
-skip-string-normalization = true
-
-[tool.isort]
-profile = "black"
-src_paths = ["testbench2robotframework"]
-skip_gitignore = true
-skip = ['external']
-
-[tool.pytest.ini_options]
-minversion = "6.0"
-addopts = "-ra --spec"
-testpaths = [
-    "tests",
-]
-spec_header_format = "{test_case}"
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[tool.pylint.FORMAT]
+max-line-length = 100
+max-module-lines = 1000
+
+[tool.pylint.MASTER]
+ignore = "tests"
+
+[tool.pylint.BASIC]
+argument-naming-style = 'snake_case'
+attr-naming-style = 'snake_case'
+class-naming-style = 'PascalCase'
+const-naming-style = 'UPPER_CASE'
+function-naming-style = 'snake_case'
+method-naming-style = 'snake_case'
+module-naming-style = 'snake_case'
+variable-naming-style = 'snake_case'
+
+[tool.pylint.DESIGN]
+# Maximum number of arguments for function / method.
+max-args = 5
+# Maximum number of statements in function / method body.
+max-statements = 50
+
+[tool.pylint."MESSAGES CONTROL"]
+disable = '''
+    logging-fstring-interpolation,
+    fixme,
+    import-error,
+    missing-module-docstring,
+    missing-class-docstring,
+    missing-function-docstring,
+    too-many-instance-attributes,
+    too-few-public-methods,
+'''
+
+[tool.pylint.REFACTORING]
+# Maximum number of nested blocks for function / method body
+max-nested-blocks = 3
+
+[tool.mypy]
+python_version = "3.8"
+ignore_missing_imports = true
+no_implicit_optional = true
+strict_optional = true
+warn_return_any = true
+warn_no_return = true
+warn_unreachable = true
+pretty = true
+
+[tool.black]
+target-version = ['py38']
+line-length = 100
+include_trailing_comma = false
+skip-string-normalization = true
+
+[tool.isort]
+profile = "black"
+src_paths = ["testbench2robotframework"]
+skip_gitignore = true
+skip = ['external']
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "-ra --spec"
+testpaths = [
+    "tests",
+]
+spec_header_format = "{test_case}"
+
+[tool.ruff]
+unfixable = [
+    "UP007"
+]
+exclude = [
+  "__pycache__",
+  "config.py",
+  "model.py",
+  "tests"
+]
+ignore = [
+  "B008",  # do not perform function calls in argument defaults
+  "E501",  # line too long
+  # "N815",  # mixedCase variable in class scope
+  # "N803",  # argument name should be lowercase
+  # "N806",  # variable in function should be lowercase
+  # "N812",  # lowercase imported as non lowercase
+  # "N999",  # Invalid module name: 'Browser'
+  "PLR0913",  # too many arguments
+  # "T201",  # Print statements
+  "UP007",
+]
+target-version = "py37"
+select = [
+  "E",
+  "F",
+  "W",
+  "C90",
+  "I",
+  "N",
+  "B",
+  "PYI",
+  "PL",
+  "PTH",
+  "UP",
+  "A",
+  "C4",
+  "DTZ",
+  "ISC",
+  "ICN",
+  "INP",
+  "PIE",
+  "T20",
+  "PYI",
+  "PT",
+  "RSE",
+  "RET",
+  "SIM",
+  "RUF"
+]
```

### Comparing `testbench2robotframework-0.5.2/setup.cfg` & `testbench2robotframework-0.6.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,58 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2074 6573 7462 656e 6368 3272 6f62   = testbench2rob
-00000020: 6f74 6672 616d 6577 6f72 6b0d 0a61 7574  otframework..aut
-00000030: 686f 7220 3d20 696d 6275 7320 4147 0d0a  hor = imbus AG..
-00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2073  author_email = s
-00000050: 7570 706f 7274 4069 6d62 7573 2e64 650d  upport@imbus.de.
-00000060: 0a76 6572 7369 6f6e 203d 2061 7474 723a  .version = attr:
-00000070: 2074 6573 7462 656e 6368 3272 6f62 6f74   testbench2robot
-00000080: 6672 616d 6577 6f72 6b2e 5f5f 7665 7273  framework.__vers
-00000090: 696f 6e5f 5f0d 0a64 6573 6372 6970 7469  ion__..descripti
-000000a0: 6f6e 203d 2052 6f62 6f74 2046 7261 6d65  on = Robot Frame
-000000b0: 776f 726b 2043 6f64 6520 4765 6e65 7261  work Code Genera
-000000c0: 746f 7220 6672 6f6d 204b 6579 776f 7264  tor from Keyword
-000000d0: 2d44 7269 7665 6e20 5465 7374 7320 696e  -Driven Tests in
-000000e0: 2069 6d62 7573 2054 6573 7442 656e 6368   imbus TestBench
-000000f0: 2033 2e30 2061 6e64 206e 6577 6572 0d0a   3.0 and newer..
-00000100: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000110: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-00000120: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-00000130: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-00000140: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000150: 6e0d 0a6c 6963 656e 7365 203d 2041 7061  n..license = Apa
-00000160: 6368 6520 322e 3020 4c69 6365 6e73 650d  che 2.0 License.
-00000170: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
-00000180: 6974 6875 622e 636f 6d2f 696d 6275 732f  ithub.com/imbus/
-00000190: 7465 7374 6265 6e63 6832 726f 626f 7466  testbench2robotf
-000001a0: 7261 6d65 776f 726b 0d0a 706c 6174 666f  ramework..platfo
-000001b0: 726d 7320 3d20 616e 790d 0a0d 0a5b 6f70  rms = any....[op
-000001c0: 7469 6f6e 735d 0d0a 7a69 705f 7361 6665  tions]..zip_safe
-000001d0: 203d 2046 616c 7365 0d0a 7061 636b 6167   = False..packag
-000001e0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-000001f0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000200: 2033 2e38 0d0a 696e 7374 616c 6c5f 7265   3.8..install_re
-00000210: 7175 6972 6573 203d 200d 0a09 726f 626f  quires = ...robo
-00000220: 7466 7261 6d65 776f 726b 203e 3d20 342e  tframework >= 4.
-00000230: 300d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  0....[options.en
-00000240: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
-00000250: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
-00000260: 0a09 7462 3272 6f62 6f74 203d 2074 6573  ..tb2robot = tes
-00000270: 7462 656e 6368 3272 6f62 6f74 6672 616d  tbench2robotfram
-00000280: 6577 6f72 6b2e 5f5f 6d61 696e 5f5f 3a72  ework.__main__:r
-00000290: 756e 0d0a 0974 6573 7462 656e 6368 3272  un...testbench2r
-000002a0: 6f62 6f74 6672 616d 6577 6f72 6b20 3d20  obotframework = 
-000002b0: 7465 7374 6265 6e63 6832 726f 626f 7466  testbench2robotf
-000002c0: 7261 6d65 776f 726b 2e5f 5f6d 6169 6e5f  ramework.__main_
-000002d0: 5f3a 7275 6e0d 0a0d 0a5b 6f70 7469 6f6e  _:run....[option
-000002e0: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
-000002f0: 5d0d 0a64 6576 203d 200d 0a09 626c 6163  ]..dev = ...blac
-00000300: 6b0d 0a09 666c 616b 6538 0d0a 0970 796c  k...flake8...pyl
-00000310: 696e 740d 0a09 6d79 7079 0d0a 0970 7974  int...mypy...pyt
-00000320: 6573 740d 0a09 7079 7465 7374 2d63 6f76  est...pytest-cov
-00000330: 0d0a 0970 7974 6573 742d 7370 6563 0d0a  ...pytest-spec..
-00000340: 0963 6865 636b 2d6d 616e 6966 6573 740d  .check-manifest.
-00000350: 0a09 7477 696e 650d 0a09 7768 6565 6c0d  ..twine...wheel.
-00000360: 0a09 7365 7475 7074 6f6f 6c73 0d0a 0d0a  ..setuptools....
-00000370: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000380: 732e 6669 6e64 5d0d 0a65 7863 6c75 6465  s.find]..exclude
-00000390: 203d 200d 0a09 7465 7374 730d 0a0d 0a5b   = ...tests....[
-000003a0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000003b0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000003c0: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7465 7374 6265 6e63 6832 726f 626f  = testbench2robo
+00000020: 7466 7261 6d65 776f 726b 0a61 7574 686f  tframework.autho
+00000030: 7220 3d20 696d 6275 7320 4147 0a61 7574  r = imbus AG.aut
+00000040: 686f 725f 656d 6169 6c20 3d20 7375 7070  hor_email = supp
+00000050: 6f72 7440 696d 6275 732e 6465 0a76 6572  ort@imbus.de.ver
+00000060: 7369 6f6e 203d 2061 7474 723a 2074 6573  sion = attr: tes
+00000070: 7462 656e 6368 3272 6f62 6f74 6672 616d  tbench2robotfram
+00000080: 6577 6f72 6b2e 5f5f 7665 7273 696f 6e5f  ework.__version_
+00000090: 5f0a 6465 7363 7269 7074 696f 6e20 3d20  _.description = 
+000000a0: 526f 626f 7420 4672 616d 6577 6f72 6b20  Robot Framework 
+000000b0: 436f 6465 2047 656e 6572 6174 6f72 2066  Code Generator f
+000000c0: 726f 6d20 4b65 7977 6f72 642d 4472 6976  rom Keyword-Driv
+000000d0: 656e 2054 6573 7473 2069 6e20 696d 6275  en Tests in imbu
+000000e0: 7320 5465 7374 4265 6e63 6820 332e 3020  s TestBench 3.0 
+000000f0: 616e 6420 6e65 7765 720a 6c6f 6e67 5f64  and newer.long_d
+00000100: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+00000110: 653a 2052 4541 444d 452e 6d64 0a6c 6f6e  e: README.md.lon
+00000120: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+00000130: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+00000140: 742f 6d61 726b 646f 776e 0a6c 6963 656e  t/markdown.licen
+00000150: 7365 203d 2041 7061 6368 6520 322e 3020  se = Apache 2.0 
+00000160: 4c69 6365 6e73 650a 7572 6c20 3d20 6874  License.url = ht
+00000170: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000180: 2f69 6d62 7573 2f74 6573 7462 656e 6368  /imbus/testbench
+00000190: 3272 6f62 6f74 6672 616d 6577 6f72 6b0a  2robotframework.
+000001a0: 706c 6174 666f 726d 7320 3d20 616e 790a  platforms = any.
+000001b0: 0a5b 6f70 7469 6f6e 735d 0a7a 6970 5f73  .[options].zip_s
+000001c0: 6166 6520 3d20 4661 6c73 650a 7061 636b  afe = False.pack
+000001d0: 6167 6573 203d 2066 696e 643a 0a70 7974  ages = find:.pyt
+000001e0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+000001f0: 3d20 332e 380a 696e 7374 616c 6c5f 7265  = 3.8.install_re
+00000200: 7175 6972 6573 203d 200a 0972 6f62 6f74  quires = ..robot
+00000210: 6672 616d 6577 6f72 6b20 3e3d 2034 2e30  framework >= 4.0
+00000220: 0a0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
+00000230: 5f70 6f69 6e74 735d 0a63 6f6e 736f 6c65  _points].console
+00000240: 5f73 6372 6970 7473 203d 200a 0974 6232  _scripts = ..tb2
+00000250: 726f 626f 7420 3d20 7465 7374 6265 6e63  robot = testbenc
+00000260: 6832 726f 626f 7466 7261 6d65 776f 726b  h2robotframework
+00000270: 2e5f 5f6d 6169 6e5f 5f3a 7275 6e0a 0974  .__main__:run..t
+00000280: 6573 7462 656e 6368 3272 6f62 6f74 6672  estbench2robotfr
+00000290: 616d 6577 6f72 6b20 3d20 7465 7374 6265  amework = testbe
+000002a0: 6e63 6832 726f 626f 7466 7261 6d65 776f  nch2robotframewo
+000002b0: 726b 2e5f 5f6d 6169 6e5f 5f3a 7275 6e0a  rk.__main__:run.
+000002c0: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+000002d0: 5f72 6571 7569 7265 5d0a 6465 7620 3d20  _require].dev = 
+000002e0: 0a09 626c 6163 6b0a 0966 6c61 6b65 380a  ..black..flake8.
+000002f0: 0970 796c 696e 740a 096d 7970 790a 0970  .pylint..mypy..p
+00000300: 7974 6573 740a 0970 7974 6573 742d 636f  ytest..pytest-co
+00000310: 760a 0970 7974 6573 742d 7370 6563 0a09  v..pytest-spec..
+00000320: 6368 6563 6b2d 6d61 6e69 6665 7374 0a09  check-manifest..
+00000330: 7477 696e 650a 0977 6865 656c 0a09 7365  twine..wheel..se
+00000340: 7475 7074 6f6f 6c73 0a0a 5b6f 7074 696f  tuptools..[optio
+00000350: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+00000360: 5d0a 6578 636c 7564 6520 3d20 0a09 7465  ].exclude = ..te
+00000370: 7374 730a 0a5b 6567 675f 696e 666f 5d0a  sts..[egg_info].
+00000380: 7461 675f 6275 696c 6420 3d20 0a74 6167  tag_build = .tag
+00000390: 5f64 6174 6520 3d20 300a 0a              _date = 0..
```

### Comparing `testbench2robotframework-0.5.2/testbench2robotframework/__init__.py` & `testbench2robotframework-0.6.0/testbench2robotframework/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Copyright 2022-     imbus AG
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from .testbench2robotframework import testbench2robotframework  # noqa: F401
-
-__version__ = "0.5.2"
+# Copyright 2022-     imbus AG
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from .testbench2robotframework import testbench2robotframework  # noqa: F401
+
+__version__ = "0.6.0"
```

### Comparing `testbench2robotframework-0.5.2/testbench2robotframework/__main__.py` & `testbench2robotframework-0.6.0/testbench2robotframework/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# Copyright 2022-     imbus AG
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-import sys
-from os import path
-
-import robot
-
-from testbench2robotframework import __version__
-
-from .config import write_default_config
-from .json_reader import read_json
-from .robotframework2testbench import robot2testbench
-from .testbench2robotframework import testbench2robotframework
-from .utils import arg_parser
-
-
-def run():
-    args = arg_parser.parse_args()
-    if args.subcommand is None and not args.version:
-        arg_parser.print_help()
-        sys.exit()
-    if args.version:
-        print_version()
-        sys.exit()
-    if not path.isfile(args.config):
-        write_default_config(args.config)
-    configuration = read_json(args.config)
-    if args.subcommand == 'write':
-        testbench2robotframework(args.jsonReport[0], configuration)
-    elif args.subcommand == 'read':
-        robot2testbench(args.jsonReport[0], args.output, args.result, configuration)
-
-
-def print_version():
-    print(
-        f'TestBench2RobotFramework {__version__} with '
-        f'[Robot Framework {robot.version.get_full_version()}]'
-    )
-
-
-if __name__ == "__main__":
-    run()
+# Copyright 2022-     imbus AG
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+import sys
+from pathlib import Path
+
+import robot
+
+from testbench2robotframework import __version__
+
+from .config import write_default_config
+from .json_reader import read_json
+from .robotframework2testbench import robot2testbench
+from .testbench2robotframework import testbench2robotframework
+from .utils import arg_parser
+
+
+def run():
+    args = arg_parser.parse_args()
+    if args.subcommand is None and not args.version:
+        arg_parser.print_help()
+        sys.exit()
+    if args.version:
+        print_version()
+        sys.exit()
+    if not Path(args.config).is_file():
+        write_default_config(args.config)
+    configuration = read_json(args.config)
+    if args.subcommand == 'write':
+        testbench2robotframework(args.jsonReport[0], configuration)
+    elif args.subcommand == 'read':
+        robot2testbench(args.jsonReport[0], args.output, args.result, configuration)
+
+
+def print_version():
+    print(  # noqa: T201
+        f'TestBench2RobotFramework {__version__} with '
+        f'[Robot Framework {robot.version.get_full_version()}]'
+    )
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `testbench2robotframework-0.5.2/testbench2robotframework/config.py` & `testbench2robotframework-0.6.0/testbench2robotframework/config.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-# pylint: skip-file
-from __future__ import annotations
-
-import json
-from dataclasses import dataclass
-from typing import Dict, List, Union
-
-from .model import StrEnum
-
-
-@dataclass
-class SubdivisionsMapping:
-    libraries: Dict
-    resources: Dict
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            libraries=dictionary.get("libraries", {}), resources=dictionary.get("resources", {})
-        )
-
-
-@dataclass
-class ForcedImport:
-    libraries: List[str]
-    resources: List[str]
-    variables: List[str]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            libraries=dictionary.get("libraries", []),
-            resources=dictionary.get("resources", []),
-            variables=dictionary.get("variables", []),
-        )
-
-
-class LogLevel(StrEnum):
-    CRITICAL = "CRITICAL"
-    FATAL = CRITICAL
-    ERROR = "ERROR"
-    WARNING = "WARNING"
-    WARN = WARNING
-    INFO = "INFO"
-    DEBUG = "DEBUG"
-    NOTSET = "NOTSET"
-
-
-@dataclass
-class ConsoleLoggerConfig:
-    logLevel: LogLevel
-    logFormat: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        log_level = dictionary.get("logLevel", "INFO").upper()
-        if log_level not in LogLevel.__members__:
-            print(
-                f"ValueError: {log_level} is not a valid logLevel. "
-                f"Available logLevel are: {list(LogLevel.__members__)}"
-            )
-            log_level = LogLevel.INFO
-        return cls(
-            logLevel=LogLevel(log_level),
-            logFormat=dictionary.get("logFormat", "%(levelname)s: %(message)s"),
-        )
-
-
-@dataclass
-class FileLoggerConfig(ConsoleLoggerConfig):
-    fileName: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        log_level = dictionary.get("logLevel", "DEBUG").upper()
-        if log_level not in LogLevel.__members__:
-            print(
-                f"ValueError: {log_level} is not a valid logLevel. "
-                f"Available logLevel are: {list(LogLevel.__members__)}"
-            )
-            log_level = LogLevel.DEBUG
-        return cls(
-            logLevel=log_level,
-            logFormat=dictionary.get(
-                "logFormat", "%(asctime)s - %(filename)s:%(lineno)d - %(levelname)8s - %(message)s"
-            ),
-            fileName=dictionary.get("fileName", "testbench2robotframework.log"),
-        )
-
-
-@dataclass
-class LoggingConfig:
-    console: ConsoleLoggerConfig
-    file: FileLoggerConfig
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            console=ConsoleLoggerConfig.from_dict(dictionary.get("console", {})),
-            file=FileLoggerConfig.from_dict(dictionary.get("file", {})),
-        )
-
-
-class ReferenceBehaviour(StrEnum):
-    ATTACHMENT = "ATTACHMENT"
-    REFERENCE = "REFERENCE"
-    NONE = "NONE"
-
-
-class AttachmentConflictBehaviour(StrEnum):
-    ERROR = "ERROR"
-    USE_NEW = "USE_NEW"
-    USE_EXISTING = "USE_EXISTING"
-    RENAME_NEW = "RENAME_NEW"
-
-
-@dataclass
-class Configuration:
-    rfLibraryRegex: List[str]
-    rfResourceRegex: List[str]
-    rfLibraryRoots: List[str]
-    rfResourceRoots: List[str]
-    fullyQualified: bool
-    subdivisionsMapping: SubdivisionsMapping
-    forcedImport: ForcedImport
-    generationDirectory: str
-    createOutputZip: bool
-    resourceDirectory: str
-    logSuiteNumbering: bool
-    clearGenerationDirectory: bool
-    loggingConfiguration: LoggingConfig
-    logCompoundInteractions: bool
-    testCaseSplitPathRegEx: str
-    phasePattern: str
-    referenceBehaviour: ReferenceBehaviour
-    attachmentConflictBehaviour: AttachmentConflictBehaviour
-
-    @classmethod
-    def from_dict(cls, dictionary) -> Configuration:
-        return cls(
-            rfLibraryRegex=dictionary.get(
-                "rfLibraryRegex", [r"(?:.*\.)?(?P<resourceName>[^.]+?)\s*\[Robot-Library\].*"]
-            ),
-            rfResourceRegex=dictionary.get(
-                "rfResourceRegex", [r"(?:.*\.)?(?P<resourceName>[^.]+?)\s*\[Robot-Resource\].*"]
-            ),
-            rfLibraryRoots=dictionary.get("rfLibraryRoots", ["RF", "RF-Library"]),
-            rfResourceRoots=dictionary.get("rfResourceRoots", ["RF-Resource"]),
-            fullyQualified=dictionary.get("fullyQualified", False),
-            subdivisionsMapping=SubdivisionsMapping.from_dict(
-                dictionary.get("subdivisionsMapping", {})
-            ),
-            forcedImport=ForcedImport.from_dict(dictionary.get("forcedImport", {})),
-            generationDirectory=dictionary.get("generationDirectory", "{root}/Generated"),
-            createOutputZip=dictionary.get("createOutputZip", False),
-            logSuiteNumbering=dictionary.get("logSuiteNumbering", False),
-            clearGenerationDirectory=dictionary.get("clearGenerationDirectory", True),
-            loggingConfiguration=LoggingConfig.from_dict(
-                dictionary.get("loggingConfiguration", {})
-            ),
-            logCompoundInteractions=dictionary.get("logCompoundInteractions", True),
-            resourceDirectory=dictionary.get("resourceDirectory", "{root}/Resources").replace(
-                '\\', '/'
-            ),
-            testCaseSplitPathRegEx=dictionary.get("testCaseSplitPathRegEx", ".*StopWithRestart.*"),
-            phasePattern=dictionary.get("phasePattern", "{testcase} : Phase {index}/{length}"),
-            referenceBehaviour=ReferenceBehaviour(
-                dictionary.get("referenceBehaviour", "ATTACHMENT").upper()
-            ),
-            attachmentConflictBehaviour=AttachmentConflictBehaviour(
-                dictionary.get("attachmentConflictBehaviour", "USE_EXISTING").upper()
-            ),
-        )
-
-
-def write_default_config(config_file):
-    with open(config_file, 'w', encoding='utf-8') as file:
-        json.dump(
-            Configuration.from_dict({}).__dict__,
-            file,
-            default=lambda o: o.__dict__,
-            indent=2,
-        )
+# pylint: skip-file
+from __future__ import annotations
+
+import json
+from dataclasses import dataclass
+from typing import Dict, List, Union
+
+from .model import StrEnum
+
+
+@dataclass
+class SubdivisionsMapping:
+    libraries: Dict
+    resources: Dict
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            libraries=dictionary.get("libraries", {}), resources=dictionary.get("resources", {})
+        )
+
+
+@dataclass
+class ForcedImport:
+    libraries: List[str]
+    resources: List[str]
+    variables: List[str]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            libraries=dictionary.get("libraries", []),
+            resources=dictionary.get("resources", []),
+            variables=dictionary.get("variables", []),
+        )
+
+
+class LogLevel(StrEnum):
+    CRITICAL = "CRITICAL"
+    FATAL = CRITICAL
+    ERROR = "ERROR"
+    WARNING = "WARNING"
+    WARN = WARNING
+    INFO = "INFO"
+    DEBUG = "DEBUG"
+    NOTSET = "NOTSET"
+
+
+@dataclass
+class ConsoleLoggerConfig:
+    logLevel: LogLevel
+    logFormat: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        log_level = dictionary.get("logLevel", "INFO").upper()
+        if log_level not in LogLevel.__members__:
+            print(
+                f"ValueError: {log_level} is not a valid logLevel. "
+                f"Available logLevel are: {list(LogLevel.__members__)}"
+            )
+            log_level = LogLevel.INFO
+        return cls(
+            logLevel=LogLevel(log_level),
+            logFormat=dictionary.get("logFormat", "%(levelname)s: %(message)s"),
+        )
+
+
+@dataclass
+class FileLoggerConfig(ConsoleLoggerConfig):
+    fileName: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        log_level = dictionary.get("logLevel", "DEBUG").upper()
+        if log_level not in LogLevel.__members__:
+            print(
+                f"ValueError: {log_level} is not a valid logLevel. "
+                f"Available logLevel are: {list(LogLevel.__members__)}"
+            )
+            log_level = LogLevel.DEBUG
+        return cls(
+            logLevel=log_level,
+            logFormat=dictionary.get(
+                "logFormat", "%(asctime)s - %(filename)s:%(lineno)d - %(levelname)8s - %(message)s"
+            ),
+            fileName=dictionary.get("fileName", "testbench2robotframework.log"),
+        )
+
+
+@dataclass
+class LoggingConfig:
+    console: ConsoleLoggerConfig
+    file: FileLoggerConfig
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            console=ConsoleLoggerConfig.from_dict(dictionary.get("console", {})),
+            file=FileLoggerConfig.from_dict(dictionary.get("file", {})),
+        )
+
+
+class ReferenceBehaviour(StrEnum):
+    ATTACHMENT = "ATTACHMENT"
+    REFERENCE = "REFERENCE"
+    NONE = "NONE"
+
+
+class AttachmentConflictBehaviour(StrEnum):
+    ERROR = "ERROR"
+    USE_NEW = "USE_NEW"
+    USE_EXISTING = "USE_EXISTING"
+    RENAME_NEW = "RENAME_NEW"
+
+
+@dataclass
+class Configuration:
+    rfLibraryRegex: List[str]
+    rfResourceRegex: List[str]
+    rfLibraryRoots: List[str]
+    rfResourceRoots: List[str]
+    fullyQualified: bool
+    subdivisionsMapping: SubdivisionsMapping
+    forcedImport: ForcedImport
+    generationDirectory: str
+    createOutputZip: bool
+    resourceDirectory: str
+    logSuiteNumbering: bool
+    clearGenerationDirectory: bool
+    loggingConfiguration: LoggingConfig
+    logCompoundInteractions: bool
+    testCaseSplitPathRegEx: str
+    phasePattern: str
+    referenceBehaviour: ReferenceBehaviour
+    attachmentConflictBehaviour: AttachmentConflictBehaviour
+
+    @classmethod
+    def from_dict(cls, dictionary) -> Configuration:
+        return cls(
+            rfLibraryRegex=dictionary.get(
+                "rfLibraryRegex", [r"(?:.*\.)?(?P<resourceName>[^.]+?)\s*\[Robot-Library\].*"]
+            ),
+            rfResourceRegex=dictionary.get(
+                "rfResourceRegex", [r"(?:.*\.)?(?P<resourceName>[^.]+?)\s*\[Robot-Resource\].*"]
+            ),
+            rfLibraryRoots=dictionary.get("rfLibraryRoots", ["RF", "RF-Library"]),
+            rfResourceRoots=dictionary.get("rfResourceRoots", ["RF-Resource"]),
+            fullyQualified=dictionary.get("fullyQualified", False),
+            subdivisionsMapping=SubdivisionsMapping.from_dict(
+                dictionary.get("subdivisionsMapping", {})
+            ),
+            forcedImport=ForcedImport.from_dict(dictionary.get("forcedImport", {})),
+            generationDirectory=dictionary.get("generationDirectory", "{root}/Generated"),
+            createOutputZip=dictionary.get("createOutputZip", False),
+            logSuiteNumbering=dictionary.get("logSuiteNumbering", False),
+            clearGenerationDirectory=dictionary.get("clearGenerationDirectory", True),
+            loggingConfiguration=LoggingConfig.from_dict(
+                dictionary.get("loggingConfiguration", {})
+            ),
+            logCompoundInteractions=dictionary.get("logCompoundInteractions", True),
+            resourceDirectory=dictionary.get("resourceDirectory", "{root}/Resources").replace(
+                '\\', '/'
+            ),
+            testCaseSplitPathRegEx=dictionary.get("testCaseSplitPathRegEx", ".*StopWithRestart.*"),
+            phasePattern=dictionary.get("phasePattern", "{testcase} : Phase {index}/{length}"),
+            referenceBehaviour=ReferenceBehaviour(
+                dictionary.get("referenceBehaviour", "ATTACHMENT").upper()
+            ),
+            attachmentConflictBehaviour=AttachmentConflictBehaviour(
+                dictionary.get("attachmentConflictBehaviour", "USE_EXISTING").upper()
+            ),
+        )
+
+
+def write_default_config(config_file):
+    with open(config_file, 'w', encoding='utf-8') as file:
+        json.dump(
+            Configuration.from_dict({}).__dict__,
+            file,
+            default=lambda o: o.__dict__,
+            indent=2,
+        )
```

### Comparing `testbench2robotframework-0.5.2/testbench2robotframework/json_reader.py` & `testbench2robotframework-0.6.0/testbench2robotframework/json_reader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import json
-import sys
-from dataclasses import dataclass
-from json import JSONDecodeError
-from os import path
-from typing import Dict, List, Optional
-
-from .log import logger
-from .model import (
-    TestCaseDetails,
-    TestCaseSetDetails,
-    TestStructureTree,
-    TestStructureTreeNodeType,
-)
-
-TEST_STRUCTURE_TREE_FILE = "TestThemeTree.json"
-
-
-@dataclass
-class TestCaseSet:
-    details: TestCaseSetDetails
-    test_cases: Dict[str, TestCaseDetails]
-
-    @property
-    def metadata(self) -> Dict[str, str]:
-        return {
-            "UniqueID": self.details.uniqueID,
-            "Name": self.details.name,
-            "Numbering": self.details.numbering,
-        }
-
-
-class TestBenchJsonReader:
-    def __init__(self, json_dir):
-        self.json_dir = json_dir
-        self._test_theme_tree: Optional[TestStructureTree] = None
-        self._test_case_sets: Dict[str, TestCaseSetDetails] = {}
-        self._test_cases: Dict[str, TestCaseDetails] = {}
-        if not json_dir:
-            logger.warning("No jsonReport path given.")
-            sys.exit()
-
-    @property
-    def test_theme_tree(self) -> TestStructureTree:
-        if not self._test_theme_tree:
-            test_theme_path = path.join(self.json_dir, TEST_STRUCTURE_TREE_FILE)
-            logger.debug(f"Loading TestThemeTree from {test_theme_path}")
-            test_structure_tree = read_json(test_theme_path)
-            self._test_theme_tree = TestStructureTree.from_dict(test_structure_tree)
-            logger.info(f"{len(self._test_theme_tree.nodes)} nodes from TestThemeTree loaded.")
-        return self._test_theme_tree
-
-    @property
-    def test_case_sets(self) -> Dict[str, TestCaseSetDetails]:
-        if not self._test_case_sets:
-            for tcs_uid in self.get_test_case_set_uids():
-                test_case_set = self.read_test_case_set(tcs_uid)
-                if test_case_set is not None:
-                    self._test_case_sets[tcs_uid] = test_case_set
-                    logger.debug(f"TestCaseSetDetails {tcs_uid} loaded.")
-                else:
-                    logger.debug(f"TestCaseSetDetails {tcs_uid} not found.")
-            logger.info(f"{len(self._test_case_sets)} TestCaseSetDetails loaded.")
-        return self._test_case_sets
-
-    @property
-    def test_cases(self) -> Dict[str, TestCaseDetails]:
-        if not self._test_cases:
-            for tcs_uid in self.test_case_sets:
-                tc_uids = self.get_test_case_uids(tcs_uid)
-                self._read_test_cases(tc_uids)
-        return self._test_cases
-
-    def _read_test_cases(self, tc_uids):
-        for tc_uid in tc_uids:
-            test_case = self.read_test_case(tc_uid)
-            if test_case is not None:
-                self._test_cases[tc_uid] = test_case
-                logger.debug(f"TestCaseDetails {tc_uid} loaded.")
-
-    def get_test_case_set_catalog(self):
-        tcs_catalog: Dict[str, TestCaseSet] = {}
-        for tcs_uid, tcs in self.test_case_sets.items():
-            tc_catalog: Dict[str, TestCaseDetails] = {}
-            for tc_uid in self.get_test_case_uids(tcs_uid):
-                tc_catalog[tc_uid] = self.test_cases[tc_uid]
-            tcs_catalog[tcs_uid] = TestCaseSet(tcs, tc_catalog)
-        return tcs_catalog
-
-    def get_test_case_set_uids(self) -> List[str]:
-        nodes = self.test_theme_tree.nodes
-        return [
-            tse.baseInformation.uniqueID
-            for tse in nodes
-            if tse.elementType == TestStructureTreeNodeType.TestCaseSet
-        ]
-
-    def get_test_case_uids(self, test_case_set_uid: str) -> List[str]:
-        if not self._test_case_sets:
-            test_case_set = self.read_test_case_set(test_case_set_uid)
-            if test_case_set is None:
-                logger.debug(f"TestCaseSet with uid '{test_case_set_uid}' not found.")
-                return []
-        else:
-            test_case_set = self.test_case_sets[test_case_set_uid]
-        return [tc.uniqueID for tc in test_case_set.testCases]
-
-    def read_test_case_set(self, uid) -> Optional[TestCaseSetDetails]:
-        tcs_dict = read_json(path.join(self.json_dir, f"{uid}.json"))
-        if tcs_dict is None:
-            return None
-        return TestCaseSetDetails.from_dict(tcs_dict)
-
-    def read_test_case(self, uid) -> Optional[TestCaseDetails]:
-        tc_dict = read_json(path.join(self.json_dir, f"{uid}.json"))
-        if tc_dict is None:
-            return None
-        return TestCaseDetails.from_dict(tc_dict)
-
-    def read_test_theme_tree(self) -> Optional[TestStructureTree]:
-        test_structure_tree = read_json(path.join(self.json_dir, TEST_STRUCTURE_TREE_FILE))
-        if test_structure_tree is None:
-            return None
-        return TestStructureTree.from_dict(test_structure_tree)
-
-
-def read_json(filepath: str):  # ToDo Configure to run silent or raise
-    try:
-        with open(filepath, encoding='utf-8') as json_file:
-            return json.load(json_file)
-    except FileNotFoundError:
-        logger.debug(f"Cannot find json file {filepath}:")
-        return None
-    except JSONDecodeError as error:  # pylint: disable=broad-except
-        logger.warning(f"Cannot decode json file {filepath}:")
-        logger.warning(error)
-        return None
+import json
+import sys
+from dataclasses import dataclass
+from json import JSONDecodeError
+from pathlib import Path
+from typing import Dict, List, Optional
+
+from .log import logger
+from .model import (
+    TestCaseDetails,
+    TestCaseSetDetails,
+    TestStructureTree,
+    TestStructureTreeNodeType,
+)
+
+TEST_STRUCTURE_TREE_FILE = "TestThemeTree.json"
+
+
+@dataclass
+class TestCaseSet:
+    details: TestCaseSetDetails
+    test_cases: Dict[str, TestCaseDetails]
+
+    @property
+    def metadata(self) -> Dict[str, str]:
+        return {
+            "UniqueID": self.details.uniqueID,
+            "Name": self.details.name,
+            "Numbering": self.details.numbering,
+        }
+
+
+class TestBenchJsonReader:
+    def __init__(self, json_dir):
+        self.json_dir = json_dir
+        self._test_theme_tree: Optional[TestStructureTree] = None
+        self._test_case_sets: Dict[str, TestCaseSetDetails] = {}
+        self._test_cases: Dict[str, TestCaseDetails] = {}
+        if not json_dir:
+            logger.warning("No jsonReport path given.")
+            sys.exit()
+
+    @property
+    def test_theme_tree(self) -> TestStructureTree:
+        if not self._test_theme_tree:
+            test_theme_path = Path(self.json_dir) / TEST_STRUCTURE_TREE_FILE
+            logger.debug(f"Loading TestThemeTree from {test_theme_path}")
+            test_structure_tree = read_json(str(test_theme_path))
+            self._test_theme_tree = TestStructureTree.from_dict(test_structure_tree)
+            logger.info(f"{len(self._test_theme_tree.nodes)} nodes from TestThemeTree loaded.")
+        return self._test_theme_tree
+
+    @property
+    def test_case_sets(self) -> Dict[str, TestCaseSetDetails]:
+        if not self._test_case_sets:
+            for tcs_uid in self.get_test_case_set_uids():
+                test_case_set = self.read_test_case_set(tcs_uid)
+                if test_case_set is not None:
+                    self._test_case_sets[tcs_uid] = test_case_set
+                    logger.debug(f"TestCaseSetDetails {tcs_uid} loaded.")
+                else:
+                    logger.debug(f"TestCaseSetDetails {tcs_uid} not found.")
+            logger.info(f"{len(self._test_case_sets)} TestCaseSetDetails loaded.")
+        return self._test_case_sets
+
+    @property
+    def test_cases(self) -> Dict[str, TestCaseDetails]:
+        if not self._test_cases:
+            for tcs_uid in self.test_case_sets:
+                tc_uids = self.get_test_case_uids(tcs_uid)
+                self._read_test_cases(tc_uids)
+        return self._test_cases
+
+    def _read_test_cases(self, tc_uids):
+        for tc_uid in tc_uids:
+            test_case = self.read_test_case(tc_uid)
+            if test_case is not None:
+                self._test_cases[tc_uid] = test_case
+                logger.debug(f"TestCaseDetails {tc_uid} loaded.")
+
+    def get_test_case_set_catalog(self):
+        tcs_catalog: Dict[str, TestCaseSet] = {}
+        for tcs_uid, tcs in self.test_case_sets.items():
+            tc_catalog: Dict[str, TestCaseDetails] = {}
+            for tc_uid in self.get_test_case_uids(tcs_uid):
+                tc_catalog[tc_uid] = self.test_cases[tc_uid]
+            tcs_catalog[tcs_uid] = TestCaseSet(tcs, tc_catalog)
+        return tcs_catalog
+
+    def get_test_case_set_uids(self) -> List[str]:
+        nodes = self.test_theme_tree.nodes
+        return [
+            tse.baseInformation.uniqueID
+            for tse in nodes
+            if tse.elementType == TestStructureTreeNodeType.TestCaseSet
+        ]
+
+    def get_test_case_uids(self, test_case_set_uid: str) -> List[str]:
+        if not self._test_case_sets:
+            test_case_set = self.read_test_case_set(test_case_set_uid)
+            if test_case_set is None:
+                logger.debug(f"TestCaseSet with uid '{test_case_set_uid}' not found.")
+                return []
+        else:
+            test_case_set = self.test_case_sets[test_case_set_uid]
+        return [tc.uniqueID for tc in test_case_set.testCases]
+
+    def read_test_case_set(self, uid) -> Optional[TestCaseSetDetails]:
+        tcs_dict = read_json(str(Path(self.json_dir, f"{uid}.json")))
+        if tcs_dict is None:
+            return None
+        return TestCaseSetDetails.from_dict(tcs_dict)
+
+    def read_test_case(self, uid) -> Optional[TestCaseDetails]:
+        tc_dict = read_json(str(Path(self.json_dir, f"{uid}.json")))
+        if tc_dict is None:
+            return None
+        return TestCaseDetails.from_dict(tc_dict)
+
+    def read_test_theme_tree(self) -> Optional[TestStructureTree]:
+        test_structure_tree = read_json(str(Path(self.json_dir, TEST_STRUCTURE_TREE_FILE)))
+        if test_structure_tree is None:
+            return None
+        return TestStructureTree.from_dict(test_structure_tree)
+
+
+def read_json(filepath: str):  # ToDo Configure to run silent or raise
+    try:
+        with Path(filepath).open(encoding='utf-8') as json_file:
+            return json.load(json_file)
+    except FileNotFoundError:
+        logger.debug(f"Cannot find json file {filepath}:")
+        return None
+    except JSONDecodeError as error:  # pylint: disable=broad-except
+        logger.warning(f"Cannot decode json file {filepath}:")
+        logger.warning(error)
+        return None
```

### Comparing `testbench2robotframework-0.5.2/testbench2robotframework/log.py` & `testbench2robotframework-0.6.0/testbench2robotframework/log.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import logging
-from logging.handlers import RotatingFileHandler
-
-from .config import Configuration
-
-logger = logging.Logger("iTB2RF", logging.DEBUG)
-
-
-def setup_logger(config: Configuration):
-    console_handler = logging.StreamHandler()
-    console_handler.setLevel(config.loggingConfiguration.console.logLevel)
-    console_handler.setFormatter(logging.Formatter(config.loggingConfiguration.console.logFormat))
-    logger.addHandler(console_handler)
-
-    file_handler = RotatingFileHandler(
-        filename=config.loggingConfiguration.file.fileName,
-        mode="a",
-        maxBytes=1 * 1024 * 1024,
-        backupCount=2,
-        encoding="utf_8",
-        delay=False,
-    )
-    file_handler.setLevel(config.loggingConfiguration.file.logLevel)
-    file_handler.setFormatter(logging.Formatter(config.loggingConfiguration.file.logFormat))
-    logger.addHandler(file_handler)
+import logging
+from logging.handlers import RotatingFileHandler
+
+from .config import Configuration
+
+logger = logging.Logger("iTB2RF", logging.DEBUG)
+
+
+def setup_logger(config: Configuration):
+    console_handler = logging.StreamHandler()
+    console_handler.setLevel(config.loggingConfiguration.console.logLevel)
+    console_handler.setFormatter(logging.Formatter(config.loggingConfiguration.console.logFormat))
+    logger.addHandler(console_handler)
+
+    file_handler = RotatingFileHandler(
+        filename=config.loggingConfiguration.file.fileName,
+        mode="a",
+        maxBytes=1 * 1024 * 1024,
+        backupCount=2,
+        encoding="utf_8",
+        delay=False,
+    )
+    file_handler.setLevel(config.loggingConfiguration.file.logLevel)
+    file_handler.setFormatter(logging.Formatter(config.loggingConfiguration.file.logFormat))
+    logger.addHandler(file_handler)
```

### Comparing `testbench2robotframework-0.5.2/testbench2robotframework/model.py` & `testbench2robotframework-0.6.0/testbench2robotframework/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,802 +1,802 @@
-# pylint: skip-file
-from __future__ import annotations
-
-from dataclasses import dataclass
-from enum import Enum, auto
-from optparse import Option
-from typing import List, Optional
-
-
-class StrEnum(str, Enum):
-    def __new__(cls, *args):
-        for arg in args:
-            if not isinstance(arg, (str, auto)):
-                raise TypeError(f"Values of StrEnums must be strings: {repr(arg)} is a {type(arg)}")
-        return super().__new__(cls, *args)
-
-    def __str__(self):
-        return self.value
-
-    def _generate_next_value_(name, *_):
-        return name
-
-
-class FilterType(StrEnum):
-    TestThemeFilter = "TestThemeFilter"
-    TestCaseSetFilter = "TestCaseSetFilter"
-    TestCaseFilter = "TestCaseFilter"
-
-
-class TestStructureTreeNodeType(StrEnum):
-    Root = "Root"
-    TestTheme = "TestTheme"
-    TestCaseSet = "TestCaseSet"
-
-
-class Priority(StrEnum):
-    High = "High"
-    Medium = "Medium"
-    Low = "Low"
-
-
-class ReferenceType(StrEnum):
-    Reference = "Reference"
-    Hyperlink = "Hyperlink"
-    Attachment = "Attachment"
-
-
-class SpecificationStatus(StrEnum):
-    NotPlanned = "NotPlanned"
-    Planned = "Planned"
-    InProgress = "InProgress"
-    InReview = "InReview"
-    Released = "Released"
-
-
-class InteractionVerdict(StrEnum):
-    Pass = "Pass"
-    Fail = "Fail"
-    Skipped = "Skipped"
-    ToVerify = "ToVerify"
-    Warn = "Warn"
-    Undefined = "Undefined"
-    Blocked = "Blocked"
-
-
-class ExecutionVerdict(StrEnum):
-    Undefined = "Undefined"
-    Pass = "Pass"
-    Fail = "Fail"
-    ToVerify = "ToVerify"
-
-
-class ActivityStatus(StrEnum):
-    NotPlanned = "NotPlanned"
-    Planned = "Planned"
-    Assigned = "Assigned"
-    Running = "Running"
-    Canceled = "Canceled"
-    Skipped = "Skipped"
-    Performed = "Performed"
-
-
-class ExecutionStatus(StrEnum):
-    NotBlocked = "NotBlocked"
-    Blocked = "Blocked"
-
-
-class UdfType(StrEnum):
-    String = "String"
-    Enumeration = "Enumeration"
-    Boolean = "Boolean"
-
-
-class SequencePhase(StrEnum):
-    Setup = "Setup"
-    TestStep = "TestStep"
-    Teardown = "Teardown"
-
-
-class CallType(StrEnum):
-    Check = "Check"
-    Flow = "Flow"
-
-
-class InteractionType(StrEnum):
-    Compound = "Compound"
-    Atomic = "Atomic"
-    Textuell = "Textuell"
-
-
-class ParameterType(StrEnum):
-    DetailedInstance = "DetailedInstance"
-    Unknown = "Unknown"
-    InstanceTable = "InstanceTable"
-    AtomicInstance = "AtomicInstance"
-
-
-class ParameterUseType(StrEnum):
-    CallByReference = "CallByReference"
-    CallByValue = "CallByValue"
-    CallByReferenceMandatory = "CallByReferenceMandatory"
-
-
-@dataclass
-class ProjectMember:
-    userkey: str
-    userLogin: str
-    userName: str
-    projectkey: str
-    projectName: str
-    roles: List[str]
-
-
-@dataclass
-class ProjectDetails:
-    key: str
-    creationTime: str
-    name: str
-    status: str
-    visibility: bool
-    tovsCount: int
-    cyclesCount: int
-    description: str
-    lockerKey: Optional[int] = None
-    startDate: Optional[str] = None
-    endDate: Optional[str] = None
-
-
-@dataclass
-class TOVDetails:
-    key: str
-    creationTime: str
-    name: str
-    status: str
-    visibility: bool
-    cyclesCount: int
-    description: str
-    lockerKey: Optional[int] = None
-    startDate: Optional[str] = None
-    endDate: Optional[str] = None
-
-
-@dataclass
-class CycleDetails:
-    key: str
-    creationTime: str
-    name: str
-    status: str
-    visibility: bool
-    description: str
-    startDate: Optional[str] = None
-    endDate: Optional[str] = None
-
-
-@dataclass
-class UserDetails:
-    key: str
-    login: str
-    name: str
-    email: str
-    passwordExpired: bool
-    active: bool
-
-
-@dataclass
-class UserSummary:
-    key: str
-    login: str
-    name: str
-    active: bool
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            login=dictionary.get("login", ""),
-            name=dictionary.get("name", ""),
-            active=dictionary.get("active", True),
-        )
-
-
-@dataclass
-class UserDefinedField:
-    key: str
-    name: str
-    value: str
-    valueType: UdfType
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            name=dictionary.get("name", ""),
-            value=dictionary.get("value", ""),
-            valueType=UdfType(dictionary.get("valueType", UdfType.String)),
-        )
-
-    @property
-    def robot_tag(self) -> Optional[str]:
-        if self.valueType == UdfType.Enumeration:
-            return f"{self.name}:{self.value}"
-        elif self.valueType == UdfType.String and self.value:
-            return f"{self.name}:{self.value}"
-        elif self.valueType == UdfType.Boolean and self.value == "true":
-            return self.name
-        return None
-
-
-@dataclass
-class Keyword:
-    key: str
-    name: str
-    isVariantsMarker: bool
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            name=dictionary.get("name", ""),
-            isVariantsMarker=dictionary.get("isVariantsMarker", False),
-        )
-
-
-@dataclass
-class Reference:
-    type: ReferenceType
-    path: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            type=ReferenceType(dictionary.get("type", ReferenceType.Reference)),
-            path=dictionary.get("path", ""),
-        )
-
-
-@dataclass
-class UserReference:
-    key: str
-    name: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(key=dictionary.get("key", ""), name=dictionary.get("name", ""))
-
-
-@dataclass
-class RequirementReference:
-    key: str
-    edited: bool
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(key=dictionary.get("key", ""), edited=dictionary.get("edited", False))
-
-
-@dataclass
-class ConditionSummary:
-    key: str
-    uniqueId: str
-    name: str
-    description: str
-    version: Optional[str] = None
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            uniqueId=dictionary.get("uniqueId", ""),
-            name=dictionary.get("name", ""),
-            description=dictionary.get("description", ""),
-            version=dictionary.get("version", None),
-        )
-
-
-@dataclass
-class TestCaseSetSpecificationSummary:
-    key: str
-    description: str
-    reviewComment: str
-    status: SpecificationStatus
-    priority: Optional[Priority]
-    responsible: Optional[UserReference]
-    dueDate: Optional[str]
-    reviewer: Optional[UserReference]
-    udfs: List[UserDefinedField]
-    keywords: List[Keyword]
-    references: List[Reference]
-    requirements: List[RequirementReference]
-    preConditions: List[ConditionSummary]
-    postConditions: List[ConditionSummary]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            description=dictionary.get("description", ""),
-            reviewComment=dictionary.get("reviewComment", ""),
-            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
-            priority=Priority(dictionary.get("priority")) if dictionary.get("priority") else None,
-            responsible=UserReference.from_dict(dictionary.get("responsible", {}))
-            if dictionary.get("responsible")
-            else None,
-            dueDate=dictionary.get("dueDate", None),
-            reviewer=UserReference.from_dict(dictionary.get("reviewer", {}))
-            if dictionary.get("reviewer")
-            else None,
-            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
-            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
-            references=dictionary.get("references", ""),
-            requirements=[
-                RequirementReference.from_dict(requirement)
-                for requirement in dictionary.get("requirements", [])
-            ],
-            preConditions=[
-                ConditionSummary.from_dict(condition)
-                for condition in dictionary.get("preConditions", [])
-            ],
-            postConditions=[
-                ConditionSummary.from_dict(condition)
-                for condition in dictionary.get("postConditions", [])
-            ],
-        )
-
-
-@dataclass
-class TestCaseSpecificationDetails:
-    key: str
-    comments: str
-    udfs: List[UserDefinedField]
-    keywords: List[Keyword]
-    requirements: List[RequirementReference]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            comments=dictionary.get("comments", ""),
-            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
-            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
-            requirements=[
-                RequirementReference.from_dict(requirement)
-                for requirement in dictionary.get("requirements", [])
-            ],
-        )
-
-
-@dataclass
-class TestCaseSetExecutionSummary:
-    key: str
-    comments: str
-    udfs: List[UserDefinedField]
-    keywords: List[Keyword]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            comments=dictionary.get("comments", ""),
-            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
-            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
-        )
-
-
-@dataclass
-class TestCaseSpecificationSummary:
-    key: str
-    comments: str
-    requirements: List[RequirementReference]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            comments=dictionary.get("comments", ""),
-            requirements=[
-                RequirementReference.from_dict(requirement)
-                for requirement in dictionary.get("requirements", [])
-            ],
-        )
-
-
-@dataclass
-class TestCaseExecutionSummary:
-    key: str
-    comments: str = ""
-    status: ActivityStatus = ActivityStatus.Planned
-    execStatus: ExecutionStatus = ExecutionStatus.NotBlocked
-    verdict: ExecutionVerdict = ExecutionVerdict.Undefined
-    defects: Optional[List[int]] = None
-    tester: Optional[UserReference] = None
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
-            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
-            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
-            comments=dictionary.get("comments", ""),
-            defects=dictionary.get("defects", []),
-            tester=UserReference.from_dict(dictionary.get("tester"))
-            if dictionary.get("tester")
-            else None,
-        )
-
-
-@dataclass
-class TestCaseSummary:
-    uniqueID: str
-    index: int
-    spec: TestCaseSpecificationSummary
-    exec: Optional[TestCaseExecutionSummary] = None
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            uniqueID=dictionary.get("uniqueID", ""),
-            index=dictionary.get("index", 0),
-            spec=TestCaseSpecificationSummary.from_dict(dictionary.get("spec", {})),
-            exec=TestCaseExecutionSummary.from_dict(dictionary.get("exec"))
-            if dictionary.get("exec")
-            else None,
-        )
-
-
-@dataclass
-class TestCaseExecutionDetails:
-    key: str
-    status: ActivityStatus
-    execStatus: ExecutionStatus
-    verdict: ExecutionVerdict
-    plannedDuration: int
-    actualDuration: int
-    currentUser: UserReference
-    tester: Optional[UserReference]
-    comments: str  # TODO: Insert htmlComment
-    version: Optional[str]
-    defects: List[int]
-    udfs: List[UserDefinedField]
-    keywords: List[Keyword]
-    references: List[Reference]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
-            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
-            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
-            plannedDuration=dictionary.get("plannedDuration", 0),
-            actualDuration=dictionary.get("actualDuration", 0),
-            currentUser=UserReference.from_dict(dictionary.get("currentUser", {})),
-            tester=UserReference.from_dict(dictionary.get("tester", {}))
-            if dictionary.get("tester")
-            else None,
-            comments=dictionary.get("comments", ""),
-            version=dictionary.get("version", None),
-            defects=dictionary.get("defects", []),
-            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
-            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
-            references=dictionary.get("references", []),
-        )
-
-
-@dataclass
-class TestCaseSetDetails:
-    key: str
-    numbering: str
-    uniqueID: str
-    name: str
-    spec: TestCaseSetSpecificationSummary
-    exec: Optional[TestCaseSetExecutionSummary]
-    testCases: List[TestCaseSummary]
-
-    @classmethod
-    def from_dict(cls, dictionary) -> TestCaseSetDetails:
-        return cls(
-            key=dictionary.get("key", ""),
-            numbering=dictionary.get("numbering", ""),
-            uniqueID=dictionary.get("uniqueID", ""),
-            name=dictionary.get("name", ""),
-            spec=TestCaseSetSpecificationSummary.from_dict(dictionary.get("spec", {})),
-            exec=TestCaseSetExecutionSummary.from_dict(dictionary.get("exec", {}))
-            if dictionary.get("exec")
-            else None,
-            testCases=[
-                TestCaseSummary.from_dict(test_case)
-                for test_case in dictionary.get("testCases", [])
-            ],
-        )
-
-
-@dataclass
-class InteractionExecutionSummary:
-    verdict: InteractionVerdict
-    time: str
-    duration: int
-    currentUser: UserReference
-    tester: UserReference
-    comments: str
-    references: List[Reference]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            verdict=InteractionVerdict(dictionary.get("verdict", InteractionVerdict.Undefined)),
-            time=dictionary.get("time", ""),
-            duration=dictionary.get("duration", 0),
-            currentUser=UserReference.from_dict(dictionary.get("currentUser", {})),
-            tester=UserReference.from_dict(dictionary.get("tester", {})),
-            comments=dictionary.get("comments", ""),
-            references=dictionary.get("references", []),
-        )
-
-
-@dataclass
-class InteractionSpecificationSummary:
-    callId: int
-    sequencePhase: SequencePhase
-    callType: CallType
-    description: str
-    comments: str
-    references: List[Reference]
-    preConditions: List[ConditionSummary]
-    postConditions: List[ConditionSummary]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            callId=dictionary.get("callId", ""),
-            sequencePhase=SequencePhase(dictionary.get("sequencePhase", SequencePhase.TestStep)),
-            callType=CallType(dictionary.get("callType", CallType.Flow)),
-            description=dictionary.get("description", ""),
-            comments=dictionary.get("comments", ""),
-            references=dictionary.get("references", ""),
-            preConditions=[
-                ConditionSummary.from_dict(condition)
-                for condition in dictionary.get("preConditions", [])
-            ],
-            postConditions=[
-                ConditionSummary.from_dict(condition)
-                for condition in dictionary.get("postConditions", [])
-            ],
-        )
-
-
-@dataclass
-class ParameterSummary:
-    name: str
-    value: str
-    version: Optional[str]
-    parameterType: ParameterType
-    parameterUseType: ParameterUseType
-    dataTypeName: str
-    dataTypePath: str
-    dataTypeUniqueID: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            name=dictionary.get("name", ""),
-            value=dictionary.get("value", ""),
-            version=dictionary.get(
-                "version",
-            ),
-            parameterType=ParameterType(
-                dictionary.get("parameterType", ParameterType.AtomicInstance)
-            ),
-            parameterUseType=ParameterUseType(
-                dictionary.get("parameterUseType", ParameterUseType.CallByValue)
-            ),
-            dataTypeName=dictionary.get("dataTypeName", ""),
-            dataTypePath=dictionary.get("dataTypePath", ""),
-            dataTypeUniqueID=dictionary.get("dataTypeUniqueID", ""),
-        )
-
-
-@dataclass
-class InteractionDetails:
-    key: str
-    uniqueID: str
-    name: str
-    version: Optional[str]
-    interactionType: InteractionType
-    path: str
-    spec: InteractionSpecificationSummary
-    exec: Optional[InteractionExecutionSummary]
-    parameters: List[ParameterSummary]
-    interactions: List[InteractionDetails]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            uniqueID=dictionary.get("uniqueID", ""),
-            name=dictionary.get("name", ""),
-            version=dictionary.get("version", ""),
-            interactionType=InteractionType(
-                dictionary.get("interactionType", InteractionType.Atomic)
-            ),
-            path=dictionary.get("path", ""),
-            spec=InteractionSpecificationSummary.from_dict(dictionary.get("spec")),
-            exec=InteractionExecutionSummary.from_dict(dictionary.get("exec"))
-            if dictionary.get("exec")
-            else None,
-            parameters=[
-                ParameterSummary.from_dict(param) for param in dictionary.get("parameters", [])
-            ],
-            interactions=[
-                InteractionDetails.from_dict(interaction)
-                for interaction in dictionary.get("interactions", [])
-            ],
-        )
-
-
-@dataclass
-class TestCaseDetails:
-    uniqueID: str
-    spec: TestCaseSpecificationDetails
-    exec: Optional[TestCaseExecutionDetails]
-    interactions: List[InteractionDetails]
-    parameters: List[ParameterSummary]
-
-    @classmethod
-    def from_dict(cls, dictionary) -> TestCaseDetails:
-        return cls(
-            uniqueID=dictionary.get("uniqueID"),
-            spec=TestCaseSpecificationDetails.from_dict(dictionary.get("spec")),
-            exec=TestCaseExecutionDetails.from_dict(dictionary.get("exec"))
-            if dictionary.get("exec")
-            else None,
-            interactions=[
-                InteractionDetails.from_dict(interaction)
-                for interaction in dictionary.get("interactions", [])
-            ],
-            parameters=[
-                ParameterSummary.from_dict(parameter)
-                for parameter in dictionary.get("parameters", [])
-            ],
-        )
-
-
-@dataclass
-class TestStructureSpecification:
-    key: str
-    locker: Optional[UserReference]
-    status: SpecificationStatus
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", "-1"),
-            locker=UserReference.from_dict(dictionary.get("locker", {}))
-            if dictionary.get("locker")
-            else None,
-            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
-        )
-
-
-@dataclass
-class TestStructureAutomation:
-    key: str
-    locker: Optional[UserReference]
-    status: SpecificationStatus
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", "-1"),
-            locker=UserReference.from_dict(dictionary.get("locker", {}))
-            if dictionary.get("locker")
-            else None,
-            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
-        )
-
-
-@dataclass
-class TestStructureExecution:
-    key: str
-    locker: Optional[UserReference]
-    status: ActivityStatus
-    execStatus: ExecutionStatus
-    verdict: ExecutionVerdict
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", "-1"),
-            locker=UserReference.from_dict(dictionary.get("locker", {}))
-            if dictionary.get("locker")
-            else None,
-            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
-            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
-            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
-        )
-
-
-@dataclass
-class AttachedFilter:
-    key: str
-    name: str
-    filterType: FilterType
-    content: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", "-1"),
-            name=dictionary.get("name", ""),
-            filterType=FilterType(dictionary.get("filterType", FilterType.TestCaseSetFilter)),
-            content=dictionary.get("content", ""),
-        )
-
-
-@dataclass
-class TestStructureTreeNodeInformation:
-    key: str
-    numbering: str
-    parentKey: str
-    name: str
-    uniqueID: str
-    orderPos: int
-    matchesFilter: bool
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", "-1"),
-            numbering=dictionary.get("numbering", "-1"),
-            parentKey=dictionary.get("parentKey", "-1"),
-            name=dictionary.get("name", ""),
-            uniqueID=dictionary.get("uniqueID", ""),
-            orderPos=dictionary.get("orderPos", "-1"),
-            matchesFilter=dictionary.get("matchesFilter", True),
-        )
-
-
-@dataclass
-class TestStructureTreeNode:
-    elementType: TestStructureTreeNodeType
-    baseInformation: TestStructureTreeNodeInformation
-    specification: Optional[TestStructureSpecification]
-    automation: Optional[TestStructureAutomation]
-    execution: Optional[TestStructureExecution]
-    filters: List[AttachedFilter]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            elementType=TestStructureTreeNodeType(
-                dictionary.get("elementType", TestStructureTreeNodeType.TestTheme)
-            ),
-            baseInformation=TestStructureTreeNodeInformation.from_dict(
-                dictionary.get("baseInformation", {})
-            ),
-            specification=TestStructureSpecification.from_dict(dictionary.get("specification"))
-            if dictionary.get("specification")
-            else None,
-            automation=TestStructureAutomation.from_dict(dictionary.get("automation"))
-            if dictionary.get("automation")
-            else None,
-            execution=TestStructureExecution.from_dict(dictionary.get("execution"))
-            if dictionary.get("execution")
-            else None,
-            filters=[AttachedFilter.from_dict(filter) for filter in dictionary.get("filters", [])],
-        )
-
-
-@dataclass
-class TestStructureTree:
-    root: TestStructureTreeNode
-    nodes: List[TestStructureTreeNode]
-
-    @classmethod
-    def from_dict(cls, dictionary) -> TestStructureTree:
-        return cls(
-            root=TestStructureTreeNode.from_dict(dictionary.get("root", {}))
-            if "root" in dictionary
-            else None,
-            nodes=[TestStructureTreeNode.from_dict(node) for node in dictionary.get("nodes", [])],
-        )
+# pylint: skip-file
+from __future__ import annotations
+
+from dataclasses import dataclass
+from enum import Enum, auto
+from optparse import Option
+from typing import List, Optional
+
+
+class StrEnum(str, Enum):
+    def __new__(cls, *args):
+        for arg in args:
+            if not isinstance(arg, (str, auto)):
+                raise TypeError(f"Values of StrEnums must be strings: {repr(arg)} is a {type(arg)}")
+        return super().__new__(cls, *args)
+
+    def __str__(self):
+        return self.value
+
+    def _generate_next_value_(name, *_):
+        return name
+
+
+class FilterType(StrEnum):
+    TestThemeFilter = "TestThemeFilter"
+    TestCaseSetFilter = "TestCaseSetFilter"
+    TestCaseFilter = "TestCaseFilter"
+
+
+class TestStructureTreeNodeType(StrEnum):
+    Root = "Root"
+    TestTheme = "TestTheme"
+    TestCaseSet = "TestCaseSet"
+
+
+class Priority(StrEnum):
+    High = "High"
+    Medium = "Medium"
+    Low = "Low"
+
+
+class ReferenceType(StrEnum):
+    Reference = "Reference"
+    Hyperlink = "Hyperlink"
+    Attachment = "Attachment"
+
+
+class SpecificationStatus(StrEnum):
+    NotPlanned = "NotPlanned"
+    Planned = "Planned"
+    InProgress = "InProgress"
+    InReview = "InReview"
+    Released = "Released"
+
+
+class InteractionVerdict(StrEnum):
+    Pass = "Pass"
+    Fail = "Fail"
+    Skipped = "Skipped"
+    ToVerify = "ToVerify"
+    Warn = "Warn"
+    Undefined = "Undefined"
+    Blocked = "Blocked"
+
+
+class ExecutionVerdict(StrEnum):
+    Undefined = "Undefined"
+    Pass = "Pass"
+    Fail = "Fail"
+    ToVerify = "ToVerify"
+
+
+class ActivityStatus(StrEnum):
+    NotPlanned = "NotPlanned"
+    Planned = "Planned"
+    Assigned = "Assigned"
+    Running = "Running"
+    Canceled = "Canceled"
+    Skipped = "Skipped"
+    Performed = "Performed"
+
+
+class ExecutionStatus(StrEnum):
+    NotBlocked = "NotBlocked"
+    Blocked = "Blocked"
+
+
+class UdfType(StrEnum):
+    String = "String"
+    Enumeration = "Enumeration"
+    Boolean = "Boolean"
+
+
+class SequencePhase(StrEnum):
+    Setup = "Setup"
+    TestStep = "TestStep"
+    Teardown = "Teardown"
+
+
+class CallType(StrEnum):
+    Check = "Check"
+    Flow = "Flow"
+
+
+class InteractionType(StrEnum):
+    Compound = "Compound"
+    Atomic = "Atomic"
+    Textuell = "Textuell"
+
+
+class ParameterType(StrEnum):
+    DetailedInstance = "DetailedInstance"
+    Unknown = "Unknown"
+    InstanceTable = "InstanceTable"
+    AtomicInstance = "AtomicInstance"
+
+
+class ParameterUseType(StrEnum):
+    CallByReference = "CallByReference"
+    CallByValue = "CallByValue"
+    CallByReferenceMandatory = "CallByReferenceMandatory"
+
+
+@dataclass
+class ProjectMember:
+    userkey: str
+    userLogin: str
+    userName: str
+    projectkey: str
+    projectName: str
+    roles: List[str]
+
+
+@dataclass
+class ProjectDetails:
+    key: str
+    creationTime: str
+    name: str
+    status: str
+    visibility: bool
+    tovsCount: int
+    cyclesCount: int
+    description: str
+    lockerKey: Optional[int] = None
+    startDate: Optional[str] = None
+    endDate: Optional[str] = None
+
+
+@dataclass
+class TOVDetails:
+    key: str
+    creationTime: str
+    name: str
+    status: str
+    visibility: bool
+    cyclesCount: int
+    description: str
+    lockerKey: Optional[int] = None
+    startDate: Optional[str] = None
+    endDate: Optional[str] = None
+
+
+@dataclass
+class CycleDetails:
+    key: str
+    creationTime: str
+    name: str
+    status: str
+    visibility: bool
+    description: str
+    startDate: Optional[str] = None
+    endDate: Optional[str] = None
+
+
+@dataclass
+class UserDetails:
+    key: str
+    login: str
+    name: str
+    email: str
+    passwordExpired: bool
+    active: bool
+
+
+@dataclass
+class UserSummary:
+    key: str
+    login: str
+    name: str
+    active: bool
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            login=dictionary.get("login", ""),
+            name=dictionary.get("name", ""),
+            active=dictionary.get("active", True),
+        )
+
+
+@dataclass
+class UserDefinedField:
+    key: str
+    name: str
+    value: str
+    valueType: UdfType
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            name=dictionary.get("name", ""),
+            value=dictionary.get("value", ""),
+            valueType=UdfType(dictionary.get("valueType", UdfType.String)),
+        )
+
+    @property
+    def robot_tag(self) -> Optional[str]:
+        if self.valueType == UdfType.Enumeration and self.value:
+            return f"{self.name}:{self.value}"
+        elif self.valueType == UdfType.String and self.value:
+            return f"{self.name}:{self.value}"
+        elif self.valueType == UdfType.Boolean and self.value == "true":
+            return self.name
+        return None
+
+
+@dataclass
+class Keyword:
+    key: str
+    name: str
+    isVariantsMarker: bool
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            name=dictionary.get("name", ""),
+            isVariantsMarker=dictionary.get("isVariantsMarker", False),
+        )
+
+
+@dataclass
+class Reference:
+    type: ReferenceType
+    path: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            type=ReferenceType(dictionary.get("type", ReferenceType.Reference)),
+            path=dictionary.get("path", ""),
+        )
+
+
+@dataclass
+class UserReference:
+    key: str
+    name: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(key=dictionary.get("key", ""), name=dictionary.get("name", ""))
+
+
+@dataclass
+class RequirementReference:
+    key: str
+    edited: bool
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(key=dictionary.get("key", ""), edited=dictionary.get("edited", False))
+
+
+@dataclass
+class ConditionSummary:
+    key: str
+    uniqueId: str
+    name: str
+    description: str
+    version: Optional[str] = None
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            uniqueId=dictionary.get("uniqueId", ""),
+            name=dictionary.get("name", ""),
+            description=dictionary.get("description", ""),
+            version=dictionary.get("version", None),
+        )
+
+
+@dataclass
+class TestCaseSetSpecificationSummary:
+    key: str
+    description: str
+    reviewComment: str
+    status: SpecificationStatus
+    priority: Optional[Priority]
+    responsible: Optional[UserReference]
+    dueDate: Optional[str]
+    reviewer: Optional[UserReference]
+    udfs: List[UserDefinedField]
+    keywords: List[Keyword]
+    references: List[Reference]
+    requirements: List[RequirementReference]
+    preConditions: List[ConditionSummary]
+    postConditions: List[ConditionSummary]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            description=dictionary.get("description", ""),
+            reviewComment=dictionary.get("reviewComment", ""),
+            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
+            priority=Priority(dictionary.get("priority")) if dictionary.get("priority") else None,
+            responsible=UserReference.from_dict(dictionary.get("responsible", {}))
+            if dictionary.get("responsible")
+            else None,
+            dueDate=dictionary.get("dueDate", None),
+            reviewer=UserReference.from_dict(dictionary.get("reviewer", {}))
+            if dictionary.get("reviewer")
+            else None,
+            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
+            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
+            references=dictionary.get("references", ""),
+            requirements=[
+                RequirementReference.from_dict(requirement)
+                for requirement in dictionary.get("requirements", [])
+            ],
+            preConditions=[
+                ConditionSummary.from_dict(condition)
+                for condition in dictionary.get("preConditions", [])
+            ],
+            postConditions=[
+                ConditionSummary.from_dict(condition)
+                for condition in dictionary.get("postConditions", [])
+            ],
+        )
+
+
+@dataclass
+class TestCaseSpecificationDetails:
+    key: str
+    comments: str
+    udfs: List[UserDefinedField]
+    keywords: List[Keyword]
+    requirements: List[RequirementReference]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            comments=dictionary.get("comments", ""),
+            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
+            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
+            requirements=[
+                RequirementReference.from_dict(requirement)
+                for requirement in dictionary.get("requirements", [])
+            ],
+        )
+
+
+@dataclass
+class TestCaseSetExecutionSummary:
+    key: str
+    comments: str
+    udfs: List[UserDefinedField]
+    keywords: List[Keyword]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            comments=dictionary.get("comments", ""),
+            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
+            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
+        )
+
+
+@dataclass
+class TestCaseSpecificationSummary:
+    key: str
+    comments: str
+    requirements: List[RequirementReference]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            comments=dictionary.get("comments", ""),
+            requirements=[
+                RequirementReference.from_dict(requirement)
+                for requirement in dictionary.get("requirements", [])
+            ],
+        )
+
+
+@dataclass
+class TestCaseExecutionSummary:
+    key: str
+    comments: str = ""
+    status: ActivityStatus = ActivityStatus.Planned
+    execStatus: ExecutionStatus = ExecutionStatus.NotBlocked
+    verdict: ExecutionVerdict = ExecutionVerdict.Undefined
+    defects: Optional[List[int]] = None
+    tester: Optional[UserReference] = None
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
+            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
+            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
+            comments=dictionary.get("comments", ""),
+            defects=dictionary.get("defects", []),
+            tester=UserReference.from_dict(dictionary.get("tester"))
+            if dictionary.get("tester")
+            else None,
+        )
+
+
+@dataclass
+class TestCaseSummary:
+    uniqueID: str
+    index: int
+    spec: TestCaseSpecificationSummary
+    exec: Optional[TestCaseExecutionSummary] = None
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            uniqueID=dictionary.get("uniqueID", ""),
+            index=dictionary.get("index", 0),
+            spec=TestCaseSpecificationSummary.from_dict(dictionary.get("spec", {})),
+            exec=TestCaseExecutionSummary.from_dict(dictionary.get("exec"))
+            if dictionary.get("exec")
+            else None,
+        )
+
+
+@dataclass
+class TestCaseExecutionDetails:
+    key: str
+    status: ActivityStatus
+    execStatus: ExecutionStatus
+    verdict: ExecutionVerdict
+    plannedDuration: int
+    actualDuration: int
+    currentUser: UserReference
+    tester: Optional[UserReference]
+    comments: str  # TODO: Insert htmlComment
+    version: Optional[str]
+    defects: List[int]
+    udfs: List[UserDefinedField]
+    keywords: List[Keyword]
+    references: List[Reference]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
+            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
+            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
+            plannedDuration=dictionary.get("plannedDuration", 0),
+            actualDuration=dictionary.get("actualDuration", 0),
+            currentUser=UserReference.from_dict(dictionary.get("currentUser", {})),
+            tester=UserReference.from_dict(dictionary.get("tester", {}))
+            if dictionary.get("tester")
+            else None,
+            comments=dictionary.get("comments", ""),
+            version=dictionary.get("version", None),
+            defects=dictionary.get("defects", []),
+            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
+            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
+            references=dictionary.get("references", []),
+        )
+
+
+@dataclass
+class TestCaseSetDetails:
+    key: str
+    numbering: str
+    uniqueID: str
+    name: str
+    spec: TestCaseSetSpecificationSummary
+    exec: Optional[TestCaseSetExecutionSummary]
+    testCases: List[TestCaseSummary]
+
+    @classmethod
+    def from_dict(cls, dictionary) -> TestCaseSetDetails:
+        return cls(
+            key=dictionary.get("key", ""),
+            numbering=dictionary.get("numbering", ""),
+            uniqueID=dictionary.get("uniqueID", ""),
+            name=dictionary.get("name", ""),
+            spec=TestCaseSetSpecificationSummary.from_dict(dictionary.get("spec", {})),
+            exec=TestCaseSetExecutionSummary.from_dict(dictionary.get("exec", {}))
+            if dictionary.get("exec")
+            else None,
+            testCases=[
+                TestCaseSummary.from_dict(test_case)
+                for test_case in dictionary.get("testCases", [])
+            ],
+        )
+
+
+@dataclass
+class InteractionExecutionSummary:
+    verdict: InteractionVerdict
+    time: str
+    duration: int
+    currentUser: UserReference
+    tester: UserReference
+    comments: str
+    references: List[Reference]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            verdict=InteractionVerdict(dictionary.get("verdict", InteractionVerdict.Undefined)),
+            time=dictionary.get("time", ""),
+            duration=dictionary.get("duration", 0),
+            currentUser=UserReference.from_dict(dictionary.get("currentUser", {})),
+            tester=UserReference.from_dict(dictionary.get("tester", {})),
+            comments=dictionary.get("comments", ""),
+            references=dictionary.get("references", []),
+        )
+
+
+@dataclass
+class InteractionSpecificationSummary:
+    callId: int
+    sequencePhase: SequencePhase
+    callType: CallType
+    description: str
+    comments: str
+    references: List[Reference]
+    preConditions: List[ConditionSummary]
+    postConditions: List[ConditionSummary]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            callId=dictionary.get("callId", ""),
+            sequencePhase=SequencePhase(dictionary.get("sequencePhase", SequencePhase.TestStep)),
+            callType=CallType(dictionary.get("callType", CallType.Flow)),
+            description=dictionary.get("description", ""),
+            comments=dictionary.get("comments", ""),
+            references=dictionary.get("references", ""),
+            preConditions=[
+                ConditionSummary.from_dict(condition)
+                for condition in dictionary.get("preConditions", [])
+            ],
+            postConditions=[
+                ConditionSummary.from_dict(condition)
+                for condition in dictionary.get("postConditions", [])
+            ],
+        )
+
+
+@dataclass
+class ParameterSummary:
+    name: str
+    value: str
+    version: Optional[str]
+    parameterType: ParameterType
+    parameterUseType: ParameterUseType
+    dataTypeName: str
+    dataTypePath: str
+    dataTypeUniqueID: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            name=dictionary.get("name", ""),
+            value=dictionary.get("value", ""),
+            version=dictionary.get(
+                "version",
+            ),
+            parameterType=ParameterType(
+                dictionary.get("parameterType", ParameterType.AtomicInstance)
+            ),
+            parameterUseType=ParameterUseType(
+                dictionary.get("parameterUseType", ParameterUseType.CallByValue)
+            ),
+            dataTypeName=dictionary.get("dataTypeName", ""),
+            dataTypePath=dictionary.get("dataTypePath", ""),
+            dataTypeUniqueID=dictionary.get("dataTypeUniqueID", ""),
+        )
+
+
+@dataclass
+class InteractionDetails:
+    key: str
+    uniqueID: str
+    name: str
+    version: Optional[str]
+    interactionType: InteractionType
+    path: str
+    spec: InteractionSpecificationSummary
+    exec: Optional[InteractionExecutionSummary]
+    parameters: List[ParameterSummary]
+    interactions: List[InteractionDetails]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            uniqueID=dictionary.get("uniqueID", ""),
+            name=dictionary.get("name", ""),
+            version=dictionary.get("version", ""),
+            interactionType=InteractionType(
+                dictionary.get("interactionType", InteractionType.Atomic)
+            ),
+            path=dictionary.get("path", ""),
+            spec=InteractionSpecificationSummary.from_dict(dictionary.get("spec")),
+            exec=InteractionExecutionSummary.from_dict(dictionary.get("exec"))
+            if dictionary.get("exec")
+            else None,
+            parameters=[
+                ParameterSummary.from_dict(param) for param in dictionary.get("parameters", [])
+            ],
+            interactions=[
+                InteractionDetails.from_dict(interaction)
+                for interaction in dictionary.get("interactions", [])
+            ],
+        )
+
+
+@dataclass
+class TestCaseDetails:
+    uniqueID: str
+    spec: TestCaseSpecificationDetails
+    exec: Optional[TestCaseExecutionDetails]
+    interactions: List[InteractionDetails]
+    parameters: List[ParameterSummary]
+
+    @classmethod
+    def from_dict(cls, dictionary) -> TestCaseDetails:
+        return cls(
+            uniqueID=dictionary.get("uniqueID"),
+            spec=TestCaseSpecificationDetails.from_dict(dictionary.get("spec")),
+            exec=TestCaseExecutionDetails.from_dict(dictionary.get("exec"))
+            if dictionary.get("exec")
+            else None,
+            interactions=[
+                InteractionDetails.from_dict(interaction)
+                for interaction in dictionary.get("interactions", [])
+            ],
+            parameters=[
+                ParameterSummary.from_dict(parameter)
+                for parameter in dictionary.get("parameters", [])
+            ],
+        )
+
+
+@dataclass
+class TestStructureSpecification:
+    key: str
+    locker: Optional[UserReference]
+    status: SpecificationStatus
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", "-1"),
+            locker=UserReference.from_dict(dictionary.get("locker", {}))
+            if dictionary.get("locker")
+            else None,
+            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
+        )
+
+
+@dataclass
+class TestStructureAutomation:
+    key: str
+    locker: Optional[UserReference]
+    status: SpecificationStatus
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", "-1"),
+            locker=UserReference.from_dict(dictionary.get("locker", {}))
+            if dictionary.get("locker")
+            else None,
+            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
+        )
+
+
+@dataclass
+class TestStructureExecution:
+    key: str
+    locker: Optional[UserReference]
+    status: ActivityStatus
+    execStatus: ExecutionStatus
+    verdict: ExecutionVerdict
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", "-1"),
+            locker=UserReference.from_dict(dictionary.get("locker", {}))
+            if dictionary.get("locker")
+            else None,
+            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
+            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
+            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
+        )
+
+
+@dataclass
+class AttachedFilter:
+    key: str
+    name: str
+    filterType: FilterType
+    content: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", "-1"),
+            name=dictionary.get("name", ""),
+            filterType=FilterType(dictionary.get("filterType", FilterType.TestCaseSetFilter)),
+            content=dictionary.get("content", ""),
+        )
+
+
+@dataclass
+class TestStructureTreeNodeInformation:
+    key: str
+    numbering: str
+    parentKey: str
+    name: str
+    uniqueID: str
+    orderPos: int
+    matchesFilter: bool
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", "-1"),
+            numbering=dictionary.get("numbering", "-1"),
+            parentKey=dictionary.get("parentKey", "-1"),
+            name=dictionary.get("name", ""),
+            uniqueID=dictionary.get("uniqueID", ""),
+            orderPos=dictionary.get("orderPos", "-1"),
+            matchesFilter=dictionary.get("matchesFilter", True),
+        )
+
+
+@dataclass
+class TestStructureTreeNode:
+    elementType: TestStructureTreeNodeType
+    baseInformation: TestStructureTreeNodeInformation
+    specification: Optional[TestStructureSpecification]
+    automation: Optional[TestStructureAutomation]
+    execution: Optional[TestStructureExecution]
+    filters: List[AttachedFilter]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            elementType=TestStructureTreeNodeType(
+                dictionary.get("elementType", TestStructureTreeNodeType.TestTheme)
+            ),
+            baseInformation=TestStructureTreeNodeInformation.from_dict(
+                dictionary.get("baseInformation", {})
+            ),
+            specification=TestStructureSpecification.from_dict(dictionary.get("specification"))
+            if dictionary.get("specification")
+            else None,
+            automation=TestStructureAutomation.from_dict(dictionary.get("automation"))
+            if dictionary.get("automation")
+            else None,
+            execution=TestStructureExecution.from_dict(dictionary.get("execution"))
+            if dictionary.get("execution")
+            else None,
+            filters=[AttachedFilter.from_dict(filter) for filter in dictionary.get("filters", [])],
+        )
+
+
+@dataclass
+class TestStructureTree:
+    root: TestStructureTreeNode
+    nodes: List[TestStructureTreeNode]
+
+    @classmethod
+    def from_dict(cls, dictionary) -> TestStructureTree:
+        return cls(
+            root=TestStructureTreeNode.from_dict(dictionary.get("root", {}))
+            if "root" in dictionary
+            else None,
+            nodes=[TestStructureTreeNode.from_dict(node) for node in dictionary.get("nodes", [])],
+        )
```

### Comparing `testbench2robotframework-0.5.2/testbench2robotframework/testbench2robotframework.py` & `testbench2robotframework-0.6.0/testbench2robotframework/testbench2robotframework.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import Dict
-
-from .config import Configuration
-from .json_reader import TestBenchJsonReader
-from .log import logger, setup_logger
-
-# from .robot_run import RobotSuiteRunner
-from .testbench2rf import create_test_suites
-from .testsuite_write import write_test_suites
-from .utils import PathResolver, get_directory
-
-
-def testbench2robotframework(json_report: str, config: Dict):
-    configuration = Configuration.from_dict(config)
-    setup_logger(configuration)
-    logger.debug("Config file loaded.")
-    json_report = get_directory(json_report)
-    reader = TestBenchJsonReader(json_report)
-    path_resolver = PathResolver(
-        reader.test_theme_tree,
-        tuple(reader.get_test_case_set_catalog().keys()),
-        configuration.logSuiteNumbering,
-    )
-    test_suites = create_test_suites(
-        reader.get_test_case_set_catalog(), path_resolver, configuration
-    )
-    # suite_runner = RobotSuiteRunner(test_suites, path_resolver)
-    # suite_runner.run_suites()
-    if not test_suites:
-        logger.warning("There are no test suites in the exported TestBench Projekt.")
-        return
-    write_test_suites(test_suites, configuration)
+from typing import Dict
+
+from .config import Configuration
+from .json_reader import TestBenchJsonReader
+from .log import logger, setup_logger
+
+# from .robot_run import RobotSuiteRunner
+from .testbench2rf import create_test_suites
+from .testsuite_write import write_test_suites
+from .utils import PathResolver, get_directory
+
+
+def testbench2robotframework(json_report: str, config: Dict):
+    configuration = Configuration.from_dict(config)
+    setup_logger(configuration)
+    logger.debug("Config file loaded.")
+    json_report = get_directory(json_report)
+    reader = TestBenchJsonReader(json_report)
+    path_resolver = PathResolver(
+        reader.test_theme_tree,
+        tuple(reader.get_test_case_set_catalog().keys()),
+        configuration.logSuiteNumbering,
+    )
+    test_suites = create_test_suites(
+        reader.get_test_case_set_catalog(), path_resolver, configuration
+    )
+    # suite_runner = RobotSuiteRunner(test_suites, path_resolver)
+    # suite_runner.run_suites()
+    if not test_suites:
+        logger.warning("There are no test suites in the exported TestBench Projekt.")
+        return
+    write_test_suites(test_suites, configuration)
```

### Comparing `testbench2robotframework-0.5.2/testbench2robotframework/testsuite_write.py` & `testbench2robotframework-0.6.0/testbench2robotframework/testsuite_write.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-import os
-import re
-import shutil
-from pathlib import Path
-from typing import Dict
-
-from robot.parsing.model.blocks import File
-
-from .config import Configuration
-from .log import logger
-from .utils import directory_to_zip
-
-
-def write_test_suites(test_suites: Dict[str, File], config: Configuration) -> None:
-    generation_directory = get_generation_directory(config.generationDirectory)
-    if config.clearGenerationDirectory:
-        clear_generation_directory(generation_directory)
-    write_test_suite_files(test_suites, generation_directory)
-    if config.createOutputZip:
-        directory_to_zip(generation_directory)
-    logger.info(f"Successfully wrote {len(test_suites)} robot files.")
-    logger.info(f"Path: {os.path.abspath(generation_directory)}")
-
-
-def get_generation_directory(generation_directory: str) -> Path:
-    root_path = Path(os.curdir).absolute()
-    if not generation_directory:
-        return root_path / "Generated"
-    return Path(
-        re.sub(
-            r"^{root}",
-            str(root_path).replace('\\', '\\\\'),
-            generation_directory,
-            flags=re.IGNORECASE,
-        )
-    )
-
-
-def clear_generation_directory(generation_dir: Path) -> None:
-    if generation_dir.is_dir():
-        shutil.rmtree(str(generation_dir))
-        logger.info("Files in generation directory deleted.")
-    zip_file = "".join([str(generation_dir), ".zip"])
-    if os.path.exists(zip_file):
-        os.remove(zip_file)
-
-
-def write_test_suite_files(test_suites: Dict[str, File], generation_directory: Path) -> None:
-    for test_suite_file in test_suites.values():
-        test_suite_file.source = Path(generation_directory / f"{test_suite_file.source}.robot")
-        logger.debug(f"File written to {os.path.relpath(test_suite_file.source)}")
-        test_suite_file.save()
+import os
+import re
+import shutil
+from pathlib import Path
+from typing import Dict
+
+from robot.parsing.model.blocks import File
+
+from .config import Configuration
+from .log import logger
+from .utils import directory_to_zip
+
+
+def write_test_suites(test_suites: Dict[str, File], config: Configuration) -> None:
+    generation_directory = get_generation_directory(config.generationDirectory)
+    if config.clearGenerationDirectory:
+        clear_generation_directory(generation_directory)
+    write_test_suite_files(test_suites, generation_directory)
+    if config.createOutputZip:
+        directory_to_zip(generation_directory)
+    logger.info(f"Successfully wrote {len(test_suites)} robot files.")
+    logger.info(f"Path: {Path(generation_directory).resolve()!s}")
+
+
+def get_generation_directory(generation_directory: str) -> Path:
+    root_path = Path(os.curdir).absolute()
+    if not generation_directory:
+        return root_path / "Generated"
+    return Path(
+        re.sub(
+            r"^{root}",
+            str(root_path).replace('\\', '\\\\'),
+            generation_directory,
+            flags=re.IGNORECASE,
+        )
+    )
+
+
+def clear_generation_directory(generation_dir: Path) -> None:
+    if generation_dir.is_dir():
+        shutil.rmtree(str(generation_dir))
+        logger.info("Files in generation directory deleted.")
+    zip_file = "".join([str(generation_dir), ".zip"])
+    Path(zip_file).unlink(missing_ok=True)
+
+
+def write_test_suite_files(test_suites: Dict[str, File], generation_directory: Path) -> None:
+    for test_suite_file in test_suites.values():
+        test_suite_file.source = Path(generation_directory / f"{test_suite_file.source}.robot")
+        logger.debug(f"File written to {os.path.relpath(test_suite_file.source)}")
+        test_suite_file.save()
```

### Comparing `testbench2robotframework-0.5.2/testbench2robotframework/utils.py` & `testbench2robotframework-0.6.0/testbench2robotframework/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-import argparse
-import os
-import re
-import shutil
-import sys
-from pathlib import Path, PurePath
-from typing import Dict, Optional, Tuple
-from zipfile import ZipFile
-
-from testbench2robotframework.model import (
-    TestStructureTree,
-    TestStructureTreeNode,
-    TestStructureTreeNodeType,
-)
-
-CONVERTER_DESCRIPTION = """tB2Robot converts TestBench JSON report to Robot Framework Code
-                        and Robot Result Model to JSON full report."""
-WRITE_SUBPARSER_HELP = """Command to convert TestBench´s JSON REPORT to Robot Framework Code."""
-READ_SUBPARSER_HELP = """Command to read a robot output xml file and
-write the results to a TestBench JSON REPORT."""
-JSON_PATH_ARGUMENT_HELP = "Path to a ZIP file or directory containing TestBenchs JSON report files."
-CONFIG_ARGUMENT_HELP = """Path to a config json file to generate robot files
-                        based on the given configuration.
-                        If no path is given testbench2robot will search for a file
-                        named \"config.json\" in the current working directory."""
-ROBOT_OUTPUT_HELP = """Path to an XML file containing the robot results."""
-ROBOT_RESULT_HELP = """Path to the directory or ZIP File the TestBench JSON reports
-with result should be saved to."""
-
-
-arg_parser = argparse.ArgumentParser(description=CONVERTER_DESCRIPTION)
-arg_parser.add_argument(
-    '--version',
-    '--info',
-    action='store_true',
-    help='Writes the TestBench2RobotFramework, Robot Framework and Python version to console.',
-)
-subparsers = arg_parser.add_subparsers(dest="subcommand")
-
-write_parser = subparsers.add_parser("write", help=WRITE_SUBPARSER_HELP)
-write_parser.add_argument(
-    "-c",
-    "--config",
-    help=CONFIG_ARGUMENT_HELP,
-    type=str,
-    required=False,
-    default=os.path.join(os.path.abspath(os.curdir), "config.json"),
-)
-
-write_parser.add_argument("jsonReport", nargs=1, type=str, help=JSON_PATH_ARGUMENT_HELP)
-
-read_parser = subparsers.add_parser("read", help=READ_SUBPARSER_HELP)
-read_parser.add_argument(
-    "-c",
-    "--config",
-    help=CONFIG_ARGUMENT_HELP,
-    type=str,
-    required=False,
-    default=os.path.join(os.path.abspath(os.curdir), "config.json"),
-)
-read_parser.add_argument(
-    "-r",
-    "--result",
-    help=ROBOT_RESULT_HELP,
-    type=str,
-    required=False,
-)
-required_named_arguments = read_parser.add_argument_group('required named arguments')
-required_named_arguments.add_argument(
-    "-o", "--output", help=ROBOT_OUTPUT_HELP, type=str, required=True
-)
-
-read_parser.add_argument("jsonReport", nargs=1, type=str, help=JSON_PATH_ARGUMENT_HELP)
-
-
-class PathResolver:
-    def __init__(
-        self,
-        test_theme_tree: TestStructureTree,
-        uids_of_existing_tcs: Tuple[str, ...],
-        log_suite_numbers: bool,
-    ):
-        self.tcs_catalog: Dict[str, TestStructureTreeNode] = {}
-        self.tt_catalog: Dict[str, TestStructureTreeNode] = {}
-        self.tree_dict: Dict[str, TestStructureTreeNode] = {}
-        self._last_child_indices: Dict[str, int] = {}
-        self._log_suite_numbers = log_suite_numbers
-        self._uids_of_existing_tcs = uids_of_existing_tcs
-        self._analyze_tree(test_theme_tree)
-        self.tcs_paths = self._get_paths(self.tcs_catalog)
-        self.tt_paths = self._get_paths(self.tt_catalog)
-
-    def _analyze_tree(self, test_theme_tree: TestStructureTree):
-        self.tree_dict[test_theme_tree.root.baseInformation.key] = test_theme_tree.root
-        for tse in test_theme_tree.nodes:
-            self._add_existing_tcs_to_catalog(tse)
-            self.tree_dict[tse.baseInformation.key] = tse
-            self._store_highest_child_index(tse)
-
-    def _store_highest_child_index(self, tse):
-        self._last_child_indices[tse.baseInformation.parentKey] = max(
-            int(get_tse_index(tse)),
-            self._last_child_indices.get(tse.baseInformation.parentKey, 0),
-        )
-
-    def _add_existing_tcs_to_catalog(self, tse):
-        if (
-            tse.elementType == TestStructureTreeNodeType.TestCaseSet
-            and tse.baseInformation.uniqueID in self._uids_of_existing_tcs
-        ):
-            self.tcs_catalog[tse.baseInformation.uniqueID] = tse
-
-    def _get_paths(self, tse_catalog: Dict[str, TestStructureTreeNode]) -> Dict[str, PurePath]:
-        return {uid: self._resolve_tse_path(tse) for uid, tse in tse_catalog.items()}
-
-    def _resolve_tse_path(self, tse: TestStructureTreeNode) -> PurePath:
-        self._add_tt_to_tt_catalog(tse)
-        if tse.elementType == TestStructureTreeNodeType.Root:
-            return PurePath()
-        tse_name = replace_invalid_characters(tse.baseInformation.name)
-        if tse.baseInformation.parentKey not in self.tree_dict:
-            return PurePath(f"{self._file_prefix(tse)}{tse_name}")
-        parent_path = self._resolve_tse_path(self.tree_dict[tse.baseInformation.parentKey])
-        return parent_path / f"{self._file_prefix(tse)}{tse_name}"
-
-    def _add_tt_to_tt_catalog(self, tse):
-        if (
-            tse.elementType == TestStructureTreeNodeType.TestTheme
-            and tse.baseInformation.uniqueID not in self.tt_catalog
-        ):
-            self.tt_catalog[tse.baseInformation.uniqueID] = tse
-
-    def _file_prefix(self, tse) -> str:
-        prefix_separator = '_' * self._log_suite_numbers
-        return f"{self._get_padded_index(tse)}_{prefix_separator}"
-
-    def _get_padded_index(self, tse) -> str:
-        index = get_tse_index(tse)
-        max_length = len(str(self._last_child_indices[tse.baseInformation.parentKey]))
-        return index.zfill(max_length)
-
-
-def get_directory(json_report_path: Optional[str]) -> str:
-    if json_report_path is None:
-        return ""
-    if not os.path.exists(json_report_path):
-        sys.exit("Error opening " + json_report_path + ". Path does not exist.")
-    if os.path.isdir(json_report_path):
-        return os.path.abspath(json_report_path)
-    filename, ext = os.path.splitext(json_report_path)
-    if ext.lower() == ".zip":
-        with ZipFile(json_report_path, 'r') as zip_ref:
-            zip_ref.extractall(filename)
-        return os.path.abspath(filename)
-    sys.exit("Error opening " + json_report_path + ". File is not a ZIP file.")
-
-
-def ensure_dir_exists(cli_output_dir):
-    if not Path(cli_output_dir).is_dir():
-        Path(cli_output_dir).mkdir(parents=True, exist_ok=True)
-
-
-def replace_invalid_characters(name: str) -> str:
-    return re.sub(r'[<>:"/\\|?* ]', "_", name)
-
-
-def get_tse_index(tse: TestStructureTreeNode) -> str:
-    return tse.baseInformation.numbering.rsplit(".", 1)[-1]
-
-
-def directory_to_zip(directory: Path, new_path: str = None):
-    if new_path:
-        shutil.make_archive(str(new_path), 'zip', str(directory))
-    else:
-        shutil.make_archive(str(directory), 'zip', str(directory))
-
-
-def get_list_item(liste, index, default: Optional[str]):
-    try:
-        item = liste[index]
-        return item
-    except IndexError:
-        return default
+import argparse
+import os
+import re
+import shutil
+import sys
+from pathlib import Path, PurePath
+from typing import Dict, Optional, Tuple
+from zipfile import ZipFile
+
+from testbench2robotframework.model import (
+    TestStructureTree,
+    TestStructureTreeNode,
+    TestStructureTreeNodeType,
+)
+
+CONVERTER_DESCRIPTION = """tB2Robot converts TestBench JSON report to Robot Framework Code
+                        and Robot Result Model to JSON full report."""
+WRITE_SUBPARSER_HELP = """Command to convert TestBench`s JSON REPORT to Robot Framework Code."""
+READ_SUBPARSER_HELP = """Command to read a robot output xml file and
+write the results to a TestBench JSON REPORT."""
+JSON_PATH_ARGUMENT_HELP = "Path to a ZIP file or directory containing TestBenchs JSON report files."
+CONFIG_ARGUMENT_HELP = """Path to a config json file to generate robot files
+                        based on the given configuration.
+                        If no path is given testbench2robot will search for a file
+                        named \"config.json\" in the current working directory."""
+ROBOT_OUTPUT_HELP = """Path to an XML file containing the robot results."""
+ROBOT_RESULT_HELP = """Path to the directory or ZIP File the TestBench JSON reports
+with result should be saved to."""
+
+
+arg_parser = argparse.ArgumentParser(description=CONVERTER_DESCRIPTION)
+arg_parser.add_argument(
+    '--version',
+    '--info',
+    action='store_true',
+    help='Writes the TestBench2RobotFramework, Robot Framework and Python version to console.',
+)
+subparsers = arg_parser.add_subparsers(dest="subcommand")
+
+write_parser = subparsers.add_parser("write", help=WRITE_SUBPARSER_HELP)
+write_parser.add_argument(
+    "-c",
+    "--config",
+    help=CONFIG_ARGUMENT_HELP,
+    type=str,
+    required=False,
+    default=str(Path(os.curdir, "config.json").resolve()),
+)
+
+write_parser.add_argument("jsonReport", nargs=1, type=str, help=JSON_PATH_ARGUMENT_HELP)
+
+read_parser = subparsers.add_parser("read", help=READ_SUBPARSER_HELP)
+read_parser.add_argument(
+    "-c",
+    "--config",
+    help=CONFIG_ARGUMENT_HELP,
+    type=str,
+    required=False,
+    default=str(Path(os.curdir, "config.json").resolve()),
+)
+read_parser.add_argument(
+    "-r",
+    "--result",
+    help=ROBOT_RESULT_HELP,
+    type=str,
+    required=False,
+)
+required_named_arguments = read_parser.add_argument_group('required named arguments')
+required_named_arguments.add_argument(
+    "-o", "--output", help=ROBOT_OUTPUT_HELP, type=str, required=True
+)
+
+read_parser.add_argument("jsonReport", nargs=1, type=str, help=JSON_PATH_ARGUMENT_HELP)
+
+
+class PathResolver:
+    def __init__(
+        self,
+        test_theme_tree: TestStructureTree,
+        uids_of_existing_tcs: Tuple[str, ...],
+        log_suite_numbers: bool,
+    ):
+        self.tcs_catalog: Dict[str, TestStructureTreeNode] = {}
+        self.tt_catalog: Dict[str, TestStructureTreeNode] = {}
+        self.tree_dict: Dict[str, TestStructureTreeNode] = {}
+        self._last_child_indices: Dict[str, int] = {}
+        self._log_suite_numbers = log_suite_numbers
+        self._uids_of_existing_tcs = uids_of_existing_tcs
+        self._analyze_tree(test_theme_tree)
+        self.tcs_paths = self._get_paths(self.tcs_catalog)
+        self.tt_paths = self._get_paths(self.tt_catalog)
+
+    def _analyze_tree(self, test_theme_tree: TestStructureTree):
+        self.tree_dict[test_theme_tree.root.baseInformation.key] = test_theme_tree.root
+        for tse in test_theme_tree.nodes:
+            self._add_existing_tcs_to_catalog(tse)
+            self.tree_dict[tse.baseInformation.key] = tse
+            self._store_highest_child_index(tse)
+
+    def _store_highest_child_index(self, tse):
+        self._last_child_indices[tse.baseInformation.parentKey] = max(
+            int(get_tse_index(tse)),
+            self._last_child_indices.get(tse.baseInformation.parentKey, 0),
+        )
+
+    def _add_existing_tcs_to_catalog(self, tse):
+        if (
+            tse.elementType == TestStructureTreeNodeType.TestCaseSet
+            and tse.baseInformation.uniqueID in self._uids_of_existing_tcs
+        ):
+            self.tcs_catalog[tse.baseInformation.uniqueID] = tse
+
+    def _get_paths(self, tse_catalog: Dict[str, TestStructureTreeNode]) -> Dict[str, PurePath]:
+        return {uid: self._resolve_tse_path(tse) for uid, tse in tse_catalog.items()}
+
+    def _resolve_tse_path(self, tse: TestStructureTreeNode) -> PurePath:
+        self._add_tt_to_tt_catalog(tse)
+        if tse.elementType == TestStructureTreeNodeType.Root:
+            return PurePath()
+        tse_name = replace_invalid_characters(tse.baseInformation.name)
+        if tse.baseInformation.parentKey not in self.tree_dict:
+            return PurePath(f"{self._file_prefix(tse)}{tse_name}")
+        parent_path = self._resolve_tse_path(self.tree_dict[tse.baseInformation.parentKey])
+        return parent_path / f"{self._file_prefix(tse)}{tse_name}"
+
+    def _add_tt_to_tt_catalog(self, tse):
+        if (
+            tse.elementType == TestStructureTreeNodeType.TestTheme
+            and tse.baseInformation.uniqueID not in self.tt_catalog
+        ):
+            self.tt_catalog[tse.baseInformation.uniqueID] = tse
+
+    def _file_prefix(self, tse) -> str:
+        prefix_separator = '_' * self._log_suite_numbers
+        return f"{self._get_padded_index(tse)}_{prefix_separator}"
+
+    def _get_padded_index(self, tse) -> str:
+        index = get_tse_index(tse)
+        max_length = len(str(self._last_child_indices[tse.baseInformation.parentKey]))
+        return index.zfill(max_length)
+
+
+def get_directory(json_report_path: Optional[str]) -> str:
+    if json_report_path is None:
+        return ""
+    if not Path(json_report_path).exists():
+        sys.exit("Error opening " + json_report_path + ". Path does not exist.")
+    if Path(json_report_path).is_dir():
+        return str(Path(json_report_path).resolve())
+    ext = Path(json_report_path).suffix
+    filename = str(Path(json_report_path).parent / Path(json_report_path).stem)
+    if ext.lower() == ".zip":
+        with ZipFile(json_report_path, 'r') as zip_ref:
+            zip_ref.extractall(filename)
+        return str(Path(filename).resolve())
+    sys.exit("Error opening " + json_report_path + ". File is not a ZIP file.")
+
+
+def ensure_dir_exists(cli_output_dir):
+    if not Path(cli_output_dir).is_dir():
+        Path(cli_output_dir).mkdir(parents=True, exist_ok=True)
+
+
+def replace_invalid_characters(name: str) -> str:
+    return re.sub(r'[<>:"/\\|?* ]', "_", name)
+
+
+def get_tse_index(tse: TestStructureTreeNode) -> str:
+    return tse.baseInformation.numbering.rsplit(".", 1)[-1]
+
+
+def directory_to_zip(directory: Path, new_path: Optional[str] = None):
+    if new_path:
+        shutil.make_archive(str(new_path), 'zip', str(directory))
+    else:
+        shutil.make_archive(str(directory), 'zip', str(directory))
+
+
+def get_list_item(liste, index, default: Optional[str]):
+    try:
+        return liste[index]
+    except IndexError:
+        return default
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `testbench2robotframework-0.5.2/testbench2robotframework.egg-info/PKG-INFO` & `testbench2robotframework-0.6.0/testbench2robotframework.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,302 +1,303 @@
-Metadata-Version: 2.1
-Name: testbench2robotframework
-Version: 0.5.2
-Summary: Robot Framework Code Generator from Keyword-Driven Tests in imbus TestBench 3.0 and newer
-Home-page: https://github.com/imbus/testbench2robotframework
-Author: imbus AG
-Author-email: support@imbus.de
-License: Apache 2.0 License
-Description: # Installation des Robot Code Generators
-        
-        Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
-        
-        ```powershell
-        python --version
-        ```
-        
-        Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
-        Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
-        
-        ```powershell
-        python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
-        ```
-        
-        Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
-        ```powershell
-        pip install testbench2robotframework
-        ```
-        
-        Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
-        
-        ```powershell
-        tb2robot --version
-        ```
-        
-        # Verwendung des Robot Code Generators
-        Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
-        
-        Der Befehl ``tb2robot --help
-        `` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
-        
-        Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
-        
-        (@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
-        
-        (@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-        
-        Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
-        ```powershell
-        tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
-        ```
-        Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
-        
-        ![](./images/testthemen.PNG)
-        ![](./images/generated.PNG)
-        
-        Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
-        
-        Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
-        Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
-        
-        (@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
-        
-        (@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
-        
-        (@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-        
-        Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
-        ```powershell
-        tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
-        ```
-        
-        # Konfiguration der Ergebnisse
-        Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
-        
-        ## rfLibraryRegex
-        Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
-        Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
-        Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
-        
-        ![](./images/testbench_rfLibraryRegex.PNG)
-        
-        ```python
-        *** Settings ***
-        Library    Browser
-        Library    BuiltIn
-        ```
-        In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-        ```json
-        "rfLibraryRegex": [
-            "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
-          ]
-        ```
-        
-        ## rfResourceRegex
-        Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
-        Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
-        Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
-        
-        ![](./images/testbench_rfResourceRegex.PNG)
-        
-        ```python
-        *** Settings ***
-        Resource    keywords.resource
-        ```
-        In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-        ```json
-        "rfResourceRegex": [
-            "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
-          ]
-        ```
-        ## rfLibraryRoots
-        Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
-        Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
-        
-        Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
-        
-        Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
-        
-        ```json
-        "rfLibraryRoots": ["RobotLibraries"]
-        ```
-        
-        ![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
-        
-        Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
-        
-        ```python
-        *** Settings ***
-        Library    BuiltIn
-        Library    OperatingSystem
-        # UNKNOWN    Process
-        ```
-        
-        ## rfResourceRoots
-        Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
-        
-        Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
-        
-        ```json
-        "rfResourceRoots": ["RF-Resources"]
-        ```
-        
-        ![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
-        
-        Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
-        
-        ```python
-        *** Settings ***
-        Resource    keywords.resource
-        # UNKNOWN    unknownKeywords
-        ```
-        
-        ## fullyQualified
-        Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
-        
-        Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
-        
-        ```python
-        SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
-        ```
-        Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
-        
-        ```python
-        Open Browser      https://robotframework.org/    firefox
-        ```
-        
-        ## resourceDirectory
-        Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
-        Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
-        
-        ```json
-        "resourceDirectory": "{root}/Resources",
-        ```
-        
-        ```robotframework
-        *** Settings ***
-        Resource    ../Resources/myKeywords.resource
-        ```
-        
-        ## generationDirectory
-        Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
-        ```json
-        "generationDirectory": "{root}/generatedRobotFiles"
-        ```
-        
-        ## createOutputZip
-        Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
-        
-        ## logSuiteNumbering
-        Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
-        
-        ```json
-        "logSuiteNumbering": true
-        ```
-        ## clearGenerationDirectory
-        Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
-        
-        ```json
-        "clearGenerationDirectory": true,
-        ```
-        
-        ## logCompoundInteractions
-        Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
-        
-        ```json
-        "logCompoundInteractions": true,
-        ```
-        
-        ## subdivisionsMapping
-        Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
-        
-        ```json
-        "subdivisionsMapping": {
-            "libraries": {
-              "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
-              "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
-            },
-            "resources": {
-              "MyKeywords": "{root}/../MyKeywords.resource",
-              "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
-            }
-          }
-        ```
-        
-        
-        ## forcedImport
-        Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
-        
-        ```json
-        "forcedImport": {
-            "libraries": [
-              "SeleniumLibrary"
-            ],
-            "resources":
-            [
-              "technical_keywords.resource"
-            ],
-            "variables": [
-              "myVars.py"
-            ]
-          }
-        ```
-        
-        ## loggingConfiguration
-        Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
-        Gültige Optionen sind:
-        
-        * "CRITICAL"
-        
-        * "FATAL"
-        
-        * "ERROR"
-        
-        * "WARNING"
-        
-        * "WARN"
-        
-        * "INFO"
-        
-        * "DEBUG"
-        
-        * "NOTSET"
-        
-        Das Default Log-Level ist ``INFO``.
-        ```json
-        "loggingConfiguration": {
-          "console": {
-            "logLevel": "info"
-          }
-        }
-        ```
-        
-        ## referenceBehaviour
-        Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
-        Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
-        Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
-        
-        ```json
-        "referenceBehaviour": "ATTACHMENT"
-        ```
-        
-        ## attachmentConflictBehaviour
-        Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
-        Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
-        
-        Die möglichen Werte haben dabei die folgende Bedeutung:
-        - ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
-        - USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
-        - USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
-        - RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
-        ```json
-        "attachmentConflictBehaviour": "USE_EXISTING"
-        ```
-        
-        ## testCaseSplitPathRegEx
-        Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
-        
-        
-Platform: any
-Requires-Python: >= 3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+Metadata-Version: 2.1
+Name: testbench2robotframework
+Version: 0.6.0
+Summary: Robot Framework Code Generator from Keyword-Driven Tests in imbus TestBench 3.0 and newer
+Home-page: https://github.com/imbus/testbench2robotframework
+Author: imbus AG
+Author-email: support@imbus.de
+License: Apache 2.0 License
+Platform: any
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Installation des Robot Code Generators
+
+Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
+
+```powershell
+python --version
+```
+
+Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
+Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
+
+```powershell
+python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
+```
+
+Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
+```powershell
+pip install testbench2robotframework
+```
+
+Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
+
+```powershell
+tb2robot --version
+```
+
+# Verwendung des Robot Code Generators
+Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
+
+Der Befehl ``tb2robot --help
+`` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
+
+Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
+
+(@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
+
+(@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+
+Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
+```powershell
+tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
+```
+Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
+
+![](./images/testthemen.PNG)
+![](./images/generated.PNG)
+
+Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
+
+Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
+Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
+
+(@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
+
+(@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
+
+(@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+
+Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
+```powershell
+tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
+```
+
+# Konfiguration der Ergebnisse
+Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
+
+## rfLibraryRegex
+Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
+Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
+Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
+
+![](./images/testbench_rfLibraryRegex.PNG)
+
+```python
+*** Settings ***
+Library    Browser
+Library    BuiltIn
+```
+In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+```json
+"rfLibraryRegex": [
+    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
+  ]
+```
+
+## rfResourceRegex
+Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
+Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
+Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
+
+![](./images/testbench_rfResourceRegex.PNG)
+
+```python
+*** Settings ***
+Resource    keywords.resource
+```
+In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+```json
+"rfResourceRegex": [
+    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
+  ]
+```
+## rfLibraryRoots
+Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
+Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
+
+Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
+
+Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
+
+```json
+"rfLibraryRoots": ["RobotLibraries"]
+```
+
+![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
+
+Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
+
+```python
+*** Settings ***
+Library    BuiltIn
+Library    OperatingSystem
+# UNKNOWN    Process
+```
+
+## rfResourceRoots
+Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
+
+Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
+
+```json
+"rfResourceRoots": ["RF-Resources"]
+```
+
+![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
+
+Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
+
+```python
+*** Settings ***
+Resource    keywords.resource
+# UNKNOWN    unknownKeywords
+```
+
+## fullyQualified
+Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
+
+Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
+
+```python
+SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
+```
+Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
+
+```python
+Open Browser      https://robotframework.org/    firefox
+```
+
+## resourceDirectory
+Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
+Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
+
+```json
+"resourceDirectory": "{root}/Resources",
+```
+
+```robotframework
+*** Settings ***
+Resource    ../Resources/myKeywords.resource
+```
+
+## generationDirectory
+Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
+```json
+"generationDirectory": "{root}/generatedRobotFiles"
+```
+
+## createOutputZip
+Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
+
+## logSuiteNumbering
+Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
+
+```json
+"logSuiteNumbering": true
+```
+## clearGenerationDirectory
+Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
+
+```json
+"clearGenerationDirectory": true,
+```
+
+## logCompoundInteractions
+Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
+
+```json
+"logCompoundInteractions": true,
+```
+
+## subdivisionsMapping
+Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
+
+```json
+"subdivisionsMapping": {
+    "libraries": {
+      "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
+      "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
+    },
+    "resources": {
+      "MyKeywords": "{root}/../MyKeywords.resource",
+      "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
+    }
+  }
+```
+
+
+## forcedImport
+Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
+
+```json
+"forcedImport": {
+    "libraries": [
+      "SeleniumLibrary"
+    ],
+    "resources":
+    [
+      "technical_keywords.resource"
+    ],
+    "variables": [
+      "myVars.py"
+    ]
+  }
+```
+
+## loggingConfiguration
+Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
+Gültige Optionen sind:
+
+* "CRITICAL"
+
+* "FATAL"
+
+* "ERROR"
+
+* "WARNING"
+
+* "WARN"
+
+* "INFO"
+
+* "DEBUG"
+
+* "NOTSET"
+
+Das Default Log-Level ist ``INFO``.
+```json
+"loggingConfiguration": {
+  "console": {
+    "logLevel": "info"
+  }
+}
+```
+
+## referenceBehaviour
+Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
+Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
+Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
+
+```json
+"referenceBehaviour": "ATTACHMENT"
+```
+
+## attachmentConflictBehaviour
+Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
+Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
+
+Die möglichen Werte haben dabei die folgende Bedeutung:
+- ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
+- USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
+- USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
+- RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
+```json
+"attachmentConflictBehaviour": "USE_EXISTING"
+```
+
+## testCaseSplitPathRegEx
+Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
+
```

### Comparing `testbench2robotframework-0.5.2/tests/test_data/configurations/invalid_config.json` & `testbench2robotframework-0.6.0/tests/test_data/configurations/valid_config.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {'delete': "['testbalala']"}*

```diff
@@ -36,10 +36,9 @@
             "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
         },
         "resources": {
             "MyKeywords": "{root}/../MyKeywords.resource",
             "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
         }
     },
-    "testCaseSplitPathRegEx": "^splitting\\..*",
-    "testbalala": true
+    "testCaseSplitPathRegEx": "^splitting\\..*"
 }
```

