# Comparing `tmp/formance-sdk-python-1.0.20230623b1.tar.gz` & `tmp/formance-sdk-python-1.0.20230627.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formance-sdk-python-1.0.20230623b1.tar", last modified: Tue Jun 27 10:30:46 2023, max compression
+gzip compressed data, was "formance-sdk-python-1.0.20230627.tar", last modified: Mon Jul 10 08:36:13 2023, max compression
```

## Comparing `formance-sdk-python-1.0.20230623b1.tar` & `formance-sdk-python-1.0.20230627.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:30:46.583957 formance-sdk-python-1.0.20230623b1/
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-06-27 10:30:46.583957 formance-sdk-python-1.0.20230623b1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    10003 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 10:30:46.583957 formance-sdk-python-1.0.20230623b1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:30:46.559957 formance-sdk-python-1.0.20230623b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:30:46.559957 formance-sdk-python-1.0.20230623b1/src/formance_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-06-27 10:30:46.000000 formance-sdk-python-1.0.20230623b1/src/formance_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-06-27 10:30:46.000000 formance-sdk-python-1.0.20230623b1/src/formance_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:30:46.000000 formance-sdk-python-1.0.20230623b1/src/formance_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 10:30:46.000000 formance-sdk-python-1.0.20230623b1/src/formance_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 10:30:46.000000 formance-sdk-python-1.0.20230623b1/src/formance_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:30:46.559957 formance-sdk-python-1.0.20230623b1/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23184 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33117 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/ledger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:30:46.559957 formance-sdk-python-1.0.20230623b1/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:30:46.567957 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7031 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/activateconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/addmetadataontransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/addmetadatatoaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/addscopetoclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/addtransientscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/cancelevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/changeconfigsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/confirmhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/connectorsstripetransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1129 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/connectorstransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/countaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/counttransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createbalance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createtransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createtransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      799 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1060 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/creditwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1052 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deactivateconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/debitwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deleteclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deleteconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deletescope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deletescopefromclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deletesecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deletetransientscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1256 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getbalance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2439 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getbalancesaggregated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1052 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getconnectortask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/gethold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1954 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getholds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getinstance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getinstancehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getinstancestagehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getledgerinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1259 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getmanyconfigs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getmapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/gettransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/gettransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getversions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1060 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getwalletsummary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/insertconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/installconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4059 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listallconnectors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listclients.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      674 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listconfigsavailableconnectors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listconnectorstransfers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1538 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listconnectortasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listinstances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listlogs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1511 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listpayments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listscopes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4820 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listtransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listusers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1752 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listwallets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listworkflows.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      752 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/orchestrationgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/paymentsgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/paymentslistaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/readclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      963 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/readconnectorconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      831 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/readscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      979 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/readstats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/readuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      730 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/resetconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/reverttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1931 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/runscript.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/runworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      603 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/searchgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/sendevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1015 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/testconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/uninstallconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/updateclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1161 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/updatemapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/updatemetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1087 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/updatescope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/updatewallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/voidhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/walletsgetserverinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:30:46.583957 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10411 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/accountresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1399 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/accountscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/accountscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/accountwithvolumesandbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activityconfirmhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitycreatetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitycreatetransactionoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitycreditwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitydebitwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitydebitwalletoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitygetaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitygetaccountoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitygetpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitygetpaymentoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      419 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitygetwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitygetwalletoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activityreverttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activityreverttransactionoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1511 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitystripetransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activityvoidhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/aggregatebalancesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      432 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/assetholder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2179 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/attempt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/attemptresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/balance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/balancescursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/balancewithassets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/bankingcircleconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2136 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      877 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/clientsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      428 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configchangesecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      720 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configinforesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      554 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      759 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/confirmholdrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/connector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/connectorconfigresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/connectorsconfigsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/connectorsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/contract.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createbalancerequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      520 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createbalanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createclientrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createscoperequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createscoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createsecretrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createsecretresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      611 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createworkflowrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      526 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1228 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/creditwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/currencycloudconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/debitwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/debitwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1062 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/dummypayconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      703 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/error.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/errorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/errorsenum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1495 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/expandeddebithold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getbalanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getholdresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getholdsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/gettransactionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getversionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getwalletsummaryresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getworkflowinstancehistoryresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getworkflowinstanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      519 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/hold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      552 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/ledgeraccountsubject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1070 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/ledgerinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/ledgerinforesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      549 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/ledgerstorage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listbalancesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listclientsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listrunsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listscopesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listusersresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listwalletsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      532 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listworkflowsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1363 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/logscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      499 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/mapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/mappingresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1346 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/migrationinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/modulrconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/monetary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3120 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/payment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1277 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/paymentadjustment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/paymentmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/paymentresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1309 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/paymentsaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/paymentscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/paymentstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      779 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/posting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/posttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/readclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/readscoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/readuserresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/runworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      931 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/scope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/script.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1921 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/scriptresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      987 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/secret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      313 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/serverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      891 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagedelay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1147 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesenddestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesenddestinationaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesenddestinationpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesenddestinationwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1235 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesendsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesendsourceaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesendsourcepayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesendsourcewallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1399 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagestatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagewaitevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      549 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      491 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/statsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1008 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stripeconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stripetransferrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stripetransferresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2346 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskbankingcircle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2178 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskcurrencycloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2500 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskdummypay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2492 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskmodulr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskstripe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskwise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1294 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transactiondata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transactionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transactionscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transactionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transferrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transferresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2045 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transfersresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/updateclientrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/updateclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/updatescoperequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/updatescoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      838 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      736 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/volume.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1198 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/wallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/walletserrorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2076 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/walletstransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/walletsubject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/walletsvolume.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/walletwithbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1498 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/webhooksconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/webhookserrorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      507 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/webhookserrorsenum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/wiseconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1212 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2038 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowinstance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1528 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowinstancehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2667 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowinstancehistorystage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowinstancehistorystageinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2340 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowinstancehistorystageoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17605 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/orchestration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21682 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4383 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/sdkconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3036 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:30:46.583957 formance-sdk-python-1.0.20230623b1/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24619 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/wallets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12374 2023-06-27 10:30:32.000000 formance-sdk-python-1.0.20230623b1/src/sdk/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:36:13.501400 formance-sdk-python-1.0.20230627/
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-07-10 08:36:13.501400 formance-sdk-python-1.0.20230627/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10003 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:36:13.501400 formance-sdk-python-1.0.20230627/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:36:13.457400 formance-sdk-python-1.0.20230627/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:36:13.461400 formance-sdk-python-1.0.20230627/src/formance_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-07-10 08:36:13.000000 formance-sdk-python-1.0.20230627/src/formance_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-07-10 08:36:13.000000 formance-sdk-python-1.0.20230627/src/formance_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:36:13.000000 formance-sdk-python-1.0.20230627/src/formance_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-10 08:36:13.000000 formance-sdk-python-1.0.20230627/src/formance_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 08:36:13.000000 formance-sdk-python-1.0.20230627/src/formance_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:36:13.461400 formance-sdk-python-1.0.20230627/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23184 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33117 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/ledger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:36:13.461400 formance-sdk-python-1.0.20230627/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:36:13.477400 formance-sdk-python-1.0.20230627/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7031 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/activateconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/addmetadataontransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/addmetadatatoaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/addscopetoclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/addtransientscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/cancelevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/changeconfigsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/confirmhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/connectorsstripetransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1129 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/connectorstransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/countaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/counttransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/createbalance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/createclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/createscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/createsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/createtransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/createtransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/createwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      799 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/createworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1060 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/creditwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1052 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/deactivateconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/debitwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/deleteclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/deleteconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/deletescope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/deletescopefromclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/deletesecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/deletetransientscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1256 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getbalance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2439 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getbalancesaggregated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1052 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getconnectortask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/gethold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1954 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getholds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getinstance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getinstancehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getinstancestagehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getledgerinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1259 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getmanyconfigs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getmapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/gettransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/gettransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getversions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1060 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getwalletsummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/getworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/insertconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/installconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4059 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listallconnectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listclients.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      674 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listconfigsavailableconnectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listconnectorstransfers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1538 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listconnectortasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listinstances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listlogs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1511 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listpayments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listscopes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4820 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listtransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listusers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1752 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listwallets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/listworkflows.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      752 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/orchestrationgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/paymentsgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/paymentslistaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/readclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      963 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/readconnectorconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      831 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/readscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      979 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/readstats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/readuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      730 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/resetconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/reverttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1931 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/runscript.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/runworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      603 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/searchgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/sendevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1015 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/testconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/uninstallconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/updateclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1161 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/updatemapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/updatemetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1087 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/updatescope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/updatewallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/voidhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/operations/walletsgetserverinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:36:13.501400 formance-sdk-python-1.0.20230627/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10411 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/accountresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1399 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/accountscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/accountscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/accountwithvolumesandbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activityconfirmhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitycreatetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitycreatetransactionoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitycreditwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitydebitwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitydebitwalletoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitygetaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitygetaccountoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitygetpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitygetpaymentoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      419 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitygetwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitygetwalletoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activityreverttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activityreverttransactionoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1511 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitystripetransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/activityvoidhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/aggregatebalancesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      432 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/assetholder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2179 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/attempt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/attemptresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/balance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/balancescursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/balancewithassets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/bankingcircleconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2136 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      877 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/clientsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      428 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/configchangesecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      720 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/configinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/configinforesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      554 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/configresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/configsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      759 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/configuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/confirmholdrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/connectorconfigresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/connectorsconfigsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/connectorsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/contract.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createbalancerequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      520 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createbalanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createclientrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createscoperequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createscoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createsecretrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createsecretresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      611 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createworkflowrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      526 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/createworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1228 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/creditwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/currencycloudconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/debitwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/debitwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1062 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/dummypayconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      703 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/error.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/errorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/errorsenum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1495 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/expandeddebithold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/getbalanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/getholdresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/getholdsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/gettransactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/getversionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/getwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/getwalletsummaryresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/getworkflowinstancehistoryresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/getworkflowinstanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      519 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/getworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/hold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      552 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/ledgeraccountsubject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1070 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/ledgerinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/ledgerinforesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      549 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/ledgerstorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/listbalancesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/listclientsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/listrunsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/listscopesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/listusersresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/listwalletsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      532 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/listworkflowsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1363 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/logscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      499 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/mapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/mappingresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1346 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/migrationinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/modulrconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/monetary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3120 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/payment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1277 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/paymentadjustment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/paymentmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/paymentresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1309 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/paymentsaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/paymentscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/paymentstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      779 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/posting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/posttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/readclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/readscoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/readuserresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/runworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      931 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/scope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/script.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1921 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/scriptresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      987 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/secret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      313 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/serverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      891 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagedelay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1147 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesenddestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesenddestinationaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesenddestinationpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesenddestinationwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1235 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesendsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesendsourceaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesendsourcepayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesendsourcewallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1399 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagestatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagewaitevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      549 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      491 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/statsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1008 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stripeconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stripetransferrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/stripetransferresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2346 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskbankingcircle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2178 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskcurrencycloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2500 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskdummypay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2492 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskmodulr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskstripe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskwise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1294 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/transactiondata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/transactionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/transactionscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/transactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/transferrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/transferresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2045 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/transfersresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/updateclientrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/updateclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/updatescoperequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/updatescoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      838 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      736 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1198 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/wallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/walletserrorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2076 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/walletstransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/walletsubject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/walletsvolume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/walletwithbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1498 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/webhooksconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/webhookserrorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      507 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/webhookserrorsenum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/wiseconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1212 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2038 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowinstance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1528 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowinstancehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2667 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowinstancehistorystage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowinstancehistorystageinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2340 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowinstancehistorystageoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17605 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/orchestration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21682 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4383 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/sdkconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3036 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:36:13.501400 formance-sdk-python-1.0.20230627/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24619 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/wallets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12374 2023-07-10 08:35:56.000000 formance-sdk-python-1.0.20230627/src/sdk/webhooks.py
```

### Comparing `formance-sdk-python-1.0.20230623b1/PKG-INFO` & `formance-sdk-python-1.0.20230627/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formance-sdk-python
-Version: 1.0.20230623b1
+Version: 1.0.20230627
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Formance
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `formance-sdk-python-1.0.20230623b1/README.md` & `formance-sdk-python-1.0.20230627/README.md`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/setup.py` & `formance-sdk-python-1.0.20230627/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="formance-sdk-python",
-    version="v1.0.20230623-beta.1",
+    version="v1.0.20230627",
     author="Formance",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
