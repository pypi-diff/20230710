# Comparing `tmp/halmos-0.0.8.tar.gz` & `tmp/halmos-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halmos-0.0.8.tar", last modified: Sat May  6 03:04:02 2023, max compression
+gzip compressed data, was "halmos-0.0.9.tar", last modified: Mon Jul 10 05:12:16 2023, max compression
```

## Comparing `halmos-0.0.8.tar` & `halmos-0.0.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.497822 halmos-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-06 03:03:54.000000 halmos-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-06 03:03:54.000000 halmos-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-06 03:03:54.000000 halmos-0.0.8/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-06 03:03:54.000000 halmos-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-06 03:03:54.000000 halmos-0.0.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-06 03:03:54.000000 halmos-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-06 03:03:54.000000 halmos-0.0.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-06 03:03:54.000000 halmos-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-06 03:04:02.497822 halmos-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-06 03:03:54.000000 halmos-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 03:03:54.000000 halmos-0.0.8/examples/foundry.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/examples/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-06 03:03:54.000000 halmos-0.0.8/examples/src/Example.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/examples/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-06 03:03:54.000000 halmos-0.0.8/examples/test/Example.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-06 03:03:54.000000 halmos-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-06 03:03:54.000000 halmos-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:04:02.497822 halmos-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/src/halmos/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23618 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/byte2op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/cheatcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    59143 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/sevm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/src/halmos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/foundry.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.497822 halmos-0.0.8/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/Const.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/Counter.sol
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/Create.sol
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/List.sol
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/SignExtend.sol
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/Storage.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.497822 halmos-0.0.8/tests/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Arith.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Block.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Const.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Counter.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Create.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Deal.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Foundry.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Invalid.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Library.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/List.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Opcode.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Prank.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Send.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Setup.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/SetupPlus.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/SignExtend.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Storage.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Struct.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Warp.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test_sevm.py
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.079452 halmos-0.0.9/
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.071124 halmos-0.0.9/.github/
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.072952 halmos-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 dpark      (502) wheel        (0)      468 2023-07-10 04:56:56.000000 halmos-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 dpark      (502) wheel        (0)      604 2023-07-10 04:56:56.000000 halmos-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.073341 halmos-0.0.9/.github/workflows/
+-rw-r--r--   0 dpark      (502) wheel        (0)     2945 2023-07-10 04:56:56.000000 halmos-0.0.9/.github/workflows/codeql.yml
+-rw-r--r--   0 dpark      (502) wheel        (0)      439 2023-07-10 04:56:56.000000 halmos-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 dpark      (502) wheel        (0)      873 2023-07-10 04:57:15.000000 halmos-0.0.9/.github/workflows/test.yml
+-rw-r--r--   0 dpark      (502) wheel        (0)      219 2023-07-10 04:56:56.000000 halmos-0.0.9/.gitignore
+-rw-r--r--   0 dpark      (502) wheel        (0)      109 2023-07-10 04:56:56.000000 halmos-0.0.9/.gitmodules
+-rw-r--r--   0 dpark      (502) wheel        (0)    34523 2023-07-10 04:56:56.000000 halmos-0.0.9/LICENSE
+-rw-r--r--   0 dpark      (502) wheel        (0)     4542 2023-07-10 05:12:16.079294 halmos-0.0.9/PKG-INFO
+-rw-r--r--   0 dpark      (502) wheel        (0)     4075 2023-07-10 04:57:15.000000 halmos-0.0.9/README.md
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.073480 halmos-0.0.9/examples/
+-rw-r--r--   0 dpark      (502) wheel        (0)      141 2023-07-10 04:56:56.000000 halmos-0.0.9/examples/foundry.toml
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.073606 halmos-0.0.9/examples/src/
+-rw-r--r--   0 dpark      (502) wheel        (0)     1030 2023-07-10 04:56:56.000000 halmos-0.0.9/examples/src/Example.sol
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.073751 halmos-0.0.9/examples/test/
+-rw-r--r--   0 dpark      (502) wheel        (0)     1587 2023-07-10 04:56:56.000000 halmos-0.0.9/examples/test/Example.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      733 2023-07-10 04:56:56.000000 halmos-0.0.9/pyproject.toml
+-rw-r--r--   0 dpark      (502) wheel        (0)       43 2023-07-10 04:56:56.000000 halmos-0.0.9/requirements.txt
+-rw-r--r--   0 dpark      (502) wheel        (0)       38 2023-07-10 05:12:16.079489 halmos-0.0.9/setup.cfg
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.071638 halmos-0.0.9/src/
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.074585 halmos-0.0.9/src/halmos/
+-rw-r--r--   0 dpark      (502) wheel        (0)       36 2023-07-10 04:56:56.000000 halmos-0.0.9/src/halmos/__init__.py
+-rw-r--r--   0 dpark      (502) wheel        (0)    23618 2023-07-10 04:57:15.000000 halmos-0.0.9/src/halmos/__main__.py
+-rw-r--r--   0 dpark      (502) wheel        (0)     1724 2023-07-10 04:57:15.000000 halmos-0.0.9/src/halmos/byte2op.py
+-rw-r--r--   0 dpark      (502) wheel        (0)     3010 2023-07-10 04:57:15.000000 halmos-0.0.9/src/halmos/cheatcodes.py
+-rw-r--r--   0 dpark      (502) wheel        (0)    59143 2023-07-10 04:57:15.000000 halmos-0.0.9/src/halmos/sevm.py
+-rw-r--r--   0 dpark      (502) wheel        (0)    28892 2023-07-10 04:57:15.000000 halmos-0.0.9/src/halmos/utils.py
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.075398 halmos-0.0.9/src/halmos.egg-info/
+-rw-r--r--   0 dpark      (502) wheel        (0)     4542 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/PKG-INFO
+-rw-r--r--   0 dpark      (502) wheel        (0)     1290 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/SOURCES.txt
+-rw-r--r--   0 dpark      (502) wheel        (0)        1 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/dependency_links.txt
+-rw-r--r--   0 dpark      (502) wheel        (0)       48 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/entry_points.txt
+-rw-r--r--   0 dpark      (502) wheel        (0)       39 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/requires.txt
+-rw-r--r--   0 dpark      (502) wheel        (0)        7 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/top_level.txt
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.075803 halmos-0.0.9/tests/
+-rw-r--r--   0 dpark      (502) wheel        (0)      140 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/foundry.toml
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.076580 halmos-0.0.9/tests/src/
+-rw-r--r--   0 dpark      (502) wheel        (0)      126 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/Const.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)     1581 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/Counter.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      334 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/Create.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      405 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/List.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      184 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/SignExtend.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      905 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/Storage.sol
+drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.079078 halmos-0.0.9/tests/test/
+-rw-r--r--   0 dpark      (502) wheel        (0)     1092 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Arith.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      785 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Block.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      345 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Const.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)     3155 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Counter.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      748 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Create.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      867 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Deal.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      732 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/test/Foundry.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      691 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Invalid.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      594 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Library.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)     1648 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/List.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)     1319 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/test/Opcode.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)     3450 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Prank.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)     1832 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Send.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      650 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Setup.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)     1986 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/test/SetupPlus.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      294 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/SignExtend.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)     1139 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Storage.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)      274 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Struct.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)     1363 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Warp.t.sol
+-rw-r--r--   0 dpark      (502) wheel        (0)     6085 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/test_cli.py
+-rw-r--r--   0 dpark      (502) wheel        (0)     6151 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/test_sevm.py
```

### Comparing `halmos-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md` & `halmos-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/.github/workflows/codeql.yml` & `halmos-0.0.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/.github/workflows/test.yml` & `halmos-0.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/LICENSE` & `halmos-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/PKG-INFO` & `halmos-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.0.8
+Version: 0.0.9
 Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
 Author: Daejun Park
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `halmos-0.0.8/README.md` & `halmos-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/examples/src/Example.sol` & `halmos-0.0.9/examples/src/Example.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/examples/test/Example.t.sol` & `halmos-0.0.9/examples/test/Example.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/pyproject.toml` & `halmos-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "crytic-compile >= 0.3.0",
+    "crytic-compile >= 0.3.0, < 0.3.2",
     "z3-solver",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 halmos = "halmos.__main__:main"
```

