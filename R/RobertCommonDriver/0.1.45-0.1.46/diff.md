# Comparing `tmp/RobertCommonDriver-0.1.45.tar.gz` & `tmp/RobertCommonDriver-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.45.tar", last modified: Fri Jul 14 14:45:45 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.46.tar", last modified: Mon Jul 24 01:53:55 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.45.tar` & `RobertCommonDriver-0.1.46.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.797523 RobertCommonDriver-0.1.45/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.45/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.45/MANIFEST.in
--rw-rw-rw-   0        0        0      850 2023-07-14 14:45:45.797523 RobertCommonDriver-0.1.45/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.45/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.709403 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0      850 2023-07-14 14:45:45.000000 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-07-14 14:45:45.000000 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 14:45:45.000000 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      198 2023-07-14 14:45:45.000000 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-14 14:45:45.000000 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      212 2023-06-30 06:01:07.000000 RobertCommonDriver-0.1.45/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.710404 RobertCommonDriver-0.1.45/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.45/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.711404 RobertCommonDriver-0.1.45/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.729010 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38348 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.754472 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    68933 2023-06-26 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566106 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0    46883 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    78954 2023-07-14 14:41:30.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    32738 2023-06-09 09:05:11.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    44863 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-07-14 14:45:45.797523 RobertCommonDriver-0.1.45/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-07-14 14:42:19.000000 RobertCommonDriver-0.1.45/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.755471 RobertCommonDriver-0.1.45/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.45/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.756472 RobertCommonDriver-0.1.45/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.45/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.771788 RobertCommonDriver-0.1.45/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.795523 RobertCommonDriver-0.1.45/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     5502 2023-07-14 12:58:58.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     9628 2023-05-25 08:18:30.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:55.014632 RobertCommonDriver-0.1.46/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.46/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.46/MANIFEST.in
+-rw-rw-rw-   0        0        0      850 2023-07-24 01:53:55.013347 RobertCommonDriver-0.1.46/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.46/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.907416 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-07-24 01:53:54.000000 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-07-24 01:53:54.000000 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 01:53:54.000000 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      198 2023-07-24 01:53:54.000000 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-24 01:53:54.000000 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      212 2023-06-30 06:01:07.000000 RobertCommonDriver-0.1.46/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.908423 RobertCommonDriver-0.1.46/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.46/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.909425 RobertCommonDriver-0.1.46/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.932626 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38348 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.959496 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    69091 2023-07-19 08:00:33.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566106 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0    95594 2023-07-21 10:00:24.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    78954 2023-07-14 14:41:30.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    32745 2023-07-21 02:43:14.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    44863 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-07-24 01:53:55.014632 RobertCommonDriver-0.1.46/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-07-24 01:52:25.000000 RobertCommonDriver-0.1.46/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.960493 RobertCommonDriver-0.1.46/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.46/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.961496 RobertCommonDriver-0.1.46/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.46/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.980735 RobertCommonDriver-0.1.46/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:55.012125 RobertCommonDriver-0.1.46/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     2245 2023-07-20 08:04:16.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     5502 2023-07-14 12:58:58.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     9630 2023-07-20 10:41:51.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.45/LICENSE` & `RobertCommonDriver-0.1.46/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/PKG-INFO` & `RobertCommonDriver-0.1.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.45
+Version: 0.1.46
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.45
+Version: 0.1.46
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,14 +569,17 @@
             self.valid = False
             self.close()
 
         def connect(self):
             self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock.settimeout(self.timeout)  # 设置连接超时
             self.sock.connect((self.host, self.port))
+            l_onoff = 1
+            l_linger = 0
+            self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_LINGER, pack('ii', l_onoff, l_linger))    #
             self.sock.settimeout(None)
 
         def close(self):
             if self.sock:
                 self.sock.close()
 
         def send(self, datas: bytes):
