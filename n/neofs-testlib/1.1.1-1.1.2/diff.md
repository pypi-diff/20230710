# Comparing `tmp/neofs-testlib-1.1.1.tar.gz` & `tmp/neofs-testlib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neofs-testlib-1.1.1.tar", last modified: Wed Feb  8 10:15:57 2023, max compression
+gzip compressed data, was "neofs-testlib-1.1.2.tar", last modified: Fri Jul  7 10:11:11 2023, max compression
```

## Comparing `neofs-testlib-1.1.1.tar` & `neofs-testlib-1.1.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.594999 neofs-testlib-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5900 2023-02-08 10:15:57.594999 neofs-testlib-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5297 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1730 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-08 10:15:57.594999 neofs-testlib-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.586999 neofs-testlib-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.586999 neofs-testlib-1.1.1/src/neofs_testlib/
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.590999 neofs-testlib-1.1.1/src/neofs_testlib/blockchain/
--rw-r--r--   0 root         (0) root         (0)      113 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/blockchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/blockchain/multisig.py
--rw-r--r--   0 root         (0) root         (0)     4640 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/blockchain/role_designation.py
--rw-r--r--   0 root         (0) root         (0)     2718 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/blockchain/rpc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.590999 neofs-testlib-1.1.1/src/neofs_testlib/cli/
--rw-r--r--   0 root         (0) root         (0)      212 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2841 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/cli_command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.590999 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/
--rw-r--r--   0 root         (0) root         (0)       53 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/adm.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/config.py
--rw-r--r--   0 root         (0) root         (0)    10847 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/morph.py
--rw-r--r--   0 root         (0) root         (0)      647 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/storage_config.py
--rw-r--r--   0 root         (0) root         (0)     7105 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/subnet.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.590999 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_authmate/
--rw-r--r--   0 root         (0) root         (0)       68 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_authmate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_authmate/authmate.py
--rw-r--r--   0 root         (0) root         (0)     3437 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_authmate/secret.py
--rw-r--r--   0 root         (0) root         (0)      315 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_authmate/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.590999 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/
--rw-r--r--   0 root         (0) root         (0)       53 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/accounting.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/acl.py
--rw-r--r--   0 root         (0) root         (0)     2155 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     9597 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/container.py
--rw-r--r--   0 root         (0) root         (0)     3802 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/netmap.py
--rw-r--r--   0 root         (0) root         (0)    12770 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/object.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/session.py
--rw-r--r--   0 root         (0) root         (0)     4263 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/shards.py
--rw-r--r--   0 root         (0) root         (0)     4907 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/storagegroup.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/util.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.594999 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/
--rw-r--r--   0 root         (0) root         (0)      106 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5037 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/candidate.py
--rw-r--r--   0 root         (0) root         (0)    14320 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/contract.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/db.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/go.py
--rw-r--r--   0 root         (0) root         (0)     8877 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/nep17.py
--rw-r--r--   0 root         (0) root         (0)      115 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/network_type.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/node.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/query.py
--rw-r--r--   0 root         (0) root         (0)      308 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/version.py
--rw-r--r--   0 root         (0) root         (0)    12857 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/wallet.py
--rw-r--r--   0 root         (0) root         (0)      259 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/defaults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.594999 neofs-testlib-1.1.1/src/neofs_testlib/hosting/
--rw-r--r--   0 root         (0) root         (0)      178 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/hosting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/hosting/config.py
--rw-r--r--   0 root         (0) root         (0)     9753 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/hosting/docker_host.py
--rw-r--r--   0 root         (0) root         (0)     3432 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/hosting/hosting.py
--rw-r--r--   0 root         (0) root         (0)     5972 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/hosting/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.594999 neofs-testlib-1.1.1/src/neofs_testlib/plugins/
--rw-r--r--   0 root         (0) root         (0)      716 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.594999 neofs-testlib-1.1.1/src/neofs_testlib/reporter/
--rw-r--r--   0 root         (0) root         (0)      570 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/reporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/reporter/allure_handler.py
--rw-r--r--   0 root         (0) root         (0)      809 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/reporter/interfaces.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/reporter/reporter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.594999 neofs-testlib-1.1.1/src/neofs_testlib/shell/
--rw-r--r--   0 root         (0) root         (0)      204 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/shell/__init__.py
--rw-r--r--   0 root         (0) root         (0)      360 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/shell/command_inspectors.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/shell/interfaces.py
--rw-r--r--   0 root         (0) root         (0)     5720 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/shell/local_shell.py
--rw-r--r--   0 root         (0) root         (0)    11187 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/shell/ssh_shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.594999 neofs-testlib-1.1.1/src/neofs_testlib/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/utils/converters.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/src/neofs_testlib/utils/wallet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.586999 neofs-testlib-1.1.1/src/neofs_testlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5900 2023-02-08 10:15:57.000000 neofs-testlib-1.1.1/src/neofs_testlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2869 2023-02-08 10:15:57.000000 neofs-testlib-1.1.1/src/neofs_testlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 10:15:57.000000 neofs-testlib-1.1.1/src/neofs_testlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      165 2023-02-08 10:15:57.000000 neofs-testlib-1.1.1/src/neofs_testlib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      200 2023-02-08 10:15:57.000000 neofs-testlib-1.1.1/src/neofs_testlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-08 10:15:57.000000 neofs-testlib-1.1.1/src/neofs_testlib.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:15:57.594999 neofs-testlib-1.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)     6230 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     1931 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/tests/test_converters.py
--rw-r--r--   0 root         (0) root         (0)     4937 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/tests/test_hosting.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/tests/test_local_shell.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/tests/test_reporter.py
--rw-r--r--   0 root         (0) root         (0)     5019 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/tests/test_ssh_shell.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-02-08 10:15:15.000000 neofs-testlib-1.1.1/tests/test_wallet.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/
+-rw-rw-r--   0 varg      (1000) varg      (1000)    35149 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/LICENSE
+-rw-rw-r--   0 varg      (1000) varg      (1000)     5900 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/PKG-INFO
+-rw-rw-r--   0 varg      (1000) varg      (1000)     5297 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/README.md
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1730 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/pyproject.toml
+-rw-rw-r--   0 varg      (1000) varg      (1000)       38 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/setup.cfg
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.342422 neofs-testlib-1.1.2/src/
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.342422 neofs-testlib-1.1.2/src/neofs_testlib/
+-rw-rw-r--   0 varg      (1000) varg      (1000)       22 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/__init__.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.342422 neofs-testlib-1.1.2/src/neofs_testlib/blockchain/
+-rw-rw-r--   0 varg      (1000) varg      (1000)      113 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/blockchain/__init__.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1622 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/blockchain/multisig.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     4640 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/blockchain/role_designation.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     2718 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/blockchain/rpc_client.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.342422 neofs-testlib-1.1.2/src/neofs_testlib/cli/
+-rw-rw-r--   0 varg      (1000) varg      (1000)      212 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/__init__.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     2841 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/cli_command.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.342422 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/
+-rw-rw-r--   0 varg      (1000) varg      (1000)       53 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/__init__.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1156 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/adm.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      645 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/config.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)    10847 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/morph.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      647 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/storage_config.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     7105 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/subnet.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      310 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/version.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.342422 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_authmate/
+-rw-rw-r--   0 varg      (1000) varg      (1000)       68 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_authmate/__init__.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      558 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_authmate/authmate.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     3437 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_authmate/secret.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      315 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_authmate/version.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/
+-rw-rw-r--   0 varg      (1000) varg      (1000)       53 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/__init__.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      961 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/accounting.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     2201 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/acl.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     2155 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/cli.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     9597 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/container.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     3802 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/netmap.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)    12770 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/object.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1241 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/session.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     4263 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/shards.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     4907 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/storagegroup.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1793 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/util.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      348 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/version.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/
+-rw-rw-r--   0 varg      (1000) varg      (1000)      106 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/__init__.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     5037 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/candidate.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)    14320 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/contract.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     2150 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/db.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1646 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/go.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     8877 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/nep17.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      115 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/network_type.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      501 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/node.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     2870 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/query.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      308 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/version.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)    12857 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/wallet.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      259 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/defaults.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/src/neofs_testlib/hosting/
+-rw-rw-r--   0 varg      (1000) varg      (1000)      235 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/hosting/__init__.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     2281 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/hosting/config.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)    10099 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/hosting/docker_host.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     3432 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/hosting/hosting.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     6236 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/hosting/interfaces.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/src/neofs_testlib/plugins/
+-rw-rw-r--   0 varg      (1000) varg      (1000)      716 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/plugins/__init__.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/src/neofs_testlib/reporter/
+-rw-rw-r--   0 varg      (1000) varg      (1000)      570 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/reporter/__init__.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1152 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/reporter/allure_handler.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      809 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/reporter/interfaces.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     3198 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/reporter/reporter.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/src/neofs_testlib/shell/
+-rw-rw-r--   0 varg      (1000) varg      (1000)      204 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/shell/__init__.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)      360 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/shell/command_inspectors.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     2804 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/shell/interfaces.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     5720 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/shell/local_shell.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)    11187 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/shell/ssh_shell.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/src/neofs_testlib/utils/
+-rw-rw-r--   0 varg      (1000) varg      (1000)        0 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/utils/__init__.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1988 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/utils/converters.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1280 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/src/neofs_testlib/utils/wallet.py
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.342422 neofs-testlib-1.1.2/src/neofs_testlib.egg-info/
+-rw-rw-r--   0 varg      (1000) varg      (1000)     5900 2023-07-07 10:11:11.000000 neofs-testlib-1.1.2/src/neofs_testlib.egg-info/PKG-INFO
+-rw-rw-r--   0 varg      (1000) varg      (1000)     2869 2023-07-07 10:11:11.000000 neofs-testlib-1.1.2/src/neofs_testlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 varg      (1000) varg      (1000)        1 2023-07-07 10:11:11.000000 neofs-testlib-1.1.2/src/neofs_testlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 varg      (1000) varg      (1000)      165 2023-07-07 10:11:11.000000 neofs-testlib-1.1.2/src/neofs_testlib.egg-info/entry_points.txt
+-rw-rw-r--   0 varg      (1000) varg      (1000)      200 2023-07-07 10:11:11.000000 neofs-testlib-1.1.2/src/neofs_testlib.egg-info/requires.txt
+-rw-rw-r--   0 varg      (1000) varg      (1000)       14 2023-07-07 10:11:11.000000 neofs-testlib-1.1.2/src/neofs_testlib.egg-info/top_level.txt
+drwxrwxr-x   0 varg      (1000) varg      (1000)        0 2023-07-07 10:11:11.346422 neofs-testlib-1.1.2/tests/
+-rw-rw-r--   0 varg      (1000) varg      (1000)     6230 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/tests/test_cli.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1931 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/tests/test_converters.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     5519 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/tests/test_hosting.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     4007 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/tests/test_local_shell.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     2396 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/tests/test_reporter.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     5019 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/tests/test_ssh_shell.py
+-rw-rw-r--   0 varg      (1000) varg      (1000)     1517 2023-07-07 09:44:06.000000 neofs-testlib-1.1.2/tests/test_wallet.py
```

### Comparing `neofs-testlib-1.1.1/LICENSE` & `neofs-testlib-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/PKG-INFO` & `neofs-testlib-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neofs-testlib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Building blocks and utilities to facilitate development of automated tests for NeoFS system
 Author-email: NSPCC <info@nspcc.ru>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/nspcc-dev/neofs-testlib
 Keywords: neofs,test
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `neofs-testlib-1.1.1/README.md` & `neofs-testlib-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/pyproject.toml` & `neofs-testlib-1.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neofs-testlib"
-version = "1.1.1"
+version = "1.1.2"
 description = "Building blocks and utilities to facilitate development of automated tests for NeoFS system"
 readme = "README.md"
 authors = [{ name = "NSPCC", email = "info@nspcc.ru" }]
 license = { text = "GNU General Public License v3 (GPLv3)" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
@@ -44,15 +44,15 @@
 line_length = 100
 
 [tool.black]
 line-length = 100
 target-version = ["py310"]
 
 [tool.bumpver]
-current_version = "1.1.1"
+current_version = "1.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/blockchain/multisig.py` & `neofs-testlib-1.1.2/src/neofs_testlib/blockchain/multisig.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/blockchain/role_designation.py` & `neofs-testlib-1.1.2/src/neofs_testlib/blockchain/role_designation.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/blockchain/rpc_client.py` & `neofs-testlib-1.1.2/src/neofs_testlib/blockchain/rpc_client.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/cli_command.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/cli_command.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/adm.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/adm.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/config.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/config.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/morph.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/morph.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/storage_config.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/storage_config.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_adm/subnet.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_adm/subnet.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_authmate/authmate.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_authmate/authmate.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_authmate/secret.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_authmate/secret.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/accounting.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/accounting.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/acl.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/acl.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/cli.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/cli.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/container.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/container.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/netmap.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/netmap.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/object.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/object.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/session.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/session.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/shards.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/shards.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/storagegroup.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/storagegroup.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neofs_cli/util.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neofs_cli/util.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/candidate.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/candidate.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/contract.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/contract.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/db.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/db.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/go.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/go.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/nep17.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/nep17.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/query.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/query.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/cli/neogo/wallet.py` & `neofs-testlib-1.1.2/src/neofs_testlib/cli/neogo/wallet.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/hosting/config.py` & `neofs-testlib-1.1.2/src/neofs_testlib/hosting/config.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/hosting/docker_host.py` & `neofs-testlib-1.1.2/src/neofs_testlib/hosting/docker_host.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,22 @@
             if message_regex:
                 matches = re.findall(message_regex, logs, re.IGNORECASE)
                 if matches:
                     return True
 
         return False
 
+    def get_service_pid(self, service_name: str) -> str:
+        client = self._get_docker_client()
+        top_info = client.top(service_name)
+        pid_index = top_info['Titles'].index('PID')
+        # In the current configuration, only one service runs in each container
+        pid = top_info['Processes'][0][pid_index]
+        return pid
+
     def _get_service_attributes(self, service_name) -> ServiceAttributes:
         service_config = self.get_service_config(service_name)
         return ServiceAttributes.parse(service_config.attributes)
 
     def _get_docker_client(self) -> docker.APIClient:
         docker_endpoint = HostAttributes.parse(self._config.attributes).docker_endpoint
```

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/hosting/hosting.py` & `neofs-testlib-1.1.2/src/neofs_testlib/hosting/hosting.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/hosting/interfaces.py` & `neofs-testlib-1.1.2/src/neofs_testlib/hosting/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,7 +186,18 @@
             since: If set, limits the time from which logs should be collected. Must be in UTC.
             until: If set, limits the time until which logs should be collected. Must be in UTC.
 
         Returns:
             True if message found in logs in the given time frame.
             False otherwise.
         """
+
+    @abstractmethod
+    def get_service_pid(self, service_name: str) -> str:
+        """Returns the PID of the specified neofs process.
+
+        Args:
+            service_name: service name.
+
+        Returns:
+            PID of the specified service.
+        """
```

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/plugins/__init__.py` & `neofs-testlib-1.1.2/src/neofs_testlib/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/reporter/__init__.py` & `neofs-testlib-1.1.2/src/neofs_testlib/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/reporter/allure_handler.py` & `neofs-testlib-1.1.2/src/neofs_testlib/reporter/allure_handler.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/reporter/interfaces.py` & `neofs-testlib-1.1.2/src/neofs_testlib/reporter/interfaces.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/reporter/reporter.py` & `neofs-testlib-1.1.2/src/neofs_testlib/reporter/reporter.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/shell/interfaces.py` & `neofs-testlib-1.1.2/src/neofs_testlib/shell/interfaces.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/shell/local_shell.py` & `neofs-testlib-1.1.2/src/neofs_testlib/shell/local_shell.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/shell/ssh_shell.py` & `neofs-testlib-1.1.2/src/neofs_testlib/shell/ssh_shell.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/utils/converters.py` & `neofs-testlib-1.1.2/src/neofs_testlib/utils/converters.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib/utils/wallet.py` & `neofs-testlib-1.1.2/src/neofs_testlib/utils/wallet.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib.egg-info/PKG-INFO` & `neofs-testlib-1.1.2/src/neofs_testlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neofs-testlib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Building blocks and utilities to facilitate development of automated tests for NeoFS system
 Author-email: NSPCC <info@nspcc.ru>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/nspcc-dev/neofs-testlib
 Keywords: neofs,test
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `neofs-testlib-1.1.1/src/neofs_testlib.egg-info/SOURCES.txt` & `neofs-testlib-1.1.2/src/neofs_testlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/tests/test_cli.py` & `neofs-testlib-1.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/tests/test_converters.py` & `neofs-testlib-1.1.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/tests/test_hosting.py` & `neofs-testlib-1.1.2/tests/test_hosting.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from unittest import TestCase
 
-from neofs_testlib.hosting import CLIConfig, Hosting, ServiceConfig
+import docker
+
+from neofs_testlib.hosting import CLIConfig, DockerHost, HostConfig, Hosting, ServiceConfig
 
 
 class TestHosting(TestCase):
     SERVICE_NAME_PREFIX = "service"
     HOST1_ADDRESS = "10.10.10.10"
     HOST1_PLUGIN = "docker"
     HOST1_ATTRIBUTES = {"param1": "value1"}
@@ -107,7 +109,23 @@
             self.assertEqual(
                 service.name[: len(self.SERVICE_NAME_PREFIX)], self.SERVICE_NAME_PREFIX
             )
 
         service1 = hosting.find_service_configs(self.SERVICE1["name"])
         self.assertEqual(len(service1), 1)
         self.assertDictEqual(service1[0].attributes, self.SERVICE1_ATTRIBUTES)
+
+    def test_get_service_pid(self):
+        config = HostConfig(plugin_name=self.HOST2_PLUGIN, address=self.HOST2_ADDRESS)
+        docker_hosting = DockerHost(config)
+
+        client = docker.from_env()
+        container = client.containers.run("alpine:latest", "tail -f /dev/null", detach=True)
+
+        top_info = container.top()
+        expected_pid = top_info["Processes"][0][1]
+        pid = docker_hosting.get_service_pid(container.name)
+
+        container.stop()
+        container.remove()
+
+        self.assertEqual(expected_pid, pid)
```

### Comparing `neofs-testlib-1.1.1/tests/test_local_shell.py` & `neofs-testlib-1.1.2/tests/test_local_shell.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/tests/test_reporter.py` & `neofs-testlib-1.1.2/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/tests/test_ssh_shell.py` & `neofs-testlib-1.1.2/tests/test_ssh_shell.py`

 * *Files identical despite different names*

### Comparing `neofs-testlib-1.1.1/tests/test_wallet.py` & `neofs-testlib-1.1.2/tests/test_wallet.py`

 * *Files identical despite different names*

