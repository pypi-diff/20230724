# Comparing `tmp/formance-sdk-python-1.0.20230718.tar.gz` & `tmp/formance-sdk-python-1.0.20230718.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formance-sdk-python-1.0.20230718.tar", last modified: Tue Jul 18 10:36:34 2023, max compression
+gzip compressed data, was "formance-sdk-python-1.0.20230718.1.tar", last modified: Tue Jul 18 14:24:11 2023, max compression
```

## Comparing `formance-sdk-python-1.0.20230718.tar` & `formance-sdk-python-1.0.20230718.1.tar`

### file list

```diff
@@ -1,297 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.410211 formance-sdk-python-1.0.20230718/
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-18 10:36:34.410211 formance-sdk-python-1.0.20230718/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9412 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:36:34.410211 formance-sdk-python-1.0.20230718/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1118 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.346211 formance-sdk-python-1.0.20230718/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.350211 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-18 10:36:34.000000 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-07-18 10:36:34.000000 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:36:34.000000 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-18 10:36:34.000000 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 10:36:34.000000 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.354211 formance-sdk-python-1.0.20230718/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20635 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16276 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/flows.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30317 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/ledger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.354211 formance-sdk-python-1.0.20230718/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.370211 formance-sdk-python-1.0.20230718/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6913 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/activateconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/addmetadataontransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1236 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/addmetadatatoaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/addscopetoclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/addtransientscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/cancelevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/changeconfigsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/confirmhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/connectorsstripetransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/connectorstransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1453 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/countaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2997 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/counttransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createbalance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createtransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createtransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/creditwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deactivateconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/debitwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deleteclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deleteconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletescope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletescopefromclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletesecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletetransientscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/flowsgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2443 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1304 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalancesaggregated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getconnectortask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/gethold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getholds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstancehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstancestagehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getledgerinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1263 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getmanyconfigs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getmapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/gettransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1716 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/gettransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getversions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getwalletsummary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/insertconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/installconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3889 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listallconnectors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      640 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listclients.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      676 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconfigsavailableconnectors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconnectorstransfers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconnectortasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listinstances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listlogs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listpayments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listscopes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4638 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listtransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listusers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listwallets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      796 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listworkflows.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/paymentsgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/paymentslistaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      846 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/readclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/readconnectorconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/readscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/readstats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/readuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/resetconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/reverttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/runscript.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/runworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/searchgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/sendevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/testconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/uninstallconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/updateclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatemapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatemetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatescope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatewallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/voidhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/walletsgetserverinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.410211 formance-sdk-python-1.0.20230718/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9954 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      591 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1403 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountwithvolumesandbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityconfirmhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreatetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreatetransactionoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreditwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitydebitwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitydebitwalletoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetaccountoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetpaymentoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      541 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetwalletoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      547 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityreverttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityreverttransactionoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1250 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitystripetransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityvoidhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/aggregatebalancesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/assetholder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/attempt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/attemptresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1013 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/balance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/balancescursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/balancewithassets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/bankingcircleconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/clientsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      430 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configchangesecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configinforesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      903 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/confirmholdrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/connector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/connectorconfigresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/connectorsconfigsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/connectorsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/contract.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createbalancerequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      522 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createbalanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createclientrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createscoperequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createscoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createsecretrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createsecretresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createworkflowrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/creditwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1151 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/currencycloudconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/debitwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/debitwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/dummypayconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      705 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/error.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/errorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/errorsenum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1497 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/expandeddebithold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getbalanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getholdresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getholdsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1498 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/gettransactionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getversionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      553 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getwalletsummaryresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstancehistoryresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/hold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      554 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgeraccountsubject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerinforesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerstorage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listbalancesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      606 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listclientsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listrunsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listscopesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listusersresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listwalletsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      534 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listworkflowsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/logscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/mapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/mappingresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/migrationinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/modulrconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/monetary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3096 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/payment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentadjustment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      505 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentsaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1371 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/posting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/posttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1920 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/readclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/readscoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/readuserresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2380 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/runworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/scope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/script.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/scriptresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/secret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/serverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagedelay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1302 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestinationaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestinationpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestinationwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsourceaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsourcepayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsourcewallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagestatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagewaitevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/statsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stripeconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1249 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stripetransferrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2282 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskbankingcircle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2114 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskcurrencycloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskdummypay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskmodulr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      457 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2328 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskstripe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2436 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskwise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactiondata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transferrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transferresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2049 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transfersresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/updateclientrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/updateclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/updatescoperequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/updatescoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/volume.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/wallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      714 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletserrorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2078 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletstransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletsubject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletsvolume.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletwithbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/webhooksconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      902 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/webhookserrorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      507 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/webhookserrorsenum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/wiseconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2040 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1530 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3399 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystageinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystageoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19606 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5284 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3152 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.410211 formance-sdk-python-1.0.20230718/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22535 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/wallets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11685 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.094396 formance-sdk-python-1.0.20230718.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-07-18 14:24:11.094396 formance-sdk-python-1.0.20230718.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9508 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:24:11.094396 formance-sdk-python-1.0.20230718.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1120 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.066396 formance-sdk-python-1.0.20230718.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.070396 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-07-18 14:24:11.000000 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-07-18 14:24:11.000000 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:24:11.000000 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-18 14:24:11.000000 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 14:24:11.000000 formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.070396 formance-sdk-python-1.0.20230718.1/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20635 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17440 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/flows.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30317 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/ledger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.070396 formance-sdk-python-1.0.20230718.1/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.078396 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7008 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/activateconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addmetadataontransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1236 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addmetadatatoaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addscopetoclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addtransientscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/cancelevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/changeconfigsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/confirmhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/connectorsstripetransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/connectorstransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1453 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/countaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2997 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/counttransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createbalance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createtransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createtransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/creditwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deactivateconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/debitwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletescope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletescopefromclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletesecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletetransientscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      782 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2443 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1304 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalancesaggregated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getconnectortask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gethold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getholds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstancehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstancestagehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getledgerinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1263 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getmanyconfigs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getmapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gettransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1716 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gettransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getversions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getwalletsummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/insertconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/installconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3889 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listallconnectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      640 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listclients.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      676 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconfigsavailableconnectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconnectorstransfers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconnectortasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listinstances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listlogs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listpayments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listscopes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4638 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listtransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listusers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listwallets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      796 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listworkflows.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/orchestrationgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/paymentsgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/paymentslistaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      846 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readconnectorconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readstats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/resetconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/reverttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/runscript.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/runworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/searchgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/sendevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/testconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/uninstallconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updateclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatemapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatemetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatescope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatewallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/voidhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/walletsgetserverinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.094396 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10236 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      591 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1403 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountwithvolumesandbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityconfirmhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreatetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreatetransactionoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreditwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitydebitwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitydebitwalletoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetaccountoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetpaymentoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      541 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetwalletoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      547 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityreverttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityreverttransactionoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1250 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitystripetransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityvoidhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/aggregatebalancesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/assetholder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/attempt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/attemptresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1013 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balancescursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balancewithassets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1440 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/bankingcircleconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/clientsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      430 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configchangesecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configinforesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      903 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/confirmholdrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connectorconfigresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connectorsconfigsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connectorsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/contract.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createbalancerequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      522 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createbalanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createclientrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createscoperequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createscoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createsecretrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createsecretresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createworkflowrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/creditwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1151 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/currencycloudconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/debitwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/debitwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/dummypayconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      705 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/error.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/errorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/errorsenum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1497 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/expandeddebithold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getbalanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getholdresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getholdsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1498 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/gettransactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getversionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      553 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getwalletsummaryresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstancehistoryresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/hold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      554 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgeraccountsubject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerinforesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerstorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listbalancesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      606 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listclientsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listrunsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listscopesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listusersresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listwalletsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      534 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listworkflowsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/logscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/mangopayconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/mapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/mappingresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/migrationinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/modulrconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/monetary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/moneycorpconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3096 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/payment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentadjustment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      505 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentsaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1371 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/posting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/posttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1920 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readscoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readuserresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2380 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/runworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/scope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/script.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/scriptresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/secret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/serverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagedelay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1302 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestinationaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestinationpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestinationwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsourceaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsourcepayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsourcewallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagestatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagewaitevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/statsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stripeconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1249 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stripetransferrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2282 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskbankingcircle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2114 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskcurrencycloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskdummypay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskmangopay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskmodulr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskmoneycorp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      457 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2328 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskstripe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2436 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskwise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactiondata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transferrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transferresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2049 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transfersresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updateclientrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updateclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updatescoperequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updatescoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/wallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      714 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletserrorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsposting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2106 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletstransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsubject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsvolume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletwithbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/webhooksconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      902 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/webhookserrorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      507 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/webhookserrorsenum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/wiseconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2040 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1530 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3399 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystageinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystageoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19606 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5286 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3152 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:24:11.094396 formance-sdk-python-1.0.20230718.1/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22535 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/wallets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11685 2023-07-18 14:23:55.000000 formance-sdk-python-1.0.20230718.1/src/sdk/webhooks.py
```

### Comparing `formance-sdk-python-1.0.20230718/PKG-INFO` & `formance-sdk-python-1.0.20230718.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formance-sdk-python
-Version: 1.0.20230718
+Version: 1.0.20230718.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Formance
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -66,23 +66,24 @@
 * [read_scope](docs/auth/README.md#read_scope) - Read scope
 * [read_user](docs/auth/README.md#read_user) - Read user
 * [update_client](docs/auth/README.md#update_client) - Update client
 * [update_scope](docs/auth/README.md#update_scope) - Update scope
 
 ### [flows](docs/flows/README.md)
 
-* [flowsget_server_info](docs/flows/README.md#flowsget_server_info) - Get server info
 * [cancel_event](docs/flows/README.md#cancel_event) - Cancel a running workflow
 * [create_workflow](docs/flows/README.md#create_workflow) - Create workflow
+* [delete_workflow](docs/flows/README.md#delete_workflow) - Delete a flow by id
 * [get_instance](docs/flows/README.md#get_instance) - Get a workflow instance by id
 * [get_instance_history](docs/flows/README.md#get_instance_history) - Get a workflow instance history by id
 * [get_instance_stage_history](docs/flows/README.md#get_instance_stage_history) - Get a workflow instance stage history
 * [get_workflow](docs/flows/README.md#get_workflow) - Get a flow by id
 * [list_instances](docs/flows/README.md#list_instances) - List instances of a workflow
 * [list_workflows](docs/flows/README.md#list_workflows) - List registered workflows
+* [orchestrationget_server_info](docs/flows/README.md#orchestrationget_server_info) - Get server info
 * [run_workflow](docs/flows/README.md#run_workflow) - Run workflow
 * [send_event](docs/flows/README.md#send_event) - Send an event to a running workflow
 
 ### [ledger](docs/ledger/README.md)
 
 * [create_transactions](docs/ledger/README.md#create_transactions) - Create a new batch of transactions to a ledger
 * [add_metadata_on_transaction](docs/ledger/README.md#add_metadata_on_transaction) - Set the metadata of a transaction by its ID
```

### Comparing `formance-sdk-python-1.0.20230718/README.md` & `formance-sdk-python-1.0.20230718.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,23 +55,24 @@
 * [read_scope](docs/auth/README.md#read_scope) - Read scope
 * [read_user](docs/auth/README.md#read_user) - Read user
 * [update_client](docs/auth/README.md#update_client) - Update client
 * [update_scope](docs/auth/README.md#update_scope) - Update scope
 
 ### [flows](docs/flows/README.md)
 
-* [flowsget_server_info](docs/flows/README.md#flowsget_server_info) - Get server info
 * [cancel_event](docs/flows/README.md#cancel_event) - Cancel a running workflow
 * [create_workflow](docs/flows/README.md#create_workflow) - Create workflow
+* [delete_workflow](docs/flows/README.md#delete_workflow) - Delete a flow by id
 * [get_instance](docs/flows/README.md#get_instance) - Get a workflow instance by id
 * [get_instance_history](docs/flows/README.md#get_instance_history) - Get a workflow instance history by id
 * [get_instance_stage_history](docs/flows/README.md#get_instance_stage_history) - Get a workflow instance stage history
 * [get_workflow](docs/flows/README.md#get_workflow) - Get a flow by id
 * [list_instances](docs/flows/README.md#list_instances) - List instances of a workflow
 * [list_workflows](docs/flows/README.md#list_workflows) - List registered workflows
+* [orchestrationget_server_info](docs/flows/README.md#orchestrationget_server_info) - Get server info
 * [run_workflow](docs/flows/README.md#run_workflow) - Run workflow
 * [send_event](docs/flows/README.md#send_event) - Send an event to a running workflow
 
 ### [ledger](docs/ledger/README.md)
 
 * [create_transactions](docs/ledger/README.md#create_transactions) - Create a new batch of transactions to a ledger
 * [add_metadata_on_transaction](docs/ledger/README.md#add_metadata_on_transaction) - Set the metadata of a transaction by its ID
```

### Comparing `formance-sdk-python-1.0.20230718/setup.py` & `formance-sdk-python-1.0.20230718.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="formance-sdk-python",
-    version="v1.0.20230718",
+    version="v1.0.20230718.1",
     author="Formance",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/PKG-INFO` & `formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formance-sdk-python
-Version: 1.0.20230718
+Version: 1.0.20230718.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Formance
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -66,23 +66,24 @@
 * [read_scope](docs/auth/README.md#read_scope) - Read scope
 * [read_user](docs/auth/README.md#read_user) - Read user
 * [update_client](docs/auth/README.md#update_client) - Update client
 * [update_scope](docs/auth/README.md#update_scope) - Update scope
 
 ### [flows](docs/flows/README.md)
 
-* [flowsget_server_info](docs/flows/README.md#flowsget_server_info) - Get server info
 * [cancel_event](docs/flows/README.md#cancel_event) - Cancel a running workflow
 * [create_workflow](docs/flows/README.md#create_workflow) - Create workflow
+* [delete_workflow](docs/flows/README.md#delete_workflow) - Delete a flow by id
 * [get_instance](docs/flows/README.md#get_instance) - Get a workflow instance by id
 * [get_instance_history](docs/flows/README.md#get_instance_history) - Get a workflow instance history by id
 * [get_instance_stage_history](docs/flows/README.md#get_instance_stage_history) - Get a workflow instance stage history
 * [get_workflow](docs/flows/README.md#get_workflow) - Get a flow by id
 * [list_instances](docs/flows/README.md#list_instances) - List instances of a workflow
 * [list_workflows](docs/flows/README.md#list_workflows) - List registered workflows
+* [orchestrationget_server_info](docs/flows/README.md#orchestrationget_server_info) - Get server info
 * [run_workflow](docs/flows/README.md#run_workflow) - Run workflow
 * [send_event](docs/flows/README.md#send_event) - Send an event to a running workflow
 
 ### [ledger](docs/ledger/README.md)
 
 * [create_transactions](docs/ledger/README.md#create_transactions) - Create a new batch of transactions to a ledger
 * [add_metadata_on_transaction](docs/ledger/README.md#add_metadata_on_transaction) - Set the metadata of a transaction by its ID
```

### Comparing `formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/SOURCES.txt` & `formance-sdk-python-1.0.20230718.1/src/formance_sdk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 src/sdk/models/operations/debitwallet.py
 src/sdk/models/operations/deleteclient.py
 src/sdk/models/operations/deleteconfig.py
 src/sdk/models/operations/deletescope.py
 src/sdk/models/operations/deletescopefromclient.py
 src/sdk/models/operations/deletesecret.py
 src/sdk/models/operations/deletetransientscope.py
-src/sdk/models/operations/flowsgetserverinfo.py
+src/sdk/models/operations/deleteworkflow.py
 src/sdk/models/operations/getaccount.py
 src/sdk/models/operations/getbalance.py
 src/sdk/models/operations/getbalances.py
 src/sdk/models/operations/getbalancesaggregated.py
 src/sdk/models/operations/getconnectortask.py
 src/sdk/models/operations/gethold.py
 src/sdk/models/operations/getholds.py
@@ -81,14 +81,15 @@
 src/sdk/models/operations/listlogs.py
 src/sdk/models/operations/listpayments.py
 src/sdk/models/operations/listscopes.py
 src/sdk/models/operations/listtransactions.py
 src/sdk/models/operations/listusers.py
 src/sdk/models/operations/listwallets.py
 src/sdk/models/operations/listworkflows.py
+src/sdk/models/operations/orchestrationgetserverinfo.py
 src/sdk/models/operations/paymentsgetserverinfo.py
 src/sdk/models/operations/paymentslistaccounts.py
 src/sdk/models/operations/readclient.py
 src/sdk/models/operations/readconnectorconfig.py
 src/sdk/models/operations/readscope.py
 src/sdk/models/operations/readstats.py
 src/sdk/models/operations/readuser.py
@@ -195,19 +196,21 @@
 src/sdk/models/shared/listrunsresponse.py
 src/sdk/models/shared/listscopesresponse.py
 src/sdk/models/shared/listusersresponse.py
 src/sdk/models/shared/listwalletsresponse.py
 src/sdk/models/shared/listworkflowsresponse.py
 src/sdk/models/shared/log.py
 src/sdk/models/shared/logscursorresponse.py
+src/sdk/models/shared/mangopayconfig.py
 src/sdk/models/shared/mapping.py
 src/sdk/models/shared/mappingresponse.py
 src/sdk/models/shared/migrationinfo.py
 src/sdk/models/shared/modulrconfig.py
 src/sdk/models/shared/monetary.py
+src/sdk/models/shared/moneycorpconfig.py
 src/sdk/models/shared/payment.py
 src/sdk/models/shared/paymentadjustment.py
 src/sdk/models/shared/paymentmetadata.py
 src/sdk/models/shared/paymentresponse.py
 src/sdk/models/shared/paymentsaccount.py
 src/sdk/models/shared/paymentscursor.py
 src/sdk/models/shared/paymentstatus.py
@@ -240,15 +243,17 @@
 src/sdk/models/shared/stats.py
 src/sdk/models/shared/statsresponse.py
 src/sdk/models/shared/stripeconfig.py
 src/sdk/models/shared/stripetransferrequest.py
 src/sdk/models/shared/taskbankingcircle.py
 src/sdk/models/shared/taskcurrencycloud.py
 src/sdk/models/shared/taskdummypay.py
+src/sdk/models/shared/taskmangopay.py
 src/sdk/models/shared/taskmodulr.py
+src/sdk/models/shared/taskmoneycorp.py
 src/sdk/models/shared/taskresponse.py
 src/sdk/models/shared/taskscursor.py
 src/sdk/models/shared/taskstripe.py
 src/sdk/models/shared/taskwise.py
 src/sdk/models/shared/transaction.py
 src/sdk/models/shared/transactiondata.py
 src/sdk/models/shared/transactionresponse.py
@@ -263,14 +268,15 @@
 src/sdk/models/shared/updatescoperequest.py
 src/sdk/models/shared/updatescoperesponse.py
 src/sdk/models/shared/user.py
 src/sdk/models/shared/version.py
 src/sdk/models/shared/volume.py
 src/sdk/models/shared/wallet.py
 src/sdk/models/shared/walletserrorresponse.py
+src/sdk/models/shared/walletsposting.py
 src/sdk/models/shared/walletstransaction.py
 src/sdk/models/shared/walletsubject.py
 src/sdk/models/shared/walletsvolume.py
 src/sdk/models/shared/walletwithbalances.py
 src/sdk/models/shared/webhooksconfig.py
 src/sdk/models/shared/webhookserrorresponse.py
 src/sdk/models/shared/webhookserrorsenum.py
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/auth.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/flows.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/flows.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,42 +18,14 @@
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     
-    def flowsget_server_info(self) -> operations.FlowsgetServerInfoResponse:
-        r"""Get server info"""
-        base_url = self._server_url
-        
-        url = base_url.removesuffix('/') + '/api/orchestration/_info'
-        headers = {}
-        headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
-        
-        client = self._security_client
-        
-        http_res = client.request('GET', url, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.FlowsgetServerInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.ServerInfo])
-                res.server_info = out
-        else:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Error])
-                res.error = out
-
-        return res
-
-    
     def cancel_event(self, request: operations.CancelEventRequest) -> operations.CancelEventResponse:
         r"""Cancel a running workflow
         Cancel a running workflow
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.CancelEventRequest, base_url, '/api/orchestration/instances/{instanceID}/abort', request)
@@ -107,14 +79,42 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Error])
                 res.error = out
 
         return res
 
     
+    def delete_workflow(self, request: operations.DeleteWorkflowRequest) -> operations.DeleteWorkflowResponse:
+        r"""Delete a flow by id
+        Delete a flow by id
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.DeleteWorkflowRequest, base_url, '/api/orchestration/workflows/{flowId}', request)
+        headers = {}
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        client = self._security_client
+        
+        http_res = client.request('DELETE', url, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.DeleteWorkflowResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 204:
+            pass
+        else:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Error])
+                res.error = out
+
+        return res
+
+    
     def get_instance(self, request: operations.GetInstanceRequest) -> operations.GetInstanceResponse:
         r"""Get a workflow instance by id
         Get a workflow instance by id
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetInstanceRequest, base_url, '/api/orchestration/instances/{instanceID}', request)
@@ -287,14 +287,42 @@
         else:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Error])
                 res.error = out
 
         return res
 
+    
+    def orchestrationget_server_info(self) -> operations.OrchestrationgetServerInfoResponse:
+        r"""Get server info"""
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/api/orchestration/_info'
+        headers = {}
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.OrchestrationgetServerInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.ServerInfo])
+                res.server_info = out
+        else:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Error])
+                res.error = out
+
+        return res
+
     
     def run_workflow(self, request: operations.RunWorkflowRequest) -> operations.RunWorkflowResponse:
         r"""Run workflow
         Run workflow
         """
         base_url = self._server_url
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/ledger.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/ledger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/__init__.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from .debitwallet import *
 from .deleteclient import *
 from .deleteconfig import *
 from .deletescope import *
 from .deletescopefromclient import *
 from .deletesecret import *
 from .deletetransientscope import *
-from .flowsgetserverinfo import *
+from .deleteworkflow import *
 from .getaccount import *
 from .getbalance import *
 from .getbalances import *
 from .getbalancesaggregated import *
 from .getconnectortask import *
 from .gethold import *
 from .getholds import *
@@ -65,14 +65,15 @@
 from .listlogs import *
 from .listpayments import *
 from .listscopes import *
 from .listtransactions import *
 from .listusers import *
 from .listwallets import *
 from .listworkflows import *
+from .orchestrationgetserverinfo import *
 from .paymentsgetserverinfo import *
 from .paymentslistaccounts import *
 from .readclient import *
 from .readconnectorconfig import *
 from .readscope import *
 from .readstats import *
 from .readuser import *
@@ -89,8 +90,8 @@
 from .updatemapping import *
 from .updatemetadata import *
 from .updatescope import *
 from .updatewallet import *
 from .voidhold import *
 from .walletsgetserverinfo import *
 
-__all__ = ["ActivateConfigRequest","ActivateConfigResponse","AddMetadataOnTransactionRequest","AddMetadataOnTransactionResponse","AddMetadataToAccountRequest","AddMetadataToAccountResponse","AddScopeToClientRequest","AddScopeToClientResponse","AddTransientScopeRequest","AddTransientScopeResponse","CancelEventRequest","CancelEventResponse","ChangeConfigSecretRequest","ChangeConfigSecretResponse","ConfirmHoldRequest","ConfirmHoldResponse","ConnectorsStripeTransferResponse","ConnectorsTransferRequest","ConnectorsTransferResponse","CountAccountsRequest","CountAccountsResponse","CountTransactionsRequest","CountTransactionsResponse","CreateBalanceRequest","CreateBalanceResponse","CreateClientResponse","CreateScopeResponse","CreateSecretRequest","CreateSecretResponse","CreateTransactionRequest","CreateTransactionResponse","CreateTransactionsRequest","CreateTransactionsResponse","CreateWalletResponse","CreateWorkflowResponse","CreditWalletRequest","CreditWalletResponse","DeactivateConfigRequest","DeactivateConfigResponse","DebitWalletRequest","DebitWalletResponse","DeleteClientRequest","DeleteClientResponse","DeleteConfigRequest","DeleteConfigResponse","DeleteScopeFromClientRequest","DeleteScopeFromClientResponse","DeleteScopeRequest","DeleteScopeResponse","DeleteSecretRequest","DeleteSecretResponse","DeleteTransientScopeRequest","DeleteTransientScopeResponse","FlowsgetServerInfoResponse","GetAccountRequest","GetAccountResponse","GetBalanceRequest","GetBalanceResponse","GetBalancesAggregatedRequest","GetBalancesAggregatedResponse","GetBalancesRequest","GetBalancesResponse","GetConnectorTaskRequest","GetConnectorTaskResponse","GetHoldRequest","GetHoldResponse","GetHoldsRequest","GetHoldsResponse","GetInfoResponse","GetInstanceHistoryRequest","GetInstanceHistoryResponse","GetInstanceRequest","GetInstanceResponse","GetInstanceStageHistoryRequest","GetInstanceStageHistoryResponse","GetLedgerInfoRequest","GetLedgerInfoResponse","GetManyConfigsRequest","GetManyConfigsResponse","GetMappingRequest","GetMappingResponse","GetPaymentRequest","GetPaymentResponse","GetServerInfoResponse","GetTransactionRequest","GetTransactionResponse","GetTransactionsRequest","GetTransactionsResponse","GetVersionsResponse","GetWalletRequest","GetWalletResponse","GetWalletSummaryRequest","GetWalletSummaryResponse","GetWorkflowRequest","GetWorkflowResponse","InsertConfigResponse","InstallConnectorRequest","InstallConnectorResponse","ListAccountsBalanceOperator","ListAccountsRequest","ListAccountsResponse","ListAllConnectorsResponse","ListBalancesRequest","ListBalancesResponse","ListClientsResponse","ListConfigsAvailableConnectorsResponse","ListConnectorTasksRequest","ListConnectorTasksResponse","ListConnectorsTransfersRequest","ListConnectorsTransfersResponse","ListInstancesRequest","ListInstancesResponse","ListLogsRequest","ListLogsResponse","ListPaymentsRequest","ListPaymentsResponse","ListScopesResponse","ListTransactionsRequest","ListTransactionsResponse","ListUsersResponse","ListWalletsRequest","ListWalletsResponse","ListWorkflowsResponse","PaymentsgetServerInfoResponse","PaymentslistAccountsRequest","PaymentslistAccountsResponse","ReadClientRequest","ReadClientResponse","ReadConnectorConfigRequest","ReadConnectorConfigResponse","ReadScopeRequest","ReadScopeResponse","ReadStatsRequest","ReadStatsResponse","ReadUserRequest","ReadUserResponse","ResetConnectorRequest","ResetConnectorResponse","RevertTransactionRequest","RevertTransactionResponse","RunScriptRequest","RunScriptResponse","RunWorkflowRequest","RunWorkflowResponse","SearchResponse","SearchgetServerInfoResponse","SendEventRequest","SendEventRequestBody","SendEventResponse","TestConfigRequest","TestConfigResponse","UninstallConnectorRequest","UninstallConnectorResponse","UpdateClientRequest","UpdateClientResponse","UpdateMappingRequest","UpdateMappingResponse","UpdateMetadataRequest","UpdateMetadataResponse","UpdateScopeRequest","UpdateScopeResponse","UpdateWalletRequest","UpdateWalletRequestBody","UpdateWalletResponse","VoidHoldRequest","VoidHoldResponse","WalletsgetServerInfoResponse"]
+__all__ = ["ActivateConfigRequest","ActivateConfigResponse","AddMetadataOnTransactionRequest","AddMetadataOnTransactionResponse","AddMetadataToAccountRequest","AddMetadataToAccountResponse","AddScopeToClientRequest","AddScopeToClientResponse","AddTransientScopeRequest","AddTransientScopeResponse","CancelEventRequest","CancelEventResponse","ChangeConfigSecretRequest","ChangeConfigSecretResponse","ConfirmHoldRequest","ConfirmHoldResponse","ConnectorsStripeTransferResponse","ConnectorsTransferRequest","ConnectorsTransferResponse","CountAccountsRequest","CountAccountsResponse","CountTransactionsRequest","CountTransactionsResponse","CreateBalanceRequest","CreateBalanceResponse","CreateClientResponse","CreateScopeResponse","CreateSecretRequest","CreateSecretResponse","CreateTransactionRequest","CreateTransactionResponse","CreateTransactionsRequest","CreateTransactionsResponse","CreateWalletResponse","CreateWorkflowResponse","CreditWalletRequest","CreditWalletResponse","DeactivateConfigRequest","DeactivateConfigResponse","DebitWalletRequest","DebitWalletResponse","DeleteClientRequest","DeleteClientResponse","DeleteConfigRequest","DeleteConfigResponse","DeleteScopeFromClientRequest","DeleteScopeFromClientResponse","DeleteScopeRequest","DeleteScopeResponse","DeleteSecretRequest","DeleteSecretResponse","DeleteTransientScopeRequest","DeleteTransientScopeResponse","DeleteWorkflowRequest","DeleteWorkflowResponse","GetAccountRequest","GetAccountResponse","GetBalanceRequest","GetBalanceResponse","GetBalancesAggregatedRequest","GetBalancesAggregatedResponse","GetBalancesRequest","GetBalancesResponse","GetConnectorTaskRequest","GetConnectorTaskResponse","GetHoldRequest","GetHoldResponse","GetHoldsRequest","GetHoldsResponse","GetInfoResponse","GetInstanceHistoryRequest","GetInstanceHistoryResponse","GetInstanceRequest","GetInstanceResponse","GetInstanceStageHistoryRequest","GetInstanceStageHistoryResponse","GetLedgerInfoRequest","GetLedgerInfoResponse","GetManyConfigsRequest","GetManyConfigsResponse","GetMappingRequest","GetMappingResponse","GetPaymentRequest","GetPaymentResponse","GetServerInfoResponse","GetTransactionRequest","GetTransactionResponse","GetTransactionsRequest","GetTransactionsResponse","GetVersionsResponse","GetWalletRequest","GetWalletResponse","GetWalletSummaryRequest","GetWalletSummaryResponse","GetWorkflowRequest","GetWorkflowResponse","InsertConfigResponse","InstallConnectorRequest","InstallConnectorResponse","ListAccountsBalanceOperator","ListAccountsRequest","ListAccountsResponse","ListAllConnectorsResponse","ListBalancesRequest","ListBalancesResponse","ListClientsResponse","ListConfigsAvailableConnectorsResponse","ListConnectorTasksRequest","ListConnectorTasksResponse","ListConnectorsTransfersRequest","ListConnectorsTransfersResponse","ListInstancesRequest","ListInstancesResponse","ListLogsRequest","ListLogsResponse","ListPaymentsRequest","ListPaymentsResponse","ListScopesResponse","ListTransactionsRequest","ListTransactionsResponse","ListUsersResponse","ListWalletsRequest","ListWalletsResponse","ListWorkflowsResponse","OrchestrationgetServerInfoResponse","PaymentsgetServerInfoResponse","PaymentslistAccountsRequest","PaymentslistAccountsResponse","ReadClientRequest","ReadClientResponse","ReadConnectorConfigRequest","ReadConnectorConfigResponse","ReadScopeRequest","ReadScopeResponse","ReadStatsRequest","ReadStatsResponse","ReadUserRequest","ReadUserResponse","ResetConnectorRequest","ResetConnectorResponse","RevertTransactionRequest","RevertTransactionResponse","RunScriptRequest","RunScriptResponse","RunWorkflowRequest","RunWorkflowResponse","SearchResponse","SearchgetServerInfoResponse","SendEventRequest","SendEventRequestBody","SendEventResponse","TestConfigRequest","TestConfigResponse","UninstallConnectorRequest","UninstallConnectorResponse","UpdateClientRequest","UpdateClientResponse","UpdateMappingRequest","UpdateMappingResponse","UpdateMetadataRequest","UpdateMetadataResponse","UpdateScopeRequest","UpdateScopeResponse","UpdateWalletRequest","UpdateWalletRequestBody","UpdateWalletResponse","VoidHoldRequest","VoidHoldResponse","WalletsgetServerInfoResponse"]
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/activateconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/activateconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/addmetadataontransaction.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addmetadataontransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/addmetadatatoaccount.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addmetadatatoaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/addscopetoclient.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addscopetoclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/addtransientscope.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/addtransientscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/cancelevent.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/cancelevent.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/changeconfigsecret.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/changeconfigsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/confirmhold.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/confirmhold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/connectorsstripetransfer.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/connectorsstripetransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/connectorstransfer.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/connectorstransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/countaccounts.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/countaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/counttransactions.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/counttransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createbalance.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createbalance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createclient.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createscope.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createsecret.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createtransaction.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createtransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createtransactions.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createtransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createwallet.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createworkflow.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/createworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/creditwallet.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/creditwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deactivateconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deactivateconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/debitwallet.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/debitwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deleteclient.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deleteconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deleteconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletescope.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletescope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletescopefromclient.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletescopefromclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletesecret.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletesecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletetransientscope.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/deletetransientscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/flowsgetserverinfo.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/orchestrationgetserverinfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import requests as requests_http
 from ..shared import error as shared_error
 from ..shared import serverinfo as shared_serverinfo
 from typing import Optional
 
 
 @dataclasses.dataclass
-class FlowsgetServerInfoResponse:
+class OrchestrationgetServerInfoResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     server_info: Optional[shared_serverinfo.ServerInfo] = dataclasses.field(default=None)
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getaccount.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalance.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalances.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalancesaggregated.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getbalancesaggregated.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getconnectortask.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getconnectortask.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/gethold.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gethold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getholds.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getholds.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinfo.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstance.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstancehistory.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstancehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstancestagehistory.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getinstancestagehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getledgerinfo.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getledgerinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getmanyconfigs.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getmanyconfigs.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getmapping.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getmapping.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getpayment.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getpayment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getserverinfo.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/gettransaction.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/gettransactions.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/gettransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getversions.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getversions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getwallet.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getwalletsummary.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getwalletsummary.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getworkflow.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/getworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/insertconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/insertconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/installconnector.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/installconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listaccounts.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listallconnectors.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listallconnectors.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listbalances.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listclients.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listclients.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconfigsavailableconnectors.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconfigsavailableconnectors.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconnectorstransfers.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconnectorstransfers.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconnectortasks.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listconnectortasks.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listinstances.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listinstances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listlogs.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listlogs.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listpayments.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listpayments.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listscopes.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listscopes.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listtransactions.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listusers.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listusers.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listwallets.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listwallets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listworkflows.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/listworkflows.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/paymentsgetserverinfo.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/paymentsgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/paymentslistaccounts.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/paymentslistaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/readclient.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/readconnectorconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readconnectorconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/readscope.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readscope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/readstats.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readstats.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/readuser.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/readuser.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/resetconnector.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/resetconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/reverttransaction.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/reverttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/runscript.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/runscript.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/runworkflow.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/runworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/search.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/search.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/searchgetserverinfo.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/searchgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/sendevent.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/sendevent.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/testconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/testconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/uninstallconnector.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/uninstallconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/updateclient.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updateclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatemapping.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatemapping.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatemetadata.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatemetadata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatescope.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatescope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatewallet.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/updatewallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/voidhold.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/voidhold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/operations/walletsgetserverinfo.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/operations/walletsgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/__init__.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,21 @@
 from .listrunsresponse import *
 from .listscopesresponse import *
 from .listusersresponse import *
 from .listwalletsresponse import *
 from .listworkflowsresponse import *
 from .log import *
 from .logscursorresponse import *
+from .mangopayconfig import *
 from .mapping import *
 from .mappingresponse import *
 from .migrationinfo import *
 from .modulrconfig import *
 from .monetary import *
+from .moneycorpconfig import *
 from .payment import *
 from .paymentadjustment import *
 from .paymentmetadata import *
 from .paymentresponse import *
 from .paymentsaccount import *
 from .paymentscursor import *
 from .paymentstatus import *
@@ -131,15 +133,17 @@
 from .stats import *
 from .statsresponse import *
 from .stripeconfig import *
 from .stripetransferrequest import *
 from .taskbankingcircle import *
 from .taskcurrencycloud import *
 from .taskdummypay import *
+from .taskmangopay import *
 from .taskmodulr import *
+from .taskmoneycorp import *
 from .taskresponse import *
 from .taskscursor import *
 from .taskstripe import *
 from .taskwise import *
 from .transaction import *
 from .transactiondata import *
 from .transactionresponse import *
@@ -154,14 +158,15 @@
 from .updatescoperequest import *
 from .updatescoperesponse import *
 from .user import *
 from .version import *
 from .volume import *
 from .wallet import *
 from .walletserrorresponse import *
+from .walletsposting import *
 from .walletstransaction import *
 from .walletsubject import *
 from .walletsvolume import *
 from .walletwithbalances import *
 from .webhooksconfig import *
 from .webhookserrorresponse import *
 from .webhookserrorsenum import *
@@ -170,8 +175,8 @@
 from .workflowconfig import *
 from .workflowinstance import *
 from .workflowinstancehistory import *
 from .workflowinstancehistorystage import *
 from .workflowinstancehistorystageinput import *
 from .workflowinstancehistorystageoutput import *
 
-__all__ = ["Account","AccountResponse","AccountWithVolumesAndBalances","AccountsCursor","AccountsCursorCursor","AccountsCursorResponse","AccountsCursorResponseCursor","ActivityConfirmHold","ActivityCreateTransaction","ActivityCreateTransactionOutput","ActivityCreditWallet","ActivityDebitWallet","ActivityDebitWalletOutput","ActivityGetAccount","ActivityGetAccountOutput","ActivityGetPayment","ActivityGetPaymentOutput","ActivityGetWallet","ActivityGetWalletOutput","ActivityRevertTransaction","ActivityRevertTransactionOutput","ActivityStripeTransfer","ActivityVoidHold","AggregateBalancesResponse","AssetHolder","Attempt","AttemptResponse","Balance","BalanceWithAssets","BalancesCursorResponse","BalancesCursorResponseCursor","BankingCircleConfig","Client","ClientSecret","Config","ConfigChangeSecret","ConfigInfo","ConfigInfoResponse","ConfigResponse","ConfigUser","ConfigsResponse","ConfigsResponseCursor","ConfirmHoldRequest","Connector","ConnectorConfigResponse","ConnectorsConfigsResponse","ConnectorsConfigsResponseData","ConnectorsConfigsResponseDataConnector","ConnectorsConfigsResponseDataConnectorKey","ConnectorsResponse","ConnectorsResponseData","Contract","CreateBalanceRequest","CreateBalanceResponse","CreateClientRequest","CreateClientResponse","CreateScopeRequest","CreateScopeResponse","CreateSecretRequest","CreateSecretResponse","CreateWalletRequest","CreateWalletResponse","CreateWorkflowRequest","CreateWorkflowResponse","CreditWalletRequest","CurrencyCloudConfig","DebitWalletRequest","DebitWalletResponse","DummyPayConfig","Error","ErrorErrorCode","ErrorResponse","ErrorsEnum","ExpandedDebitHold","GetBalanceResponse","GetHoldResponse","GetHoldsResponse","GetHoldsResponseCursor","GetTransactionsResponse","GetTransactionsResponseCursor","GetVersionsResponse","GetWalletResponse","GetWalletSummaryResponse","GetWorkflowInstanceHistoryResponse","GetWorkflowInstanceHistoryStageResponse","GetWorkflowInstanceResponse","GetWorkflowResponse","Hold","LedgerAccountSubject","LedgerInfo","LedgerInfoResponse","LedgerInfoStorage","LedgerStorage","ListBalancesResponse","ListBalancesResponseCursor","ListClientsResponse","ListRunsResponse","ListScopesResponse","ListUsersResponse","ListWalletsResponse","ListWalletsResponseCursor","ListWorkflowsResponse","Log","LogType","LogsCursorResponse","LogsCursorResponseCursor","Mapping","MappingResponse","MigrationInfo","MigrationInfoState","ModulrConfig","Monetary","Payment","PaymentAdjustment","PaymentMetadata","PaymentResponse","PaymentScheme","PaymentStatus","PaymentType","PaymentsAccount","PaymentsAccountType","PaymentsCursor","PaymentsCursorCursor","PostTransaction","PostTransactionScript","Posting","Query","ReadClientResponse","ReadScopeResponse","ReadUserResponse","Response","ResponseCursor","ResponseCursorTotal","RunWorkflowResponse","Scope","Script","ScriptResponse","Secret","Security","ServerInfo","StageDelay","StageSend","StageSendDestination","StageSendDestinationAccount","StageSendDestinationPayment","StageSendDestinationWallet","StageSendSource","StageSendSourceAccount","StageSendSourcePayment","StageSendSourceWallet","StageStatus","StageWaitEvent","Stats","StatsResponse","StripeConfig","StripeTransferRequest","TaskBankingCircle","TaskBankingCircleDescriptor","TaskCurrencyCloud","TaskCurrencyCloudDescriptor","TaskDummyPay","TaskDummyPayDescriptor","TaskModulr","TaskModulrDescriptor","TaskResponse","TaskStripe","TaskStripeDescriptor","TaskWise","TaskWiseDescriptor","TasksCursor","TasksCursorCursor","Transaction","TransactionData","TransactionResponse","Transactions","TransactionsCursorResponse","TransactionsCursorResponseCursor","TransactionsResponse","TransferRequest","TransferResponse","TransfersResponse","TransfersResponseData","UpdateClientRequest","UpdateClientResponse","UpdateScopeRequest","UpdateScopeResponse","User","Version","Volume","Wallet","WalletSubject","WalletWithBalances","WalletWithBalancesBalances","WalletsErrorResponse","WalletsErrorResponseErrorCode","WalletsTransaction","WalletsVolume","WebhooksConfig","WebhooksErrorResponse","WebhooksErrorsEnum","WiseConfig","Workflow","WorkflowConfig","WorkflowInstance","WorkflowInstanceHistory","WorkflowInstanceHistoryStage","WorkflowInstanceHistoryStageInput","WorkflowInstanceHistoryStageOutput"]
+__all__ = ["Account","AccountResponse","AccountWithVolumesAndBalances","AccountsCursor","AccountsCursorCursor","AccountsCursorResponse","AccountsCursorResponseCursor","ActivityConfirmHold","ActivityCreateTransaction","ActivityCreateTransactionOutput","ActivityCreditWallet","ActivityDebitWallet","ActivityDebitWalletOutput","ActivityGetAccount","ActivityGetAccountOutput","ActivityGetPayment","ActivityGetPaymentOutput","ActivityGetWallet","ActivityGetWalletOutput","ActivityRevertTransaction","ActivityRevertTransactionOutput","ActivityStripeTransfer","ActivityVoidHold","AggregateBalancesResponse","AssetHolder","Attempt","AttemptResponse","Balance","BalanceWithAssets","BalancesCursorResponse","BalancesCursorResponseCursor","BankingCircleConfig","Client","ClientSecret","Config","ConfigChangeSecret","ConfigInfo","ConfigInfoResponse","ConfigResponse","ConfigUser","ConfigsResponse","ConfigsResponseCursor","ConfirmHoldRequest","Connector","ConnectorConfigResponse","ConnectorsConfigsResponse","ConnectorsConfigsResponseData","ConnectorsConfigsResponseDataConnector","ConnectorsConfigsResponseDataConnectorKey","ConnectorsResponse","ConnectorsResponseData","Contract","CreateBalanceRequest","CreateBalanceResponse","CreateClientRequest","CreateClientResponse","CreateScopeRequest","CreateScopeResponse","CreateSecretRequest","CreateSecretResponse","CreateWalletRequest","CreateWalletResponse","CreateWorkflowRequest","CreateWorkflowResponse","CreditWalletRequest","CurrencyCloudConfig","DebitWalletRequest","DebitWalletResponse","DummyPayConfig","Error","ErrorErrorCode","ErrorResponse","ErrorsEnum","ExpandedDebitHold","GetBalanceResponse","GetHoldResponse","GetHoldsResponse","GetHoldsResponseCursor","GetTransactionsResponse","GetTransactionsResponseCursor","GetVersionsResponse","GetWalletResponse","GetWalletSummaryResponse","GetWorkflowInstanceHistoryResponse","GetWorkflowInstanceHistoryStageResponse","GetWorkflowInstanceResponse","GetWorkflowResponse","Hold","LedgerAccountSubject","LedgerInfo","LedgerInfoResponse","LedgerInfoStorage","LedgerStorage","ListBalancesResponse","ListBalancesResponseCursor","ListClientsResponse","ListRunsResponse","ListScopesResponse","ListUsersResponse","ListWalletsResponse","ListWalletsResponseCursor","ListWorkflowsResponse","Log","LogType","LogsCursorResponse","LogsCursorResponseCursor","MangoPayConfig","Mapping","MappingResponse","MigrationInfo","MigrationInfoState","ModulrConfig","Monetary","MoneycorpConfig","Payment","PaymentAdjustment","PaymentMetadata","PaymentResponse","PaymentScheme","PaymentStatus","PaymentType","PaymentsAccount","PaymentsAccountType","PaymentsCursor","PaymentsCursorCursor","PostTransaction","PostTransactionScript","Posting","Query","ReadClientResponse","ReadScopeResponse","ReadUserResponse","Response","ResponseCursor","ResponseCursorTotal","RunWorkflowResponse","Scope","Script","ScriptResponse","Secret","Security","ServerInfo","StageDelay","StageSend","StageSendDestination","StageSendDestinationAccount","StageSendDestinationPayment","StageSendDestinationWallet","StageSendSource","StageSendSourceAccount","StageSendSourcePayment","StageSendSourceWallet","StageStatus","StageWaitEvent","Stats","StatsResponse","StripeConfig","StripeTransferRequest","TaskBankingCircle","TaskBankingCircleDescriptor","TaskCurrencyCloud","TaskCurrencyCloudDescriptor","TaskDummyPay","TaskDummyPayDescriptor","TaskMangoPay","TaskMangoPayDescriptor","TaskModulr","TaskModulrDescriptor","TaskMoneycorp","TaskMoneycorpDescriptor","TaskResponse","TaskStripe","TaskStripeDescriptor","TaskWise","TaskWiseDescriptor","TasksCursor","TasksCursorCursor","Transaction","TransactionData","TransactionResponse","Transactions","TransactionsCursorResponse","TransactionsCursorResponseCursor","TransactionsResponse","TransferRequest","TransferResponse","TransfersResponse","TransfersResponseData","UpdateClientRequest","UpdateClientResponse","UpdateScopeRequest","UpdateScopeResponse","User","Version","Volume","Wallet","WalletSubject","WalletWithBalances","WalletWithBalancesBalances","WalletsErrorResponse","WalletsErrorResponseErrorCode","WalletsPosting","WalletsTransaction","WalletsVolume","WebhooksConfig","WebhooksErrorResponse","WebhooksErrorsEnum","WiseConfig","Workflow","WorkflowConfig","WorkflowInstance","WorkflowInstanceHistory","WorkflowInstanceHistoryStage","WorkflowInstanceHistoryStageInput","WorkflowInstanceHistoryStageOutput"]
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/account.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/account.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountscursor.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountscursorresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountwithvolumesandbalances.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/accountwithvolumesandbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreatetransaction.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreatetransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreatetransactionoutput.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreatetransactionoutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ActivityCreateTransactionOutput:
     
-    data: list[shared_transaction.Transaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    data: shared_transaction.Transaction = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreditwallet.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitycreditwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitydebitwallet.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitydebitwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetaccount.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetaccountoutput.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetaccountoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetwalletoutput.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitygetwalletoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityreverttransaction.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityreverttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityreverttransactionoutput.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activityreverttransactionoutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ActivityRevertTransactionOutput:
     
-    data: list[shared_transaction.Transaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    data: shared_transaction.Transaction = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitystripetransfer.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/activitystripetransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/attempt.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/attempt.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/balance.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/balancescursorresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balancescursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/balancewithassets.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/balancewithassets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/bankingcircleconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/clientsecret.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class BankingCircleConfig:
+class ClientSecret:
     
-    authorization_endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('authorizationEndpoint') }})
-    endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint') }})
-    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    last_digits: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastDigits') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/client.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/client.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/clientsecret.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/secret.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ClientSecret:
+class Secret:
     
+    clear: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clear') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     last_digits: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastDigits') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/configinfo.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/configinforesponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configinforesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/configresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/configsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/configuser.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/configuser.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/confirmholdrequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/confirmholdrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/connectorsconfigsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connectorsconfigsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/connectorsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/connectorsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/contract.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/contract.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createbalancerequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createbalancerequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createbalanceresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createbalanceresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createclientrequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createclientrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createclientresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createscoperequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createscoperequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createscoperesponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createscoperesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createsecretrequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createsecretrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createsecretresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createsecretresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createwalletrequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createwalletrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createwalletresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createwalletresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createworkflowrequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createworkflowrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createworkflowresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/createworkflowresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/creditwalletrequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/creditwalletrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/currencycloudconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/currencycloudconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/debitwalletrequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/debitwalletrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/debitwalletresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/debitwalletresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/dummypayconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/dummypayconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/error.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/error.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/errorresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/errorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/expandeddebithold.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/expandeddebithold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getbalanceresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getbalanceresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getholdresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getholdresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getholdsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getholdsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/gettransactionsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/gettransactionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getversionsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getversionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getwalletresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getwalletresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getwalletsummaryresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getwalletsummaryresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstancehistoryresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstancehistoryresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstanceresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowinstanceresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/getworkflowresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/hold.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/hold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgeraccountsubject.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgeraccountsubject.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerinfo.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerinforesponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerinforesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerstorage.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/ledgerstorage.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listbalancesresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listbalancesresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listclientsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listclientsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listrunsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listrunsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listscopesresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listscopesresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listusersresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listusersresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listwalletsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listwalletsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listworkflowsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/listworkflowsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/log.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/log.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/logscursorresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/logscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/mappingresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/mappingresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/migrationinfo.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/migrationinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/modulrconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsubject.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ModulrConfig:
+class WalletSubject:
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiKey') }})
-    api_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiSecret') }})
-    endpoint: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint'), 'exclude': lambda f: f is None }})
+    identifier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier') }})
+    type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/monetary.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/monetary.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/payment.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/payment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentadjustment.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentadjustment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentsaccount.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentsaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentscursor.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/paymentscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/posting.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/posting.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/posttransaction.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/posttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/query.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/query.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/readclientresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/readscoperesponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readscoperesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/readuserresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/readuserresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/response.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/response.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/runworkflowresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/runworkflowresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/scope.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/scope.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/script.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/script.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/scriptresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/scriptresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/secret.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsposting.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Secret:
+class WalletsPosting:
     
-    clear: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clear') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    last_digits: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastDigits') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
+    asset: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset') }})
+    destination: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination') }})
+    source: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source') }})
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagedelay.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagedelay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesend.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesend.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestination.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestination.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestinationaccount.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestinationaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestinationwallet.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesenddestinationwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsource.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsource.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsourceaccount.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsourceaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsourcewallet.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagesendsourcewallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagestatus.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stagestatus.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stats.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stats.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stripeconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stripeconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stripetransferrequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/stripetransferrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskbankingcircle.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskbankingcircle.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskcurrencycloud.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskcurrencycloud.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskdummypay.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskdummypay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskmodulr.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskmodulr.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskscursor.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskstripe.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskstripe.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskwise.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/taskwise.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transaction.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactiondata.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactiondata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactions.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionscursorresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionsresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transactionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transferrequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transferrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transferresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transferresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transfersresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/transfersresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/updateclientrequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updateclientrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/updateclientresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updateclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/updatescoperequest.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updatescoperequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/updatescoperesponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/updatescoperesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/user.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/version.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/version.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/volume.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/volume.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/wallet.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/wallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletserrorresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletserrorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletstransaction.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletstransaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from ..shared import posting as shared_posting
+from ..shared import walletsposting as shared_walletsposting
 from ..shared import walletsvolume as shared_walletsvolume
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class WalletsTransaction:
     
     metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     r"""Metadata associated with the wallet."""
-    postings: list[shared_posting.Posting] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postings') }})
+    postings: list[shared_walletsposting.WalletsPosting] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postings') }})
     timestamp: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     txid: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('txid') }})
     ledger: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger'), 'exclude': lambda f: f is None }})
     post_commit_volumes: Optional[dict[str, dict[str, shared_walletsvolume.WalletsVolume]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postCommitVolumes'), 'exclude': lambda f: f is None }})
     pre_commit_volumes: Optional[dict[str, dict[str, shared_walletsvolume.WalletsVolume]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('preCommitVolumes'), 'exclude': lambda f: f is None }})
     reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletsubject.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/moneycorpconfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,13 +5,15 @@
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class WalletSubject:
+class MoneycorpConfig:
     
-    identifier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier') }})
-    type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
+    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiKey') }})
+    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clientID') }})
+    endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint') }})
+    polling_period: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pollingPeriod'), 'exclude': lambda f: f is None }})
+    r"""The frequency at which the connector will try to fetch new BalanceTransaction objects from Stripe API."""
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletsvolume.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletsvolume.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletwithbalances.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/walletwithbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/webhooksconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/webhooksconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/webhookserrorresponse.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/webhookserrorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflow.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowconfig.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstance.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistory.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystage.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystage.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystageinput.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystageinput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystageoutput.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/models/shared/workflowinstancehistorystageoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/payments.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/payments.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/sdk.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     wallets: Wallets
     webhooks: Webhooks
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "v1.0.20230718"
+    _sdk_version: str = "v1.0.20230718.1"
     _gen_version: str = "2.31.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
```

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/search.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/search.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/utils/retries.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/utils/utils.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/wallets.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/wallets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230718/src/sdk/webhooks.py` & `formance-sdk-python-1.0.20230718.1/src/sdk/webhooks.py`

 * *Files identical despite different names*