```

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1208 +1,863 @@
-from scapy.fields import ByteEnumField, BitEnumField, BitField, ConditionalField, Field, PacketField, LEShortField, ShortField, XByteField, ByteField, PacketListField
-from scapy.packet import Packet, Padding, NoPayload
-from struct import unpack, pack
-from typing import List, Dict, Any
-from threading import Event
+from typing import List, Dict, Any, Union, Optional
 
 from .base import IOTBaseCommon, IOTDriver
 
-
 '''
-pip install scapy==2.4.5
+https://blog.csdn.net/lishiming0308/article/details/85243041
+
+Rockwell Allen-Bradley(AB)PLC
+罗克韦尔CIP
+AB PLC的数据通信类，使用CIP协议实现，适用1756，1769等型号，支持使用标签的形式进行读写操作，支持标量数据，一维数组，二维数组，三维数组等等。如果是局部变量，那么使用 Program:MainProgram.[变量名]
+
+ABPLC的通讯采用小端模式。一般情况实现注册、请求、读写数据即可。不实现关闭请求、卸载注册在实际测试过程中也不会出现问题。在断开连接时不提交关闭请求和卸载注册指令。再重新连接plc执行注册、打开请求、读写数据还是一样可以成功的。
+连接：
+    客户端发送注册会话请求， PLC收到请求后，生成会话句柄并返回客户端
+    客户端收到句柄后生成连接标识，通过开放数据连接(ForwardOpen)请求发送给PLC， OLC收到后发送O2T给客户端
+    读取数据请求
+    应答
 '''
 
-"""
-ACPI
-    68(1)
-    长度(1)
-    控制域(4)
-        I帧
-            发送序号， 接收序号
-        S帧
-            01 00 接收序号
-        U帧
-            0x 00 00 00
-ASDU
-    类型(1)
-        监视方向
-            1 单点遥信（带品质 不带时标）
-            2 双点遥信
-            13 段浮点遥测（带品质 不带时标）
-        控制方向
-            45 单点遥控
-        监视方向系统类型
-            70 初始化结束
-        控制方向系统类型
-            100 总召
-            101 累积量召唤
-            102 读命令
-            103 时钟同步
-    限定词(1)
-        SQ = 0 地址连续 SQ=1地址不连续
-    传送原因(2)
-        PN
-            6 激活
-            7 激活确认
-            8 停止激活
-    地址(2)
-    (信息体)(长度-10)
-        连续信息传输型
-            带绝对时标（遥测）
-                地址编号(3字节) 信息体数据 品质描述词(1字节) 重复 信息体数据 品质描述词(1字节) 绝对时标(7字节)
-            不带绝对时标（遥测）
-                地址编号(3字节) 信息体数据 品质描述词(1字节) 重复 信息体数据 品质描述词(1字节)
-            带绝对时标（遥信）
-                地址编号(3字节) 信息体数据(1字节) 重复 信息体数据(1字节) 绝对时标(7字节)
-            不带绝对时标（遥信）
-                地址编号(3字节) 信息体数据(1字节) 重复 信息体数据(1字节)
-        非连续信息传输型
-            带绝对时标（遥测）
-                地址编号(3字节) 信息体数据 品质描述词(1字节) 重复 地址编号(3字节) 信息体数据 品质描述词(1字节) 绝对时标(7字节)
-            不带绝对时标（遥测）
-                地址编号(3字节) 信息体数据 品质描述词(1字节) 重复 地址编号(3字节) 信息体数据 品质描述词(1字节)
-            带绝对时标（遥信）
-                地址编号(3字节) 信息体数据(1字节) 重复 地址编号(3字节) 信息体数据(1字节) 绝对时标(7字节)
-            不带绝对时标（遥信）
-                地址编号(3字节) 信息体数据(1字节) 重复 地址编号(3字节) 信息体数据(1字节)
-                
-        遥控和设定值
-            单点遥控(1字节)   (S/E QU[6:2] RES SCS)
-                S/E = 0 遥控执行命令；S/E=1 遥控选择命令；
-                QU = 0 被控占内部确定遥控输出方式，不有控制站选择；
-                    1 短脉冲方式输出
-                    2 长脉冲方式输出
-                    3 持续脉冲方式输出
-                其他值没有定义
-                RES ：保留位
-                SCS ： 设置值； 0 = 控开 ；1 = 控合 
-            双电遥控(1字节)   (S/E QU[6:2] DCS)
-                S/E = 0 遥控执行命令；S/E=1 遥控选择命令；
-                QU = 0 被控占内部确定遥控输出方式，不有控制站选择；
-                    1 短脉冲方式输出
-                    2 长脉冲方式输出
-                    3 持续脉冲方式输出
-                DCS； 0 无效控制
-                    1 控分
-                    2 控合
-                    3 无效控制
-            设定值QOS
-"""
-
-
-class IECDefine:
-
-    # 类型标识(1字节)
-    ASDU_TYPE = {
-        0x01: 'M_SP_NA_1',  # 单点遥信(带品质描述 不带时标)
-        0x03: 'M_DP_NA_1',  # 双点遥信(带品质描述 不带时标)
-        0x05: 'M_ST_NA_1',  # 步位置信息(带品质描述 不带时标)
-        0x07: 'M_BO_NA_1',  # 32比特串(带品质描述 不带时标)
-        0x09: 'M_ME_NA_1',  # 规一化遥测值(带品质描述 不带时标)
-        0x0B: 'M_ME_NB_1',  # 标度化遥测值(带品质描述 不带时标)
-        0x0D: 'M_ME_NC_1',  # 短浮点遥测值(带品质描述 不带时标)
-        0x0F: 'M_IT_NA_1',  # 累积量(带品质描述 不带时标)
-        0x14: 'M_PS_NA_1',  # 成组单点遥信(只带变量标志)
-        0x15: 'M_ME_ND_1',  # 规一化遥测值(不带品质描述 不带时标)
-        0x1E: 'M_SP_TB_1',  # 单点遥信(带品质描述 带绝对时标)
-        0x1F: 'M_DP_TB_1',  # 双点遥信(带品质描述 带绝对时标)
-        0x20: 'M_ST_TB_1',  # 步位置信息(带品质描述 带绝对时标)
-        0x21: 'M_BO_TB_1',  # 32比特串(带品质描述 带绝对时标)
-        0x22: 'M_ME_TD_1',  # 规一化遥测值(带品质描述 带绝对时标)
-        0x23: 'M_ME_TE_1',  # 标度化遥测值(带品质描述 带绝对时标)
-        0x24: 'M_ME_TF_1',  # 短浮点遥测值(带品质描述 带绝对时标)
-        0x25: 'M_IT_TB_1',  # 累积量(带品质描述 带绝对时标)
-        0x26: 'M_EP_TD_1',  # 继电保护装置事件(带品质描述 带绝对时标)
-        0x27: 'M_EP_TE_1',  # 继电保护装置成组启动事件(带品质描述 带绝对时标)
-        0x28: 'M_EP_TF_1',  # 继电保护装置成组出口信息(带品质描述 带绝对时标)
-        0x2D: 'C_SC_NA_1',  # 单点遥控(一个报文只有一个遥控信息体 不带时标)
-        0x2E: 'C_DC_NA_1',  # 双点遥控(一个报文只有一个遥控信息体 不带时标)
-        0x2F: 'C_RC_NA_1',  # 升降遥控(一个报文只有一个遥控信息体 不带时标)
-        0x30: 'C_SE_NA_1',  # 规一化设定值(一个报文只有一个设定值 不带时标)
-        0x31: 'C_SE_NB_1',  # 标度化设定值(一个报文只有一个设定值 不带时标)
-        0x32: 'C_SE_NC_1',  # 短浮点设定值(一个报文只有一个设定值 不带时标)
-        0x33: 'C_SE_ND_1',  # 32比特串(一个报文只有一个设定值 不带时标)
-        0x3A: 'C_SE_TA_1',  # 单点遥控(一个报文只有一个设定值 带时标)
-        0x3B: 'C_SE_TB_1',  # 双点遥控(一个报文只有一个设定值 带时标)
-        0x3C: 'C_SE_TC_1',  # 升降遥控(一个报文只有一个设定值 带时标)
-        0x3D: 'C_SE_TD_1',  # 规一化设定值(一个报文只有一个设定值 带时标)
-        0x3E: 'C_SE_TE_1',  # 标度化设定值(一个报文只有一个设定值 带时标)
-        0x3F: 'C_SE_TF_1',  # 短浮点设定值(一个报文只有一个设定值 带时标)
-        0x40: 'C_SE_TG_1',  # 32比特串(一个报文只有一个设定值 带时标)
-        0x46: 'M_EI_NA_1',  # 初始化结束(从站发送，主站收到时候会做一次总召)
-        0x64: 'C_IC_NA_1',  # 总召
-        0x65: 'C_CI_NA_1',  # 累积量召唤
-        0x66: 'C_RD_NA_1',  # 读命令
-        0x67: 'C_CS_NA_1',  # 时钟同步命令
-        0x69: 'C_RS_NA_1',  # 复位进程命令
-        0x6B: 'C_TS_NA_1',  # 带时标的测试命令
-        0x88: 'C_SE_NE_1',  # 规一化设定值(一个报文可以包含多个设定值 不带时标)
-    }
-
-    # 帧类型
-    APCI_TYPE = {
-        0x00: 'I',
-        0x01: 'S',
-        0x03: 'U'
-    }
-
-    # U帧类型
-    APCI_U_TYPE = {
-        0x01: 'STARTDT act',
-        0x02: 'STARTDT con',
-        0x04: 'STOPDT act',
-        0x08: 'STOPDT con',
-        0x10: 'TESTFR act',
-        0x20: 'TESTFR con',
-    }
-
-    # 可变结构限定词(1字节)
-    ASDU_SQ = {
-        0X00: 0,
-        0x80: 1  # 信息对象的地址连续 总召唤时，为了压缩信息传输时间SQ=
-    }
-
-    # 传送原因(2字节)
-    ASDU_CAUSE = {
-        0: 'not used',
-        1: 'per/cyc',  # 周期 循环
-        2: 'back',  # 背景扫描
-        3: 'spont',  # 突发
-        4: 'init',  # 初始化
-        5: 'req',  # 请求或被请求
-        6: 'act',  # 激活
-        7: 'act config',  # 激活确认
-        8: 'deact',  # 停止激活
-        9: 'deact config',  # 停止激活确认
-        10: 'act term',  # 激活终止
-        11: 'retrem',  # 远方命令引起的返送信息
-        12: 'retloc',  # 当地命令引起的返送信息
-        13: 'file',
-        20: 'inrogen',  # 响应站召唤
-        21: 'inro1',  # 响应第1组召唤
-        22: 'inro2',  # 响应第2组召唤
-        23: 'inro3',
-        24: 'inro4',
-        25: 'inro5',
-        26: 'inro6',
-        27: 'inro7',
-        28: 'inro8',
-        29: 'inro9',
-        30: 'inro10',
-        31: 'inro11',
-        32: 'inro12',
-        33: 'inro13',
-        34: 'inro14',
-        35: 'inro15',
-        36: 'inro16',
-        37: 'reqcogen',  # 响应累积量站召唤
-        38: 'reqco1',
-        39: 'reqco2',
-        40: 'reqco3',
-        41: 'reqco4',
-        44: 'unknown type identification',  # 未知的类型标识
-        45: 'unknown cause of transmission',  # 未知的传送原因
-        46: 'unknown common address of ASDU',  # 未知的应用服务数据单元公共地址
-        47: 'unknown information object address'  # 未知的信息对象地址
-    }
-
-    # 传送原因 P/N
-    ASDU_PN = {
-        0x00: 'Positive confirm',
-        0x40: 'Negative confirm'
-    }
-
-    ASDU_OV = {
-        0X00: 'no overflow',
-        0x01: 'overflow'
-    }
-
-    ASDU_BL = {
-        0X00: 'not blocked',
-        0x10: 'blocked'
-    }
-
-    ASDU_SB = {
-        0X00: 'not substituted',
-        0x20: 'substituted'
-    }
-
-    ASDU_NT = {
-        0X00: 'topical',
-        0x40: 'not topical'
-    }
-
-    ASDU_IV = {
-        0X00: 'valid',
-        0x80: 'invalid'
-    }
-
-    # 遥测品质描述词
-    ASDU_QDS_FLAGS = ['OV', '*', '*', '*', 'BL', 'SB', 'NT', 'IV']
-
-    # 双点信息品质描述词
-    ASDU_DIQ_FLAGS = ['*', '*', '*', '*', 'BL', 'SB', 'NT', 'IV']
-
-    # 单点信息品质描述词
-    ASDU_SIQ_FLAGS = ['SPI', '*', '*', '*', 'BL', 'SB', 'NT', 'IV']
-
-    # 命令方式
-    ASDU_SEL_EXEC = {
-        0x00: 'Execute',
-        0x80: 'Select',
-        0x01: 'Select',
-    }
-
-    # 遥控输出方式
-    ASDU_QU = {
-        0x00: 'no pulse defined',
-        0x01: 'short pulse duration (circuit-breaker)',  # 短脉冲方式输出
-        0x02: 'long pulse duration',  # 长脉冲方式输出
-        0x03: 'persistent output',  # 持续脉冲方式输出
-        0x04: 'reserved',
-        0x05: 'reserved',
-        0x06: 'reserved',
-    }
-
-    # 设置值
-    ASDU_SCS = {
-        0x00: 'OFF',
-        0x01: 'ON'
-    }
-
-    #
-    ASDU_SU = {
-        0X80: 'summer time',
-        0x00: 'normal time'
-    }
-
-    # Day Of Week
-    ASDU_DOW = {
-        0x00: 'undefined',
-        0x01: 'monday',
-        0x02: 'tuesday',
-        0x03: 'wednesday',
-        0x04: 'thursday',
-        0x05: 'friday',
-        0x06: 'saturday',
-        0x07: 'sunday'
-    }
-
-    ASDU_DPI = {
-        0x00: 'Indeterminate or Intermediate state',
-        0x01: 'Determined state OFF',
-        0x02: 'Determined state ON',
-        0x03: 'Indeterminate state'
-    }
-
-    ASDU_TRANSIENT = {
-        0x00: 'not in transient',
-        0x80: 'in transient'
-    }
-
-    ASDU_QOI = {
-        0x14: 'Station interrogation (global)',
-        0x15: 'Interrogation of group 1',
-        0x16: 'Interrogation of group 2',
-        0x17: 'Interrogation of group 3',
-        0x18: 'Interrogation of group 4',
-        0x19: 'Interrogation of group 5',
-        0x1A: 'Interrogation of group 6',
-        0x1B: 'Interrogation of group 7',
-        0x1C: 'Interrogation of group 8',
-        0x1D: 'Interrogation of group 9',
-        0x1E: 'Interrogation of group 10',
-        0x1F: 'Interrogation of group 11',
-        0x20: 'Interrogation of group 12',
-        0x21: 'Interrogation of group 13',
-        0x22: 'Interrogation of group 14',
-        0x23: 'Interrogation of group 15',
-        0x24: 'Interrogation of group 16'
-    }
-
-    ASDU_SPI = {
-        0x00: 'OFF',
-        0x01: 'ON'
-    }
-
-    ASDU_R = {
-        0x00: 'Local power switch on',
-        0x01: 'Local manual reset',
-        0x02: 'Remote reset',
-    }
-
-    for i in range(0x03, 0x7f):
-        ASDU_R[i] = 'Undefined'
-
-    ASDU_I = {
-        0x00: 'Initialization with unchanged local parameters',
-        0x80: 'Initialization after change of local parameters'
-    }
-
-
-class IECPacket:
-
-    class BSI(Packet):
-        name = 'BSI'
-        fields_desc = [
-            ShortField('BSI', None),
-        ]
-
-        def do_dissect(self, s):
-            self.BSI = ''.join(format(bt, '08b') for bt in s[0:4])
-            return s[4:]
-
-    class COI(Packet):
-        name = 'COI'
-        fields_desc = [
-            BitEnumField('I', None, 1, IECDefine.ASDU_I),
-            BitEnumField('R', None, 7, IECDefine.ASDU_R),
-        ]
-
-    class SIQ(Packet):
-        name = 'SIQ'
-        fields_desc = [
-            ByteField('SPI', None),
-            ByteField('BL', None),
-            ByteField('SB', None),
-            ByteField('NT', None),
-            ByteField('IV', None)
-        ]
-
-        def do_dissect(self, s):
-            self.SPI = IECDefine.ASDU_SPI[s[0] & 0x01]
-            self.BL = IECDefine.ASDU_BL[s[0] & 0x10]
-            self.SB = IECDefine.ASDU_SB[s[0] & 0x20]
-            self.NT = IECDefine.ASDU_NT[s[0] & 0x40]
-            self.IV = IECDefine.ASDU_IV[s[0] & 0x80]
-            return s[1:]
-
-    class QOI(Packet):
-        name = 'QOI'
-        fields_desc = [
-            ByteField('QOI', None),
-        ]
-
-        def do_dissect(self, s):
-            self.QOI = IECDefine.ASDU_QOI.get(s[0])
-            return s[1:]
-
-    class VTI(Packet):
-        name = 'VTI'
-        fields_desc = [
-            ByteField('Value', False),
-            ByteField('Transient', None)
-        ]
-
-        def do_dissect(self, s):
-            self.Value = unpack("<B", bytes([s[0] & 0x7F]))[0]
-            self.Transient = IECDefine.ASDU_TRANSIENT[s[0] & 0x80]
-            return s[1:]
-
-    class DIQ(Packet):
-        name = 'QDS'
-
-        fields_desc = [
-            ByteField('DPI', False),
-            ByteField('BL', None),
-            ByteField('SB', None),
-            ByteField('NT', None),
-            ByteField('IV', None)
-        ]
-
-        def do_dissect(self, s):
-            self.DPI = IECDefine.ASDU_DPI[s[0] & 0x03]
-            self.BL = IECDefine.ASDU_BL[s[0] & 0x10]
-            self.SB = IECDefine.ASDU_SB[s[0] & 0x20]
-            self.NT = IECDefine.ASDU_NT[s[0] & 0x40]
-            self.IV = IECDefine.ASDU_IV[s[0] & 0x80]
-
-            return s[1:]
-
-    class QOS(Packet):  # Section 7.2.6.39
-        name = 'QOS'
-        fields_desc = [
-            BitEnumField('SE', 0x00, 1, IECDefine.ASDU_SEL_EXEC),
-            BitField('QL', 0x00, 7),
-        ]
-
-    class QDS(Packet):
-        name = 'QDS'
-        fields_desc = [
-            ByteField('OV', False),
-            ByteField('BL', None),
-            ByteField('SB', None),
-            ByteField('NT', None),
-            ByteField('IV', None)
-        ]
-
-        def do_dissect(self, s):
-            self.OV = IECDefine.ASDU_OV[s[0] & 0x01]
-            self.BL = IECDefine.ASDU_BL[s[0] & 0x10]
-            self.SB = IECDefine.ASDU_SB[s[0] & 0x20]
-            self.NT = IECDefine.ASDU_NT[s[0] & 0x40]
-            self.IV = IECDefine.ASDU_IV[s[0] & 0x80]
-
-            return s[1:]
-
-    class CP56Time(Packet):
-        name = 'CP56Time'
-
-        fields_desc = [
-            ByteField('MS', None),
-            ByteField('Min', None),
-            ByteField('IV', None),
-            ByteField('Hour', None),
-            ByteField('SU', None),
-            ByteField('Day', None),
-            ByteField('DOW', None),
-            ByteField('Month', None),
-            ByteField('Year', None),
-        ]
-
-        def do_dissect(self, s):
-            self.MS = unpack('<H', s[0:2])[0]
-            self.Min = int(s[2] & 0x3f)
-            self.IV = IECDefine.ASDU_IV[s[2] & 0x80]
-            self.Hour = int(s[3] & 0x1F)
-            self.SU = IECDefine.ASDU_SU[s[3] & 0x80]
-            self.Day = int(s[4] & 0x1F)
-            self.DOW = IECDefine.ASDU_DOW[s[4] & 0xE0]
-            self.Month = int(s[5] & 0x0F)
-            self.Year = int(s[6] & 0x7F)
-            return s[7:]
-
-    class SCO(Packet):
-        name = 'SCO'
-        fields_desc = [
-            BitEnumField('SE', 0, 1, IECDefine.ASDU_SEL_EXEC),
-            BitEnumField('QU', 0, 6, IECDefine.ASDU_QU),
-            BitEnumField('SCS', 0, 1, IECDefine.ASDU_SCS),
-        ]
-
-    class DCO(Packet):
-        name = 'DCO'
-        fields_desc = [
-            BitEnumField('SE', 0, 1, IECDefine.ASDU_SEL_EXEC),
-            BitEnumField('QU', 0, 6, IECDefine.ASDU_QU),
-            BitEnumField('SCS', 0, 1, IECDefine.ASDU_SCS),
-        ]
-
-    class RCO(Packet):
-        name = 'RCO'
-        fields_desc = [
-            BitEnumField('SE', 0, 1, IECDefine.ASDU_SEL_EXEC),
-            BitEnumField('QU', 0, 6, IECDefine.ASDU_QU),
-            BitEnumField('SCS', 0, 1, IECDefine.ASDU_SCS),
-        ]
-
-    class LEFloatField(Field):
-        def __init__(self, name, default):
-            Field.__init__(self, name, default, '<f')
-
-    class LEIntField(Field):
-        def __init__(self, name, default):
-            Field.__init__(self, name, default, '<i')
-
-    class SignedShortField(Field):
-        def __init__(self, name, default):
-            Field.__init__(self, name, default, "<h")
-
-    class IOAID(Field):
-
-        def __init__(self, name, default):
-            Field.__init__(self, name, default, '<I')
-
-        def addfield(self, pkt, s, val):
-            if val is None:
-                return s
-            return s + pack('BBB', int(val & 0xff), int((val & 0xff00) / 0x0100), int((val & 0xff0000) / 0x010000))
-            #return s + pack('BB', int(val & 0xff), int((val & 0xff00) / 0x0100))  # NOTE: For malformed packets
-
-        def getfield(self, pkt, s):
-            return s[3:], self.m2i(pkt, unpack(self.fmt, s[:3] + b'\x00')[0])
-            #return s[2:], self.m2i(pkt, unpack(self.fmt, s[:2] + b'\x00\x00')[0])
-
-
-class IECData:
-
-    class IOA1(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('SIQ', None, IECPacket.SIQ)
-        ]
-
-    class IOA3(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('DIQ', None, IECPacket.DIQ)
-        ]
-
-    class IOA5(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('VTI', None, IECPacket.VTI),
-            PacketField('QDS', None, IECPacket.QDS)
-        ]
-
-    class IOA7(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('BSI', None, IECPacket.BSI),
-            PacketField('QDS', None, IECPacket.QDS)
-        ]
-
-    class IOA9(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.SignedShortField('Value', None),
-            PacketField('QDS', None, IECPacket.QDS)
-        ]
-
-    class IOA13(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEFloatField('Value', None),
-            PacketField('QDS', None, IECPacket.QDS)
-        ]
-
-    class IOA30(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('SIQ', None, IECPacket.SIQ),
-            PacketField('CP56Time', None, IECPacket.CP56Time)
-        ]
-
-    class IOA31(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('DIQ', None, IECPacket.DIQ),
-            PacketField('CP56Time', None, IECPacket.CP56Time)
-        ]
-
-    class IOA36(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEFloatField('Value', None),
-            PacketField('QDS', None, IECPacket.QDS),
-            PacketField('CP56Time', None, IECPacket.CP56Time),
-        ]
-
-    class IOA37(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEIntField('Binary_Counter', None),
-            ByteField('SQ', 0),
-            PacketField('CP56Time', None, IECPacket.CP56Time),
-        ]
-
-    class IOA45(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('SCO', None, IECPacket.SCO)
-        ]
-
-    class IOA46(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('DCO', None, IECPacket.DCO)
-        ]
-
-    class IOA47(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('RCO', None, IECPacket.RCO)
-        ]
-
-    class IOA48(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEIntField('Value', None),
-            PacketField('QOS', None, IECPacket.QOS)
-        ]
-
-    class IOA49(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEIntField('Value', None),
-            PacketField('QOS', None, IECPacket.QOS)
-        ]
-
-    class IOA50(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEFloatField('Value', None),
-            PacketField('QOS', None, IECPacket.QOS)
-        ]
-
-    class IOA51(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEIntField('Value', None)
-        ]
-
-    class IOA58(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('SCO', None, IECPacket.SCO),
-            PacketField('CP56Time', None, IECPacket.CP56Time)
-        ]
-
-    class IOA59(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('DCO', None, IECPacket.DCO),
-            PacketField('CP56Time', None, IECPacket.CP56Time)
-        ]
-
-    class IOA60(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('DCO', None, IECPacket.DCO),
-            PacketField('CP56Time', None, IECPacket.CP56Time)
-        ]
-
-    class IOA61(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEIntField('Value', None),
-            PacketField('QOS', None, IECPacket.QOS),
-            PacketField('CP56Time', None, IECPacket.CP56Time)
-        ]
-
-    class IOA62(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEIntField('Value', None),
-            PacketField('QOS', None, IECPacket.QOS),
-            PacketField('CP56Time', None, IECPacket.CP56Time)
-        ]
-
-    class IOA63(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEFloatField('Value', None),
-            PacketField('QOS', None, IECPacket.QOS),
-            PacketField('CP56Time', None, IECPacket.CP56Time)
-        ]
-
-    class IOA64(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            IECPacket.LEIntField('Value', None),
-            PacketField('CP56Time', None, IECPacket.CP56Time)
-        ]
-
-    class IOA70(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('COI', None, IECPacket.COI),
-        ]
-
-    class IOA100(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            ByteEnumField('QOI', None, IECDefine.ASDU_QOI)   #PacketField('QOI', None, IECPacket.QOI)
-        ]
-
-    class IOA101(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            XByteField('Operation', 0x05)
-        ]
-
-    class IOA103(Packet):
-        name = 'IOA'
-        fields_desc = [
-            IECPacket.IOAID('IOA', None),
-            PacketField('CP56Time', None, IECPacket.CP56Time)
-        ]
-
-    IOAS = {
-        1: IOA1,    # 单点遥信(带品质描述 不带时标)
-        3: IOA3,    # 双点遥信(带品质描述 不带时标)
-        5: IOA5,    # 步位置信息(带品质描述 不带时标)
-        7: IOA7,    # 32比特串(带品质描述 不带时标)
-        9: IOA9,    # 规一化遥测值(带品质描述 不带时标)
-        13: IOA13,  # 短浮点遥测值(带品质描述 不带时标)
-        30: IOA30,  # 单点遥信(带品质描述 带绝对时标)
-        31: IOA31,  # 双点遥信(带品质描述 带绝对时标)
-        36: IOA36,  # 短浮点遥测值(带品质描述 带绝对时标)
-        37: IOA37,   # 累积量(带品质描述 带绝对时标)
-        45: IOA45,  # 单点遥控(一个报文只有一个遥控信息体 不带时标)
-        50: IOA50,   # 短浮点设定值(一个报文只有一个设定值 不带时标)
-        70: IOA70,   # 初始化结束(从站发送，主站收到时候会做一次总召)
-        100: IOA100,    # 总召
-        103: IOA103,     # 时钟同步命令
-    }
-
-    IOALEN = {
-        1: 4,
-        3: 4,
-        5: 5,
-        7: 8,
-        9: 6,
-        13: 8,  # NOTE: For malformed packets
-        30: 10,
-        31: 11,
-        36: 15,
-        37: 25,
-        45: 4,
-        50: 8,
-        70: 4,
-        100: 4,
-        103: 10,
-    }
-
-
-class IOTIEC104(IOTDriver):
-
-    class ASDU(Packet):
-        name = 'ASDU'
-
-        fields_desc = [
-            ByteEnumField('Type', None, IECDefine.ASDU_TYPE),
-            ByteEnumField('SQ', None, IECDefine.ASDU_SQ),
-            ByteField('Num', 0),
-            ByteEnumField('Cause', None, IECDefine.ASDU_CAUSE),
-            ByteEnumField('PN', 0x00, IECDefine.ASDU_PN),
-            ByteField('Test', None),
-            ByteField('OA', None),
-            LEShortField('Addr', None),
-            PacketListField('IOA', None)
-        ]
-
-        def do_dissect(self, s):
-            self.Type = s[0] & 0xff   # 类型(1)
-            self.SQ = s[1] & 0x80 == 0x80   # 限定词(1)
-            self.Num = s[1] & 0x7f  # 数量
-            self.Cause = s[2] & 0x3F    # 原因
-            self.PN = s[2] & 0x40   # 第6位为P/N = 0 肯定 ； P/N = 1 否定 （正常为P/N = 0；P/N = 1说明该报文无效
-            self.Test = s[2] & 0x80 # 第7为为测试 T = 0 未试验 ； T = 1 试验 （一般 T= 0）
-            self.OA = s[3]          # 源发地址：用来记录来时哪个主站的响应数据，一般写 0；
-            self.Addr = unpack('<H', s[4:6])[0] # 公共地址
-
-            flag = True
-            IOAS = list()
-            remain = s[6:]
-
-            idx = 6
-            offset = 0
-            if self.Type not in IECData.IOAS.keys():
-                raise Exception(f"unsupport type({self.Type}")
-
-            ioa_type = IECData.IOAS.get(self.Type)
-            ioa_length = IECData.IOALEN.get(self.Type)
-            if self.SQ:
-                for i in range(1, self.Num + 1):
-                    if flag:
-                        if len(remain[:ioa_length]) >= ioa_length:
-                            IOAS.append(ioa_type(remain[:ioa_length]))
-                            offset = IOAS[0].IOA
-                            remain = remain[ioa_length:]
-                            idx = idx + ioa_length
-                            ioa_length = ioa_length - 3
+
+class AllenBradleyMessage(IOTBaseCommon.IOTNetMessage):
+    """用于和 AllenBradley PLC 交互的消息协议类"""
+
+    def get_head_length(self) -> int:
+        """协议头数据长度，也即是第一次接收的数据长度"""
+        return 24
+
+    def get_content_length(self) -> int:
+        """二次接收的数据长度"""
+        if self.heads is not None:
+            return IOTBaseCommon.DataTransform.unpack_bytes(self.heads[2:4], '<h')
+        else:
+            return 0
+
+    def check_response(self) -> bool:
+        """回复报文校验"""
+        return True
+
+
+# 初始化指令交互报文
+class AllenBradleyConstant:
+    CIP_READ_DATA = 0x4C    # CIP命令中的读取数据的服务
+    CIP_WRITE_DATA = 0x4D   # CIP命令中的写数据的服务
+    CIP_READ_WRITE_DATA = 0x4E
+    CIP_READ_FRAGMENT = 0x52    # CIP命令中的读片段的数据服务
+    CIP_WRITE_FRAGMENT = 0x53   # CIP命令中的写片段的数据服务
+    CIP_READ_LIST = 0x55
+    CIP_MULTIREAD_DATA = 0x1000  # CIP命令中的对数据读取服务
+    CIP_TYPE_BOOL = 0xC1    # bool型数据，一个字节长度
+    CIP_TYPE_BYTE = 0xC2    # byte型数据，一个字节长度
+    CIP_TYPE_WORD = 0xC3    # 整型，两个字节长度
+    CIP_TYPE_DWORD = 0xC4   # 长整型，四个字节长度
+    CIP_TYPE_LINT = 0xC5
+    CIP_TYPE_REAL = 0xCA    # 实数数据，四个字节长度
+    CIP_TYPE_DOUBLE = 0xCB
+    CIP_TYPE_STRUCT = 0xCC
+    CIP_TYPE_STRING = 0xD0
+    CIP_TYPE_BIT_ARRAY = 0xD3   # 二进制数据内容
+
+    RegisteredCommand = bytearray([0x65, 0x00,                              # 注册请求
+                                   0x04, 0x00,                              # 命令数据长度(单位字节)
+                                   0x00, 0x00, 0x00, 0x00,                    # 会话句柄,初始值为0x00000000
+                                   0x00, 0x00, 0x00, 0x00,                    # 状态，初始值为0x00000000（状态好）
+                                   0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,  # 请求通信一方的说明
+                                   0x00, 0x00, 0x00, 0x00,                    # 选项，默认为0x00000000
+                                   0x01, 0x00,                              # 协议版本（0x0001）
+                                   0x00, 0x00                               # 选项标记（0x0000
+                                   ])
+
+
+# 基础方法
+class AllenBradleyTools:
+
+    # 创建路径指令
+    @staticmethod
+    def parse_address(address: str, type: int):
+        """
+            0: address 1: path 2: type 3: type_code 8: value 9: result 10: msg
+        """
+        result = IOTBaseCommon.IOTNetResult()
+        try:
+            result.contents[0] = address
+            result.contents[1] = address[0:1]
+            result.contents[2] = type
+            result.contents[3] = AllenBradleyTools.get_type_code(type)
+            result.contents[4] = 1
+
+            ms = bytearray(0)
+            tag_names = address.split(".")
+
+            for i, tag_name in enumerate(tag_names):
+                index = ""
+                index_first = tag_name.find("[")
+                index_second = tag_name.find("]")
+                if 0 < index_first < index_second:
+                    index = tag_name[index_first + 1: index_second]
+                    tag_name = tag_name[0: index_first]
+
+                ms.append(0x91)  # 固定
+                ms.append(len(tag_name))
+                name = tag_name.encode(encoding='utf-8')
+                ms.extend(name)
+                if len(name) % 2 == 1:
+                    ms.append(0x00)
+
+                if index.strip() != "":
+                    indexs = index.split(",")
+                    for j in range(len(indexs)):
+                        index = int(indexs[j])
+                        if index < 256:
+                            ms.append(0x28)
+                            ms.append(index)
+                        else:
+                            ms.append(0x29)
+                            ms.append(0x00)
+                            ms.append(IOTBaseCommon.DataTransform.pack_value(index, '<i')[0])
+                            ms.append(IOTBaseCommon.DataTransform.pack_value(index, '<i')[1])
+
+            result.contents[1] = ms
+            result.is_success = True
+            return result
+        except Exception as e:
+            return IOTBaseCommon.IOTNetResult(msg=e.__str__())
+
+    @staticmethod
+    def get_type_code(type: int):
+        type_code = AllenBradleyConstant.CIP_TYPE_WORD
+        if type in [IOTBaseCommon.DataTransform.TypeFormat.BOOL.value]:
+            type_code = AllenBradleyConstant.CIP_TYPE_BOOL
+        elif type in [IOTBaseCommon.DataTransform.TypeFormat.INT8.value, IOTBaseCommon.DataTransform.TypeFormat.UINT8.value]:
+            type_code = AllenBradleyConstant.CIP_TYPE_BYTE
+        elif type in [IOTBaseCommon.DataTransform.TypeFormat.UINT16.value, IOTBaseCommon.DataTransform.TypeFormat.UINT16.value]:
+            type_code = AllenBradleyConstant.CIP_TYPE_WORD
+        elif type in [IOTBaseCommon.DataTransform.TypeFormat.INT32.value, IOTBaseCommon.DataTransform.TypeFormat.UINT32.value]:
+            type_code = AllenBradleyConstant.CIP_TYPE_DWORD
+        elif type in [IOTBaseCommon.DataTransform.TypeFormat.INT64.value, IOTBaseCommon.DataTransform.TypeFormat.UINT64.value]:
+            type_code = AllenBradleyConstant.CIP_TYPE_LINT
+        elif type in [IOTBaseCommon.DataTransform.TypeFormat.FLOAT.value]:
+            type_code = AllenBradleyConstant.CIP_TYPE_REAL
+        elif type in [IOTBaseCommon.DataTransform.TypeFormat.DOUBLE.value]:
+            type_code = AllenBradleyConstant.CIP_TYPE_DOUBLE
+        elif type in [IOTBaseCommon.DataTransform.TypeFormat.STRING.value]:
+            type_code = AllenBradleyConstant.CIP_TYPE_STRING
+        elif type in [IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY.value]:
+            type_code = AllenBradleyConstant.CIP_TYPE_BIT_ARRAY
+        return type_code
+
+    @staticmethod
+    def build_request_path_command(address: str) -> bytearray:
+        ms = bytearray(0)
+        tag_names = address.split(".")
+
+        for i, tag_name in enumerate(tag_names):
+            index = ""
+            index_first = tag_name.find("[")
+            index_second = tag_name.find("]")
+            if 0 < index_first < index_second:
+                index = tag_name[index_first + 1: index_second]
+                tag_name = tag_name[0: index_first]
+
+            ms.append(0x91)  # 固定
+            ms.append(len(tag_name))
+            name = tag_name.encode(encoding='utf-8')
+            ms.extend(name)
+            if len(name) % 2 == 1:
+                ms.append(0x00)
+
+            if index.strip() != "":
+                indexs = index.split(",")
+                for j in range(len(indexs)):
+                    index = int(indexs[j])
+                    if index < 256:
+                        ms.append(0x28)
+                        ms.append(index)
                     else:
-                        if len(remain[:ioa_length]) >= ioa_length:
-                            _offset = pack("<H", (i - 1) + offset) + b'\x00'  # See 7.2.2.1 of IEC 60870-5-101
-                            IOAS.append(ioa_type(_offset + remain[:ioa_length]))
-                            remain = remain[ioa_length:]
-                            idx = idx + ioa_length
-                    flag = False
-            else:
-                for i in range(1, self.Num + 1):
-                    if len(remain[:ioa_length]) >= ioa_length:
-                        IOAS.append(ioa_type(remain[: ioa_length]))
-                        remain = remain[ioa_length:]
-                        idx = idx + ioa_length
-            self.IOA = IOAS
-            return s[idx:]
-
-        def do_build(self):
-            s = bytearray()
-            s.append(self.Type)
-            s.append(self.SQ | self.Num)
-            s.append(self.Test | self.PN | self.Cause)
-            s.append(self.OA)
-            s.append(int(self.Addr) & 0xff)
-            s.append(int(self.Addr) >> 8)
-            s = bytes(s)
-            if self.IOA is not None:
-                for i in self.IOA:
-                    s += i.build()
-
-            return s
-
-        def info(self, pkt: Packet = None):
-            pkt = self if pkt is None else pkt
-            values = {}
-            for key in pkt.fields.keys():
-                if isinstance(pkt.fields[key], list):
-                    for filed in pkt.fields[key]:
-                        if isinstance(filed, Packet):
-                            if filed.name not in values.keys():
-                                values[filed.name] = []
-                            values[filed.name].append(self.info(filed))
-                elif isinstance(pkt.fields[key], Packet):
-                    values[pkt.fields[key].name] = self.info(pkt.fields[key])
+                        ms.append(0x29)
+                        ms.append(0x00)
+                        ms.append(IOTBaseCommon.DataTransform.pack_value(index, '<i')[0])
+                        ms.append(IOTBaseCommon.DataTransform.pack_value(index, '<i')[1])
+        return ms
+
+    # 打包成可发送的数据指令
+    @staticmethod
+    def pack_request_header(command: int, session: int, command_specific_data: bytearray) -> bytes:
+        """
+        command_specific_data，打包成可发送的数据指令 -> bytes
+        Prarameter
+          command: ushort 实际的命令暗号
+          session: uint 当前会话的id
+          command_specific_data: byteArray CommandSpecificData命令
+        """
+        buffer = bytearray(len(command_specific_data) + 24)
+        buffer[24: 24 + len(command_specific_data)] = command_specific_data
+        buffer[0:2] = IOTBaseCommon.DataTransform.pack_value(command, '<H')  # 注册请求
+        buffer[2:4] = IOTBaseCommon.DataTransform.pack_value(len(command_specific_data), '<H')  # 命令数据长度(单位字节)
+        buffer[4:8] = IOTBaseCommon.DataTransform.pack_value(session, '<I')  # 会话句柄,初始值为0x00000000
+        buffer[8: 12] = bytes.fromhex('00 00 00 00')    # 初始值为0x000000
+        buffer[12: 20] = bytes.fromhex('00 00 00 00 00 00 00 00')  # 发送方描述
+        buffer[20: 24] = bytes.fromhex('00 00 00 00')  # 选项
+        return buffer
+
+    # 打包生成一个请求读取数据的节点信息，CIP指令信息
+    @staticmethod
+    def pack_requset_read(request_path: bytearray, length: int) -> bytes:
+        buffer = bytearray(4 + len(request_path))
+        buffer[0] = AllenBradleyConstant.CIP_READ_DATA  # 读
+        buffer[1] = len(request_path) // 2
+        buffer[2: 2 + len(request_path)] = request_path
+        buffer[2 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[0]
+        buffer[1 + 2 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[1]
+        return buffer
+
+    # 打包生成一个请求读取数据片段的节点信息
+    @staticmethod
+    def pack_request_read_segment(address: str, start: int, length: int) -> bytes:
+        buffer = bytearray(1024)
+        offect = 0
+        buffer[offect] = AllenBradleyConstant.CIP_READ_FRAGMENT
+        offect += 1
+        offect += 1
+
+        request_path = AllenBradleyTools.build_request_path_command(address)
+        buffer[offect:offect + len(request_path)] = request_path
+        offect += len(request_path)
+
+        buffer[1] = (offect - 2) // 2
+        buffer[offect] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[0]
+        offect += 1
+        buffer[offect] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[1]
+        offect += 1
+        buffer[offect + 0] = IOTBaseCommon.DataTransform.pack_value(start, '<i')[0]
+        buffer[offect + 1] = IOTBaseCommon.DataTransform.pack_value(start, '<i')[1]
+        buffer[offect + 2] = IOTBaseCommon.DataTransform.pack_value(start, '<i')[2]
+        buffer[offect + 3] = IOTBaseCommon.DataTransform.pack_value(start, '<i')[3]
+        offect += 4
+
+        return buffer[0:offect]
+
+    # 据指定的数据和类型，生成对应的数据
+    @staticmethod
+    def pack_request_write(request_path: bytearray, type_code: int, value: bytes, length: int = 1) -> bytes:
+        buffer = bytearray(6 + len(request_path) + len(value))
+        buffer[0] = AllenBradleyConstant.CIP_WRITE_DATA  # 写
+        buffer[1] = len(request_path) // 2
+        buffer[2: 2 + len(request_path)] = request_path
+        buffer[2 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(type_code, '<i')[0]
+        buffer[3 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(type_code, '<i')[1]
+        buffer[4 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[0]
+        buffer[5 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[1]
+        buffer[6 + len(request_path): 6 + len(request_path) + len(value)] = value
+        return buffer
+
+    # 将所有的cip指定进行打包操作
+    @staticmethod
+    def pack_command_service(slot: bytearray, cips: list) -> bytes:
+        ms = bytearray(0)
+        ms.append(0xB2)     # 连接的项数
+        ms.append(0x00)
+        ms.append(0x00)     # 后面数据包的长度，等全部生成后在赋值
+        ms.append(0x00)
+
+        ms.append(0x52)     # 服务
+        ms.append(0x02)     # 请求路径大小
+        ms.append(0x20)     # 请求路径
+        ms.append(0x06)
+        ms.append(0x24)
+        ms.append(0x01)
+        ms.append(0x0A)     # 超时时间
+        ms.append(0xF0)
+        ms.append(0x00)     # CIP指令长度
+        ms.append(0x00)
+
+        count = 0
+        if len(cips) == 1:
+            ms.extend(cips[0])
+            count += len(cips[0])
+        else:
+            ms.append(0x0A)
+            ms.append(0x02)
+            ms.append(0x20)
+            ms.append(0x02)
+            ms.append(0x24)
+            ms.append(0x01)
+            count += 8
+
+            ms.extend(IOTBaseCommon.DataTransform.pack_value(len(cips), '<H'))
+            offect = 0x02 + 2 * len(cips)
+            count += 2 * len(cips)
+
+            for i in range(len(cips)):
+                ms.extend(IOTBaseCommon.DataTransform.pack_value(offect, '<H'))
+                offect = offect + len(cips[i])
+
+            for i in range(len(cips)):
+                ms.extend(cips[i])
+                count += len(cips[i])
+
+        ms.append((len(slot) + 1) // 2)
+        ms.append(0x00)
+        ms.extend(slot)
+        if len(slot) % 2 == 1:
+            ms.append(0x00)
+
+        ms[12:14] = IOTBaseCommon.DataTransform.pack_value(count, '<H')
+        ms[2:4] = IOTBaseCommon.DataTransform.pack_value(len(ms) - 4, '<H')
+        return ms
+
+    # 生成读取直接节点数据信息的内容
+    @staticmethod
+    def pack_command_specific_data(service: List[bytearray]) -> bytes:
+        buffer = bytearray(0)
+        buffer.append(0x00)
+        buffer.append(0x00)
+        buffer.append(0x00)
+        buffer.append(0x00)
+        buffer.append(0x01)  # 超时
+        buffer.append(0x00)
+        buffer.extend(IOTBaseCommon.DataTransform.pack_value(len(service), '<H'))
+        for i in range(len(service)):
+            buffer.extend(service[i])
+        return buffer
+
+    # 从PLC反馈的数据解析
+    @staticmethod
+    def extract_actual_data(response: bytearray, is_read: bool):
+        data = bytearray()
+        offset = 38
+        has_more_data = False
+        data_type = 0
+        count = IOTBaseCommon.DataTransform.unpack_bytes(response[38:40], '<H')  # 剩余总字节长度，在剩余的字节里，有可能是一项数据，也有可能是多项
+        if IOTBaseCommon.DataTransform.unpack_bytes(response[40:44], '<i') == 0x8A:  # 多项数据
+            offset = 44
+            data_count = IOTBaseCommon.DataTransform.unpack_bytes(response[offset:offset + 2], '<H')
+            for i in range(data_count):
+                offset_start = IOTBaseCommon.DataTransform.unpack_bytes(response[offset + 2 + i * 2: offset + 4 + i * 2], '<H')
+                if i == data_count - 1:
+                    offset_end = len(response)
                 else:
-                    values[key] = pkt.fields[key]
-            return values
+                    offset_end = IOTBaseCommon.DataTransform.unpack_bytes(response[offset + 2 + i * 2: offset + 4 + i * 2], '<H')
 
-    class APCI(Packet):
-        name = 'ACPI'
+                err = IOTBaseCommon.DataTransform.unpack_bytes(response[offset_start + 2: offset_start + 4], '<H')
+                if err in [0x04, 0x05, 0x0A, 0x13, 0x1C, 0x1E, 0x26]:
+                    return IOTBaseCommon.IOTNetResult(code=err, msg=AllenBradleyTools.get_status_description(err))
+                elif err == 0x06:
+                    if response[offset + 2] == 0xD2 or response[offset + 2] == 0xCC:
+                        return IOTBaseCommon.IOTNetResult(code=err, msg=AllenBradleyTools.get_status_description(err))
+                elif err == 0x00:
+                    pass
+                else:
+                    return IOTBaseCommon.IOTNetResult(code=err, msg=AllenBradleyTools.get_status_description(err))
 
-        fields_desc = [
-            XByteField('START', 0x68),      # 68H
-            ByteField('ApduLen', 4),        # 长度
-            ByteEnumField('Type', 0x00, IECDefine.APCI_TYPE),   # 帧类型
-            ConditionalField(XByteField('UType', None), lambda pkt: pkt.Type == 0x03),  # U帧类型
-            ConditionalField(ShortField('Tx', 0x00), lambda pkt: pkt.Type == 0x00),
-            ConditionalField(ShortField('Rx', 0x00), lambda pkt: pkt.Type < 3),
-        ]
-
-        def do_dissect(self, s):
-            self.START = s[0]       # 68H
-            self.ApduLen = s[1]     # 长度
-            self.Type = s[2] & 0x03 if bool(s[2] & 0x01) else 0x00
-            if self.Type == 3:      # U帧
-                self.UType = (s[2] & 0xfc) >> 2
+                if is_read is True:
+                    for j in range(offset_start + 6, offset_end, 1):
+                        data.append(response[j])
+        else:   # 单项数据
+            err = response[offset + 4]
+            if err in [0x04, 0x05, 0x0A, 0x13, 0x1C, 0x1E, 0x26]:
+                return IOTBaseCommon.IOTNetResult(code=err, msg=AllenBradleyTools.get_status_description(err))
+            elif err == 0x06:
+                has_more_data = True
+
+            elif err == 0x00:
+                if response[offset + 2] == 0xCD or response[offset + 2] == 0xD3:    # 写服务应答为0xD3
+                    return IOTBaseCommon.IOTNetResult.create_success([data, data_type, has_more_data])
+                if response[offset + 2] == 0xCC or response[offset + 2] == 0xD2:    # 0xD2为读取数据标签应答
+                    for i in range(offset + 8, offset + 2 + count, 1):
+                        data.append(response[i])
+                    data_type = IOTBaseCommon.DataTransform.unpack_bytes(response[offset + 6:offset + 8], '<H')
+                elif response[offset + 2] == 0xD5:
+                    for i in range(offset + 6, offset + 2 + count, 1):
+                        data.append(response[i])
             else:
-                if self.Type == 0:  # I帧
-                    self.Tx = (s[3] << 7) | (s[2] >> 1)
-                self.Rx = (s[5] << 7) | (s[4] >> 1)
-            return s[6:]
-
-        def dissect(self, s):
-            s = self.pre_dissect(s)
-            s = self.do_dissect(s)
-            s = self.post_dissect(s)
-            payl, pad = self.extract_padding(s)
-            self.do_dissect_payload(payl)
-            if pad:
-                self.add_payload(IOTIEC104.APDU(pad))
-
-        def do_build(self):
-            s = list(range(6))
-            s[0] = 0x68
-            s[1] = self.ApduLen
-            if self.Type == 0x03:
-                s[2] = ((self.UType << 2) & 0xfc) | self.Type
-                s[3] = 0
-                s[4] = 0
-                s[5] = 0
-            else:
-                if self.Type == 0x00:
-                    s[2] = ((self.Tx << 1) & 0x00fe) | self.Type
-                    s[3] = ((self.Tx << 1) & 0xff00) >> 8
-                else:
-                    s[2] = self.Type
-                    s[3] = 0
-                s[4] = (self.Rx << 1) & 0x00fe
-                s[5] = ((self.Rx << 1) & 0xff00) >> 8
-            s = bytes(s)
-            if self.haslayer('ASDU'):
-                s += self.payload.build()
-            return s
-
-        def extract_padding(self, s):
-            if self.Type == 0x00 and self.ApduLen > 4:
-                return s[:self.ApduLen - 4], s[self.ApduLen - 4:]
-            return None, s
-
-        def do_dissect_payload(self, s):
-            if s is not None:
-                p = IOTIEC104.ASDU(s, _internal=1, _underlayer=self)
-                self.add_payload(p)
-        def info(self):
-            values = {}
-            for key in self.fields.keys():
-                values[key] = self.fields[key]
-            return values
-
-    class APDU(Packet):
-        name = 'APDU'
-
-        def dissect(self, s):
-            s = self.pre_dissect(s)
-            s = self.do_dissect(s)
-            s = self.post_dissect(s)
-            payl, pad = self.extract_padding(s)
-            self.do_dissect_payload(payl)
-            if pad:
-                if pad[0] in [0x68]:
-                    self.add_payload(IOTIEC104.APDU(pad, _internal=1, _underlayer=self))
-                else:
-                    self.add_payload(Padding(pad))
+                return IOTBaseCommon.IOTNetResult(code=err, msg=AllenBradleyTools.get_status_description(err))
+        return IOTBaseCommon.IOTNetResult.create_success([data, data_type, has_more_data])
+
+    @staticmethod
+    def get_status_description(err):
+        """获取错误信息的字符串描述文本"""
+        if err == 0:
+            return f"Communication is normal."
+        elif err == 1:
+            return f"The message header is not fins"
+        elif err == 2:
+            return f"Data length too long"
+        elif err == 3:
+            return f"This command does not support"
+        elif err == 20:
+            return f"Exceeding connection limit"
+        elif err == 21:
+            return f"The specified node is already in the connection"
+        elif err == 22:
+            return f"Attempt to connect to a protected network node that is not yet configured in the PLC"
+        elif err == 23:
+            return f"The current client's network node exceeds the normal range"
+        elif err == 24:
+            return f"The current client's network node is already in use"
+        elif err == 25:
+            return f"All network nodes are already in use"
+        else:
+            return f"Unknown Error"
+
+    @staticmethod
+    def get_session_status_description(status: int) -> str:
+        """获取错误信息的字符串描述文本"""
+        if status == 0x01:
+            return f"The sender issued an invalid or unsupported encapsulation command."
+        elif status == 0x02:
+            return f"Insufficient memory resources in the receiver to handle the command. This is not an application error. Instead, it only results if the encapsulation layer cannot obtain memory resources that it need."
+        elif status == 0x03:
+            return f"Poorly formed or incorrect data in the data portion of the encapsulation message."
+        elif status == 0x64:
+            return f"An originator used an invalid session handle when sending an encapsulation message."
+        elif status == 0x65:
+            return f"The target received a message of invalid length."
+        elif status == 0x69:
+            return f"Unsupported encapsulation protocol revision."
+        else:
+            return f"Unknown"
+
+
+class AllenBradleyClient(IOTBaseCommon.IOTNetworkDeviceClient):
+
+    def __init__(self, host: str, port: int, slot: int = 0, timeout: int = 10):
+        super().__init__(host, port, timeout)
+
+        self.slot = slot  # 插槽
+        self.cip_command = 0x6F  # 实际的命令暗号
+        self.session_handle = 0  # 当前会话的id
+
+    def get_net_msg(self):
+        return AllenBradleyMessage()
+
+    def pack_command_with_header(self, command: bytearray):
+        return AllenBradleyTools.pack_request_header(self.cip_command, self.session_handle, command)
+
+    def register_session_handle(self):
+        """
+            向PLC注册会话ID的报文(协议版本（0x0001) 选项标记（0x0000))
+            65 00 04 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 01 00 00 00
+        """
+        return AllenBradleyTools.pack_request_header(0x65, 0, bytearray([0x01, 0x00, 0x00, 0x00]))
+
+    def unregister_session_handle(self):
+        """
+            获取卸载一个已注册的会话的报文
+            66 00 04 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 01 00 00 00
+        """
+        return AllenBradleyTools.pack_request_header(0x66, self.session_handle, bytearray(0))
+
+    def check_response(self, response: bytes):
+        try:
+            status = IOTBaseCommon.DataTransform.convert_value(response[8:12], IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, IOTBaseCommon.DataTransform.TypeFormat.INT32, pos=0)
+            if status == 0:
+                return IOTBaseCommon.IOTNetResult.create_success()
+            return IOTBaseCommon.IOTNetResult(msg=AllenBradleyTools.get_session_status_description(status))
+        except Exception as ex:
+            return IOTBaseCommon.IOTNetResult(msg=str(ex))
+
+    def initialization_on_connect(self, socket):
+        """在连接上PLC后，需要进行一步握手协议"""
+        # 握手信号
+        read = self.read_from_socket(socket, self.register_session_handle(), has_response=True, pack_unpack=False)
+        if read.is_success is False:
+            return read
+
+        # 检查返回的状态
+        check = self.check_response(read.contents[0])
+        if check.is_success is False:
+            return check
+
+        self.session_handle = IOTBaseCommon.DataTransform.unpack_bytes(read.contents[0][4:8], '<I')
+
+        # 返回成功的信号
+        return IOTBaseCommon.IOTNetResult.create_success()
+
+    def extra_on_disconnect(self, socket):
+        read = self.read_from_socket(socket, self.unregister_session_handle(), has_response=True, pack_unpack=False)
+        if read.is_success is False:
+            return read
+
+        return IOTBaseCommon.IOTNetResult.create_success()
+
+    def read(self, address: Union[tuple, list]):
+        """从PLC读取数据"""
+        if isinstance(address, list):
+            results = []
+            for (adr, type) in address:
+                tmp = AllenBradleyTools.parse_address(adr, type)
+                if tmp.is_success is False:
+                    return IOTBaseCommon.IOTNetResult.create_fail(tmp)
+                results.append(tmp)
+            return self._read(results)
+        elif isinstance(address, tuple):
+            result = AllenBradleyTools.parse_address(address[0], address[1])
+            if result.is_success is False:
+                return IOTBaseCommon.IOTNetResult.create_fail(result)
+            return self._read([result])
+
+    def write(self, address: Union[tuple, list]):
+        """将数据写入到PLC数据，地址格式为I100，Q100，DB20.100，M100，以字节为单位"""
+        if isinstance(address, list):
+            results = []
+            for (adr, type, value) in address:
+                tmp = AllenBradleyTools.parse_address(adr, type)
+                if tmp.is_success is False:
+                    return IOTBaseCommon.IOTNetResult.create_fail(tmp)
+                tmp.contents[8] = IOTBaseCommon.DataTransform.convert_value(value, IOTBaseCommon.DataTransform.TypeFormat(type), IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, format=IOTBaseCommon.DataTransform.DataFormat.ABCD)
+                results.append(tmp)
+            return self._write(results)
+        elif isinstance(address, tuple):
+            result = AllenBradleyTools.parse_address(address[0], address[1])
+            if result.is_success is False:
+                return IOTBaseCommon.IOTNetResult.create_fail(result)
+            result.contents[8] = IOTBaseCommon.DataTransform.convert_value(address[2], IOTBaseCommon.DataTransform.TypeFormat(address[1]), IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, format=IOTBaseCommon.DataTransform.DataFormat.ABCD)
+            return self._write([result])
+
+    def ping(self):
+        return self.get_socket().is_success
+
+    def get_real_command(self, address: Optional[IOTBaseCommon.IOTNetResult]):
+        try:
+            command_specific_data = AllenBradleyTools.pack_command_specific_data([bytearray(4), AllenBradleyTools.pack_command_service(self.slot if self.slot is None else bytearray([0x01, self.slot]), [AllenBradleyTools.pack_requset_read(address.contents[1], address.contents[4])])])
+            return IOTBaseCommon.IOTNetResult.create_success([command_specific_data])
+        except Exception as e:
+            return IOTBaseCommon.IOTNetResult(code=10000, msg=f"{e.__str__()}")
+
+    def get_write_command(self, address: Optional[IOTBaseCommon.IOTNetResult]):
+        try:
+            cip = AllenBradleyTools.pack_request_write(address.contents[1], address.contents[3], address.contents[8])
+            command_specific_data = AllenBradleyTools.pack_command_specific_data([bytearray(4), AllenBradleyTools.pack_command_service(self.slot if self.slot is None else bytearray([0x01, self.slot]), [cip])])
+            return IOTBaseCommon.IOTNetResult.create_success([command_specific_data])
+        except Exception as e:
+            return IOTBaseCommon.IOTNetResult(code=10000, msg=f"{e.__str__()}")
+
+    def get_command(self, address: Optional[IOTBaseCommon.IOTNetResult] = None, is_read: bool = True):
+        """生成一个读取字数据指令头的通用方法"""
+        return self.get_real_command(address) if is_read else self.get_write_command(address)
+
+    def _read(self, addresss: list):
+        """基础的读取方法，外界不应该调用本方法"""
+        for address in addresss:
+            command = self.get_command(address)
+            if command.is_success is False:
+                address.contents[9] = False
+                address.contents[10] = command.msg
+                continue
+
+            # 核心数据交互
+            read = self.read_server(command.contents[0])
+            if read.is_success is False:
+                address.contents[9] = False
+                address.contents[10] = read.msg
+                continue
+
+            # 数据有效性分析
+            valid = self.check_response(read.contents[0])
+            if valid.is_success is False:
+                address.contents[9] = False
+                address.contents[10] = valid.msg
+                continue
+
+            # 提取数据 -> Extracting data
+            extract = AllenBradleyTools.extract_actual_data(read.contents[0], True)
+            if extract.is_success is True:
+                length, type_fmt = IOTBaseCommon.DataTransform.get_type_size_fmt(IOTBaseCommon.DataTransform.TypeFormat(address.contents[2]))
+                response_data = bytearray(length)
+                response_data[0: length] = extract.contents[0][0: length]
+                address.contents[9] = True
+                address.contents[8] = IOTBaseCommon.DataTransform.convert_value(response_data, IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, IOTBaseCommon.DataTransform.TypeFormat(address.contents[2]), format=IOTBaseCommon.DataTransform.DataFormat.ABCD, pos=0)
+
+        return IOTBaseCommon.IOTNetResult.create_success(addresss)
+
+    def _write(self, addresss: list):
+        """基础的写入数据的操作支持"""
+        for address in addresss:
+            command = self.get_command(address, False)
+            if command.is_success is False:
+                address.contents[9] = False
+                address.contents[10] = command.msg
+                continue
+
+            # 核心数据交互
+            read = self.read_server(command.contents[0])
+            if read.is_success is False:
+                address.contents[9] = False
+                address.contents[10] = read.msg
+                continue
+
+            # 数据有效性分析
+            valid = self.check_response(read.contents[0])
+            if valid.is_success is False:
+                address.contents[9] = False
+                address.contents[10] = valid.msg
+                continue
+
+            # 提取数据 -> Extracting data
+            extract = AllenBradleyTools.extract_actual_data(read.contents[0], False)
+            if extract.is_success is True:
+                address.contents[9] = True
+
+        return IOTBaseCommon.IOTNetResult.create_success(addresss)
 
-        def do_dissect(self, s):
-            apci = IOTIEC104.APCI(s, _internal=1, _underlayer=self)
-            self.add_payload(apci)
-
-        def info(self):
-            values = {}
-            if not isinstance(self.payload, NoPayload):
-                values[self.payload.name] = self.payload.info()
-                if not isinstance(self.payload.payload, NoPayload):
-                    values[self.payload.payload.name] = self.payload.payload.info()
-            return values
+
+class IOTPlcAllenBradley(IOTDriver):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.reinit()
 
     def reinit(self):
         self.exit_flag = False
-        self.values = {}
-        self.send_count = 0
-        self.recv_count = 0
-        self.wait_event = None
+        self.clients = {}
 
     def exit(self):
         self.exit_flag = True
-        if self.wait_event is not None:
-            self.wait_event.set()
+        address = list(self.clients.keys())
+        for address in address:
+            if address in self.clients.keys():
+                self._release_client(address)
+
+        self.reinit()
 
     @classmethod
     def template(cls, mode: int, type: str, lan: str) -> List[Dict[str, Any]]:
         templates = []
         if type == 'point':
             templates.extend([
-                {'required': True, 'name': '是否可写' if lan == 'ch' else 'writable'.upper(), 'code': 'point_writable', 'type': 'bool', 'default': 'TRUE', 'enum': [], 'tip': ''},
-                {'required': True, 'name': '物理点名' if lan == 'ch' else 'name'.upper(), 'code': 'point_name', 'type': 'string', 'default': 'Chiller_1_CHW_ENT', 'enum': [], 'tip': ''},
-                {'required': True, 'name': '点地址' if lan == 'ch' else 'Address', 'code': 'point_address', 'type': 'int', 'default': 16385, 'enum': [], 'tip': ''},
-                {'required': True, 'name': '点类型' if lan == 'ch' else 'Type'.upper(), 'code': 'point_type', 'type': 'int', 'default': 13, 'enum': [], 'tip': ''},
-                {'required': False, 'name': '点描述' if lan == 'ch' else 'description'.upper(), 'code': 'point_description', 'type': 'string', 'default': 'Chiller_1_CHW_ENT', 'enum': [], 'tip': ''},
-                {'required': False, 'name': '逻辑点名' if lan == 'ch' else 'name alias'.upper(), 'code': 'point_name_alias', 'type': 'string', 'default': 'Chiller_1_CHW_ENT1', 'enum': [], 'tip': ''},
-                {'required': True, 'name': '是否启用' if lan == 'ch' else 'enable'.upper(), 'code': 'point_enabled', 'type': 'bool', 'default': 'TRUE', 'enum': [], 'tip': ''},
-                {'required': True, 'name': '倍率' if lan == 'ch' else 'scale'.upper(), 'code': 'point_scale', 'type': 'string', 'default': '1', 'enum': [], 'tip': ''}
+                                {'required': True, 'name': '是否可写' if lan == 'ch' else 'writable'.upper(), 'code': 'point_writable', 'type': 'bool', 'default': 'TRUE', 'enum': [], 'tip': ''},
+                                {'required': True, 'name': '物理点名' if lan == 'ch' else 'name'.upper(), 'code': 'point_name', 'type': 'string', 'default': 'Chiller_1_CHW_ENT', 'enum': [], 'tip': ''}
+                                ])
+            if mode == 0:
+                templates.append({'required': True, 'name': '设备地址' if lan == 'ch' else 'device address'.upper(), 'code': 'point_device_address', 'type': 'string', 'default': '192.168.1.184/44818/0', 'enum': [], 'tip': ''})
+            else:
+                templates.append({'required': True, 'name': '设备地址' if lan == 'ch' else 'device address'.upper(), 'code': 'point_device_address', 'type': 'string', 'default': '0.0.0.0/44818/0', 'enum': [], 'tip': ''})
+            templates.extend([
+                {'required': True, 'name': '点地址' if lan == 'ch' else 'address'.upper(), 'code': 'point_address', 'type': 'string', 'default': 'DB3,REAL4', 'enum': [], 'tip': ''},
+                {'required': True, 'name': '点类型' if lan == 'ch' else 'address'.upper(), 'code': 'point_type', 'type': 'int', 'default': 1, 'enum': [], 'tip': ''},
+                {'required': False, 'name': '点描述' if lan == 'ch' else 'description'.upper(), 'code': 'point_description', 'type': 'string', 'default': 'Chiller_1_CHW_ENT', 'enum': [], 'tip': ''}
             ])
-        elif type == 'config':
+            if mode == 0:
+                templates.extend([{'required': False, 'name': '逻辑点名' if lan == 'ch' else 'name alias'.upper(), 'code': 'point_name_alias', 'type': 'string', 'default': 'Chiller_1_CHW_ENT1', 'enum': [], 'tip': ''}])
+            else:
+                templates.append(
+                    {'required': True, 'name': '点值' if lan == 'ch' else 'value'.upper(), 'code': 'point_value', 'type': 'int', 'default': 0, 'enum': [], 'tip': ''})
             templates.extend([
-                {'required': True, 'name': '地址' if lan == 'ch' else 'Host', 'code': 'host', 'type': 'string', 'default': '192.168.1.1', 'enum': [], 'tip': ''},
-                {'required': True, 'name': '端口' if lan == 'ch' else 'Port', 'code': 'port', 'type': 'int', 'default': 2404, 'enum': [], 'tip': ''},
-                {'required': True, 'name': '超时(s)' if lan == 'ch' else 'Timeout(s)', 'code': 'timeout', 'type': 'float', 'default': 4, 'enum': [], 'tip': ''}
+                {'required': True, 'name': '是否启用' if lan == 'ch' else 'enable'.upper(), 'code': 'point_enabled', 'type': 'bool', 'default': 'TRUE', 'enum': [], 'tip': ''},
+                {'required': True, 'name': '倍率' if lan == 'ch' else 'scale'.upper(), 'code': 'point_scale', 'type': 'string', 'default': '1', 'enum': [], 'tip': ''}
             ])
 
+        elif type == 'config':
+            if mode == 0:
+                templates.extend([
+                    {'required': True, 'name': '批量读取个数' if lan == 'ch' else 'Multi Read', 'code': 'multi_read', 'type': 'int', 'default': 100, 'enum': [], 'tip': ''},
+                    {'required': True, 'name': '命令间隔(s)' if lan == 'ch' else 'Cmd Interval(s)', 'code': 'cmd_interval', 'type': 'float', 'default': 0.3, 'enum': [], 'tip': ''},
+                ])
+            templates.append({'required': True, 'name': '超时(s)' if lan == 'ch' else 'Timeout(s)', 'code': 'timeout', 'type': 'int', 'default': 15, 'enum': [], 'tip': ''})
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         names = kwargs.get('names', list(self.points.keys()))
         self.update_results(names, True, None)
-        read_items = []
+
+        read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
-                type = point.get('point_type')  # 单点遥信
-                address = point.get('point_address')    # 点地址
-                if type is not None and address is not None:
-                    read_items.append(f"{type}_{address}")
+                device_address = point.get('point_device_address')
+                address = point.get('point_address')
+                type = point.get('point_type')
+                if device_address is not None and address is not None and type is not None:
+                    if device_address not in read_items.keys():
+                        read_items[device_address] = []
+                    if (address, type) not in read_items[device_address]:
+                        read_items[device_address].append((address, type))
 
-        self._read(list(set(read_items)))
+        self._read(read_items)
 
         for name in names:
             point = self.points.get(name)
             if point:
-                type = point.get('point_type')  # 单点遥信
-                address = point.get('point_address')  # 点地址
-                if type is not None and address is not None:
-                    value = self._get_value(name, f"{self.configs.get('host')}:{self.configs.get('port')}", address, type)
+                device_address = point.get('point_device_address')
+                address = point.get('point_address')
+                type = point.get('point_type')
+                if device_address is not None and address is not None and type is not None:
+                    value = self._get_value(name, device_address, address, type)
                     if value is not None:
                         self.update_results(name, True, value)
             else:
                 self.update_results(name, False, 'UnExist')
         return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
+
         results = {}
         values = kwargs.get('values', {})
+        write_items = {}
+        for name, value in values.items():
+            point = self.points.get(name)
+            if point:
+                device_address = point.get('point_device_address')
+                address = point.get('point_address')
+                type = point.get('point_type')
+                if device_address is not None and address is not None and type is not None:
+                    if device_address not in write_items.keys():
+                        write_items[device_address] = []
+                    if (address, type, value) not in write_items[device_address]:
+                        write_items[device_address].append((address, type, value))
+
+        self._write(write_items)
+
         for name, value in values.items():
             point = self.points.get(name)
-            result = [False, 'Unknown']
             if point:
-                type = point.get('point_type')  # 单点遥信
-                address = point.get('point_address')  # 点地址
-                if type is not None and address is not None:
-                    self._write(type, address, value)
-                    result = self.get_device_property(f"{self.configs.get('host')}:{self.configs.get('port')}", f"{type}_{address}", [self.get_write_quality, self.get_write_result])
+                device_address = point.get('point_device_address')
+                address = point.get('point_address')
+                type = point.get('point_type')
+                if device_address is not None and address is not None and type is not None:
+                    result = self.get_device_property(device_address, f"{address}_{type}", [self.get_write_quality, self.get_write_result])
                 else:
                     result = [False, 'Invalid Params']
             else:
                 result = [False, 'Point UnExist']
+
             results[name] = result
             if result[0] is not True:
                 self.logging(content=f"write value({name}) fail({result[1]})", level='ERROR', source=name, pos=self.stack_pos)
         return results
 
     def ping(self, **kwargs) -> bool:
         self.update_info(used=IOTBaseCommon.get_datetime_str())
+        if kwargs.get('address') is not None:
+            if self._get_client(kwargs.get('address')) is not None:
+                return self._get_client(kwargs.get('address')).ping()
+            return False
         return True
 
-    def _read(self, read_items: list):
-        try:
-            if len(read_items) > 0 and self._get_client():
-                self.wait_event = Event()
-                self._send_zongzhao(self._get_client())
-                if self.wait_event.wait(self.configs.get('timeout', 4)) is False:
-                    raise Exception(f"response time out")
-        except Exception as e:
-            for read_item in read_items:
-                self.update_device(f"{self.configs.get('host')}:{self.configs.get('port')}", read_item, **self.gen_read_write_result(False, e.__str__()))
-
-    def _write(self, type: int, address: int, value):
-        raise NotImplementedError()
+    def _get_address_info(self, device_address: str) -> dict:
+        # ip/port/slot
+        info_list = device_address.split('/')
+        return {'host': info_list[0] if len(info_list) > 1 else '', 'port': int(float(info_list[1])) if len(info_list) > 2 else 44818, 'slot': int(float(info_list[2])) if len(info_list) > 3 else 0}
 
-    def _release_client(self):
+    def _release_client(self, address: str):
+        client = self.clients.get(address)
         try:
-            if self.client:
-                self.client.exit()
+            if client:
+                client.exit()
         except Exception as e:
             pass
         finally:
-            self.client = None
-
-    def _get_client(self):
-        if self.client is not None and self.client.check_invalid() is False:
-            self._release_client()
-
-        if self.client is None:
-            client = IOTBaseCommon.IECSocketClient(self.configs.get('host'), self.configs.get('port'), self.configs.get('timeout', 4), callbacks={'handle_data': self.handle_data, 'handle_connect': self.handle_connect, 'handle_close': self.handle_close, 'handle_error': self.handle_error})
-            self.client = client
-        return self.client
-
-    def handle_connect(self, client):
-        start_frame = (IOTIEC104.APDU() / IOTIEC104.APCI(ApduLen=4, Type=0x03, UType=0x01)).build()
-        self.logging(content=f"iec104({client}) connect success", pos=self.stack_pos)
-
-        # 连接成功 U帧启动报文
-        client.send(start_frame)
+            if address in self.clients.keys():
+                del self.clients[address]
 
-    # 关闭事件
-    def handle_close(self, client, reason: str):
-        self.logging(content=f"iec104({client}) close({reason})", pos=self.stack_pos)
-
-    def handle_error(self, client, e: Exception):
-        self.logging(content=f"iec104({client}) error({e.__str__()})", level='ERROR', pos=self.stack_pos)
-
-    def _update_value(self, type_id: int, address: int, value):
-        self.update_device(f"{self.configs.get('host')}:{self.configs.get('port')}", f"{type_id}_{address}", **self.gen_read_write_result(True, value))
+    def _get_client(self, address: str):
+        client = self.clients.get(address)
+        if client is not None and client.get_connected() is False:
+            self._release_client(address)
+            client = None
+
+        if client is None:
+            info = self._get_address_info(address)
+            if len(info) > 0:
+                client = AllenBradleyClient(info['host'], info['port'], info['slot'], self.configs.get('timeout'))
+                client.logging(call_logging=self.logging)
+                result = client.connect()
+                if result.is_success is True and client.get_connected() is True:
+                    self.clients[address] = client
+                else:
+                    raise Exception(f"{result.msg}")
+        return self.clients.get(address)
 
-    def handle_data(self, client, datas: bytes):
+    def _send_read_cmd(self, address: str, ab_item_list: list):
         try:
-            if len(datas) > 0 and client is not None:
-                info = IOTIEC104.APDU(datas).info()
-                acpi = info.get('ACPI', {})
-                asdu = info.get('ASDU', {})
-                type = acpi.get('Type')
-                if type == 0:  # I帧
-                    self.recv_count = info.get('ACPI', {}).get('Rx', self.recv_count) + 1
-                    type_id = asdu.get('Type')
-                    cause_id = asdu.get('Cause')
-                    self.logging(content=f"iec104 recv {self._get_frame_name(type_id, cause_id)}: [{self.client.format_bytes(datas)}]", pos=self.stack_pos)
-                    if type_id == 100:  # 总召
-                        if cause_id == 7:   # 总召确认
-                            pass
-                        elif cause_id == 10:   # 总召结束
-                            self.wait_event.set()   # self._send_zongzhao(client)
-                    elif type_id in [1, 30]:  # 单点遥信(带品质描述 不带时标) 单点遥信(带品质描述 带绝对时标)
-                        for ioa in asdu.get('IOA', []):
-                            if 'SIQ' in ioa.keys():
-                                self._update_value(type_id, ioa.get('IOA'), ioa.get('SIQ').get('SPI'))
-                    elif type_id in [3, 31]:  # 双点遥信(带品质描述 不带时标) 双点遥信(带品质描述 带绝对时标)
-                        for ioa in asdu.get('IOA', []):
-                            if 'DIQ' in ioa.keys():
-                                self._update_value(type_id, ioa.get('IOA'), ioa.get('DIQ').get('DPI'))
-                    elif type_id == 5:  # 步位置信息(带品质描述 不带时标)
-                        for ioa in asdu.get('IOA', []):
-                            if 'VTI' in ioa.keys():
-                                self._update_value(type_id, ioa.get('IOA'), ioa.get('VTI').get('Value'))
-                    elif type_id == 7:  # 32比特串(带品质描述 不带时标)
-                        pass
-                    elif type_id == 9:  # 规一化遥测值(带品质描述 不带时标)
-                        for ioa in asdu.get('IOA', []):
-                            if 'DIQ' in ioa.keys():
-                                self._update_value(type_id, ioa.get('IOA'), ioa.get('DIQ').get('DPI'))
-                    elif type_id in [13, 36]:     # 短浮点遥测值(带品质描述 不带时标) 短浮点遥测值(带品质描述 带绝对时标)
-                        for ioa in asdu.get('IOA', []):
-                            if 'Value' in ioa.keys():
-                                self._update_value(type_id, ioa.get('IOA'), ioa.get('Value'))
-                    elif type_id == 37:  # 累积量(带品质描述 带绝对时标)
-                        pass
-                    elif type_id == 45:     # 单点遥控(一个报文只有一个遥控信息体 不带时标)
-                        pass
-                    elif type_id == 50:     # 短浮点设定值(一个报文只有一个设定值 不带时标)
-                        pass
-                elif type == 1:  # S帧
-                    pass
-                elif type == 3:
-                    if info.get('ACPI', {}).get('UType') == 0x02:  # U帧激活确认 发送总召命令
-                        self._send_zongzhao(client)
-                    elif info.get('ACPI', {}).get('UType') == 0x08:     # U帧结束确认
-                        pass
+            if self._get_client(address) is not None and len(ab_item_list) > 0:
+                result = self._get_client(address).read(ab_item_list)
+                if isinstance(result, IOTBaseCommon.IOTNetResult):
+                    if result.is_success is True:
+                        for item in result.contents:
+                            if isinstance(item, IOTBaseCommon.IOTNetResult):
+                                if item.is_success:
+                                    if item.contents[9] is True:
+                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}", **self.gen_read_write_result(True, item.contents[8]))
+                                    else:
+                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}", **self.gen_read_write_result(False, item.contents[10]))
+                                else:
+                                    self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}", **self.gen_read_write_result(False, item.msg))
+                    else:
+                        raise Exception(f"{result.msg}")
         except Exception as e:
-            self.logging(content=f"handle data fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
+            for (ad, type) in ab_item_list:
+                self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__()))
+
+    def _read_address(self, *args, **kwargs) -> dict:
+        (address, ab_items) = args
+        results = {}
+        units = IOTBaseCommon.chunk_list(ab_items, self.configs.get('multi_read'))
+        for unit in units:
+            self._send_read_cmd(address, unit)
+            self.delay(self.configs.get('cmd_interval', 0.3))
+        return results
+
+    def _read(self, read_items: dict):
+        if len(read_items) > 0:
+            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items), f"{self}")
+            for address, ab_items in read_items.items():
+                jobs.submit_task(self._read_address, address, ab_items)
+            return jobs.done()
+        return {}
 
     def _get_value(self, name: str, device_address: str, address: str, type: int):
         try:
-            [result, value] = self.get_device_property(device_address, f"{type}_{address}", [self.get_read_quality, self.get_read_result])
+            [result, value] = self.get_device_property(device_address, f"{address}_{type}", [self.get_read_quality, self.get_read_result])
             if result is True:
                 if value is not None:
                     return value
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
             self.update_results(name, False, e.__str__())
         return None
 
-    def _send_frame(self, type_id: int, cause_id: int, datas: bytes):
-        if self.client is not None:
-            self.logging(content=f"iec104 send {self._get_frame_name(type_id, cause_id)}: [{self.client.format_bytes(datas)}]", pos=self.stack_pos)
-            self.client.send(datas)
-        
-            if len(datas) > 6:
-                self.send_count = self.send_count + 1
-        else:
-            raise Exception(f"no client")
+    def _send_write_cmd(self, address: str, ab_item_list: list):
+        try:
+            if self._get_client(address) is not None and len(ab_item_list) > 0:
+                result = self._get_client(address).write(ab_item_list)
+                if isinstance(result, IOTBaseCommon.IOTNetResult):
+                    if result.is_success is True:
+                        for item in result.contents:
+                            if isinstance(item, IOTBaseCommon.IOTNetResult):
+                                if item.is_success:
+                                    if item.contents[9] is True:
+                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}",  **self.gen_read_write_result(True, item.contents[9], False))
+                                    else:
+                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}",  **self.gen_read_write_result(False, item.contents[10], False))
+                                else:
+                                    self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}",  **self.gen_read_write_result(False, item.msg, False))
+                    else:
+                        raise Exception(f"{result.msg}")
+        except Exception as e:
+            for (ad, type, value) in ab_item_list:
+                self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__(), False))
 
-    def _get_frame_name(self, type_id: int, cause_id: int) -> str:
-        return f"{IECDefine.ASDU_TYPE.get(type_id)} {IECDefine.ASDU_CAUSE.get(cause_id)}"
+    def _write_address(self, *args, **kwargs) -> dict:
+        (address, ab_items) = args
+        results = {}
+        units = IOTBaseCommon.chunk_list(ab_items, self.configs.get('multi_read'))
+        for unit in units:
+            self._send_write_cmd(address, unit)
+            self.delay(self.configs.get('cmd_interval', 0.3))
+        return results
 
-    # 发送总召命令
-    def _send_zongzhao(self, client):
-        if client is not None:
-            pkt = IOTIEC104.APDU()
-            pkt /= IOTIEC104.APCI(ApduLen=14, Type=0x00, Tx=self.send_count, Rx=self.recv_count)
-            pkt /= IOTIEC104.ASDU(Type=100, SQ=0, Cause=6, Num=1, Test=0, OA=0, Addr=1, IOA=[IECData.IOAS[100](IOA=0, QOI=0x14)])
-            self._send_frame(100, 6, pkt.build())
+    def _write(self, write_items: dict):
+        if len(write_items) > 0:
+            jobs = IOTBaseCommon.SimpleThreadPool(len(write_items), f"{self}")
+            for address, ab_items in write_items.items():
+                jobs.submit_task(self._write_address, address, ab_items)
+            return jobs.done()
+        return {}
```

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,669 +1,660 @@
+from enum import Enum
+
 from typing import List, Dict, Any, Union, Optional
 
 from .base import IOTBaseCommon, IOTDriver
 