```

### Comparing `formance-sdk-python-1.0.20230623b1/src/formance_sdk_python.egg-info/PKG-INFO` & `formance-sdk-python-1.0.20230627/src/formance_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formance-sdk-python
-Version: 1.0.20230623b1
+Version: 1.0.20230627
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Formance
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `formance-sdk-python-1.0.20230623b1/src/formance_sdk_python.egg-info/SOURCES.txt` & `formance-sdk-python-1.0.20230627/src/formance_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/auth.py` & `formance-sdk-python-1.0.20230627/src/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/ledger.py` & `formance-sdk-python-1.0.20230627/src/sdk/ledger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/__init__.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/activateconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/activateconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/addmetadataontransaction.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/addmetadataontransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/addmetadatatoaccount.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/addmetadatatoaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/addscopetoclient.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/addscopetoclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/addtransientscope.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/addtransientscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/cancelevent.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/cancelevent.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/changeconfigsecret.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/changeconfigsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/confirmhold.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/confirmhold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/connectorsstripetransfer.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/connectorsstripetransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/connectorstransfer.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/connectorstransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/countaccounts.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/countaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/counttransactions.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/counttransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createbalance.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/createbalance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createclient.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/createclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createscope.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/createscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createsecret.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/createsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createtransaction.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/createtransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createtransactions.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/createtransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createwallet.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/createwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/createworkflow.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/createworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/creditwallet.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/creditwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deactivateconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/deactivateconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/debitwallet.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/debitwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deleteclient.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/deleteclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deleteconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/deleteconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deletescope.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/deletescope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deletescopefromclient.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/deletescopefromclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deletesecret.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/deletesecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/deletetransientscope.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/deletetransientscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getaccount.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getbalance.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getbalance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getbalances.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getbalancesaggregated.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getbalancesaggregated.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getconnectortask.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getconnectortask.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/gethold.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/gethold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getholds.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getholds.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getinfo.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getinstance.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getinstance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getinstancehistory.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getinstancehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getinstancestagehistory.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getinstancestagehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getledgerinfo.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getledgerinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getmanyconfigs.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getmanyconfigs.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getmapping.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getmapping.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getpayment.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getpayment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getserverinfo.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/gettransaction.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/gettransactions.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/gettransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getversions.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getversions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getwallet.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getwalletsummary.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getwalletsummary.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/getworkflow.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/getworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/insertconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/insertconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/installconnector.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/installconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listaccounts.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listallconnectors.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listallconnectors.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listbalances.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listclients.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listclients.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listconfigsavailableconnectors.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listconfigsavailableconnectors.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listconnectorstransfers.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listconnectorstransfers.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listconnectortasks.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listconnectortasks.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listinstances.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listinstances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listlogs.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listlogs.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listpayments.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listpayments.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listscopes.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listscopes.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listtransactions.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listusers.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listusers.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listwallets.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listwallets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/listworkflows.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/listworkflows.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/orchestrationgetserverinfo.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/orchestrationgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/paymentsgetserverinfo.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/paymentsgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/paymentslistaccounts.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/paymentslistaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/readclient.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/readclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/readconnectorconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/readconnectorconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/readscope.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/readscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/readstats.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/readstats.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/readuser.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/readuser.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/resetconnector.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/resetconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/reverttransaction.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/reverttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/runscript.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/runscript.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/runworkflow.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/runworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/search.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/search.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/searchgetserverinfo.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/searchgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/sendevent.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/sendevent.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/testconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/testconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/uninstallconnector.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/uninstallconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/updateclient.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/updateclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/updatemapping.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/updatemapping.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/updatemetadata.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/updatemetadata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/updatescope.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/updatescope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/updatewallet.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/updatewallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/voidhold.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/voidhold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/operations/walletsgetserverinfo.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/operations/walletsgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/__init__.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/account.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/account.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/accountresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/accountresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/accountscursor.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/accountscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/accountscursorresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/accountscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/accountwithvolumesandbalances.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/accountwithvolumesandbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitycreatetransaction.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitycreatetransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitycreatetransactionoutput.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitycreatetransactionoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitycreditwallet.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitycreditwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitydebitwallet.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitydebitwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitygetaccount.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitygetaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitygetaccountoutput.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitygetaccountoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitygetwalletoutput.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitygetwalletoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activityreverttransaction.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/activityreverttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activityreverttransactionoutput.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/activityreverttransactionoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/activitystripetransfer.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/activitystripetransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/attempt.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/attempt.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/balance.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/balance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/balancescursorresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/balancescursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/balancewithassets.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/balancewithassets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/bankingcircleconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/bankingcircleconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/client.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/client.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/clientsecret.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/clientsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configinfo.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/configinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configinforesponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/configinforesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/configresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/configsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/configuser.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/configuser.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/confirmholdrequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/confirmholdrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/connectorsconfigsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/connectorsconfigsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/connectorsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/connectorsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/contract.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/contract.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createbalancerequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createbalancerequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createbalanceresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createbalanceresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createclientrequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createclientrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createclientresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createscoperequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createscoperequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createscoperesponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createscoperesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createsecretrequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createsecretrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createsecretresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createsecretresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createwalletrequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createwalletrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createwalletresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createwalletresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createworkflowrequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createworkflowrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/createworkflowresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/createworkflowresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/creditwalletrequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/creditwalletrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/currencycloudconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/currencycloudconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/debitwalletrequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/debitwalletrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/debitwalletresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/debitwalletresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/dummypayconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/dummypayconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/error.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/error.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/errorresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/errorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/expandeddebithold.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/expandeddebithold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getbalanceresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/getbalanceresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getholdresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/getholdresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getholdsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/getholdsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/gettransactionsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/gettransactionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getversionsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/getversionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getwalletresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/getwalletresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getwalletsummaryresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/getwalletsummaryresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getworkflowinstancehistoryresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/getworkflowinstancehistoryresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getworkflowinstanceresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/getworkflowinstanceresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/getworkflowresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/getworkflowresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/hold.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/hold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/ledgeraccountsubject.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/ledgeraccountsubject.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/ledgerinfo.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/ledgerinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/ledgerinforesponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/ledgerinforesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/ledgerstorage.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/ledgerstorage.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listbalancesresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/listbalancesresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listclientsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/listclientsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listrunsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/listrunsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listscopesresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/listscopesresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listusersresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/listusersresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listwalletsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/listwalletsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/listworkflowsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/listworkflowsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/log.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/log.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/logscursorresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/logscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/mappingresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/mappingresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/migrationinfo.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/migrationinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/modulrconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/modulrconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/monetary.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/monetary.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/payment.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/payment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/paymentadjustment.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/paymentadjustment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/paymentsaccount.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/paymentsaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/paymentscursor.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/paymentscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/posting.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/posting.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/posttransaction.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/posttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/query.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/query.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/readclientresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/readclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/readscoperesponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/readscoperesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/readuserresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/readuserresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/response.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/response.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/runworkflowresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/runworkflowresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/scope.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/scope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/script.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/script.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/scriptresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/scriptresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/secret.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/secret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagedelay.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagedelay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesend.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesend.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesenddestination.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesenddestination.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesenddestinationaccount.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesenddestinationaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesenddestinationwallet.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesenddestinationwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesendsource.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesendsource.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesendsourceaccount.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesendsourceaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagesendsourcewallet.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagesendsourcewallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stagestatus.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stagestatus.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stats.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stats.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stripeconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stripeconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/stripetransferrequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/stripetransferrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskbankingcircle.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskbankingcircle.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskcurrencycloud.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskcurrencycloud.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskdummypay.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskdummypay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskmodulr.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskmodulr.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskscursor.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskstripe.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskstripe.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/taskwise.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/taskwise.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transaction.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/transaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transactiondata.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/transactiondata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transactionresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/transactionresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transactions.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/transactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transactionscursorresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/transactionscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transactionsresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/transactionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transferrequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/transferrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transferresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/transferresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/transfersresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/transfersresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/updateclientrequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/updateclientrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/updateclientresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/updateclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/updatescoperequest.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/updatescoperequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/updatescoperesponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/updatescoperesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/user.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/version.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/version.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/volume.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/volume.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/wallet.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/wallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/walletserrorresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/walletserrorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/walletstransaction.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/walletstransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/walletsubject.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/walletsubject.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/walletsvolume.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/walletsvolume.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/walletwithbalances.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/walletwithbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/webhooksconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/webhooksconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/webhookserrorresponse.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/webhookserrorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflow.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowconfig.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowinstance.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowinstance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowinstancehistory.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowinstancehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowinstancehistorystage.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowinstancehistorystage.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowinstancehistorystageinput.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowinstancehistorystageinput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/models/shared/workflowinstancehistorystageoutput.py` & `formance-sdk-python-1.0.20230627/src/sdk/models/shared/workflowinstancehistorystageoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/orchestration.py` & `formance-sdk-python-1.0.20230627/src/sdk/orchestration.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/payments.py` & `formance-sdk-python-1.0.20230627/src/sdk/payments.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/sdk.py` & `formance-sdk-python-1.0.20230627/src/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/sdkconfiguration.py` & `formance-sdk-python-1.0.20230627/src/sdk/sdkconfiguration.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     server_defaults: list[dict[str, str]] = field(default_factory=list)
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.20230623'
-    sdk_version: str = 'v1.0.20230623-beta.1'
-    gen_version: str = '2.50.2'
+    sdk_version: str = 'v1.0.20230627'
+    gen_version: str = '2.58.0'
 
     def get_server_details(self) -> tuple[str, dict[str, str]]:
         if self.server_url:
             return self.server_url.removesuffix('/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/search.py` & `formance-sdk-python-1.0.20230627/src/sdk/search.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/utils/retries.py` & `formance-sdk-python-1.0.20230627/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/utils/utils.py` & `formance-sdk-python-1.0.20230627/src/sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/wallets.py` & `formance-sdk-python-1.0.20230627/src/sdk/wallets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230623b1/src/sdk/webhooks.py` & `formance-sdk-python-1.0.20230627/src/sdk/webhooks.py`

 * *Files identical despite different names*

