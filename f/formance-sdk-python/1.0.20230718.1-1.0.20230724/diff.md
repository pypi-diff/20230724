# Comparing `tmp/formance-sdk-python-1.0.20230718.1.tar.gz` & `tmp/formance-sdk-python-1.0.20230724.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formance-sdk-python-1.0.20230718.1.tar", last modified: Tue Jul 18 14:24:11 2023, max compression
+gzip compressed data, was "formance-sdk-python-1.0.20230724.tar", last modified: Mon Jul 24 16:34:45 2023, max compression
```

## Comparing `formance-sdk-python-1.0.20230718.1.tar` & `formance-sdk-python-1.0.20230724.tar`

### file list

```diff
@@ -1,303 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.094396 formance-sdk-python-1.0.20230718.1/
--rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-07-18 14:24:11.094396 formance-sdk-python-1.0.20230718.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9508 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:24:11.094396 formance-sdk-python-1.0.20230718.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1120 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.066396 formance-sdk-python-1.0.20230718.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.070396 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-07-18 14:24:11.000000 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-07-18 14:24:11.000000 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:24:11.000000 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-18 14:24:11.000000 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 14:24:11.000000 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.070396 formance-sdk-python-1.0.20230718.1/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20635 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17440 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/flows.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30317 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/ledger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.070396 formance-sdk-python-1.0.20230718.1/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.078396 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7008 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/activateconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addmetadataontransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1236 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addmetadatatoaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addscopetoclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addtransientscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/cancelevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/changeconfigsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/confirmhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/connectorsstripetransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/connectorstransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1453 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/countaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2997 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/counttransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createbalance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createtransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createtransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/creditwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deactivateconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/debitwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletescope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletescopefromclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletesecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletetransientscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      782 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2443 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1304 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalancesaggregated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getconnectortask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gethold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getholds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstancehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstancestagehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getledgerinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1263 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getmanyconfigs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getmapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gettransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1716 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gettransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getversions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getwalletsummary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/insertconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/installconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3889 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listallconnectors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      640 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listclients.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      676 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconfigsavailableconnectors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconnectorstransfers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconnectortasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listinstances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listlogs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listpayments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listscopes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4638 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listtransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listusers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listwallets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      796 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listworkflows.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/orchestrationgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/paymentsgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/paymentslistaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      846 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readconnectorconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readstats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/resetconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/reverttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/runscript.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/runworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/searchgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/sendevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/testconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/uninstallconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updateclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatemapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatemetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatescope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatewallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/voidhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/walletsgetserverinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.094396 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10236 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      591 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1403 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountwithvolumesandbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityconfirmhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreatetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreatetransactionoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreditwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitydebitwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitydebitwalletoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetaccountoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetpaymentoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      541 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetwalletoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      547 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityreverttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityreverttransactionoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1250 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitystripetransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityvoidhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/aggregatebalancesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/assetholder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/attempt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/attemptresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1013 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balancescursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balancewithassets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1440 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/bankingcircleconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/clientsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      430 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configchangesecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configinforesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      903 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/confirmholdrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connectorconfigresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connectorsconfigsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connectorsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/contract.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createbalancerequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      522 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createbalanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createclientrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createscoperequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createscoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createsecretrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createsecretresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createworkflowrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/creditwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1151 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/currencycloudconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/debitwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/debitwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/dummypayconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      705 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/error.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/errorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/errorsenum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1497 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/expandeddebithold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getbalanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getholdresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getholdsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1498 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/gettransactionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getversionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      553 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getwalletsummaryresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstancehistoryresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/hold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      554 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgeraccountsubject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerinforesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerstorage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listbalancesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      606 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listclientsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listrunsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listscopesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listusersresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listwalletsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      534 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listworkflowsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/logscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/mangopayconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/mapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/mappingresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/migrationinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/modulrconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/monetary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/moneycorpconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3096 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/payment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentadjustment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      505 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentsaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1371 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/posting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/posttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1920 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readscoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readuserresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2380 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/runworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/scope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/script.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/scriptresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/secret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/serverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagedelay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1302 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestinationaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestinationpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestinationwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsourceaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsourcepayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsourcewallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagestatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagewaitevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/statsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stripeconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1249 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stripetransferrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2282 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskbankingcircle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2114 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskcurrencycloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskdummypay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskmangopay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskmodulr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskmoneycorp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      457 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2328 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskstripe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2436 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskwise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactiondata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transferrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transferresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2049 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transfersresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updateclientrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updateclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updatescoperequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updatescoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/volume.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/wallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      714 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletserrorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsposting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2106 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletstransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsubject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsvolume.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletwithbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/webhooksconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      902 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/webhookserrorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      507 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/webhookserrorsenum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/wiseconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2040 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1530 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3399 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystageinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystageoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19606 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5286 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3152 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.094396 formance-sdk-python-1.0.20230718.1/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22535 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/wallets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11685 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:34:45.875444 formance-sdk-python-1.0.20230724/
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-24 16:34:45.875444 formance-sdk-python-1.0.20230724/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9508 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:34:45.875444 formance-sdk-python-1.0.20230724/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1118 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:34:45.795440 formance-sdk-python-1.0.20230724/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:34:45.803440 formance-sdk-python-1.0.20230724/src/formance_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-24 16:34:45.000000 formance-sdk-python-1.0.20230724/src/formance_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-07-24 16:34:45.000000 formance-sdk-python-1.0.20230724/src/formance_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:34:45.000000 formance-sdk-python-1.0.20230724/src/formance_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-24 16:34:45.000000 formance-sdk-python-1.0.20230724/src/formance_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 16:34:45.000000 formance-sdk-python-1.0.20230724/src/formance_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:34:45.803440 formance-sdk-python-1.0.20230724/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20635 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17440 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/flows.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30317 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/ledger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:34:45.807440 formance-sdk-python-1.0.20230724/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:34:45.831441 formance-sdk-python-1.0.20230724/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7008 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/activateconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/addmetadataontransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1236 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/addmetadatatoaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/addscopetoclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/addtransientscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/cancelevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/changeconfigsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/confirmhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/connectorsstripetransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/connectorstransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1453 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/countaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2997 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/counttransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/createbalance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/createclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/createscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/createsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/createtransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/createtransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/createwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/createworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/creditwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/deactivateconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/debitwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/deleteclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/deleteconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/deletescope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/deletescopefromclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/deletesecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/deletetransientscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      782 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/deleteworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getbalance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2443 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1304 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getbalancesaggregated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getconnectortask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/gethold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getholds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getinstance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getinstancehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getinstancestagehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getledgerinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1263 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getmanyconfigs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getmapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/gettransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1716 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/gettransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getversions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getwalletsummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/getworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/insertconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/installconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3889 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listallconnectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      640 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listclients.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      676 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listconfigsavailableconnectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listconnectorstransfers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listconnectortasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listinstances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listlogs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listpayments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listscopes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4638 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listtransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listusers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listwallets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      796 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/listworkflows.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/orchestrationgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/paymentsgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/paymentslistaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      846 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/readclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/readconnectorconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/readscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/readstats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/readuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/resetconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/reverttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/runscript.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/runworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/searchgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/sendevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/testconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/uninstallconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/updateclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/updatemapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/updatemetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/updatescope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/updatewallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/voidhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/operations/walletsgetserverinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:34:45.871444 formance-sdk-python-1.0.20230724/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10236 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      591 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/accountresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1403 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/accountscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/accountscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/accountwithvolumesandbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activityconfirmhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitycreatetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitycreatetransactionoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitycreditwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitydebitwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitydebitwalletoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitygetaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitygetaccountoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitygetpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitygetpaymentoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitygetwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      541 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitygetwalletoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      547 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activityreverttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activityreverttransactionoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1250 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitystripetransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/activityvoidhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/aggregatebalancesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/assetholder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/attempt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/attemptresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1013 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/balance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/balancescursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/balancewithassets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1440 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/bankingcircleconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/clientsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      430 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/configchangesecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/configinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/configinforesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/configresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      903 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/configsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/configuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/confirmholdrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/connectorconfigresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/connectorsconfigsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/connectorsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/contract.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createbalancerequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      522 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createbalanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createclientrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createscoperequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createscoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createsecretrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createsecretresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createworkflowrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/createworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/creditwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1151 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/currencycloudconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/debitwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/debitwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/dummypayconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      705 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/error.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/errorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/errorsenum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1497 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/expandeddebithold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/getbalanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/getholdresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/getholdsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1498 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/gettransactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/getversionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      553 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/getwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/getwalletsummaryresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/getworkflowinstancehistoryresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/getworkflowinstanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/getworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/hold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      554 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/ledgeraccountsubject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/ledgerinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/ledgerinforesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/ledgerstorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/listbalancesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      606 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/listclientsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/listrunsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/listscopesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/listusersresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/listwalletsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      534 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/listworkflowsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/logscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/mangopayconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/mapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/mappingresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/migrationinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/modulrconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/monetary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/moneycorpconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3096 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/payment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/paymentadjustment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      505 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/paymentmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/paymentresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/paymentsaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1371 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/paymentscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/paymentstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/posting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/posttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1920 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/readclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/readscoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/readuserresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2380 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/runworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/scope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/script.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/scriptresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/secret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/serverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagedelay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1302 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesenddestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesenddestinationaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesenddestinationpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesenddestinationwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesendsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesendsourceaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesendsourcepayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesendsourcewallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagestatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagewaitevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/statsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stripeconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1249 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/stripetransferrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2282 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskbankingcircle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2114 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskcurrencycloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskdummypay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskmangopay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskmodulr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskmoneycorp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      457 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2328 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskstripe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2436 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskwise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/transactiondata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/transactionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/transactionscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/transactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/transferrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/transferresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2049 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/transfersresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/updateclientrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/updateclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/updatescoperequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/updatescoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/wallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      714 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletserrorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletsposting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2106 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletstransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletsubject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletsvolume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletwithbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/webhooksconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      902 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/webhookserrorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      507 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/webhookserrorsenum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/wiseconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2040 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowinstance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1530 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowinstancehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowinstancehistorystage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3399 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowinstancehistorystageinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowinstancehistorystageoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19606 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5284 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3152 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:34:45.871444 formance-sdk-python-1.0.20230724/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22535 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/wallets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11685 2023-07-24 16:34:30.000000 formance-sdk-python-1.0.20230724/src/sdk/webhooks.py
```

### Comparing `formance-sdk-python-1.0.20230718.1/PKG-INFO` & `formance-sdk-python-1.0.20230724/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formance-sdk-python
-Version: 1.0.20230718.1
+Version: 1.0.20230724
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Formance
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `formance-sdk-python-1.0.20230718.1/README.md` & `formance-sdk-python-1.0.20230724/README.md`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/setup.py` & `formance-sdk-python-1.0.20230724/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="formance-sdk-python",
-    version="v1.0.20230718.1",
+    version="v1.0.20230724",
     author="Formance",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/PKG-INFO` & `formance-sdk-python-1.0.20230724/src/formance_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formance-sdk-python