-'''
-https://blog.csdn.net/lishiming0308/article/details/85243041
+"""
+大端模式
+        网络传输一般采用大端序，也被称之为网络字节序，或网络序。IP协议中定义大端序为网络字节序。
+        高字节放在内存的地地址
+        
+点地址
+    6/192.168.1.172/102/0/1
+
+rack是机架号，slot卡槽号
+    s7-200 0, 1
+    s7-300 0, 2
+    s7-400 具体看硬件组态
+    s7-1200/1500 0, 0/1
+
+dbnumber:
+    地址编号（int），只适用于DB区和200samart的V区，其它区全默认0，V区只能填1
+
+read_multi_vars：
+    这是可以一次读取<=19个不同地址类型的变量，由于pdu大小限制一次性读取不能超过19个变量
+
+Address:
+    bool
+        I0.1
+        Q2.3
+        M0.0
+        DB1.DBX0.0
+    Byte:
+        IB2
+        MB0
+        QB0
+        VB0
+        DB1.DBB2
+    WORD:
+        MW10
+        IW
+        QW
+        VW
+        DB1.DBW2
+    DWORD:
+        MD10
+        QD
+        ID
+        VD
+        DB1.DBD2
+"""
 
-Rockwell Allen-Bradley(AB)PLC
-罗克韦尔CIP
-AB PLC的数据通信类，使用CIP协议实现，适用1756，1769等型号，支持使用标签的形式进行读写操作，支持标量数据，一维数组，二维数组，三维数组等等。如果是局部变量，那么使用 Program:MainProgram.[变量名]
-
-ABPLC的通讯采用小端模式。一般情况实现注册、请求、读写数据即可。不实现关闭请求、卸载注册在实际测试过程中也不会出现问题。在断开连接时不提交关闭请求和卸载注册指令。再重新连接plc执行注册、打开请求、读写数据还是一样可以成功的。
-连接：
-    客户端发送注册会话请求， PLC收到请求后，生成会话句柄并返回客户端
-    客户端收到句柄后生成连接标识，通过开放数据连接(ForwardOpen)请求发送给PLC， OLC收到后发送O2T给客户端
-    读取数据请求
-    应答
-'''
 