### Comparing `halmos-0.0.8/src/halmos/__main__.py` & `halmos-0.0.9/src/halmos/__main__.py`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/src/halmos/byte2op.py` & `halmos-0.0.9/src/halmos/byte2op.py`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/src/halmos/cheatcodes.py` & `halmos-0.0.9/src/halmos/cheatcodes.py`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/src/halmos/sevm.py` & `halmos-0.0.9/src/halmos/sevm.py`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/src/halmos/utils.py` & `halmos-0.0.9/src/halmos/utils.py`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/src/halmos.egg-info/PKG-INFO` & `halmos-0.0.9/src/halmos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.0.8
+Version: 0.0.9
 Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
 Author: Daejun Park
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `halmos-0.0.8/src/halmos.egg-info/SOURCES.txt` & `halmos-0.0.9/src/halmos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/src/Counter.sol` & `halmos-0.0.9/tests/src/Counter.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/src/Storage.sol` & `halmos-0.0.9/tests/src/Storage.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Arith.t.sol` & `halmos-0.0.9/tests/test/Arith.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Block.t.sol` & `halmos-0.0.9/tests/test/Block.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Counter.t.sol` & `halmos-0.0.9/tests/test/Counter.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Create.t.sol` & `halmos-0.0.9/tests/test/Create.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Deal.t.sol` & `halmos-0.0.9/tests/test/Deal.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Foundry.t.sol` & `halmos-0.0.9/tests/test/Foundry.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Invalid.t.sol` & `halmos-0.0.9/tests/test/Invalid.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Library.t.sol` & `halmos-0.0.9/tests/test/Library.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/List.t.sol` & `halmos-0.0.9/tests/test/List.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Opcode.t.sol` & `halmos-0.0.9/tests/test/Opcode.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Prank.t.sol` & `halmos-0.0.9/tests/test/Prank.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Send.t.sol` & `halmos-0.0.9/tests/test/Send.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Setup.t.sol` & `halmos-0.0.9/tests/test/Setup.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/SetupPlus.t.sol` & `halmos-0.0.9/tests/test/SetupPlus.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Storage.t.sol` & `halmos-0.0.9/tests/test/Storage.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test/Warp.t.sol` & `halmos-0.0.9/tests/test/Warp.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test_cli.py` & `halmos-0.0.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `halmos-0.0.8/tests/test_sevm.py` & `halmos-0.0.9/tests/test_sevm.py`

 * *Files identical despite different names*