-Version: 1.0.20230718.1
+Version: 1.0.20230724
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Formance
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/SOURCES.txt` & `formance-sdk-python-1.0.20230724/src/formance_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/auth.py` & `formance-sdk-python-1.0.20230724/src/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/flows.py` & `formance-sdk-python-1.0.20230724/src/sdk/flows.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/ledger.py` & `formance-sdk-python-1.0.20230724/src/sdk/ledger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/__init__.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/activateconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/activateconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addmetadataontransaction.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/addmetadataontransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addmetadatatoaccount.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/addmetadatatoaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addscopetoclient.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/addscopetoclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addtransientscope.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/addtransientscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/cancelevent.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/cancelevent.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/changeconfigsecret.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/changeconfigsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/confirmhold.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/confirmhold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/connectorsstripetransfer.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/connectorsstripetransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/connectorstransfer.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/connectorstransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/countaccounts.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/countaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/counttransactions.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/counttransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createbalance.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/createbalance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createclient.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/createclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createscope.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/createscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createsecret.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/createsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createtransaction.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/createtransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createtransactions.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/createtransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createwallet.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/createwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createworkflow.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/createworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/creditwallet.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/creditwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deactivateconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/deactivateconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/debitwallet.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/debitwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteclient.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/deleteclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/deleteconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletescope.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/deletescope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletescopefromclient.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/deletescopefromclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletesecret.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/deletesecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletetransientscope.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/deletetransientscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteworkflow.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/deleteworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getaccount.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalance.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getbalance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalances.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalancesaggregated.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getbalancesaggregated.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getconnectortask.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getconnectortask.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gethold.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/gethold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getholds.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getholds.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinfo.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstance.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getinstance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstancehistory.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getinstancehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstancestagehistory.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getinstancestagehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getledgerinfo.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getledgerinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getmanyconfigs.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getmanyconfigs.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getmapping.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getmapping.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getpayment.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getpayment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getserverinfo.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gettransaction.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gettransactions.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/gettransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getversions.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getversions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getwallet.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getwalletsummary.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getwalletsummary.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getworkflow.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/getworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/insertconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/insertconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/installconnector.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/installconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listaccounts.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listallconnectors.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listallconnectors.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listbalances.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listclients.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listclients.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconfigsavailableconnectors.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listconfigsavailableconnectors.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconnectorstransfers.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listconnectorstransfers.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconnectortasks.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listconnectortasks.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listinstances.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listinstances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listlogs.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listlogs.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listpayments.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listpayments.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listscopes.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listscopes.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listtransactions.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listusers.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listusers.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listwallets.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listwallets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listworkflows.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/listworkflows.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/orchestrationgetserverinfo.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/orchestrationgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/paymentsgetserverinfo.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/paymentsgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/paymentslistaccounts.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/paymentslistaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readclient.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/readclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readconnectorconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/readconnectorconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readscope.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/readscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readstats.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/readstats.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readuser.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/readuser.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/resetconnector.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/resetconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/reverttransaction.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/reverttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/runscript.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/runscript.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/runworkflow.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/runworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/search.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/search.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/searchgetserverinfo.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/searchgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/sendevent.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/sendevent.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/testconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/testconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/uninstallconnector.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/uninstallconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updateclient.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/updateclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatemapping.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/updatemapping.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatemetadata.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/updatemetadata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatescope.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/updatescope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatewallet.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/updatewallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/voidhold.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/voidhold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/walletsgetserverinfo.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/operations/walletsgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/__init__.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/account.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/account.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/accountresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountscursor.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/accountscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountscursorresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/accountscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountwithvolumesandbalances.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/accountwithvolumesandbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreatetransaction.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitycreatetransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreatetransactionoutput.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitycreatetransactionoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreditwallet.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitycreditwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitydebitwallet.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitydebitwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetaccount.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitygetaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetaccountoutput.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitygetaccountoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetwalletoutput.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitygetwalletoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityreverttransaction.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/activityreverttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityreverttransactionoutput.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/activityreverttransactionoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitystripetransfer.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/activitystripetransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/attempt.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/attempt.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balance.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/balance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balancescursorresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/balancescursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balancewithassets.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/balancewithassets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/bankingcircleconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/bankingcircleconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/client.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/client.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/clientsecret.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/clientsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configinfo.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/configinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configinforesponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/configinforesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/configresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/configsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configuser.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/configuser.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/confirmholdrequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/confirmholdrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connectorsconfigsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/connectorsconfigsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connectorsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/connectorsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/contract.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/contract.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createbalancerequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createbalancerequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createbalanceresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createbalanceresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createclientrequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createclientrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createclientresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createscoperequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createscoperequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createscoperesponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createscoperesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createsecretrequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createsecretrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createsecretresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createsecretresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createwalletrequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createwalletrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createwalletresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createwalletresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createworkflowrequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createworkflowrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createworkflowresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/createworkflowresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/creditwalletrequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/creditwalletrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/currencycloudconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/currencycloudconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/debitwalletrequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/debitwalletrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/debitwalletresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/debitwalletresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/dummypayconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/dummypayconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/error.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/error.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/errorresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/errorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/expandeddebithold.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/expandeddebithold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getbalanceresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/getbalanceresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getholdresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/getholdresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getholdsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/getholdsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/gettransactionsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/gettransactionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getversionsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/getversionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getwalletresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/getwalletresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getwalletsummaryresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/getwalletsummaryresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstancehistoryresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/getworkflowinstancehistoryresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstanceresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/getworkflowinstanceresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/getworkflowresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/hold.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/hold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgeraccountsubject.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/ledgeraccountsubject.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerinfo.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/ledgerinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerinforesponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/ledgerinforesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerstorage.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/ledgerstorage.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listbalancesresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/listbalancesresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listclientsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/listclientsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listrunsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/listrunsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listscopesresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/listscopesresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listusersresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/listusersresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listwalletsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/listwalletsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listworkflowsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/listworkflowsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/log.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/log.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/logscursorresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/logscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/mangopayconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/mangopayconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/mappingresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/mappingresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/migrationinfo.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/migrationinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/modulrconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/modulrconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/monetary.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/monetary.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/moneycorpconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/moneycorpconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/payment.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/payment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentadjustment.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/paymentadjustment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentsaccount.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/paymentsaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentscursor.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/paymentscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/posting.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/posting.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/posttransaction.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/posttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/query.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/query.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readclientresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/readclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readscoperesponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/readscoperesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readuserresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/readuserresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/response.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/response.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/runworkflowresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/runworkflowresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/scope.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/scope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/script.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/script.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/scriptresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/scriptresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/secret.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/secret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagedelay.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagedelay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesend.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesend.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestination.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesenddestination.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestinationaccount.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesenddestinationaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestinationwallet.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesenddestinationwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsource.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesendsource.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsourceaccount.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesendsourceaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsourcewallet.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagesendsourcewallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagestatus.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stagestatus.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stats.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stats.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stripeconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stripeconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stripetransferrequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/stripetransferrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskbankingcircle.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskbankingcircle.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskcurrencycloud.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskcurrencycloud.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskdummypay.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskdummypay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskmangopay.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskmangopay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskmodulr.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskmodulr.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskmoneycorp.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskmoneycorp.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskscursor.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskstripe.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskstripe.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskwise.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/taskwise.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transaction.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/transaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactiondata.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/transactiondata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/transactionresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactions.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/transactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionscursorresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/transactionscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionsresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/transactionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transferrequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/transferrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transferresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/transferresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transfersresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/transfersresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updateclientrequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/updateclientrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updateclientresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/updateclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updatescoperequest.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/updatescoperequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updatescoperesponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/updatescoperesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/user.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/version.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/version.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/volume.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/volume.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/wallet.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/wallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletserrorresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletserrorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsposting.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletsposting.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletstransaction.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletstransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsubject.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletsubject.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsvolume.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletsvolume.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletwithbalances.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/walletwithbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/webhooksconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/webhooksconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/webhookserrorresponse.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/webhookserrorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/wiseconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/wiseconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflow.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowconfig.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstance.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowinstance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistory.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowinstancehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystage.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowinstancehistorystage.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystageinput.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowinstancehistorystageinput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystageoutput.py` & `formance-sdk-python-1.0.20230724/src/sdk/models/shared/workflowinstancehistorystageoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/payments.py` & `formance-sdk-python-1.0.20230724/src/sdk/payments.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/sdk.py` & `formance-sdk-python-1.0.20230724/src/sdk/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     wallets: Wallets
     webhooks: Webhooks
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "v1.0.20230718.1"
+    _sdk_version: str = "v1.0.20230724"
     _gen_version: str = "2.31.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
```

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/search.py` & `formance-sdk-python-1.0.20230724/src/sdk/search.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/utils/retries.py` & `formance-sdk-python-1.0.20230724/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/utils/utils.py` & `formance-sdk-python-1.0.20230724/src/sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/wallets.py` & `formance-sdk-python-1.0.20230724/src/sdk/wallets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718.1/src/sdk/webhooks.py` & `formance-sdk-python-1.0.20230724/src/sdk/webhooks.py`

 * *Files identical despite different names*