+class SiemensS7Message(IOTBaseCommon.IOTNetMessage):
 
-class AllenBradleyMessage(IOTBaseCommon.IOTNetMessage):
-    """用于和 AllenBradley PLC 交互的消息协议类"""
+    """西门子s7协议的消息接收规则"""
 
     def get_head_length(self) -> int:
         """协议头数据长度，也即是第一次接收的数据长度"""
-        return 24
+        return 4
 
     def get_content_length(self) -> int:
         """二次接收的数据长度"""
         if self.heads is not None:
-            return IOTBaseCommon.DataTransform.unpack_bytes(self.heads[2:4], '<h')
+            return self.heads[2] * 256 + self.heads[3] - 4
         else:
             return 0
 
     def check_response(self) -> bool:
         """回复报文校验"""
-        return True
+        if self.heads is not None:
+            if self.heads[0] == 0x03 and self.heads[1] == 0x00:
+                return True
+            else:
+                return False
+        else:
+            return False
 
 
-# 初始化指令交互报文
-class AllenBradleyConstant:
-    CIP_READ_DATA = 0x4C    # CIP命令中的读取数据的服务
-    CIP_WRITE_DATA = 0x4D   # CIP命令中的写数据的服务
-    CIP_READ_WRITE_DATA = 0x4E
-    CIP_READ_FRAGMENT = 0x52    # CIP命令中的读片段的数据服务
-    CIP_WRITE_FRAGMENT = 0x53   # CIP命令中的写片段的数据服务
-    CIP_READ_LIST = 0x55
-    CIP_MULTIREAD_DATA = 0x1000  # CIP命令中的对数据读取服务
-    CIP_TYPE_BOOL = 0xC1    # bool型数据，一个字节长度
-    CIP_TYPE_BYTE = 0xC2    # byte型数据，一个字节长度
-    CIP_TYPE_WORD = 0xC3    # 整型，两个字节长度
-    CIP_TYPE_DWORD = 0xC4   # 长整型，四个字节长度
-    CIP_TYPE_LINT = 0xC5
-    CIP_TYPE_REAL = 0xCA    # 实数数据，四个字节长度
-    CIP_TYPE_DOUBLE = 0xCB
-    CIP_TYPE_STRUCT = 0xCC
-    CIP_TYPE_STRING = 0xD0
-    CIP_TYPE_BIT_ARRAY = 0xD3   # 二进制数据内容
-
-    RegisteredCommand = bytearray([0x65, 0x00,                              # 注册请求
-                                   0x04, 0x00,                              # 命令数据长度(单位字节)
-                                   0x00, 0x00, 0x00, 0x00,                    # 会话句柄,初始值为0x00000000
-                                   0x00, 0x00, 0x00, 0x00,                    # 状态，初始值为0x00000000（状态好）
-                                   0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,  # 请求通信一方的说明
-                                   0x00, 0x00, 0x00, 0x00,                    # 选项，默认为0x00000000
-                                   0x01, 0x00,                              # 协议版本（0x0001）
-                                   0x00, 0x00                               # 选项标记（0x0000
-                                   ])
+# 西门子PLC的类型对象
+class SiemensS7Version(Enum):
+    S7_200 = 1  # 西门子S7-200 需要配置网络模块
+    S7_200Smart = 2
+    S7_300 = 3
+    S7_400 = 4
+    S7_1200 = 5
+    S7_1500 = 6
 
 
-# 基础方法
-class AllenBradleyTools:
+# 初始化指令交互报文
+class SiemensS7Constant:
+    Head1 = bytearray([0x03, 0x00, 0x00, 0x16, 0x11, 0xE0, 0x00, 0x00, 0x00, 0x01, 0x00, 0xC0, 0x01, 0x0A, 0xC1, 0x02, 0x01, 0x02, 0xC2, 0x02, 0x01, 0x00])
+    Head2 = bytearray([0x03, 0x00, 0x00, 0x19, 0x02, 0xF0, 0x80, 0x32, 0x01, 0x00, 0x00, 0x04, 0x00, 0x00, 0x08, 0x00, 0x00, 0xF0, 0x00, 0x00, 0x01, 0x00, 0x01, 0x01, 0xE0])
+    Head1_200Smart = bytearray([0x03, 0x00, 0x00, 0x16, 0x11, 0xE0, 0x00, 0x00, 0x00, 0x01, 0x00, 0xC1, 0x02, 0x10, 0x00, 0xC2, 0x02, 0x03, 0x00, 0xC0, 0x01, 0x0A])
+    Head2_200Smart = bytearray([0x03, 0x00, 0x00, 0x19, 0x02, 0xF0, 0x80, 0x32, 0x01, 0x00, 0x00, 0xCC, 0xC1, 0x00, 0x08, 0x00, 0x00, 0xF0, 0x00, 0x00, 0x01, 0x00, 0x01, 0x03, 0xC0])
+    Head1_200 = bytearray([0x03, 0x00, 0x00, 0x16, 0x11, 0xE0, 0x00, 0x00, 0x00, 0x01, 0x00, 0xC1, 0x02, 0x4D, 0x57, 0xC2, 0x02, 0x4D, 0x57, 0xC0, 0x01, 0x09])
+    Head2_200 = bytearray([0x03, 0x00, 0x00, 0x19, 0x02, 0xF0, 0x80, 0x32, 0x01, 0x00, 0x00, 0x00, 0x00, 0x00, 0x08, 0x00, 0x00, 0xF0, 0x00, 0x00, 0x01, 0x00, 0x01, 0x03, 0xC0])
 
-    # 创建路径指令
-    @staticmethod
-    def parse_address(address: str, type: int):
-        """
-            0: address 1: path 2: type 3: type_code 8: value 9: result 10: msg
-        """
-        result = IOTBaseCommon.IOTNetResult()
-        try:
-            result.contents[0] = address
-            result.contents[1] = address[0:1]
-            result.contents[2] = type
-            result.contents[3] = AllenBradleyTools.get_type_code(type)
-            result.contents[4] = 1
-
-            ms = bytearray(0)
-            tag_names = address.split(".")
-
-            for i, tag_name in enumerate(tag_names):
-                index = ""
-                index_first = tag_name.find("[")
-                index_second = tag_name.find("]")
-                if 0 < index_first < index_second:
-                    index = tag_name[index_first + 1: index_second]
-                    tag_name = tag_name[0: index_first]
-
-                ms.append(0x91)  # 固定
-                ms.append(len(tag_name))
-                name = tag_name.encode(encoding='utf-8')
-                ms.extend(name)
-                if len(name) % 2 == 1:
-                    ms.append(0x00)
-
-                if index.strip() != "":
-                    indexs = index.split(",")
-                    for j in range(len(indexs)):
-                        index = int(indexs[j])
-                        if index < 256:
-                            ms.append(0x28)
-                            ms.append(index)
-                        else:
-                            ms.append(0x29)
-                            ms.append(0x00)
-                            ms.append(IOTBaseCommon.DataTransform.pack_value(index, '<i')[0])
-                            ms.append(IOTBaseCommon.DataTransform.pack_value(index, '<i')[1])
 
-            result.contents[1] = ms
-            result.is_success = True
-            return result
-        except Exception as e:
-            return IOTBaseCommon.IOTNetResult(msg=e.__str__())
+# 基础方法
+class SiemensS7Tools:
 
     @staticmethod
-    def get_type_code(type: int):
-        type_code = AllenBradleyConstant.CIP_TYPE_WORD
-        if type in [IOTBaseCommon.DataTransform.TypeFormat.BOOL.value]:
-            type_code = AllenBradleyConstant.CIP_TYPE_BOOL
-        elif type in [IOTBaseCommon.DataTransform.TypeFormat.INT8.value, IOTBaseCommon.DataTransform.TypeFormat.UINT8.value]:
-            type_code = AllenBradleyConstant.CIP_TYPE_BYTE
-        elif type in [IOTBaseCommon.DataTransform.TypeFormat.UINT16.value, IOTBaseCommon.DataTransform.TypeFormat.UINT16.value]:
-            type_code = AllenBradleyConstant.CIP_TYPE_WORD
-        elif type in [IOTBaseCommon.DataTransform.TypeFormat.INT32.value, IOTBaseCommon.DataTransform.TypeFormat.UINT32.value]:
-            type_code = AllenBradleyConstant.CIP_TYPE_DWORD
-        elif type in [IOTBaseCommon.DataTransform.TypeFormat.INT64.value, IOTBaseCommon.DataTransform.TypeFormat.UINT64.value]:
-            type_code = AllenBradleyConstant.CIP_TYPE_LINT
-        elif type in [IOTBaseCommon.DataTransform.TypeFormat.FLOAT.value]:
-            type_code = AllenBradleyConstant.CIP_TYPE_REAL
-        elif type in [IOTBaseCommon.DataTransform.TypeFormat.DOUBLE.value]:
-            type_code = AllenBradleyConstant.CIP_TYPE_DOUBLE
-        elif type in [IOTBaseCommon.DataTransform.TypeFormat.STRING.value]:
-            type_code = AllenBradleyConstant.CIP_TYPE_STRING
-        elif type in [IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY.value]:
-            type_code = AllenBradleyConstant.CIP_TYPE_BIT_ARRAY
-        return type_code
+    def get_begin_address(address: str):
+        address = IOTBaseCommon.format_name(address, r'[^0-9.]+', '')  # 去除地址中的多余字符
+        if address.find('.') >= 0:
+            temp = address.split(".")
+            return int(temp[0]) * 8 + int(temp[1])
+        else:
+            return int(address) * 8
 
     @staticmethod
-    def build_request_path_command(address: str) -> bytearray:
-        ms = bytearray(0)
-        tag_names = address.split(".")
-
-        for i, tag_name in enumerate(tag_names):
-            index = ""
-            index_first = tag_name.find("[")
-            index_second = tag_name.find("]")
-            if 0 < index_first < index_second:
-                index = tag_name[index_first + 1: index_second]
-                tag_name = tag_name[0: index_first]
-
-            ms.append(0x91)  # 固定
-            ms.append(len(tag_name))
-            name = tag_name.encode(encoding='utf-8')
-            ms.extend(name)
-            if len(name) % 2 == 1:
-                ms.append(0x00)
-
-            if index.strip() != "":
-                indexs = index.split(",")
-                for j in range(len(indexs)):
-                    index = int(indexs[j])
-                    if index < 256:
-                        ms.append(0x28)
-                        ms.append(index)
-                    else:
-                        ms.append(0x29)
-                        ms.append(0x00)
-                        ms.append(IOTBaseCommon.DataTransform.pack_value(index, '<i')[0])
-                        ms.append(IOTBaseCommon.DataTransform.pack_value(index, '<i')[1])
-        return ms
+    def get_db(address: str) -> int:
+        return int(IOTBaseCommon.format_name(address, r'[^0-9]+', ''))
 
-    # 打包成可发送的数据指令
     @staticmethod
-    def pack_request_header(command: int, session: int, command_specific_data: bytearray) -> bytes:
-        """
-        command_specific_data，打包成可发送的数据指令 -> bytes
-        Prarameter
-          command: ushort 实际的命令暗号
-          session: uint 当前会话的id
-          command_specific_data: byteArray CommandSpecificData命令
-        """
-        buffer = bytearray(len(command_specific_data) + 24)
-        buffer[24: 24 + len(command_specific_data)] = command_specific_data
-        buffer[0:2] = IOTBaseCommon.DataTransform.pack_value(command, '<H')  # 注册请求
-        buffer[2:4] = IOTBaseCommon.DataTransform.pack_value(len(command_specific_data), '<H')  # 命令数据长度(单位字节)
-        buffer[4:8] = IOTBaseCommon.DataTransform.pack_value(session, '<I')  # 会话句柄,初始值为0x00000000
-        buffer[8: 12] = bytes.fromhex('00 00 00 00')    # 初始值为0x000000
-        buffer[12: 20] = bytes.fromhex('00 00 00 00 00 00 00 00')  # 发送方描述
-        buffer[20: 24] = bytes.fromhex('00 00 00 00')  # 选项
-        return buffer
+    def get_is_bit(address: str) -> bool:
+        return IOTBaseCommon.format_name(address, r'[^0-9.]+', '').find('.') >= 0
 
-    # 打包生成一个请求读取数据的节点信息，CIP指令信息
     @staticmethod
-    def pack_requset_read(request_path: bytearray, length: int) -> bytes:
-        buffer = bytearray(4 + len(request_path))
-        buffer[0] = AllenBradleyConstant.CIP_READ_DATA  # 读
-        buffer[1] = len(request_path) // 2
-        buffer[2: 2 + len(request_path)] = request_path
-        buffer[2 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[0]
-        buffer[1 + 2 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[1]
-        return buffer
+    def parse_address(address: str, type: int):
+        """解析数据地址，解析出地址类型，起始地址，DB块的地址"""
+        result = IOTBaseCommon.IOTNetResult()
+        try:
+            # 1: area 2: start 3: db 4: is_bit 5: length 6: type 7: fmt 8: value
+            type_size, type_fmt = IOTBaseCommon.DataTransform.get_type_size_fmt(IOTBaseCommon.DataTransform.TypeFormat(type))
+            result.contents[0] = address
+            result.contents[3] = 0
+            result.contents[5] = type_size
+            result.contents[6] = type
+            result.contents[7] = type_fmt
+
+            if address[0] == 'I':
+                result.contents[1] = 0x81
+            elif address[0] == 'Q':
+                result.contents[1] = 0x82
+            elif address[0] == 'M':
+                result.contents[1] = 0x83
+            elif address[0] == 'D' or address[0:2] == "DB":
+                result.contents[1] = 0x84
+                pos = address.find(',')
+                if pos > 0:
+                    result.contents[3] = SiemensS7Tools.get_db(address[0:pos])
+                else:
+                    pos = address.find('.')
+                    result.contents[3] = SiemensS7Tools.get_db(address[0:pos])
+            elif address[0] == 'T':
+                result.contents[1] = 0x1D
+            elif address[0] == 'C':
+                result.contents[1] = 0x1C
+            elif address[0] == 'V':
+                result.contents[1] = 0x84
+                result.contents[3] = 1
+            else:
+                result.msg = f"Unsupported DataType"
+                result.is_success = False
+                return result
+
+            if address[0] == 'D' and address[1] == 'B':
+                pos = address.find(',') + 1
+                if pos > 0:
+                    result.contents[2] = SiemensS7Tools.get_begin_address(address[pos:])
+                    result.contents[4] = SiemensS7Tools.get_is_bit(address[pos:])
+                else:
+                    pos = address.find('.') + 1
+                    if pos > 0:
+                        result.contents[2] = SiemensS7Tools.get_begin_address(address[pos:])
+                        result.contents[4] = SiemensS7Tools.get_is_bit(address[pos:])
 
-    # 打包生成一个请求读取数据片段的节点信息
-    @staticmethod
-    def pack_request_read_segment(address: str, start: int, length: int) -> bytes:
-        buffer = bytearray(1024)
-        offect = 0
-        buffer[offect] = AllenBradleyConstant.CIP_READ_FRAGMENT
-        offect += 1
-        offect += 1
-
-        request_path = AllenBradleyTools.build_request_path_command(address)
-        buffer[offect:offect + len(request_path)] = request_path
-        offect += len(request_path)
-
-        buffer[1] = (offect - 2) // 2
-        buffer[offect] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[0]
-        offect += 1
-        buffer[offect] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[1]
-        offect += 1
-        buffer[offect + 0] = IOTBaseCommon.DataTransform.pack_value(start, '<i')[0]
-        buffer[offect + 1] = IOTBaseCommon.DataTransform.pack_value(start, '<i')[1]
-        buffer[offect + 2] = IOTBaseCommon.DataTransform.pack_value(start, '<i')[2]
-        buffer[offect + 3] = IOTBaseCommon.DataTransform.pack_value(start, '<i')[3]
-        offect += 4
+            else:
+                # I0.0、V1004的情况（非PLC地址）
+                result.contents[2] = SiemensS7Tools.get_begin_address(address)
+                result.contents[4] = SiemensS7Tools.get_is_bit(address)
 
-        return buffer[0:offect]
+            result.is_success = True
+            return result
 
-    # 据指定的数据和类型，生成对应的数据
-    @staticmethod
-    def pack_request_write(request_path: bytearray, type_code: int, value: bytes, length: int = 1) -> bytes:
-        buffer = bytearray(6 + len(request_path) + len(value))
-        buffer[0] = AllenBradleyConstant.CIP_WRITE_DATA  # 写
-        buffer[1] = len(request_path) // 2
-        buffer[2: 2 + len(request_path)] = request_path
-        buffer[2 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(type_code, '<i')[0]
-        buffer[3 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(type_code, '<i')[1]
-        buffer[4 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[0]
-        buffer[5 + len(request_path)] = IOTBaseCommon.DataTransform.pack_value(length, '<i')[1]
-        buffer[6 + len(request_path): 6 + len(request_path) + len(value)] = value
-        return buffer
+        except Exception as e:
+            result.msg = e.__str__()
+            return result
 
-    # 将所有的cip指定进行打包操作
     @staticmethod
-    def pack_command_service(slot: bytearray, cips: list) -> bytes:
-        ms = bytearray(0)
-        ms.append(0xB2)     # 连接的项数
-        ms.append(0x00)
-        ms.append(0x00)     # 后面数据包的长度，等全部生成后在赋值
-        ms.append(0x00)
-
-        ms.append(0x52)     # 服务
-        ms.append(0x02)     # 请求路径大小
-        ms.append(0x20)     # 请求路径
-        ms.append(0x06)
-        ms.append(0x24)
-        ms.append(0x01)
-        ms.append(0x0A)     # 超时时间
-        ms.append(0xF0)
-        ms.append(0x00)     # CIP指令长度
-        ms.append(0x00)
-
-        count = 0
-        if len(cips) == 1:
-            ms.extend(cips[0])
-            count += len(cips[0])
-        else:
-            ms.append(0x0A)
-            ms.append(0x02)
-            ms.append(0x20)
-            ms.append(0x02)
-            ms.append(0x24)
-            ms.append(0x01)
-            count += 8
-
-            ms.extend(IOTBaseCommon.DataTransform.pack_value(len(cips), '<H'))
-            offect = 0x02 + 2 * len(cips)
-            count += 2 * len(cips)
-
-            for i in range(len(cips)):
-                ms.extend(IOTBaseCommon.DataTransform.pack_value(offect, '<H'))
-                offect = offect + len(cips[i])
-
-            for i in range(len(cips)):
-                ms.extend(cips[i])
-                count += len(cips[i])
-
-        ms.append((len(slot) + 1) // 2)
-        ms.append(0x00)
-        ms.extend(slot)
-        if len(slot) % 2 == 1:
-            ms.append(0x00)
-
-        ms[12:14] = IOTBaseCommon.DataTransform.pack_value(count, '<H')
-        ms[2:4] = IOTBaseCommon.DataTransform.pack_value(len(ms) - 4, '<H')
-        return ms
+    def get_real_command(address: Optional[list] = None):
+        """生成一个读取字数据指令头的通用方法"""
+        if address is None:
+            raise Exception(f"address is empty")
 
-    # 生成读取直接节点数据信息的内容
-    @staticmethod
-    def pack_command_specific_data(service: List[bytearray]) -> bytes:
-        buffer = bytearray(0)
-        buffer.append(0x00)
-        buffer.append(0x00)
-        buffer.append(0x00)
-        buffer.append(0x00)
-        buffer.append(0x01)  # 超时
-        buffer.append(0x00)
-        buffer.extend(IOTBaseCommon.DataTransform.pack_value(len(service), '<H'))
-        for i in range(len(service)):
-            buffer.extend(service[i])
-        return buffer
+        if len(address) > 19:
+            raise Exception("size must be less than 19")
 
-    # 从PLC反馈的数据解析
-    @staticmethod
-    def extract_actual_data(response: bytearray, is_read: bool):
-        data = bytearray()
-        offset = 38
-        has_more_data = False
-        data_type = 0
-        count = IOTBaseCommon.DataTransform.unpack_bytes(response[38:40], '<H')  # 剩余总字节长度，在剩余的字节里，有可能是一项数据，也有可能是多项
-        if IOTBaseCommon.DataTransform.unpack_bytes(response[40:44], '<i') == 0x8A:  # 多项数据
-            offset = 44
-            data_count = IOTBaseCommon.DataTransform.unpack_bytes(response[offset:offset + 2], '<H')
-            for i in range(data_count):
-                offset_start = IOTBaseCommon.DataTransform.unpack_bytes(response[offset + 2 + i * 2: offset + 4 + i * 2], '<H')
-                if i == data_count - 1:
-                    offset_end = len(response)
+        read_count = len(address)
+        command = bytearray(19 + read_count * 12)
+        # ======================================================================================
+        command[0] = 0x03  # 固定报文头
+        command[1] = 0x00  # 固定报文头
+        command[2] = len(command) // 256  # 长度 向下取整
+        command[3] = len(command) % 256  # 整个读取请求长度为0x1F = 31
+        command[4] = 0x02  # 固定
+        command[5] = 0xF0
+        command[6] = 0x80  # COTP
+        command[7] = 0x32  # 协议标识 协议ID
+        command[8] = 0x01  # 1 客户端发送命令 3 服务器回复命令
+        command[9] = 0x00  # 冗余标识 (reserved): 0x0000;
+        command[10] = 0x00  # 协议数据单元参考； 它由请求事件增加；
+        command[11] = 0x00
+        command[12] = 0x01  # [11][12] 两个字节，标识序列号，回复报文相同位置和这个完全一样；范围是0~65535
+        command[13] = (len(command) - 17) // 256
+        command[14] = (len(command) - 17) % 256  # parameter length（减17是因为从[17] 到最后属于parameter）
+        command[15] = 0x00  # 读取内部数据时为00，读取CPU型号为Data数据长度
+        command[16] = 0x00
+        # =====================================================================================
+        command[17] = 0x04  # 读写指令，04读，05写
+        command[18] = read_count  # 读取数据块个数
+
+        for i, adr in enumerate(address):
+            # ===========================================================================================
+            # 指定有效值类型
+            command[19 + i * 12] = 0x12
+            # 接下来本次地址访问长度
+            command[20 + i * 12] = 0x0A
+            # 语法标记，ANY
+            command[21 + i * 12] = 0x10
+            # 按字为单位
+            command[22 + i * 12] = 0x01 if adr.contents[4] else 0x02
+            # 访问数据的个数
+            command[23 + i * 12] = adr.contents[5] // 256
+            command[24 + i * 12] = adr.contents[5] % 256
+            # DB块编号，如果访问的是DB块的话
+            command[25 + i * 12] = adr.contents[3] // 256
+            command[26 + i * 12] = adr.contents[3] % 256
+            # 访问数据类型
+            command[27 + i * 12] = adr.contents[1]
+            # 偏移位置
+            command[28 + i * 12] = adr.contents[2] // 256 // 256 % 256
+            command[29 + i * 12] = adr.contents[2] // 256 % 256
+            command[30 + i * 12] = adr.contents[2] % 256
+
+        return IOTBaseCommon.IOTNetResult.create_success([command])
+
+    @staticmethod
+    def get_write_command(address: Optional[list] = None):
+        write_length = 0
+        for i, add in enumerate(address):
+            write_length = write_length + (2 if len(add.contents[8]) == 1 else len(add.contents[8]))
+            if i == len(address) - 1 and len(add.contents[8]) == 1:
+                write_length = write_length - 1
+
+        # 前19个固定的、16为Item长度、writes.Length为Imte的个数
+        command = bytearray(19 + len(address) * 16 + write_length)
+        command[0] = 0x03
+        command[1] = 0x00  # [0][1] 固定报文头
+        command[2] = len(command) // 256
+        command[3] = len(command) % 256  # [2][3] 整个读取请求长度为0x1F = 31
+        command[4] = 0x02
+        command[5] = 0xF0
+        command[6] = 0x80  # COTP
+        command[7] = 0x32  # 协议ID
+        command[8] = 0x01  # 1 客户端发送命令 3 服务器回复命令
+        command[9] = 0x00
+        command[10] = 0x00  # [4] - [10] 固定6个字节
+        command[11] = 0x00
+        command[12] = 0x01  # [11][12] 两个字节，标识序列号，回复报文相同位置和这个完全一样；范围是0~65535
+        command[13] = (12 * len(address) + 2) // 256
+        command[14] = (12 * len(address) + 2) % 256  # parameter length（减17是因为从[17] 到最后属于parameter）
+        command[15] = (write_length + 4 * len(address)) // 256
+        command[16] = (write_length + 4 * len(address)) % 256  # data length
+        command[17] = 0x05  # 04读 05写
+        command[18] = len(address)  # 读取数据块个数
+        for i, data in enumerate(address):
+            command[19 + i * 12] = 0x12
+            command[20 + i * 12] = 0x0A
+            command[21 + i * 12] = 0x10
+            command[22 + i * 12] = 0x01 if data.contents[4] else 0x02
+            command[23 + i * 12] = len(data.contents[8]) // 256
+            command[24 + i * 12] = len(data.contents[8]) % 256  # 写入数据个数
+            command[25 + i * 12] = data.contents[3] // 256
+            command[26 + i * 12] = data.contents[3] % 256  # [25][26] DB块的编号
+            command[27 + i * 12] = data.contents[1]  # 访问数据块的类型
+            command[28 + i * 12] = data.contents[2] // 256 // 256 % 256
+            command[29 + i * 12] = data.contents[2] // 256 % 256
+            command[30 + i * 12] = data.contents[2] % 256  # [28][29][30] 访问DB块的偏移量
+
+        index = 18 + len(address) * 12
+        for i, data in enumerate(address):
+            coefficient = 1 if data.contents[4] else 8
+            command[1 + index] = 0x00
+            command[2 + index] = 0x03 if data.contents[4] else 0x04
+            command[3 + index] = len(data.contents[8]) * coefficient // 256
+            command[4 + index] = len(data.contents[8]) * coefficient % 256  # 按位计算出的长度
+
+            if len(data.contents[8]) == 1:
+                if data.contents[4]:
+                    command[5 + index] = 0x01 if data.contents[8][0] == 0x01 else 0x00
                 else:
-                    offset_end = IOTBaseCommon.DataTransform.unpack_bytes(response[offset + 2 + i * 2: offset + 4 + i * 2], '<H')
-
-                err = IOTBaseCommon.DataTransform.unpack_bytes(response[offset_start + 2: offset_start + 4], '<H')
-                if err in [0x04, 0x05, 0x0A, 0x13, 0x1C, 0x1E, 0x26]:
-                    return IOTBaseCommon.IOTNetResult(code=err, msg=AllenBradleyTools.get_status_description(err))
-                elif err == 0x06:
-                    if response[offset + 2] == 0xD2 or response[offset + 2] == 0xCC:
-                        return IOTBaseCommon.IOTNetResult(code=err, msg=AllenBradleyTools.get_status_description(err))
-                elif err == 0x00:
-                    pass
+                    command[5 + index] = data.contents[8][0]
+                if i >= len(address) - 1:
+                    index = index + (4 + 1)
                 else:
-                    return IOTBaseCommon.IOTNetResult(code=err, msg=AllenBradleyTools.get_status_description(err))
-
-                if is_read is True:
-                    for j in range(offset_start + 6, offset_end, 1):
-                        data.append(response[j])
-        else:   # 单项数据
-            err = response[offset + 4]
-            if err in [0x04, 0x05, 0x0A, 0x13, 0x1C, 0x1E, 0x26]:
-                return IOTBaseCommon.IOTNetResult(code=err, msg=AllenBradleyTools.get_status_description(err))
-            elif err == 0x06:
-                has_more_data = True
-
-            elif err == 0x00:
-                if response[offset + 2] == 0xCD or response[offset + 2] == 0xD3:    # 写服务应答为0xD3
-                    return IOTBaseCommon.IOTNetResult.create_success([data, data_type, has_more_data])
-                if response[offset + 2] == 0xCC or response[offset + 2] == 0xD2:    # 0xD2为读取数据标签应答
-                    for i in range(offset + 8, offset + 2 + count, 1):
-                        data.append(response[i])
-                    data_type = IOTBaseCommon.DataTransform.unpack_bytes(response[offset + 6:offset + 8], '<H')
-                elif response[offset + 2] == 0xD5:
-                    for i in range(offset + 6, offset + 2 + count, 1):
-                        data.append(response[i])
+                    index = index + (4 + 2)  # fill byte  （如果不是最后一个bit，则需要填充一个空数据）
             else:
-                return IOTBaseCommon.IOTNetResult(code=err, msg=AllenBradleyTools.get_status_description(err))
-        return IOTBaseCommon.IOTNetResult.create_success([data, data_type, has_more_data])
-
-    @staticmethod
-    def get_status_description(err):
-        """获取错误信息的字符串描述文本"""
-        if err == 0:
-            return f"Communication is normal."
-        elif err == 1:
-            return f"The message header is not fins"
-        elif err == 2:
-            return f"Data length too long"
-        elif err == 3:
-            return f"This command does not support"
-        elif err == 20:
-            return f"Exceeding connection limit"
-        elif err == 21:
-            return f"The specified node is already in the connection"
-        elif err == 22:
-            return f"Attempt to connect to a protected network node that is not yet configured in the PLC"
-        elif err == 23:
-            return f"The current client's network node exceeds the normal range"
-        elif err == 24:
-            return f"The current client's network node is already in use"
-        elif err == 25:
-            return f"All network nodes are already in use"
-        else:
-            return f"Unknown Error"
-
-    @staticmethod
-    def get_session_status_description(status: int) -> str:
-        """获取错误信息的字符串描述文本"""
-        if status == 0x01:
-            return f"The sender issued an invalid or unsupported encapsulation command."
-        elif status == 0x02:
-            return f"Insufficient memory resources in the receiver to handle the command. This is not an application error. Instead, it only results if the encapsulation layer cannot obtain memory resources that it need."
-        elif status == 0x03:
-            return f"Poorly formed or incorrect data in the data portion of the encapsulation message."
-        elif status == 0x64:
-            return f"An originator used an invalid session handle when sending an encapsulation message."
-        elif status == 0x65:
-            return f"The target received a message of invalid length."
-        elif status == 0x69:
-            return f"Unsupported encapsulation protocol revision."
-        else:
-            return f"Unknown"
-
+                command[5 + index: 5 + index + len(data.contents[8])] = data.contents[8]
+                index = index + 4 + len(data.contents[8])
+        return IOTBaseCommon.IOTNetResult.create_success([command])
 
-class AllenBradleyClient(IOTBaseCommon.IOTNetworkDeviceClient):
 
-    def __init__(self, host: str, port: int, slot: int = 0, timeout: int = 10):
+class SiemensS7Client(IOTBaseCommon.IOTNetworkDeviceClient):
+ 
+    def __init__(self, version: SiemensS7Version, host: str, port: int, slot: int = 0, rack: int = 0, timeout: int = 10):
         super().__init__(host, port, timeout)
-
-        self.slot = slot  # 插槽
-        self.cip_command = 0x6F  # 实际的命令暗号
-        self.session_handle = 0  # 当前会话的id
+        self.version = version
+        self.word_length = 2
+        self.slot = slot
+        self.rack = rack
 
     def get_net_msg(self):
-        return AllenBradleyMessage()
-
-    def pack_command_with_header(self, command: bytearray):
-        return AllenBradleyTools.pack_request_header(self.cip_command, self.session_handle, command)
-
-    def register_session_handle(self):
-        """
-            向PLC注册会话ID的报文(协议版本（0x0001) 选项标记（0x0000))
-            65 00 04 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 01 00 00 00
-        """
-        return AllenBradleyTools.pack_request_header(0x65, 0, bytearray([0x01, 0x00, 0x00, 0x00]))
-
-    def unregister_session_handle(self):
-        """
-            获取卸载一个已注册的会话的报文
-            66 00 04 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 01 00 00 00
-        """
-        return AllenBradleyTools.pack_request_header(0x66, self.session_handle, bytearray(0))
-
-    def check_response(self, response: bytes):
-        try:
-            status = IOTBaseCommon.DataTransform.convert_value(response[8:12], IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, IOTBaseCommon.DataTransform.TypeFormat.INT32, pos=0)
-            if status == 0:
-                return IOTBaseCommon.IOTNetResult.create_success()
-            return IOTBaseCommon.IOTNetResult(msg=AllenBradleyTools.get_session_status_description(status))
-        except Exception as ex:
-            return IOTBaseCommon.IOTNetResult(msg=str(ex))
-
+        return SiemensS7Message()
+    
     def initialization_on_connect(self, socket):
-        """在连接上PLC后，需要进行一步握手协议"""
-        # 握手信号
-        read = self.read_from_socket(socket, self.register_session_handle(), has_response=True, pack_unpack=False)
-        if read.is_success is False:
-            return read
-
-        # 检查返回的状态
-        check = self.check_response(read.contents[0])
-        if check.is_success is False:
-            return check
-
-        self.session_handle = IOTBaseCommon.DataTransform.unpack_bytes(read.contents[0][4:8], '<I')
+        """连接上服务器后需要进行的二次握手操作"""
+        head1, head2 = self.init_head()
+        
+        # 第一次握手
+        read_first = self.read_from_socket(socket, head1)
+        if read_first.is_success is False: 
+            return read_first
+
+        # 第二次握手
+        read_second = self.read_from_socket(socket, head2)
+        if read_second.is_success is False: 
+            return read_second
 
         # 返回成功的信号
         return IOTBaseCommon.IOTNetResult.create_success()
 
     def extra_on_disconnect(self, socket):
-        read = self.read_from_socket(socket, self.unregister_session_handle(), has_response=True, pack_unpack=False)
-        if read.is_success is False:
-            return read
-
         return IOTBaseCommon.IOTNetResult.create_success()
 
+    def init_head(self):
+        head1 = SiemensS7Constant.Head1
+        head2 = SiemensS7Constant.Head2
+        if self.version == SiemensS7Version.S7_200.value:  # 0, 1
+            head1 = SiemensS7Constant.Head1_200
+            head2 = SiemensS7Constant.Head2_200
+        elif self.version == SiemensS7Version.S7_200Smart.value:  #
+            head1 = SiemensS7Constant.Head1_200Smart
+            head2 = SiemensS7Constant.Head2_200Smart
+        elif self.version == SiemensS7Version.S7_300.value:   # 0, 2
+            head1[21] = self.rack * 0x20 + self.slot
+        elif self.version == SiemensS7Version.S7_400.value:  # 具体看硬件组态
+            head1[21] = self.rack * 0x20 + self.slot
+            head1[17] = 0
+        elif self.version == SiemensS7Version.S7_1200.value:   # 0, 0/1
+            head1[21] = self.rack * 0x20 + self.slot
+        elif self.version == SiemensS7Version.S7_1500.value:   # 0, 0/1
+            head1[21] = self.rack * 0x20 + self.slot
+        else:
+            head1[18] = 0
+
+        return head1, head2
+
     def read(self, address: Union[tuple, list]):
-        """从PLC读取数据"""
+        """从PLC读取数据，地址格式为I100，Q100，DB20.100，M100，T100，C100以字节为单位"""
         if isinstance(address, list):
             results = []
             for (adr, type) in address:
-                tmp = AllenBradleyTools.parse_address(adr, type)
+                tmp = SiemensS7Tools.parse_address(adr, type)
                 if tmp.is_success is False:
                     return IOTBaseCommon.IOTNetResult.create_fail(tmp)
                 results.append(tmp)
             return self._read(results)
         elif isinstance(address, tuple):
-            result = AllenBradleyTools.parse_address(address[0], address[1])
+            result = SiemensS7Tools.parse_address(address[0], address[1])
             if result.is_success is False:
                 return IOTBaseCommon.IOTNetResult.create_fail(result)
             return self._read([result])
 
     def write(self, address: Union[tuple, list]):
         """将数据写入到PLC数据，地址格式为I100，Q100，DB20.100，M100，以字节为单位"""
         if isinstance(address, list):
             results = []
             for (adr, type, value) in address:
-                tmp = AllenBradleyTools.parse_address(adr, type)
+                tmp = SiemensS7Tools.parse_address(adr, type)
                 if tmp.is_success is False:
                     return IOTBaseCommon.IOTNetResult.create_fail(tmp)
-                tmp.contents[8] = IOTBaseCommon.DataTransform.convert_value(value, IOTBaseCommon.DataTransform.TypeFormat(type), IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, format=IOTBaseCommon.DataTransform.DataFormat.ABCD)
+                tmp.contents[8] = IOTBaseCommon.DataTransform.convert_value(value, IOTBaseCommon.DataTransform.TypeFormat(type), IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, format=IOTBaseCommon.DataTransform.DataFormat.DCBA)
                 results.append(tmp)
             return self._write(results)
         elif isinstance(address, tuple):
-            result = AllenBradleyTools.parse_address(address[0], address[1])
+            result = SiemensS7Tools.parse_address(address[0], address[1])
             if result.is_success is False:
                 return IOTBaseCommon.IOTNetResult.create_fail(result)
-            result.contents[8] = IOTBaseCommon.DataTransform.convert_value(address[2], IOTBaseCommon.DataTransform.TypeFormat(address[1]), IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, format=IOTBaseCommon.DataTransform.DataFormat.ABCD)
+            result.contents[8] = IOTBaseCommon.DataTransform.convert_value(address[2], IOTBaseCommon.DataTransform.TypeFormat(address[1]), IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, format=IOTBaseCommon.DataTransform.DataFormat.DCBA)
             return self._write([result])
 
     def ping(self):
         return self.get_socket().is_success
 
-    def get_real_command(self, address: Optional[IOTBaseCommon.IOTNetResult]):
-        try:
-            command_specific_data = AllenBradleyTools.pack_command_specific_data([bytearray(4), AllenBradleyTools.pack_command_service(self.slot if self.slot is None else bytearray([0x01, self.slot]), [AllenBradleyTools.pack_requset_read(address.contents[1], address.contents[4])])])
-            return IOTBaseCommon.IOTNetResult.create_success([command_specific_data])
-        except Exception as e:
-            return IOTBaseCommon.IOTNetResult(code=10000, msg=f"{e.__str__()}")
+    def _read(self, address: list):
+        """基础的读取方法，外界不应该调用本方法"""
+        command = SiemensS7Tools.get_real_command(address)
+        if command.is_success is False:
+            return command
 
-    def get_write_command(self, address: Optional[IOTBaseCommon.IOTNetResult]):
-        try:
-            cip = AllenBradleyTools.pack_request_write(address.contents[1], address.contents[3], address.contents[8])
-            command_specific_data = AllenBradleyTools.pack_command_specific_data([bytearray(4), AllenBradleyTools.pack_command_service(self.slot if self.slot is None else bytearray([0x01, self.slot]), [cip])])
-            return IOTBaseCommon.IOTNetResult.create_success([command_specific_data])
-        except Exception as e:
-            return IOTBaseCommon.IOTNetResult(code=10000, msg=f"{e.__str__()}")
+        read = self.read_server(command.contents[0])
+        if read.is_success is False:
+            return read
 
-    def get_command(self, address: Optional[IOTBaseCommon.IOTNetResult] = None, is_read: bool = True):
-        """生成一个读取字数据指令头的通用方法"""
-        return self.get_real_command(address) if is_read else self.get_write_command(address)
+        length = len(read.contents[0]) - 21
+        response_data = bytearray(length)
+        response_data[0: length] = read.contents[0][21: 21 + length]
+        cursor = 0
+
+        for i, adr in enumerate(address):
+            adr.contents[9] = True
+            if (response_data[cursor] == 0x0A and response_data[cursor+1] == 0x00) or (response_data[cursor] == 0x05 and response_data[cursor+1] == 0x00):
+                adr.contents[9] = False
+                adr.contents[10] = f"读取{adr.contents[0]}失败，请确认是否存在该地址"
+            elif response_data[cursor] != 0xFF:
+                adr.contents[9] = False
+                adr.contents[10] = f"读取{adr.contents[0]}失败，异常代码: {response_data[cursor]}"
 
-    def _read(self, addresss: list):
-        """基础的读取方法，外界不应该调用本方法"""
-        for address in addresss:
-            command = self.get_command(address)
-            if command.is_success is False:
-                address.contents[9] = False
-                address.contents[10] = command.msg
+            cursor += 4
+            if adr.contents[9] is False:
                 continue
 
-            # 核心数据交互
-            read = self.read_server(command.contents[0])
-            if read.is_success is False:
-                address.contents[9] = False
-                address.contents[10] = read.msg
-                continue
+            read_result = response_data[cursor: cursor + adr.contents[5]]
+            cursor += 2 if adr.contents[5] == 1 else adr.contents[5]
+            adr.contents[8] = IOTBaseCommon.DataTransform.convert_value(read_result, None, IOTBaseCommon.DataTransform.TypeFormat(adr.contents[6]), format=IOTBaseCommon.DataTransform.DataFormat.DCBA)[0]
 
-            # 数据有效性分析
-            valid = self.check_response(read.contents[0])
-            if valid.is_success is False:
-                address.contents[9] = False
-                address.contents[10] = valid.msg
-                continue
+        return IOTBaseCommon.IOTNetResult.create_success(address)
 
-            # 提取数据 -> Extracting data
-            extract = AllenBradleyTools.extract_actual_data(read.contents[0], True)
-            if extract.is_success is True:
-                length, type_fmt = IOTBaseCommon.DataTransform.get_type_size_fmt(IOTBaseCommon.DataTransform.TypeFormat(address.contents[2]))
-                response_data = bytearray(length)
-                response_data[0: length] = extract.contents[0][0: length]
-                address.contents[9] = True
-                address.contents[8] = IOTBaseCommon.DataTransform.convert_value(response_data, IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, IOTBaseCommon.DataTransform.TypeFormat(address.contents[2]), format=IOTBaseCommon.DataTransform.DataFormat.ABCD, pos=0)
+    def _write(self, address: list):
+        """基础的写入数据的操作支持"""
+        command = SiemensS7Tools.get_write_command(address)
+        if command.is_success is False:
+            return command
+
+        write = self.read_server(command.contents[0])
+        if write.is_success is False:
+            return write
+
+        response_data = write.contents[0]
+        for i, adr in enumerate(address):
+            offset = 21 + i
+            adr.contents[9] = False
+            adr.contents[10] = f"UnResponse"
+            if offset <= len(response_data) - 1:
+                if response_data[offset] == 0x0A or response_data[offset] == 0x05:
+                    adr.contents[9] = False
+                    adr.contents[10] = f"读取{adr.contents[0]}失败，请确认是否存在该地址"
+                elif response_data[offset] != 0xFF:
+                    adr.contents[9] = False
+                    adr.contents[10] = f"读取{adr.contents[0]}失败，异常代码: {response_data[offset]}"
+                else:
+                    adr.contents[9] = True
+        return IOTBaseCommon.IOTNetResult.create_success(address)
 
-        return IOTBaseCommon.IOTNetResult.create_success(addresss)
 
-    def _write(self, addresss: list):
-        """基础的写入数据的操作支持"""
-        for address in addresss:
-            command = self.get_command(address, False)
-            if command.is_success is False:
-                address.contents[9] = False
-                address.contents[10] = command.msg
-                continue
+class SiemensS7Server(IOTBaseCommon.IOTNetworkDeviceServer):
 
-            # 核心数据交互
-            read = self.read_server(command.contents[0])
-            if read.is_success is False:
-                address.contents[9] = False
-                address.contents[10] = read.msg
-                continue
+    def __init__(self, version: SiemensS7Version, host: str, port: int, slot: int = 0, rack: int = 0, timeout: int = 10):
+        super().__init__(host, port, timeout)
+        self.version = version
+        self.word_length = 2
+        self.slot = slot
+        self.rack = rack
 
-            # 数据有效性分析
-            valid = self.check_response(read.contents[0])
-            if valid.is_success is False:
-                address.contents[9] = False
-                address.contents[10] = valid.msg
-                continue
+    def get_net_msg(self):
+        return SiemensS7Message()
+
+    def initialization_on_connect(self, socket):
+        # 返回成功的信号
+        return IOTBaseCommon.IOTNetResult.create_success()
 
-            # 提取数据 -> Extracting data
-            extract = AllenBradleyTools.extract_actual_data(read.contents[0], False)
-            if extract.is_success is True:
-                address.contents[9] = True
+    def extra_on_disconnect(self, socket):
+        return IOTBaseCommon.IOTNetResult.create_success()
+
+    def extra_on_receive(self, socket, datas: bytes):
+        if datas[3] == len(SiemensS7Constant.Head1_200Smart) or datas[3] == len(SiemensS7Constant.Head2_200Smart):
+            self.send(socket, datas)
+        else:
+            self._analyze_data(datas, socket)
+
+    def simulate(self, address: Union[tuple, list]):
+        """将数据写入到PLC数据，地址格式为I100，Q100，DB20.100，M100，以字节为单位"""
+        if isinstance(address, list):
+            results = []
+            for (adr, type, value) in address:
+                tmp = SiemensS7Tools.parse_address(adr, type)
+                if tmp.is_success is False:
+                    return IOTBaseCommon.IOTNetResult.create_fail(tmp)
+                tmp.contents[8] = IOTBaseCommon.DataTransform.convert_value(value, IOTBaseCommon.DataTransform.TypeFormat(type), IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, format=IOTBaseCommon.DataTransform.DataFormat.DCBA)
+                results.append(tmp)
+            return self._simulate(results)
+        elif isinstance(address, tuple):
+            result = SiemensS7Tools.parse_address(address[0], address[1])
+            if result.is_success is False:
+                return IOTBaseCommon.IOTNetResult.create_fail(result)
+            result.contents[8] = IOTBaseCommon.DataTransform.convert_value(address[2], IOTBaseCommon.DataTransform.TypeFormat(address[1]), IOTBaseCommon.DataTransform.TypeFormat.BYTE_ARRAY, format=IOTBaseCommon.DataTransform.DataFormat.DCBA)
+            return self._simulate([result])
 
-        return IOTBaseCommon.IOTNetResult.create_success(addresss)
+    def _simulate(self, address: list):
+        """基础的写入数据的操作支持"""
+        command = SiemensS7Tools.get_write_command(address)
+        if command.is_success is True:
+            self._analyze_data(command.contents[0])
+    
+    def _analyze_data(self, datas: bytes, socket=None):
+        if len(datas) > 21:
+            if datas[17] == 4:  # 读
+                db_size = datas[18]  # 数据块个数
+                read_length = 0  # 读取数据总长度
+                for i in range(db_size):
+                    byte_length = datas[23 + i * 12] * 256 + datas[24 + i * 12]  # 访问数据的个数，以byte为单位
+                    if byte_length == 1 and i < db_size - 1:  # 非最后一个bit/byte，需要补全
+                        byte_length += 1
+                    read_length += byte_length
+    
+                data_content = bytearray(4 * db_size + read_length)  # 数据报文总长度
+                cursor = 0
+                for i in range(db_size):
+                    begin_address = datas[28 + i * 12] * 256 * 256 + datas[29 + i * 12] * 256 + datas[30 + i * 12]  # DB块的偏移量
+                    byte_length = datas[23 + i * 12] * 256 + datas[24 + i * 12]  # 访问数据的个数
+                    if byte_length == 1 and i < db_size - 1:  # 非最后一个bit/byte，需要补全
+                        byte_length += 1
+                    is_bit = datas[22 + i * 12] == 0x01  # 是否是bit类型
+                    db_type = datas[27 + i * 12]
+                    data_key = f"s200-{db_type}"
+                    if data_key not in self.values.keys():
+                        self.values[data_key] = bytearray(65536)
+                    db_byte_array = self.values.get(data_key)
+                    data_content[0 + cursor] = 0xFF
+                    data_content[1 + cursor] = 0x03 if is_bit else 0x04  # 04 byte(字节) 03 bit（位）
+                    data_content[2 + cursor] = byte_length // 256  # 后半截数据数的Length
+                    data_content[3 + cursor] = byte_length % 256  # 后半截数据数的Length
+                    pos = begin_address // 8
+                    if is_bit:  # 按bit
+                        data_content[4 + cursor] = IOTBaseCommon.DataTransform.get_bool(db_byte_array[pos], begin_address % 8)
+                    else:
+                        data_content[4 + cursor: 4 + cursor + byte_length] = db_byte_array[pos: pos + byte_length]
+                    cursor += 4 + byte_length
+    
+                if socket:
+                    response = bytearray(21 + len(data_content))
+                    response[0:21] = bytes.fromhex("03 00 00 1A 02 F0 80 32 03 00 00 00 01 00 02 00 00 00 00 04 01")
+                    response[8] = 0x03  # 1 客户端发送命令 3 服务器回复命令
+                    response[2] = len(response) // 256  # 返回数据长度
+                    response[3] = len(response) % 256
+                    response[15] = len(response) // 256  # 读取数据长度
+                    response[16] = len(response) % 256
+                    response[20] = datas[18]  # 读取数据块个数
+                    response[21:] = data_content[:]
+                    self.send(socket, response)
+            elif datas[17] == 5:  # 写
+                writes_length = datas[18]  # 写如数据的个数
+                cursor = 0
+                for i in range(writes_length):
+                    begin_address = datas[28 + i * 12] * 256 * 256 + datas[29 + i * 12] * 256 + datas[30 + i * 12]  # DB块的偏移量
+                    db_type = datas[27 + i * 12]
+                    data_key = f"s200-{db_type}"
+                    if data_key not in self.values.keys():
+                        self.values[data_key] = bytearray(65536)
+                    data_before_index = 18 + writes_length * 12  # Data之前的下标
+                    is_bit = datas[data_before_index + 4 * (i + 1) - 2 + cursor] == 0x03  # [2 + index]是否是bit类型
+                    coefficient = 1 if is_bit else 8
+                    write_value = bytearray(datas[data_before_index + 4 * (i + 1) + cursor] // coefficient)  # 初始化要写入的字节数组长度
+                    requet_begin_location = data_before_index + 4 * (i + 1) + cursor + 1  # 开始写入的地址（报文中的数据的位置）
+    
+                    if len(write_value) == 1 and i < writes_length - 1:
+                        cursor = cursor + 1
+                    cursor += len(write_value)
+    
+                    write_value[:len(write_value)] = datas[requet_begin_location: requet_begin_location + len(write_value)]
+                    db_byte_array = self.values.get(data_key)
+    
+                    pos = begin_address // 8
+                    if is_bit:  # 按bit
+                        db_byte_array[pos] = IOTBaseCommon.DataTransform.set_bool(db_byte_array[pos], begin_address % 8, write_value[0])
+                    else:
+                        db_byte_array[pos: pos + len(write_value)] = write_value
+    
+                    self.values[data_key] = db_byte_array
+                
+                if socket:
+                    response = bytearray(21)
+                    response[0:22] = bytes.fromhex("03 00 00 16 02 F0 80 32 03 00 00 00 01 00 02 00 01 00 00 05 01")
+                    response[21: 21 + writes_length] = bytes([0xFF] * writes_length)
+                    self.send(socket, response)
 
 
-class IOTPlcAllenBradley(IOTDriver):
+class IOTPlcSiemensS7(IOTDriver):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.reinit()
 
     def reinit(self):
         self.exit_flag = False
         self.clients = {}
+        self.servers = {}
+        self.plc_objects = {}
 
     def exit(self):
         self.exit_flag = True
+        for port, server in self.servers.items():
+            self._release_server(port)
+
         address = list(self.clients.keys())
         for address in address:
             if address in self.clients.keys():
                 self._release_client(address)
 
         self.reinit()
 
     @classmethod
     def template(cls, mode: int, type: str, lan: str) -> List[Dict[str, Any]]:
         templates = []
         if type == 'point':
             templates.extend([
-                                {'required': True, 'name': '是否可写' if lan == 'ch' else 'writable'.upper(), 'code': 'point_writable', 'type': 'bool', 'default': 'TRUE', 'enum': [], 'tip': ''},
-                                {'required': True, 'name': '物理点名' if lan == 'ch' else 'name'.upper(), 'code': 'point_name', 'type': 'string', 'default': 'Chiller_1_CHW_ENT', 'enum': [], 'tip': ''}
-                                ])
+                {'required': True, 'name': '是否可写' if lan == 'ch' else 'writable'.upper(), 'code': 'point_writable', 'type': 'bool', 'default': 'TRUE', 'enum': [], 'tip': ''},
+                {'required': True, 'name': '物理点名' if lan == 'ch' else 'name'.upper(), 'code': 'point_name', 'type': 'string', 'default': 'Chiller_1_CHW_ENT', 'enum': [], 'tip': ''}])
             if mode == 0:
-                templates.append({'required': True, 'name': '设备地址' if lan == 'ch' else 'device address'.upper(), 'code': 'point_device_address', 'type': 'string', 'default': '192.168.1.184/44818/0', 'enum': [], 'tip': ''})
+                templates.append({'required': True, 'name': '设备地址' if lan == 'ch' else 'device address'.upper(), 'code': 'point_device_address', 'type': 'string', 'default': '192.168.1.184/102/0/1', 'enum': [], 'tip': ''})
             else:
-                templates.append({'required': True, 'name': '设备地址' if lan == 'ch' else 'device address'.upper(), 'code': 'point_device_address', 'type': 'string', 'default': '0.0.0.0/44818/0', 'enum': [], 'tip': ''})
+                templates.append({'required': True, 'name': '设备地址' if lan == 'ch' else 'device address'.upper(), 'code': 'point_device_address', 'type': 'string', 'default': '0.0.0.0/102/0/1', 'enum': [], 'tip': ''})
             templates.extend([
                 {'required': True, 'name': '点地址' if lan == 'ch' else 'address'.upper(), 'code': 'point_address', 'type': 'string', 'default': 'DB3,REAL4', 'enum': [], 'tip': ''},
                 {'required': True, 'name': '点类型' if lan == 'ch' else 'address'.upper(), 'code': 'point_type', 'type': 'int', 'default': 1, 'enum': [], 'tip': ''},
                 {'required': False, 'name': '点描述' if lan == 'ch' else 'description'.upper(), 'code': 'point_description', 'type': 'string', 'default': 'Chiller_1_CHW_ENT', 'enum': [], 'tip': ''}
-            ])
+                ])
             if mode == 0:
                 templates.extend([{'required': False, 'name': '逻辑点名' if lan == 'ch' else 'name alias'.upper(), 'code': 'point_name_alias', 'type': 'string', 'default': 'Chiller_1_CHW_ENT1', 'enum': [], 'tip': ''}])
             else:
-                templates.append(
-                    {'required': True, 'name': '点值' if lan == 'ch' else 'value'.upper(), 'code': 'point_value', 'type': 'int', 'default': 0, 'enum': [], 'tip': ''})
+                templates.append({'required': True, 'name': '点值' if lan == 'ch' else 'value'.upper(), 'code': 'point_value', 'type': 'int', 'default': 0, 'enum': [], 'tip': ''})
             templates.extend([
                 {'required': True, 'name': '是否启用' if lan == 'ch' else 'enable'.upper(), 'code': 'point_enabled', 'type': 'bool', 'default': 'TRUE', 'enum': [], 'tip': ''},
                 {'required': True, 'name': '倍率' if lan == 'ch' else 'scale'.upper(), 'code': 'point_scale', 'type': 'string', 'default': '1', 'enum': [], 'tip': ''}
             ])
 
         elif type == 'config':
             if mode == 0:
                 templates.extend([
-                    {'required': True, 'name': '批量读取个数' if lan == 'ch' else 'Multi Read', 'code': 'multi_read', 'type': 'int', 'default': 100, 'enum': [], 'tip': ''},
-                    {'required': True, 'name': '命令间隔(s)' if lan == 'ch' else 'Cmd Interval(s)', 'code': 'cmd_interval', 'type': 'float', 'default': 0.3, 'enum': [], 'tip': ''},
+                    {'required': True, 'name': '批量读取个数' if lan == 'ch' else 'Multi Read', 'code': 'multi_read', 'type': 'int', 'default': 19, 'enum': [], 'tip': ''},
+                    {'required': True, 'name': '命令间隔(s)' if lan == 'ch' else 'Cmd Interval(s)', 'code': 'cmd_interval', 'type': 'float', 'default': 0.1, 'enum': [], 'tip': ''},
                 ])
             templates.append({'required': True, 'name': '超时(s)' if lan == 'ch' else 'Timeout(s)', 'code': 'timeout', 'type': 'int', 'default': 15, 'enum': [], 'tip': ''})
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
+        results = {}
         names = kwargs.get('names', list(self.points.keys()))
         self.update_results(names, True, None)
 
         read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
@@ -734,22 +725,48 @@
         self.update_info(used=IOTBaseCommon.get_datetime_str())
         if kwargs.get('address') is not None:
             if self._get_client(kwargs.get('address')) is not None:
                 return self._get_client(kwargs.get('address')).ping()
             return False
         return True
 
+    def simulate(self, **kwargs):
+        self.update_info(used=IOTBaseCommon.get_datetime_str())
+        points = kwargs.get('points', {})
+        self.logging(content=f"simulate({len(points)})")
+        server_objects = {}
+        for name, point in points.items():
+            point = points.get(name)
+            if point:
+                device_address = point.get('point_device_address')
+                address = point.get('point_address')
+                type = point.get('point_type')
+                value = point.get('point_value')
+                if device_address is not None and address is not None and type is not None:
+                    if device_address not in server_objects.keys():
+                        server_objects[device_address] = []
+                    if (address, type, value) not in server_objects[device_address]:
+                        server_objects[device_address].append((address, type, value))
+
+        if len(server_objects) > 0:
+            for address, objects in server_objects.items():
+                if self._get_server(address) is not None:
+                    self._refresh_objects(address, objects)
+
+    def _gen_key(self, area, db: int, start: int, length: int) -> str:
+        return f"{area}_{db}_{start}_{length}"
+
     def _get_address_info(self, device_address: str) -> dict:
-        # ip/port/slot
+        # version/ip/port/rack/slot
         info_list = device_address.split('/')
-        return {'host': info_list[0] if len(info_list) > 1 else '', 'port': int(float(info_list[1])) if len(info_list) > 2 else 44818, 'slot': int(float(info_list[2])) if len(info_list) > 3 else 0}
+        return {'host': info_list[1] if len(info_list) > 1 else '', 'port': int(float(info_list[2])) if len(info_list) > 2 else 102, 'rack': int(float(info_list[3])) if len(info_list) > 3 else 0, 'slot': int(float(info_list[4])) if len(info_list) > 4 else 1, 'type': int(float(info_list[0])) if len(info_list) > 1 else 1}
 
     def _release_client(self, address: str):
-        client = self.clients.get(address)
         try:
+            client = self.clients.get(address)
             if client:
                 client.exit()
         except Exception as e:
             pass
         finally:
             if address in self.clients.keys():
                 del self.clients[address]
@@ -758,59 +775,59 @@
         client = self.clients.get(address)
         if client is not None and client.get_connected() is False:
             self._release_client(address)
             client = None
 
         if client is None:
             info = self._get_address_info(address)
-            if len(info) > 0:
-                client = AllenBradleyClient(info['host'], info['port'], info['slot'], self.configs.get('timeout'))
+            if 'type' in info.keys():
+                client = SiemensS7Client(SiemensS7Version(info['type']), info['host'], info['port'], info['rack'], info['slot'], self.configs.get('timeout'))
                 client.logging(call_logging=self.logging)
                 result = client.connect()
                 if result.is_success is True and client.get_connected() is True:
                     self.clients[address] = client
                 else:
                     raise Exception(f"{result.msg}")
         return self.clients.get(address)
 
-    def _send_read_cmd(self, address: str, ab_item_list: list):
+    def _send_read_cmd(self, address: str, s7_item_list: list):
         try:
-            if self._get_client(address) is not None and len(ab_item_list) > 0:
-                result = self._get_client(address).read(ab_item_list)
+            if self._get_client(address) is not None and len(s7_item_list) > 0:
+                result = self._get_client(address).read(s7_item_list)
                 if isinstance(result, IOTBaseCommon.IOTNetResult):
                     if result.is_success is True:
                         for item in result.contents:
                             if isinstance(item, IOTBaseCommon.IOTNetResult):
                                 if item.is_success:
                                     if item.contents[9] is True:
-                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}", **self.gen_read_write_result(True, item.contents[8]))
+                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[6]}", **self.gen_read_write_result(True, item.contents[8]))
                                     else:
-                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}", **self.gen_read_write_result(False, item.contents[10]))
+                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[6]}", **self.gen_read_write_result(False, item.contents[10]))
                                 else:
-                                    self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}", **self.gen_read_write_result(False, item.msg))
+                                    self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[6]}", **self.gen_read_write_result(False, item.msg))
                     else:
                         raise Exception(f"{result.msg}")
         except Exception as e:
-            for (ad, type) in ab_item_list:
+            for (ad, type) in s7_item_list:
                 self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__()))
 
     def _read_address(self, *args, **kwargs) -> dict:
-        (address, ab_items) = args
+        (address, s7_items) = args
         results = {}
-        units = IOTBaseCommon.chunk_list(ab_items, self.configs.get('multi_read'))
+        units = IOTBaseCommon.chunk_list(s7_items, self.configs.get('multi_read'))
         for unit in units:
             self._send_read_cmd(address, unit)
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _read(self, read_items: dict):
         if len(read_items) > 0:
             jobs = IOTBaseCommon.SimpleThreadPool(len(read_items), f"{self}")
-            for address, ab_items in read_items.items():
-                jobs.submit_task(self._read_address, address, ab_items)
+            for address, s7_items in read_items.items():
+                jobs.submit_task(self._read_address, address, s7_items)
             return jobs.done()
         return {}
 
     def _get_value(self, name: str, device_address: str, address: str, type: int):
         try:
             [result, value] = self.get_device_property(device_address, f"{address}_{type}", [self.get_read_quality, self.get_read_result])
             if result is True:
@@ -820,44 +837,75 @@
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
             self.update_results(name, False, e.__str__())
         return None
 
-    def _send_write_cmd(self, address: str, ab_item_list: list):
+    def _send_write_cmd(self, address: str, s7_item_list: list):
         try:
-            if self._get_client(address) is not None and len(ab_item_list) > 0:
-                result = self._get_client(address).write(ab_item_list)
+            if self._get_client(address) is not None and len(s7_item_list) > 0:
+                result = self._get_client(address).write(s7_item_list)
                 if isinstance(result, IOTBaseCommon.IOTNetResult):
                     if result.is_success is True:
                         for item in result.contents:
                             if isinstance(item, IOTBaseCommon.IOTNetResult):
                                 if item.is_success:
                                     if item.contents[9] is True:
-                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}",  **self.gen_read_write_result(True, item.contents[9], False))
+                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[6]}",  **self.gen_read_write_result(True, item.contents[9], False))
                                     else:
-                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}",  **self.gen_read_write_result(False, item.contents[10], False))
+                                        self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[6]}",  **self.gen_read_write_result(False, item.contents[10], False))
                                 else:
-                                    self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}",  **self.gen_read_write_result(False, item.msg, False))
+                                    self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[6]}",  **self.gen_read_write_result(False, item.msg, False))
                     else:
                         raise Exception(f"{result.msg}")
         except Exception as e:
-            for (ad, type, value) in ab_item_list:
+            for (ad, type, value) in s7_item_list:
                 self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__(), False))
 
     def _write_address(self, *args, **kwargs) -> dict:
-        (address, ab_items) = args
+        (address, s7_items) = args
         results = {}
-        units = IOTBaseCommon.chunk_list(ab_items, self.configs.get('multi_read'))
+        units = IOTBaseCommon.chunk_list(s7_items, self.configs.get('multi_read'))
         for unit in units:
             self._send_write_cmd(address, unit)
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _write(self, write_items: dict):
         if len(write_items) > 0:
             jobs = IOTBaseCommon.SimpleThreadPool(len(write_items), f"{self}")
-            for address, ab_items in write_items.items():
-                jobs.submit_task(self._write_address, address, ab_items)
+            for address, s7_items in write_items.items():
+                jobs.submit_task(self._write_address, address, s7_items)
             return jobs.done()
         return {}
+
+    def _get_server(self, address: str):
+        server = self.servers.get(address, {}).get('server')
+        if server is None:
+            info = self._get_address_info(address)
+            if 'type' in info.keys():
+                server = SiemensS7Server(SiemensS7Version(info['type']), info['host'], info['port'], info['rack'], info['slot'])
+                server.logging(call_logging=self.logging)
+                server.start_server()
+                self.servers[address] = {'server': server, 'blocks': {}}
+        return server
+
+    def _release_server(self, address: str):
+        try:
+            server = self.servers.get(address, {}).get('server')
+            if server is not None:
+                server.stop_server()
+            server = None
+        except:
+            pass
+        finally:
+            if 'server' in self.servers.get(address, {}).keys():
+                del self.servers[address]['server']
+
+    def _refresh_objects(self, address: str, objects: list):
+        server_cache = self.servers.get(address, {})
+        server = server_cache.get('server')
+        if server is not None and len(objects) > 0:
+            units = IOTBaseCommon.chunk_list(objects, self.configs.get('multi_read'))
+            for unit in units:
+                server.simulate(unit)
```

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
         if IOTBaseCommon.is_windows():
             library = self.configs.get('library')
             if isinstance(library, str) and len(library) > 0 and IOTBaseCommon.check_file_exist(library):
                 load_library(library)
 
     def _get_client(self, address: str):
         client = self.clients.get(address)
-        if client is not None and (client.get_connected() is False or str(client.get_cpu_state()) != 'S7CpuStatusRun'):
+        if client is not None and (client.get_connected() is False or str(client.get_cpu_state()) == 'S7CpuStatusStop'):
             self._release_client(address)
             client = None
 
         if client is None:
             info = self._get_address_info(address)
             if 'type' in info.keys():
                 self._load_library()
@@ -525,15 +525,15 @@
                     length = 1
                     pos = infos[1].find('.')
                     if pos >= 1:
                         start = int(float(infos[1][1:pos]))
                         addr = int(float(infos[1][pos + 1:]))
 
         else:   # I2.0 VD200
-            db = 1 if area == 'V' else 0
+            db = 1 if address[0] == 'V' else 0
             if address[1] == 'B':   # BYTE
                 type = IOTBaseCommon.DataTransform.TypeFormat.INT8
                 length = 1
             elif address[1] == 'W':
                 type = IOTBaseCommon.DataTransform.TypeFormat.INT16
                 length = 2
             elif address[1] == 'D':
```

### Comparing `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/setup.py` & `RobertCommonDriver-0.1.46/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.45'
-DATE = '2023-07-14'
+VERSION = '0.1.46'
+DATE = '2023-07-24'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from robertcommondriver.system.iot.iot_iec104 import IOTIEC104
+from robertcommondriver.system.iot.iot_iec104 import IOTIEC104, unpack
 
 
 def logging_print(**kwargs):
     print(kwargs)
 
 
 def test_read():
@@ -26,8 +26,30 @@
 def test_parse():
     #r = IOTIEC104.APDU(bytes.fromhex('68 0E 06 00 08 00 64 01 06 00 01 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00'))
     r = IOTIEC104.APDU(bytes.fromhex('68 0E 02 00 02 00 01 82 14 00 01 00 01 00 00 01 68 0E 04 00 02 00 64 01 0A 00 01 00 00 00 00 14'))
     #r = IOTIEC104.APDU(bytes.fromhex('68 0E 02 00 02 00 01 82 14 00 01 00 01 00 00 01'))
     print(r.info())
 
 
-test_read()
+def test_read1():
+    dict_config = {'host': '192.168.1.184', 'port': 2404, 'timeout': 5, 'zongzhao_interval': 0, 'zongzhao_timeout': 30, 'u_test_timeout': 10,  's_interval': 1}
+    dict_point = {}
+    dict_point['iec1'] = {'point_writable': True, 'point_name': 'iec1', 'point_type': 1, 'point_address': 100, 'point_scale': '1'}
+    dict_point['iec2'] = {'point_writable': True, 'point_name': 'iec2', 'point_type': 13, 'point_address': 600, 'point_scale': '1'}
+
+    client = IOTIEC104(configs = dict_config, points= dict_point)
+    client.logging(call_logging=logging_print)
+    while True:
+        try:
+            result = client.read(names=list(dict_point.keys()))
+            print(result)
+        except Exception as e:
+            print(f"error: {e.__str__()}")
+        time.sleep(5)
+
+
+def test_frame():
+    info = IOTIEC104.APDU(bytes.fromhex('68 0f 08 00 02 00 05 01 14 00 01 00 2c 01 00 00 00 ')).info()
+    print(info)
+
+
+test_frame()
```

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             print(f"error: {e.__str__()}")
         time.sleep(4)
 
 
 def test_read_200():
     dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'send_timeout': 15, 'rec_timeout': 3500}
     dict_point = {}
-    dict_point['plc1'] = {'point_writable': True, 'point_name': 'plc1', 'point_device_address': '192.168.1.12/102/0/1', 'point_address': 'I1.1', 'point_scale': '1'}
+    dict_point['plc1'] = {'point_writable': True, 'point_name': 'plc1', 'point_device_address': '192.168.100.107/102', 'point_address': 'I1.1', 'point_scale': '1'}
     client = IOTPlcS7(configs=dict_config, points=dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
             re = client.read()
             print(re)
         except Exception as e:
@@ -123,8 +123,8 @@
             client.write(values={'plc3': 1})
             print(client.read())
         except Exception as e:
             print(f"error: {e.__str__()}")
         time.sleep(4)
 
 
-test_read2()
+test_read_200()
```

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

