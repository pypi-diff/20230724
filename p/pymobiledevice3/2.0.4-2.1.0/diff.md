# Comparing `tmp/pymobiledevice3-2.0.4.tar.gz` & `tmp/pymobiledevice3-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymobiledevice3-2.0.4.tar", last modified: Sun Jul 16 15:36:35 2023, max compression
+gzip compressed data, was "pymobiledevice3-2.1.0.tar", last modified: Mon Jul 24 06:18:25 2023, max compression
```

## Comparing `pymobiledevice3-2.0.4.tar` & `pymobiledevice3-2.1.0.tar`

### file list

```diff
@@ -1,158 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.217844 pymobiledevice3-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-07-16 15:36:35.217844 pymobiledevice3-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.201843 pymobiledevice3-2.0.4/pymobiledevice3/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/bonjour.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/ca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.205843 pymobiledevice3-2.0.4/pymobiledevice3/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/afc.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/bonjour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/companion_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/developer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/mounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/provision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/springboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/cli/webinspector.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/irecv.py
--rw-r--r--   0 runner    (1001) docker     (123)    32198 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/irecv_devices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29015 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/pair_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.205843 pymobiledevice3-2.0.4/pymobiledevice3/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/remote/bonjour.py
--rw-r--r--   0 runner    (1001) docker     (123)    20387 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/remote/core_device_tunnel_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/remote/remote_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/remote/remotexpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/remote/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/remote/xpc_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.209843 pymobiledevice3-2.0.4/pymobiledevice3/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1023280 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/dsc_uuid_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/dsc_uuid_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/firmware_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/notifications.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.209843 pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/element_attribute.js
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/element_clear.js
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/enter_fullscreen.js
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/find_nodes.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/focus.js
--rw-r--r--   0 runner    (1001) docker     (123)    42234 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/get_attribute.js
--rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/is_displayed.js
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/is_editable.js
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/is_enabled.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.213843 pymobiledevice3-2.0.4/pymobiledevice3/restore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/base_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/fdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/ftab.py
--rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/restore_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/restored_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28752 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/restore/tss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6768 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/service_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.217844 pymobiledevice3-2.0.4/pymobiledevice3/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/accessibilityaudit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31043 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/afc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/crash_reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/debugserver_applist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/device_arbitration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/device_link.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6154 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/diagnostics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dtfetchsymbols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.217844 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.217844 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/application_listing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/condition_inducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/energy_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/network_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/process_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/sysmontap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/file_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/heartbeat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/house_arrest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/installation_proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/misagent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3410 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/mobile_activation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4517 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/mobile_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13592 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/mobile_image_mounter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16752 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/mobilebackup2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1544 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/notification_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/os_trace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9223 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/pcapd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/preboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/remote_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1270 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/screenshot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/simulate_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/springboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/syslog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.217844 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/automation_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/cdp_screencast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/cdp_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/cdp_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/inspector_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/selenium_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/session_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/switch_to.py
--rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/services/webinspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/tcp_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pymobiledevice3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.201843 pymobiledevice3-2.0.4/pymobiledevice3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-07-16 15:36:35.000000 pymobiledevice3-2.0.4/pymobiledevice3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-16 15:36:35.000000 pymobiledevice3-2.0.4/pymobiledevice3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:36:35.000000 pymobiledevice3-2.0.4/pymobiledevice3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-16 15:36:35.000000 pymobiledevice3-2.0.4/pymobiledevice3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-16 15:36:35.000000 pymobiledevice3-2.0.4/pymobiledevice3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-16 15:36:35.000000 pymobiledevice3-2.0.4/pymobiledevice3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:36:35.217844 pymobiledevice3-2.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:36:35.217844 pymobiledevice3-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-16 15:36:17.000000 pymobiledevice3-2.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.367654 pymobiledevice3-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    57708 2023-07-24 06:18:25.367654 pymobiledevice3-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.343653 pymobiledevice3-2.1.0/misc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/misc/extract_plist_from_pcaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/misc/remotexpc_sniffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.347653 pymobiledevice3-2.1.0/pymobiledevice3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/bonjour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/ca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.351653 pymobiledevice3-2.1.0/pymobiledevice3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/afc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/bonjour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/companion_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38256 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/developer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/mounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/provision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/cli/webinspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/irecv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32198 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/irecv_devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28953 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/lockdown_service_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/pair_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.351653 pymobiledevice3-2.1.0/pymobiledevice3/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/bonjour.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.355654 pymobiledevice3-2.1.0/pymobiledevice3/remote/core_device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/core_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/core_device/app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/core_device/core_device_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/core_device/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/core_device/diagnostics_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/core_device_tunnel_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/remote_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/remote_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/remotexpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/remote/xpc_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.355654 pymobiledevice3-2.1.0/pymobiledevice3/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1023280 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/dsc_uuid_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/dsc_uuid_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/firmware_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/notifications.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.359654 pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/element_attribute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/element_clear.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/enter_fullscreen.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/find_nodes.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/focus.js
+-rw-r--r--   0 runner    (1001) docker     (123)    42234 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/get_attribute.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/is_displayed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/is_editable.js
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/is_enabled.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.359654 pymobiledevice3-2.1.0/pymobiledevice3/restore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/base_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/fdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/ftab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49852 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/restored_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28752 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/restore/tss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6957 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/service_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.363654 pymobiledevice3-2.1.0/pymobiledevice3/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/accessibilityaudit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31443 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/afc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/crash_reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/debugserver_applist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/device_arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/device_link.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6494 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/diagnostics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dtfetchsymbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.363654 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.367654 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/application_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/condition_inducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28098 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/energy_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/network_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/process_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/sysmontap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/file_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/heartbeat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/house_arrest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/installation_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/lockdown_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2127 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/misagent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3428 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/mobile_activation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4722 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/mobile_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13817 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/mobile_image_mounter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16764 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/mobilebackup2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2094 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/notification_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/os_trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9504 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/pcapd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/preboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/remote_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/restore_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/screenshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1820 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/simulate_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/syslog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.367654 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/automation_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/cdp_screencast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/cdp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/cdp_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/inspector_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/selenium_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/session_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/switch_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/services/webinspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/tcp_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pymobiledevice3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.347653 pymobiledevice3-2.1.0/pymobiledevice3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    57708 2023-07-24 06:18:25.000000 pymobiledevice3-2.1.0/pymobiledevice3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-24 06:18:25.000000 pymobiledevice3-2.1.0/pymobiledevice3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:18:25.000000 pymobiledevice3-2.1.0/pymobiledevice3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 06:18:25.000000 pymobiledevice3-2.1.0/pymobiledevice3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-24 06:18:25.000000 pymobiledevice3-2.1.0/pymobiledevice3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 06:18:25.000000 pymobiledevice3-2.1.0/pymobiledevice3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:18:25.367654 pymobiledevice3-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:18:25.367654 pymobiledevice3-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 06:18:02.000000 pymobiledevice3-2.1.0/tests/test_utils.py
```

### Comparing `pymobiledevice3-2.0.4/LICENSE` & `pymobiledevice3-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/PKG-INFO` & `pymobiledevice3-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymobiledevice3
-Version: 2.0.4
+Version: 2.1.0
 Summary: Pure python3 implementation for working with iDevices (iPhone, etc...)
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -872,26 +872,26 @@
 * The following will require Web Inspector feature to be turned on:
     * Get interactive JavaScript shell on any open tab:
         * `pymobiledevice3 webinspector js_shell`
     * List currently opened tabs is device's browser:
         * `pymobiledevice3 webinspector opened-tabs`
     * The following will require also the Remote Automation feature to be turned on:
         * Get interactive JavaScript shell on new remote automation tab:
-            * `pymobiledevice3 webinspector js_shell --automation` 
+            * `pymobiledevice3 webinspector js_shell --automation`
         * Launch an automation session to view a given URL:
             * `pymobiledevice3 webinspector launch URL`
         * Get a a selenium-like shell:
             * `pymobiledevice3 webinspector shell`
-* Mount DeveloperDiskImage:
-    * `pymobiledevice3 mounter mount`
+* Mount DeveloperDiskImage (On iOS>=17.0, each command will require an additional `--rsd` option):
+    * `pymobiledevice3 mounter auto-mount`
     * The following will assume the DeveloperDiskImage is already mounted:
         * Simulate an `x y` location:
             * `pymobiledevice3 developer simulate-location set x y`
         * Taking a screenshot from the device:
-            * `pymobiledevice3 developer screenshot /path/to/screen.png`
+            * `pymobiledevice3 developer dvt screenshot /path/to/screen.png`
         * View detailed process list (including ppid, uid, guid, sandboxed, etc...):
             * `pymobiledevice3 developer dvt sysmon process single`
         * Sniffing oslog:
             * `pymobiledevice3 developer dvt oslog`
         * Kill a process:
             * `pymobiledevice3 developer dvt kill PID`
         * List files in a given directory (un-chrooted):
```

### Comparing `pymobiledevice3-2.0.4/README.md` & `pymobiledevice3-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -175,26 +175,26 @@
 * The following will require Web Inspector feature to be turned on:
     * Get interactive JavaScript shell on any open tab:
         * `pymobiledevice3 webinspector js_shell`
     * List currently opened tabs is device's browser:
         * `pymobiledevice3 webinspector opened-tabs`
     * The following will require also the Remote Automation feature to be turned on:
         * Get interactive JavaScript shell on new remote automation tab:
-            * `pymobiledevice3 webinspector js_shell --automation` 
+            * `pymobiledevice3 webinspector js_shell --automation`
         * Launch an automation session to view a given URL:
             * `pymobiledevice3 webinspector launch URL`
         * Get a a selenium-like shell:
             * `pymobiledevice3 webinspector shell`
-* Mount DeveloperDiskImage:
-    * `pymobiledevice3 mounter mount`
+* Mount DeveloperDiskImage (On iOS>=17.0, each command will require an additional `--rsd` option):
+    * `pymobiledevice3 mounter auto-mount`
     * The following will assume the DeveloperDiskImage is already mounted:
         * Simulate an `x y` location:
             * `pymobiledevice3 developer simulate-location set x y`
         * Taking a screenshot from the device:
-            * `pymobiledevice3 developer screenshot /path/to/screen.png`
+            * `pymobiledevice3 developer dvt screenshot /path/to/screen.png`
         * View detailed process list (including ppid, uid, guid, sandboxed, etc...):
             * `pymobiledevice3 developer dvt sysmon process single`
         * Sniffing oslog:
             * `pymobiledevice3 developer dvt oslog`
         * Kill a process:
             * `pymobiledevice3 developer dvt kill PID`
         * List files in a given directory (un-chrooted):
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/__main__.py` & `pymobiledevice3-2.1.0/pymobiledevice3/__main__.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/bonjour.py` & `pymobiledevice3-2.1.0/pymobiledevice3/bonjour.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/ca.py` & `pymobiledevice3-2.1.0/pymobiledevice3/ca.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/activation.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/activation.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 @cli.group()
 def activation():
     """ activation options """
     pass
 
 
 @activation.command(cls=Command)
-def state(lockdown: LockdownClient):
+def state(service_provider: LockdownClient):
     """ Get current activation state """
-    print(MobileActivationService(lockdown).state)
+    print(MobileActivationService(service_provider).state)
 
 
 @activation.command(cls=Command)
 @click.option('--now', is_flag=True, help='when --offline is used, dont wait for next nonce cycle')
-def activate(lockdown: LockdownClient, now):
+def activate(service_provider: LockdownClient, now):
     """ Activate device """
-    activation_service = MobileActivationService(lockdown)
+    activation_service = MobileActivationService(service_provider)
     if not now:
         activation_service.wait_for_activation_session()
     activation_service.activate()
 
 
 @activation.command(cls=Command)
-def deactivate(lockdown: LockdownClient):
+def deactivate(service_provider: LockdownClient):
     """ Deactivate device """
-    MobileActivationService(lockdown).deactivate()
+    MobileActivationService(service_provider).deactivate()
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/afc.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/afc.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 @cli.group()
 def afc():
     """ FileSystem utils """
     pass
 
 
 @afc.command('shell', cls=Command)
-def afc_shell(lockdown: LockdownClient):
+def afc_shell(service_provider: LockdownClient):
     """ open an AFC shell rooted at /var/mobile/Media """
-    AfcShell(lockdown=lockdown, service_name='com.apple.afc').cmdloop()
+    AfcShell(lockdown=service_provider).cmdloop()
 
 
 @afc.command('pull', cls=Command)
 @click.argument('remote_file', type=click.Path(exists=False))
 @click.argument('local_file', type=click.File('wb'))
-def afc_pull(lockdown: LockdownClient, remote_file, local_file):
+def afc_pull(service_provider: LockdownClient, remote_file, local_file):
     """ pull remote file from /var/mobile/Media """
-    local_file.write(AfcService(lockdown=lockdown).get_file_contents(remote_file))
+    local_file.write(AfcService(lockdown=service_provider).get_file_contents(remote_file))
 
 
 @afc.command('push', cls=Command)
 @click.argument('local_file', type=click.File('rb'))
 @click.argument('remote_file', type=click.Path(exists=False))
-def afc_push(lockdown: LockdownClient, local_file, remote_file):
+def afc_push(service_provider: LockdownClient, local_file, remote_file):
     """ push local file into /var/mobile/Media """
-    AfcService(lockdown=lockdown).set_file_contents(remote_file, local_file.read())
+    AfcService(lockdown=service_provider).set_file_contents(remote_file, local_file.read())
 
 
 @afc.command('ls', cls=Command)
 @click.argument('remote_file', type=click.Path(exists=False))
 @click.option('-r', '--recursive', is_flag=True)
-def afc_ls(lockdown: LockdownClient, remote_file, recursive):
+def afc_ls(service_provider: LockdownClient, remote_file, recursive):
     """ perform a dirlist rooted at /var/mobile/Media """
-    for path in AfcService(lockdown=lockdown).dirlist(remote_file, -1 if recursive else 1):
+    for path in AfcService(lockdown=service_provider).dirlist(remote_file, -1 if recursive else 1):
         print(path)
 
 
 @afc.command('rm', cls=Command)
 @click.argument('remote_file', type=click.Path(exists=False))
-def afc_rm(lockdown: LockdownClient, remote_file):
+def afc_rm(service_provider: LockdownClient, remote_file):
     """ remove a file rooted at /var/mobile/Media """
-    AfcService(lockdown=lockdown).rm(remote_file)
+    AfcService(lockdown=service_provider).rm(remote_file)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/amfi.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/amfi.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 @cli.group()
 def amfi():
     """ amfi options """
     pass
 
 
 @amfi.command(cls=Command)
-def enable_developer_mode(lockdown: LockdownClient):
+def enable_developer_mode(service_provider: LockdownClient):
     """ enable developer mode """
-    AmfiService(lockdown).enable_developer_mode()
+    AmfiService(service_provider).enable_developer_mode()
 
 
 @amfi.command(cls=Command)
 @click.option('--color/--no-color', default=True)
-def developer_mode_status(lockdown: LockdownClient, color):
+def developer_mode_status(service_provider: LockdownClient, color):
     """ query developer mode status """
-    print_json(lockdown.developer_mode_status, colored=color)
+    print_json(service_provider.developer_mode_status, colored=color)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/apps.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/apps.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,38 +19,38 @@
 
 
 @apps.command('list', cls=Command)
 @click.option('--color/--no-color', default=True)
 @click.option('-u', '--user', is_flag=True, help='include user apps')
 @click.option('-s', '--system', is_flag=True, help='include system apps')
 @click.option('--hidden', is_flag=True, help='include hidden apps')
-def apps_list(lockdown: LockdownClient, color, user, system, hidden):
+def apps_list(service_provider: LockdownClient, color, user, system, hidden):
     """ list installed apps """
     app_types = []
     if user:
         app_types.append('User')
     if system:
         app_types.append('System')
     if hidden:
         app_types.append('Hidden')
-    print_json(InstallationProxyService(lockdown=lockdown).get_apps(app_types), colored=color)
+    print_json(InstallationProxyService(lockdown=service_provider).get_apps(app_types), colored=color)
 
 
 @apps.command('uninstall', cls=Command)
 @click.argument('bundle_id')
-def uninstall(lockdown: LockdownClient, bundle_id):
+def uninstall(service_provider: LockdownClient, bundle_id):
     """ uninstall app by given bundle_id """
-    InstallationProxyService(lockdown=lockdown).uninstall(bundle_id)
+    InstallationProxyService(lockdown=service_provider).uninstall(bundle_id)
 
 
 @apps.command('install', cls=Command)
 @click.argument('ipa_path', type=click.Path(exists=True))
-def install(lockdown: LockdownClient, ipa_path):
+def install(service_provider: LockdownClient, ipa_path):
     """ install given .ipa """
-    InstallationProxyService(lockdown=lockdown).install_from_local(ipa_path)
+    InstallationProxyService(lockdown=service_provider).install_from_local(ipa_path)
 
 
 @apps.command('afc', cls=Command)
 @click.argument('bundle_id')
 def afc(lockdown: LockdownClient, bundle_id):
     """ open an AFC shell for given bundle_id, assuming its profile is installed """
     HouseArrestService(lockdown=lockdown).shell(bundle_id)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/backup.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/backup.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,21 +28,21 @@
     pass
 
 
 @backup2.command(cls=Command)
 @click.argument('backup-directory', type=click.Path(file_okay=False))
 @click.option('--full', is_flag=True, help=('Whether to do a full backup.'
                                             ' If full is True, any previous backup attempts will be discarded.'))
-def backup(lockdown: LockdownClient, backup_directory, full):
+def backup(service_provider: LockdownClient, backup_directory, full):
     """
     Backup device.
 
     All backup data will be written to BACKUP_DIRECTORY, under a directory named with the device's udid.
     """
-    backup_client = Mobilebackup2Service(lockdown)
+    backup_client = Mobilebackup2Service(service_provider)
     with tqdm(total=100, dynamic_ncols=True) as pbar:
         def update_bar(percentage):
             pbar.n = percentage
             pbar.refresh()
 
         backup_client.backup(full=full, backup_directory=backup_directory, progress_callback=update_bar)
 
@@ -52,121 +52,121 @@
 @click.option('--system/--no-system', default=False, help='Restore system files.')
 @click.option('--reboot/--no-reboot', default=True, help='Reboot the device when done.')
 @click.option('--copy/--no-copy', default=True, help='Create a copy of backup folder before restoring.')
 @click.option('--settings/--no-settings', default=True, help='Restore device settings.')
 @click.option('--remove/--no-remove', default=False, help='Remove items which aren\'t being restored.')
 @password_option
 @source_option
-def restore(lockdown: LockdownClient, backup_directory, system, reboot, copy, settings, remove, password, source):
+def restore(service_provider: LockdownClient, backup_directory, system, reboot, copy, settings, remove, password, source):
     """
     Restore a backup to a device.
 
     The backup will be restored from a directory with the device udid under BACKUP_DIRECTORY.
     """
-    backup_client = Mobilebackup2Service(lockdown)
+    backup_client = Mobilebackup2Service(service_provider)
     with tqdm(total=100, dynamic_ncols=True) as pbar:
         def update_bar(percentage):
             pbar.n = percentage
             pbar.refresh()
 
         backup_client.restore(backup_directory=backup_directory, progress_callback=update_bar, system=system,
                               reboot=reboot, copy=copy, settings=settings, remove=remove, password=password,
                               source=source)
 
 
 @backup2.command(cls=Command)
 @backup_directory_arg
 @source_option
-def info(lockdown: LockdownClient, backup_directory, source):
+def info(service_provider: LockdownClient, backup_directory, source):
     """
     Print information about a backup.
     """
-    backup_client = Mobilebackup2Service(lockdown)
+    backup_client = Mobilebackup2Service(service_provider)
     print(backup_client.info(backup_directory=backup_directory, source=source))
 
 
 @backup2.command('list', cls=Command)
 @backup_directory_arg
 @source_option
-def list_(lockdown: LockdownClient, backup_directory, source):
+def list_(service_provider: LockdownClient, backup_directory, source):
     """
     List all file in the backup in a CSV format.
     """
-    backup_client = Mobilebackup2Service(lockdown)
+    backup_client = Mobilebackup2Service(service_provider)
     print(backup_client.list(backup_directory=backup_directory, source=source))
 
 
 @backup2.command(cls=Command)
 @backup_directory_arg
 @password_option
 @source_option
-def unback(lockdown: LockdownClient, backup_directory, password, source):
+def unback(service_provider: LockdownClient, backup_directory, password, source):
     """
     Convert all files in the backup to the correct directory hierarchy.
     """
-    backup_client = Mobilebackup2Service(lockdown)
+    backup_client = Mobilebackup2Service(service_provider)
     backup_client.unback(backup_directory=backup_directory, password=password, source=source)
 
 
 @backup2.command(cls=Command)
 @click.argument('domain-name')
 @click.argument('relative-path')
 @backup_directory_arg
 @password_option
 @source_option
-def extract(lockdown: LockdownClient, domain_name, relative_path, backup_directory, password, source):
+def extract(service_provider: LockdownClient, domain_name, relative_path, backup_directory, password, source):
     """
     Extract a file from the backup.
 
     The file that belongs to the domain DOMAIN_NAME and located on the device in the path RELATIVE_PATH,
     will be extracted to the BACKUP_DIRECTORY.
     """
-    backup_client = Mobilebackup2Service(lockdown)
+    backup_client = Mobilebackup2Service(service_provider)
     backup_client.extract(domain_name, relative_path, backup_directory=backup_directory, password=password,
                           source=source)
 
 
 @backup2.command(cls=Command)
 @click.argument('mode', type=click.Choice(['on', 'off'], case_sensitive=False))
 @click.argument('password')
 @backup_directory_option
-def encryption(lockdown: LockdownClient, backup_directory, mode, password):
+def encryption(service_provider: LockdownClient, backup_directory, mode, password):
     """
     Set backup encryption on / off.
 
     When on, PASSWORD will be the new backup password.
     When off, PASSWORD is the current backup password.
     """
-    backup_client = Mobilebackup2Service(lockdown)
+    backup_client = Mobilebackup2Service(service_provider)
     should_encrypt = mode.lower() == 'on'
     if should_encrypt == backup_client.will_encrypt:
         logger.error('Encryption already ' + ('on!' if should_encrypt else 'off!'))
         return
     if should_encrypt:
         backup_client.change_password(backup_directory, new=password)
     else:
         backup_client.change_password(backup_directory, old=password)
 
 
 @backup2.command(cls=Command)
 @click.argument('old-password')
 @click.argument('new-password')
 @backup_directory_option
-def change_password(lockdown: LockdownClient, old_password, new_password, backup_directory):
+def change_password(service_provider: LockdownClient, old_password, new_password, backup_directory):
     """
     Change the backup password.
     """
-    backup_client = Mobilebackup2Service(lockdown)
+    backup_client = Mobilebackup2Service(service_provider)
     if not backup_client.will_encrypt:
         logger.error('Encryption is not turned on!')
         return
     backup_client.change_password(backup_directory, old=old_password, new=new_password)
 
 
 @backup2.command(cls=Command)
 @backup_directory_arg
-def erase_device(lockdown: LockdownClient, backup_directory):
+def erase_device(service_provider: LockdownClient, backup_directory):
     """
     Erase all data on the device.
     """
-    backup_client = Mobilebackup2Service(lockdown)
+    backup_client = Mobilebackup2Service(service_provider)
     backup_client.erase_device(backup_directory)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/bonjour.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/bonjour.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/companion_proxy.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/companion_proxy.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 def companion():
     """ companion options """
     pass
 
 
 @companion.command('list', cls=Command)
 @click.option('--color/--no-color', default=True)
-def companion_list(lockdown: LockdownClient, color):
+def companion_list(service_provider: LockdownClient, color):
     """ list all paired companion devices """
-    print_json(CompanionProxyService(lockdown).list(), colored=color, default=lambda x: '<non-serializable>')
+    print_json(CompanionProxyService(service_provider).list(), colored=color, default=lambda x: '<non-serializable>')
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/crash.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/crash.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,65 +15,65 @@
 def crash():
     """ crash report options """
     pass
 
 
 @crash.command('clear', cls=Command)
 @click.option('-f', '--flush', is_flag=True, default=False, help='flush before clear')
-def crash_clear(lockdown: LockdownClient, flush):
+def crash_clear(service_provider: LockdownClient, flush):
     """ clear(/remove) all crash reports """
-    crash_manager = CrashReportsManager(lockdown)
+    crash_manager = CrashReportsManager(service_provider)
     if flush:
         crash_manager.flush()
     crash_manager.clear()
 
 
 @crash.command('pull', cls=Command)
 @click.argument('out', type=click.Path(file_okay=False))
 @click.argument('remote_file', type=click.Path(), required=False)
 @click.option('-e', '--erase', is_flag=True)
-def crash_pull(lockdown: LockdownClient, out, remote_file, erase):
+def crash_pull(service_provider: LockdownClient, out, remote_file, erase):
     """ pull all crash reports """
     if remote_file is None:
         remote_file = '/'
-    CrashReportsManager(lockdown).pull(out, remote_file, erase)
+    CrashReportsManager(service_provider).pull(out, remote_file, erase)
 
 
 @crash.command('shell', cls=Command)
-def crash_shell(lockdown: LockdownClient):
+def crash_shell(service_provider: LockdownClient):
     """ start an afc shell """
-    CrashReportsShell(lockdown=lockdown).cmdloop()
+    CrashReportsShell(lockdown=service_provider).cmdloop()
 
 
 @crash.command('ls', cls=Command)
 @click.argument('remote_file', type=click.Path(), required=False)
 @click.option('-d', '--depth', type=click.INT, default=1)
-def crash_ls(lockdown: LockdownClient, remote_file, depth):
+def crash_ls(service_provider: LockdownClient, remote_file, depth):
     """ List  """
     if remote_file is None:
         remote_file = '/'
-    for path in CrashReportsManager(lockdown).ls(remote_file, depth):
+    for path in CrashReportsManager(service_provider).ls(remote_file, depth):
         print(path)
 
 
 @crash.command('flush', cls=Command)
-def crash_mover_flush(lockdown: LockdownClient):
+def crash_mover_flush(service_provider: LockdownClient):
     """ trigger com.apple.crashreportmover to flush all products into CrashReports directory """
-    CrashReportsManager(lockdown).flush()
+    CrashReportsManager(service_provider).flush()
 
 
 @crash.command('watch', cls=Command)
 @click.argument('name', required=False)
 @click.option('-r', '--raw', is_flag=True)
-def crash_mover_watch(lockdown: LockdownClient, name, raw):
+def crash_mover_watch(service_provider: LockdownClient, name, raw):
     """ watch for crash report generation """
-    for crash_report in CrashReportsManager(lockdown).watch(name=name, raw=raw):
+    for crash_report in CrashReportsManager(service_provider).watch(name=name, raw=raw):
         print(crash_report)
 
 
 @crash.command('sysdiagnose', cls=Command)
 @click.argument('out', type=click.Path(exists=False, dir_okay=False, file_okay=True))
 @click.option('-e', '--erase', is_flag=True, help='erase file after pulling')
-def crash_sysdiagnose(lockdown: LockdownClient, out, erase):
+def crash_sysdiagnose(service_provider: LockdownClient, out, erase):
     """ get a sysdiagnose archive from device (requires user interaction) """
     print('Press Power+VolUp+VolDown for 0.215 seconds')
-    CrashReportsManager(lockdown).get_new_sysdiagnose(out, erase=erase)
+    CrashReportsManager(service_provider).get_new_sysdiagnose(out, erase=erase)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/developer.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/developer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # flake8: noqa: C901
 import json
 import logging
 import os
 import posixpath
 import shlex
 import signal
-import time
 from collections import namedtuple
 from dataclasses import asdict
 from datetime import datetime
 from pathlib import Path
 from typing import List
 
 import click
 from click.exceptions import MissingParameter, UsageError
 from pykdebugparser.pykdebugparser import PyKdebugParser
 from termcolor import colored
 
 import pymobiledevice3
-from pymobiledevice3.cli.cli_common import BASED_INT, Command, default_json_encoder, print_json, wait_return
+from pymobiledevice3.cli.cli_common import BASED_INT, Command, RSDCommand, default_json_encoder, print_json, wait_return
 from pymobiledevice3.exceptions import DeviceAlreadyInUseError, DvtDirListError, ExtractingStackshotError, \
     UnrecognizedSelectorError
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.remote.core_device.app_service import AppServiceService
+from pymobiledevice3.remote.core_device.device_info import DeviceInfoService
+from pymobiledevice3.remote.remote_service_discovery import RemoteServiceDiscoveryService
 from pymobiledevice3.services.accessibilityaudit import AccessibilityAudit
 from pymobiledevice3.services.debugserver_applist import DebugServerAppList
 from pymobiledevice3.services.device_arbitration import DtDeviceArbitration
 from pymobiledevice3.services.dtfetchsymbols import DtFetchSymbols
 from pymobiledevice3.services.dvt.dvt_secure_socket_proxy import DvtSecureSocketProxyService
 from pymobiledevice3.services.dvt.instruments.activity_trace_tap import ActivityTraceTap, decode_message_format
 from pymobiledevice3.services.dvt.instruments.application_listing import ApplicationListing
@@ -69,82 +72,82 @@
     """
     pass
 
 
 @developer.command('shell', cls=Command)
 @click.argument('service')
 @click.option('-r', '--remove-ssl-context', is_flag=True)
-def developer_shell(lockdown: LockdownClient, service, remove_ssl_context):
+def developer_shell(service_provider: LockdownClient, service, remove_ssl_context):
     """ Launch developer shell. """
-    with RemoteServer(lockdown, service, remove_ssl_context) as service:
+    with RemoteServer(service_provider, service, remove_ssl_context) as service:
         service.shell()
 
 
 @developer.group()
 def dvt():
     """ dvt operations """
     pass
 
 
 @dvt.command('proclist', cls=Command)
 @click.option('--color/--no-color', default=True)
-def proclist(lockdown: LockdownClient, color):
+def proclist(service_provider: LockdownClient, color):
     """ show process list """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         processes = DeviceInfo(dvt).proclist()
         for process in processes:
             if 'startDate' in process:
                 process['startDate'] = str(process['startDate'])
 
         print_json(processes, colored=color)
 
 
 @dvt.command('applist', cls=Command)
 @click.option('--color/--no-color', default=True)
-def applist(lockdown: LockdownClient, color):
+def applist(service_provider: LockdownClient, color):
     """ show application list """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         apps = ApplicationListing(dvt).applist()
         print_json(apps, colored=color)
 
 
 @dvt.command('signal', cls=Command)
 @click.argument('pid', type=click.INT)
 @click.argument('sig', type=click.INT, required=False)
 @click.option('-s', '--signal-name', type=click.Choice([s.name for s in signal.Signals]))
-def send_signal(lockdown, pid, sig, signal_name):
+def send_signal(service_provider, pid, sig, signal_name):
     """ Send SIGNAL to process by its PID """
     if not sig and not signal_name:
         raise MissingParameter(param_type='argument|option', param_hint='\'SIG|SIGNAL-NAME\'')
     if sig and signal_name:
         raise UsageError(message='Cannot give SIG and SIGNAL-NAME together')
     sig = sig or signal.Signals[signal_name].value
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         ProcessControl(dvt).signal(pid, sig)
 
 
 @dvt.command('kill', cls=Command)
 @click.argument('pid', type=click.INT)
-def kill(lockdown: LockdownClient, pid):
+def kill(service_provider: LockdownClient, pid):
     """ Kill a process by its pid. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         ProcessControl(dvt).kill(pid)
 
 
 @dvt.command('pkill', cls=Command)
 @click.argument('expression')
-def pkill(lockdown: LockdownClient, expression):
+def pkill(service_provider: LockdownClient, expression):
     """ kill all processes containing `expression` in their name. """
-    processes = OsTraceService(lockdown=lockdown).get_pid_list()['Payload']
+    processes = OsTraceService(lockdown=service_provider).get_pid_list()['Payload']
     if len(processes) == 0:
         # no point at trying to use DvtSecureSocketProxyService if no processes
         # were matched
         return
 
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         process_control = ProcessControl(dvt)
         for pid, process_info in processes.items():
             process_name = process_info['ProcessName']
             if expression in process_name:
                 logger.info(f'killing {process_name}({pid})')
                 process_control.kill(pid)
 
@@ -152,28 +155,28 @@
 @dvt.command('launch', cls=Command)
 @click.argument('arguments', type=click.STRING)
 @click.option('--kill-existing/--no-kill-existing', default=True,
               help='Whether to kill an existing instance of this process')
 @click.option('--suspended', is_flag=True, help='Same as WaitForDebugger')
 @click.option('--env', multiple=True, type=click.Tuple((str, str)),
               help='Environment variables to pass to process given as a list of key value')
-def launch(lockdown: LockdownClient, arguments: str, kill_existing: bool, suspended: bool, env: tuple):
+def launch(service_provider: LockdownClient, arguments: str, kill_existing: bool, suspended: bool, env: tuple):
     """ Launch a process. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         parsed_arguments = shlex.split(arguments)
         pid = ProcessControl(dvt).launch(bundle_id=parsed_arguments[0], arguments=parsed_arguments[1:],
                                          kill_existing=kill_existing, start_suspended=suspended,
                                          environment=dict(env))
         print(f'Process launched with pid {pid}')
 
 
 @dvt.command('shell', cls=Command)
-def dvt_shell(lockdown: LockdownClient):
+def dvt_shell(service_provider: LockdownClient):
     """ Launch developer shell. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         dvt.shell()
 
 
 def show_dirlist(device_info: DeviceInfo, dirname, recursive=False):
     try:
         filenames = device_info.ls(dirname)
     except DvtDirListError:
@@ -185,25 +188,25 @@
         if recursive:
             show_dirlist(device_info, filename, recursive=recursive)
 
 
 @dvt.command('ls', cls=Command)
 @click.argument('path', type=click.Path(exists=False, readable=False))
 @click.option('-r', '--recursive', is_flag=True)
-def ls(lockdown: LockdownClient, path, recursive):
+def ls(service_provider: LockdownClient, path, recursive):
     """ List directory. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         show_dirlist(DeviceInfo(dvt), path, recursive=recursive)
 
 
 @dvt.command('device-information', cls=Command)
 @click.option('--color/--no-color', default=True)
-def device_information(lockdown: LockdownClient, color):
+def device_information(service_provider: LockdownClient, color):
     """ Print system information. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         device_info = DeviceInfo(dvt)
         info = {
             'hardware': device_info.hardware_information(),
             'network': device_info.network_information(),
             'kernel-name': device_info.mach_kernel_name(),
             'kpep-database': device_info.kpep_database(),
         }
@@ -211,30 +214,30 @@
             info['system'] = device_info.system_information()
         except UnrecognizedSelectorError:
             pass
         print_json(info, colored=color)
 
 
 @dvt.command('netstat', cls=Command)
-def netstat(lockdown: LockdownClient):
+def netstat(service_provider: LockdownClient):
     """ Print information about current network activity. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         with NetworkMonitor(dvt) as monitor:
             for event in monitor:
                 if isinstance(event, ConnectionDetectionEvent):
                     logger.info(
                         f'Connection detected: {event.local_address.data.hostname}:{event.local_address.port} -> '
                         f'{event.remote_address.data.hostname}:{event.remote_address.port}')
 
 
 @dvt.command('screenshot', cls=Command)
 @click.argument('out', type=click.File('wb'))
-def screenshot(lockdown: LockdownClient, out):
+def screenshot(service_provider: LockdownClient, out):
     """ get device screenshot """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         out.write(Screenshot(dvt).get_screenshot())
 
 
 @dvt.group('sysmon')
 def sysmon():
     """ System monitor options. """
 
@@ -242,41 +245,41 @@
 @sysmon.group('process')
 def sysmon_process():
     """ Process monitor options. """
 
 
 @sysmon_process.command('monitor', cls=Command)
 @click.argument('threshold', type=click.FLOAT)
-def sysmon_process_monitor(lockdown: LockdownClient, threshold):
+def sysmon_process_monitor(service_provider: LockdownClient, threshold):
     """ monitor all most consuming processes by given cpuUsage threshold. """
 
     Process = namedtuple('process', 'pid name cpuUsage')
 
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         with Sysmontap(dvt) as sysmon:
             for process_snapshot in sysmon.iter_processes():
                 entries = []
                 for process in process_snapshot:
                     if (process['cpuUsage'] is not None) and (process['cpuUsage'] >= threshold):
                         entries.append(Process(pid=process['pid'], name=process['name'], cpuUsage=process['cpuUsage']))
 
                 logger.info(entries)
 
 
 @sysmon_process.command('single', cls=Command)
 @click.option('-a', '--attributes', multiple=True,
               help='filter processes by given attribute value given as key=value')
 @click.option('--color/--no-color', default=True)
-def sysmon_process_single(lockdown: LockdownClient, attributes: List[str], color: bool):
+def sysmon_process_single(service_provider: LockdownClient, attributes: List[str], color: bool):
     """ show a single snapshot of currently running processes. """
 
     count = 0
 
     result = []
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         device_info = DeviceInfo(dvt)
 
         with Sysmontap(dvt) as sysmon:
             for process_snapshot in sysmon.iter_processes():
                 count += 1
 
                 if count < 2:
@@ -302,21 +305,21 @@
                 # exit after single snapshot
                 break
     print_json(result, colored=color)
 
 
 @sysmon.command('system', cls=Command)
 @click.option('-f', '--fields', help='field names splitted by ",".')
-def sysmon_system(lockdown: LockdownClient, fields):
+def sysmon_system(service_provider: LockdownClient, fields):
     """ show current system stats. """
 
     if fields is not None:
         fields = fields.split(',')
 
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         sysmontap = Sysmontap(dvt)
         with sysmontap as sysmon:
             for row in sysmon:
                 if 'System' in row:
                     system = sysmon.system_attributes_cls(*row['System'])
                     break
 
@@ -361,15 +364,15 @@
 @click.option('--tid', type=click.INT, default=None, help='Thread ID to filter. Omit for all.')
 @click.option('--timestamp/--no-timestamp', default=True, help='Whether to print timestamp or not.')
 @click.option('--event-name/--no-event-name', default=True, help='Whether to print event name or not.')
 @click.option('--func-qual/--no-func-qual', default=True, help='Whether to print function qualifier or not.')
 @click.option('--show-tid/--no-show-tid', default=True, help='Whether to print thread id or not.')
 @click.option('--process-name/--no-process-name', default=True, help='Whether to print process name or not.')
 @click.option('--args/--no-args', default=True, help='Whether to print event arguments or not.')
-def live_profile_session(lockdown: LockdownClient, count, bsc, class_filters, subclass_filters, tid, timestamp,
+def live_profile_session(service_provider: LockdownClient, count, bsc, class_filters, subclass_filters, tid, timestamp,
                          event_name, func_qual, show_tid, process_name, args):
     """ Print kevents received from the device in real time. """
 
     parser = PyKdebugParser()
     parser.filter_class = class_filters
     if bsc:
         subclass_filters = list(subclass_filters) + [BSC_SUBCLASS]
@@ -378,15 +381,15 @@
     parser.filter_tid = tid
     parser.show_timestamp = timestamp
     parser.show_name = event_name
     parser.show_func_qual = func_qual
     parser.show_tid = show_tid
     parser.show_process = process_name
     parser.show_args = args
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         trace_codes_map = DeviceInfo(dvt).trace_codes()
         time_config = CoreProfileSessionTap.get_time_config(dvt)
         parser.numer = time_config['numer']
         parser.denom = time_config['denom']
         parser.mach_absolute_time = time_config['mach_absolute_time']
         parser.usecs_since_epoch = time_config['usecs_since_epoch']
         parser.timezone = time_config['timezone']
@@ -400,30 +403,30 @@
 
 
 @core_profile_session.command('save', cls=Command)
 @click.argument('out', type=click.File('wb'))
 @bsc_filter
 @class_filter
 @subclass_filter
-def save_profile_session(lockdown: LockdownClient, out, bsc, class_filters, subclass_filters):
+def save_profile_session(service_provider: LockdownClient, out, bsc, class_filters, subclass_filters):
     """ Dump core profiling information. """
     if bsc:
         subclass_filters = list(subclass_filters) + [BSC_SUBCLASS]
     filters = parse_filters(subclass_filters, class_filters)
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         with CoreProfileSessionTap(dvt, {}, filters) as tap:
             tap.dump(out)
 
 
 @core_profile_session.command('stackshot', cls=Command)
 @click.option('--out', type=click.File('w'), default=None)
 @click.option('--color/--no-color', default=True)
-def stackshot(lockdown: LockdownClient, out, color):
+def stackshot(service_provider: LockdownClient, out, color):
     """ Dump stackshot information. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         with CoreProfileSessionTap(dvt, {}) as tap:
             try:
                 data = tap.get_stackshot()
             except ExtractingStackshotError:
                 logger.error(f'Extracting stackshot failed')
                 return
 
@@ -438,18 +441,19 @@
 @click.option('--tid', type=click.INT, default=None, help='Thread ID to filter. Omit for all.')
 @click.option('--show-tid/--no-show-tid', default=False, help='Whether to print thread id or not.')
 @bsc_filter
 @class_filter
 @subclass_filter
 @click.option('--process', default=None, help='Process ID / name to filter. Omit for all.')
 @click.option('--color/--no-color', default=True)
-def parse_live_profile_session(lockdown: LockdownClient, count, tid, show_tid, bsc, class_filters, subclass_filters,
+def parse_live_profile_session(service_provider: LockdownClient, count, tid, show_tid, bsc, class_filters,
+                               subclass_filters,
                                process, color):
     """ Print traces (syscalls, thread events, etc.) received from the device in real time. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         print('Receiving time information')
         time_config = CoreProfileSessionTap.get_time_config(dvt)
         parser = PyKdebugParser()
         parser.filter_class = list(class_filters)
         if bsc:
             subclass_filters = list(subclass_filters) + [BSC_SUBCLASS]
         parser.filter_subclass = subclass_filters
@@ -498,17 +502,17 @@
 
 @core_profile_session.command('callstacks-live', cls=Command)
 @click.option('-c', '--count', type=click.INT, default=-1, help='Number of events to print. Omit to endless sniff.')
 @click.option('--process', default=None, help='Process to filter. Omit for all.')
 @click.option('--tid', type=click.INT, default=None, help='Thread ID to filter. Omit for all.')
 @click.option('--show-tid/--no-show-tid', default=False, help='Whether to print thread id or not.')
 @click.option('--color/--no-color', default=True)
-def callstacks_live_profile_session(lockdown: LockdownClient, count, process, tid, show_tid, color):
+def callstacks_live_profile_session(service_provider: LockdownClient, count, process, tid, show_tid, color):
     """ Print callstacks received from the device in real time. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         print('Receiving time information')
         time_config = CoreProfileSessionTap.get_time_config(dvt)
         parser = PyKdebugParser()
         parser.numer = time_config['numer']
         parser.denom = time_config['denom']
         parser.mach_absolute_time = time_config['mach_absolute_time']
         parser.usecs_since_epoch = time_config['usecs_since_epoch']
@@ -529,45 +533,45 @@
                 i += 1
                 if i == count:
                     break
 
 
 @dvt.command('trace-codes', cls=Command)
 @click.option('--color/--no-color', default=True)
-def dvt_trace_codes(lockdown: LockdownClient, color):
+def dvt_trace_codes(service_provider: LockdownClient, color):
     """ Print KDebug trace codes. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         device_info = DeviceInfo(dvt)
         print_json({hex(k): v for k, v in device_info.trace_codes().items()}, colored=color)
 
 
 @dvt.command('name-for-uid', cls=Command)
 @click.argument('uid', type=click.INT)
-def dvt_name_for_uid(lockdown: LockdownClient, uid):
+def dvt_name_for_uid(service_provider: LockdownClient, uid):
     """ Print the assiciated username for the given uid. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         device_info = DeviceInfo(dvt)
         print(device_info.name_for_uid(uid))
 
 
 @dvt.command('name-for-gid', cls=Command)
 @click.argument('gid', type=click.INT)
-def dvt_name_for_gid(lockdown: LockdownClient, gid):
+def dvt_name_for_gid(service_provider: LockdownClient, gid):
     """ Print the assiciated group name for the given gid. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         device_info = DeviceInfo(dvt)
         print(device_info.name_for_gid(gid))
 
 
 @dvt.command('oslog', cls=Command)
 @click.option('--color/--no-color', default=True)
 @click.option('--pid', type=click.INT)
-def dvt_oslog(lockdown: LockdownClient, color, pid):
+def dvt_oslog(service_provider: LockdownClient, color, pid):
     """ oslog. """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         with ActivityTraceTap(dvt) as tap:
             for message in tap:
                 message_pid = message.process
                 # without message_type maybe signpost have event_type
                 message_type = message.message_type if hasattr(message, 'message_type') else message.event_type \
                     if hasattr(message, 'event_type') else 'unknown'
                 sender_image_path = message.sender_image_path
@@ -594,65 +598,65 @@
 
                 print(f'[{timestamp}][{subsystem}][{category}][{message_pid}][{image_name}] '
                       f'<{message_type}>: {formatted_message}')
 
 
 @dvt.command('energy', cls=Command)
 @click.argument('pid-list', nargs=-1)
-def dvt_energy(lockdown: LockdownClient, pid_list):
+def dvt_energy(service_provider: LockdownClient, pid_list):
     """ energy monitoring for given pid list. """
 
     if len(pid_list) == 0:
         logger.error('pid_list must not be empty')
         return
 
     pid_list = [int(pid) for pid in pid_list]
 
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         with EnergyMonitor(dvt, pid_list) as energy_monitor:
             for telemetry in energy_monitor:
                 logger.info(telemetry)
 
 
 @dvt.command('notifications', cls=Command)
-def dvt_notifications(lockdown: LockdownClient):
+def dvt_notifications(service_provider: LockdownClient):
     """ monitor memory and app notifications """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         with Notifications(dvt) as notifications:
             for notification in notifications:
                 logger.info(notification)
 
 
 @dvt.command('graphics', cls=Command)
-def dvt_notifications(lockdown: LockdownClient):
+def dvt_notifications(service_provider: LockdownClient):
     """ monitor graphics statistics """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         with Graphics(dvt) as graphics:
             for stats in graphics:
                 logger.info(stats)
 
 
 @developer.group('fetch-symbols')
 def fetch_symbols():
     """ fetch-symbols options. """
     pass
 
 
 @fetch_symbols.command('list', cls=Command)
 @click.option('--color/--no-color', default=True)
-def fetch_symbols_list(lockdown: LockdownClient, color: bool):
+def fetch_symbols_list(service_provider: LockdownClient, color: bool):
     """ list of files to be downloaded """
-    print_json(DtFetchSymbols(lockdown).list_files(), colored=color)
+    print_json(DtFetchSymbols(service_provider).list_files(), colored=color)
 
 
 @fetch_symbols.command('download', cls=Command)
 @click.argument('out', type=click.Path(dir_okay=True, file_okay=False))
-def fetch_symbols_download(lockdown: LockdownClient, out):
+def fetch_symbols_download(service_provider: LockdownClient, out):
     """ download the linker and dyld cache to a specified directory """
-    fetch_symbols = DtFetchSymbols(lockdown)
+    fetch_symbols = DtFetchSymbols(service_provider)
     files = fetch_symbols.list_files()
     out = Path(out)
 
     if not os.path.exists(out):
         os.makedirs(out)
 
     downloaded_files = set()
@@ -678,103 +682,103 @@
 @developer.group('simulate-location')
 def simulate_location():
     """ simulate-location options. """
     pass
 
 
 @simulate_location.command('clear', cls=Command)
-def simulate_location_clear(lockdown: LockdownClient):
+def simulate_location_clear(service_provider: LockdownClient):
     """ clear simulated location """
-    DtSimulateLocation(lockdown).clear()
+    DtSimulateLocation(service_provider).clear()
 
 
 @simulate_location.command('set', cls=Command)
 @click.argument('latitude', type=click.FLOAT)
 @click.argument('longitude', type=click.FLOAT)
-def simulate_location_set(lockdown: LockdownClient, latitude, longitude):
+def simulate_location_set(service_provider: LockdownClient, latitude, longitude):
     """
     set a simulated location.
     try:
         ... set -- 40.690008 -74.045843 for liberty island
     """
-    DtSimulateLocation(lockdown).set(latitude, longitude)
+    DtSimulateLocation(service_provider).set(latitude, longitude)
 
 
 @simulate_location.command('play', cls=Command)
 @click.argument('filename', type=click.Path(exists=True, file_okay=True, dir_okay=False))
 @click.option('--disable-sleep', is_flag=True, default=False)
-def simulate_location_play(lockdown: LockdownClient, filename, disable_sleep):
+def simulate_location_play(service_provider: LockdownClient, filename, disable_sleep):
     """
     play a .gpx file
     """
-    DtSimulateLocation(lockdown).play_gpx_file(filename, disable_sleep=disable_sleep)
+    DtSimulateLocation(service_provider).play_gpx_file(filename, disable_sleep=disable_sleep)
 
 
 @developer.group('accessibility')
 def accessibility():
     """ accessibility options. """
     pass
 
 
 @accessibility.command('capabilities', cls=Command)
-def accessibility_capabilities(lockdown: LockdownClient):
+def accessibility_capabilities(service_provider: LockdownClient):
     """ display accessibility capabilities """
-    print_json(AccessibilityAudit(lockdown).capabilities)
+    print_json(AccessibilityAudit(service_provider).capabilities)
 
 
 @accessibility.group('settings')
 def accessibility_settings():
     """ accessibility settings. """
     pass
 
 
 @accessibility_settings.command('show', cls=Command)
-def accessibility_settings_show(lockdown: LockdownClient):
+def accessibility_settings_show(service_provider: LockdownClient):
     """ show current settings """
-    for setting in AccessibilityAudit(lockdown).settings:
+    for setting in AccessibilityAudit(service_provider).settings:
         print(setting)
 
 
 @accessibility_settings.command('set', cls=Command)
 @click.argument('setting')
 @click.argument('value')
-def accessibility_settings_set(lockdown: LockdownClient, setting, value):
+def accessibility_settings_set(service_provider: LockdownClient, setting, value):
     """
     change current settings
 
     in order to list all available use the "show" command
     """
-    service = AccessibilityAudit(lockdown)
+    service = AccessibilityAudit(service_provider)
     service.set_setting(setting, eval(value))
     wait_return()
 
 
 @accessibility.command('shell', cls=Command)
-def accessibility_shell(lockdown: LockdownClient):
+def accessibility_shell(service_provider: LockdownClient):
     """ start and ipython accessibility shell """
-    AccessibilityAudit(lockdown).shell()
+    AccessibilityAudit(service_provider).shell()
 
 
 @accessibility.command('notifications', cls=Command)
-def accessibility_notifications(lockdown: LockdownClient):
+def accessibility_notifications(service_provider: LockdownClient):
     """ show notifications """
 
-    service = AccessibilityAudit(lockdown)
+    service = AccessibilityAudit(service_provider)
     for event in service.iter_events():
         if event.name in ('hostAppStateChanged:',
                           'hostInspectorCurrentElementChanged:',):
             for focus_item in event.data:
                 logger.info(focus_item)
 
 
 @accessibility.command('list-items', cls=Command)
-def accessibility_list_items(lockdown: LockdownClient):
+def accessibility_list_items(service_provider: LockdownClient):
     """ list items available in currently shown menu """
 
-    service = AccessibilityAudit(lockdown)
+    service = AccessibilityAudit(service_provider)
     iterator = service.iter_events()
 
     # every focus change is expected publish a "hostInspectorCurrentElementChanged:"
     service.move_focus_next()
 
     first_item = None
 
@@ -806,101 +810,158 @@
 def condition_list(lockdown: LockdownClient):
     """ list all available conditions """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         print_json(ConditionInducer(dvt).list())
 
 
 @condition.command('clear', cls=Command)
-def condition_clear(lockdown: LockdownClient):
+def condition_clear(service_provider: LockdownClient):
     """ clear current condition """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         ConditionInducer(dvt).clear()
 
 
 @condition.command('set', cls=Command)
 @click.argument('profile_identifier')
-def condition_set(lockdown: LockdownClient, profile_identifier):
+def condition_set(service_provider: LockdownClient, profile_identifier):
     """ set a specific condition """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         ConditionInducer(dvt).set(profile_identifier)
         wait_return()
 
 
 @developer.command(cls=Command)
 @click.argument('out', type=click.File('wb'))
-def screenshot(lockdown: LockdownClient, out):
+def screenshot(service_provider: LockdownClient, out):
     """ take a screenshot in PNG format """
-    out.write(ScreenshotService(lockdown=lockdown).take_screenshot())
+    out.write(ScreenshotService(lockdown=service_provider).take_screenshot())
 
 
 @developer.group('debugserver')
 def debugserver():
     """ debugserver options. """
     pass
 
 
 @debugserver.command('applist', cls=Command)
-def debugserver_applist(lockdown: LockdownClient):
+def debugserver_applist(service_provider: LockdownClient):
     """ get applist xml """
-    print_json(DebugServerAppList(lockdown).get())
+    print_json(DebugServerAppList(service_provider).get())
 
 
 @debugserver.command('start-server', cls=Command)
 @click.argument('local_port', type=click.INT)
-def debugserver_start_server(lockdown: LockdownClient, local_port):
+def debugserver_start_server(service_provider: LockdownClient, local_port):
     """
     start a debugserver at remote listening on a given port locally.
 
     Please note the connection must be done soon afterwards using your own lldb client.
     This can be done using the following commands within lldb shell:
 
     (lldb) platform select remote-ios
 
     (lldb) platform connect connect://localhost:<local_port>
     """
-    attr = lockdown.get_service_connection_attributes('com.apple.debugserver.DVTSecureSocketProxy')
-    TcpForwarder(local_port, attr['Port'], serial=lockdown.identifier,
+    attr = service_provider.get_service_connection_attributes('com.apple.debugserver.DVTSecureSocketProxy')
+    TcpForwarder(local_port, attr['Port'], serial=service_provider.identifier,
                  enable_ssl=attr.get('EnableServiceSSL', False)).start()
 
 
 @developer.group('arbitration')
 def arbitration():
     """ arbitration options. """
     pass
 
 
 @arbitration.command('version', cls=Command)
 @click.option('--color/--no-color', default=True)
-def version(lockdown: LockdownClient, color):
+def version(service_provider: LockdownClient, color):
     """ get arbitration version """
-    with DtDeviceArbitration(lockdown) as device_arbitration:
+    with DtDeviceArbitration(service_provider) as device_arbitration:
         print_json(device_arbitration.version, colored=color)
 
 
 @arbitration.command('check-in', cls=Command)
 @click.argument('hostname')
 @click.option('-f', '--force', default=False, is_flag=True)
-def check_in(lockdown: LockdownClient, hostname, force):
+def check_in(service_provider: LockdownClient, hostname, force):
     """ owner check-in """
-    with DtDeviceArbitration(lockdown) as device_arbitration:
+    with DtDeviceArbitration(service_provider) as device_arbitration:
         try:
             device_arbitration.check_in(hostname, force=force)
             wait_return()
         except DeviceAlreadyInUseError as e:
             logger.error(e.message)
 
 
 @arbitration.command('check-out', cls=Command)
-def check_out(lockdown: LockdownClient):
+def check_out(service_provider: LockdownClient):
     """ owner check-out """
-    with DtDeviceArbitration(lockdown) as device_arbitration:
+    with DtDeviceArbitration(service_provider) as device_arbitration:
         device_arbitration.check_out()
 
 
 @dvt.command('har', cls=Command)
-def dvt_har(lockdown: LockdownClient):
+def dvt_har(service_provider: LockdownClient):
     """ enable har-logging """
-    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+    with DvtSecureSocketProxyService(lockdown=service_provider) as dvt:
         print('> Press Ctrl-C to abort')
         with ActivityTraceTap(dvt, enable_http_archive_logging=True) as tap:
             while True:
                 tap.channel.receive_message()
+
+
+@developer.group()
+def core_device():
+    """ core-device options """
+    pass
+
+
+@core_device.command('list-processes', cls=RSDCommand)
+@click.option('--color/--no-color', default=True)
+def core_device_list_processes(service_provider: RemoteServiceDiscoveryService, color: bool):
+    """ Get process list """
+    with AppServiceService(service_provider) as app_service:
+        print_json(app_service.list_processes(), colored=color)
+
+
+@core_device.command('uninstall', cls=RSDCommand)
+@click.argument('bundle_identifier')
+def core_device_uninstall_app(service_provider: RemoteServiceDiscoveryService, bundle_identifier: str):
+    """ Uninstall application """
+    with AppServiceService(service_provider) as app_service:
+        app_service.uninstall_app(bundle_identifier)
+
+
+@core_device.command('send-signal-to-process', cls=RSDCommand)
+@click.argument('pid', type=click.INT)
+@click.argument('signal', type=click.INT)
+@click.option('--color/--no-color', default=True)
+def core_device_send_signal_to_process(service_provider: RemoteServiceDiscoveryService, pid: int, signal: int,
+                                       color: bool):
+    """ Send signal to process """
+    with AppServiceService(service_provider) as app_service:
+        print_json(app_service.send_signal_to_process(pid, signal), colored=color)
+
+
+@core_device.command('get-device-info', cls=RSDCommand)
+@click.option('--color/--no-color', default=True)
+def core_device_get_device_info(service_provider: RemoteServiceDiscoveryService, color: bool):
+    """ Get device information """
+    with DeviceInfoService(service_provider) as app_service:
+        print_json(app_service.get_device_info(), colored=color)
+
+
+@core_device.command('get-lockstate', cls=RSDCommand)
+@click.option('--color/--no-color', default=True)
+def core_device_get_lockstate(service_provider: RemoteServiceDiscoveryService, color: bool):
+    """ Get lockstate """
+    with DeviceInfoService(service_provider) as app_service:
+        print_json(app_service.get_lockstate(), colored=color)
+
+
+@core_device.command('list-apps', cls=RSDCommand)
+@click.option('--color/--no-color', default=True)
+def core_device_list_apps(service_provider: RemoteServiceDiscoveryService, color: bool):
+    """ Get application list """
+    with AppServiceService(service_provider) as app_service:
+        print_json(app_service.list_apps(), colored=color)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/diagnostics.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/diagnostics.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,74 +19,75 @@
 @cli.group()
 def diagnostics():
     """ diagnostics options """
     pass
 
 
 @diagnostics.command('restart', cls=Command)
-def diagnostics_restart(lockdown: LockdownClient):
+def diagnostics_restart(service_provider: LockdownClient):
     """ restart device """
-    DiagnosticsService(lockdown=lockdown).restart()
+    DiagnosticsService(lockdown=service_provider).restart()
 
 
 @diagnostics.command('shutdown', cls=Command)
-def diagnostics_shutdown(lockdown: LockdownClient):
+def diagnostics_shutdown(service_provider: LockdownClient):
     """ shutdown device """
-    DiagnosticsService(lockdown=lockdown).shutdown()
+    DiagnosticsService(lockdown=service_provider).shutdown()
 
 
 @diagnostics.command('sleep', cls=Command)
-def diagnostics_sleep(lockdown: LockdownClient):
+def diagnostics_sleep(service_provider: LockdownClient):
     """ put device into sleep """
-    DiagnosticsService(lockdown=lockdown).sleep()
+    DiagnosticsService(lockdown=service_provider).sleep()
 
 
 @diagnostics.command('info', cls=Command)
 @click.option('--color/--no-color', default=True)
-def diagnostics_info(lockdown: LockdownClient, color):
+def diagnostics_info(service_provider: LockdownClient, color):
     """ get diagnostics info """
-    print_json(DiagnosticsService(lockdown=lockdown).info(), colored=color)
+    print_json(DiagnosticsService(lockdown=service_provider).info(), colored=color)
 
 
 @diagnostics.command('ioregistry', cls=Command)
 @click.option('--plane')
 @click.option('--name')
 @click.option('--ioclass')
 @click.option('--color/--no-color', default=True)
-def diagnostics_ioregistry(lockdown: LockdownClient, plane, name, ioclass, color):
+def diagnostics_ioregistry(service_provider: LockdownClient, plane, name, ioclass, color):
     """ get ioregistry info """
-    print_json(DiagnosticsService(lockdown=lockdown).ioregistry(plane=plane, name=name, ioclass=ioclass), colored=color)
+    print_json(DiagnosticsService(lockdown=service_provider).ioregistry(plane=plane, name=name, ioclass=ioclass),
+               colored=color)
 
 
 @diagnostics.command('mg', cls=Command)
 @click.argument('keys', nargs=-1, default=None)
 @click.option('--color/--no-color', default=True)
-def diagnostics_mg(lockdown: LockdownClient, keys, color):
+def diagnostics_mg(service_provider: LockdownClient, keys, color):
     """ get MobileGestalt key values from given list. If empty, return all known. """
-    print_json(DiagnosticsService(lockdown=lockdown).mobilegestalt(keys=keys), colored=color)
+    print_json(DiagnosticsService(lockdown=service_provider).mobilegestalt(keys=keys), colored=color)
 
 
 @diagnostics.group('battery')
 def diagnostics_battery():
     """ battery options """
     pass
 
 
 @diagnostics_battery.command('single', cls=Command)
 @click.option('--color/--no-color', default=True)
-def diagnostics_battery_single(lockdown: LockdownClient, color):
+def diagnostics_battery_single(service_provider: LockdownClient, color):
     """ get single snapshot of battery data """
-    raw_info = DiagnosticsService(lockdown=lockdown).get_battery()
+    raw_info = DiagnosticsService(lockdown=service_provider).get_battery()
     print_json(raw_info, colored=color)
 
 
 @diagnostics_battery.command('monitor', cls=Command)
-def diagnostics_battery_monitor(lockdown: LockdownClient):
+def diagnostics_battery_monitor(service_provider: LockdownClient):
     """ monitor battery usage """
-    diagnostics = DiagnosticsService(lockdown=lockdown)
+    diagnostics = DiagnosticsService(lockdown=service_provider)
     while True:
         raw_info = diagnostics.get_battery()
         info = {
             'InstantAmperage': raw_info.get('InstantAmperage'),
             'Temperature': raw_info.get('Temperature'),
             'Voltage': raw_info.get('Voltage'),
             'IsCharging': raw_info.get('IsCharging'),
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/lockdown.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/lockdown.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,116 +19,116 @@
 @cli.group('lockdown')
 def lockdown_group():
     """ lockdown options """
     pass
 
 
 @lockdown_group.command('recovery', cls=Command)
-def lockdown_recovery(lockdown: LockdownClient):
+def lockdown_recovery(service_provider: LockdownClient):
     """ enter recovery """
-    print_json(lockdown.enter_recovery())
+    print_json(service_provider.enter_recovery())
 
 
 @lockdown_group.command('service', cls=Command)
 @click.argument('service_name')
-def lockdown_service(lockdown: LockdownClient, service_name):
+def lockdown_service(service_provider: LockdownClient, service_name):
     """ send-receive raw service messages """
-    lockdown.start_service(service_name).shell()
+    service_provider.start_lockdown_service(service_name).shell()
 
 
 @lockdown_group.command('info', cls=Command)
 @click.option('-a', '--all', is_flag=True, help='include all domain information')
 @click.option('--color/--no-color', default=True)
-def lockdown_info(lockdown: LockdownClient, all, color):
+def lockdown_info(service_provider: LockdownClient, all, color):
     """ query all lockdown values """
-    print_json(lockdown.all_domains if all else lockdown.all_values, colored=color)
+    print_json(service_provider.all_domains if all else service_provider.all_values, colored=color)
 
 
 @lockdown_group.command('get', cls=Command)
 @click.argument('domain', required=False)
 @click.argument('key', required=False)
 @click.option('--color/--no-color', default=True)
-def lockdown_get(lockdown: LockdownClient, domain, key, color):
+def lockdown_get(service_provider: LockdownClient, domain, key, color):
     """ query lockdown values by their domain and key names """
-    print_json(lockdown.get_value(domain=domain, key=key), colored=color)
+    print_json(service_provider.get_value(domain=domain, key=key), colored=color)
 
 
 @lockdown_group.command('set', cls=Command)
 @click.argument('value')
 @click.argument('domain', required=False)
 @click.argument('key', required=False)
 @click.option('--color/--no-color', default=True)
-def lockdown_set(lockdown: LockdownClient, value, domain, key, color):
+def lockdown_set(service_provider: LockdownClient, value, domain, key, color):
     """ set a lockdown value using python's eval() """
-    print_json(lockdown.set_value(value=eval(value), domain=domain, key=key), colored=color)
+    print_json(service_provider.set_value(value=eval(value), domain=domain, key=key), colored=color)
 
 
 @lockdown_group.command('remove', cls=Command)
 @click.argument('domain')
 @click.argument('key')
 @click.option('--color/--no-color', default=True)
-def lockdown_remove(lockdown: LockdownClient, domain, key, color):
+def lockdown_remove(service_provider: LockdownClient, domain, key, color):
     """ remove a domain/key pair """
-    print_json(lockdown.remove_value(domain=domain, key=key), colored=color)
+    print_json(service_provider.remove_value(domain=domain, key=key), colored=color)
 
 
 @lockdown_group.command('unpair', cls=CommandWithoutAutopair)
 @click.argument('host_id', required=False)
-def lockdown_unpair(lockdown: LockdownClient, host_id: str = None):
+def lockdown_unpair(service_provider: LockdownClient, host_id: str = None):
     """ unpair from connected device """
-    lockdown.unpair(host_id=host_id)
+    service_provider.unpair(host_id=host_id)
 
 
 @lockdown_group.command('pair', cls=CommandWithoutAutopair)
-def lockdown_pair(lockdown: LockdownClient):
+def lockdown_pair(service_provider: LockdownClient):
     """ pair device """
-    lockdown.pair()
+    service_provider.pair()
 
 
 @lockdown_group.command('save-pair-record', cls=CommandWithoutAutopair)
 @click.argument('output', type=click.File('wb'))
-def lockdown_save_pair_record(lockdown: LockdownClient, output):
+def lockdown_save_pair_record(service_provider: LockdownClient, output):
     """ save pair record to specified location """
-    if lockdown.pair_record is None:
+    if service_provider.pair_record is None:
         logger.error('no pairing record was found')
         return
-    plistlib.dump(lockdown.pair_record, output)
+    plistlib.dump(service_provider.pair_record, output)
 
 
 @lockdown_group.command('date', cls=Command)
-def lockdown_date(lockdown: LockdownClient):
+def lockdown_date(service_provider: LockdownClient):
     """ get device date """
-    print(lockdown.date)
+    print(service_provider.date)
 
 
 @lockdown_group.command('heartbeat', cls=Command)
-def lockdown_heartbeat(lockdown: LockdownClient):
+def lockdown_heartbeat(service_provider: LockdownClient):
     """ start heartbeat service """
-    HeartbeatService(lockdown).start()
+    HeartbeatService(service_provider).start()
 
 
 @lockdown_group.command('language', cls=Command)
-def lockdown_language(lockdown: LockdownClient):
+def lockdown_language(service_provider: LockdownClient):
     """ get current language settings """
-    print(f'{lockdown.language} {lockdown.locale}')
+    print(f'{service_provider.language} {service_provider.locale}')
 
 
 @lockdown_group.command('device-name', cls=Command)
 @click.argument('new_name', required=False)
-def lockdown_device_name(lockdown: LockdownClient, new_name):
+def lockdown_device_name(service_provider: LockdownClient, new_name):
     """ get/set current device name """
     if new_name:
-        lockdown.set_value(new_name, key='DeviceName')
+        service_provider.set_value(new_name, key='DeviceName')
     else:
-        print(f'{lockdown.get_value(key="DeviceName")}')
+        print(f'{service_provider.get_value(key="DeviceName")}')
 
 
 @lockdown_group.command('wifi-connections', cls=Command)
 @click.argument('state', type=click.Choice(['on', 'off']), required=False)
-def lockdown_wifi_connections(lockdown: LockdownClient, state):
+def lockdown_wifi_connections(service_provider: LockdownClient, state):
     """ get/set wifi connections state """
     if not state:
         # show current state
-        print_json(lockdown.get_value(domain='com.apple.mobile.wireless_lockdown'))
+        print_json(service_provider.get_value(domain='com.apple.mobile.wireless_lockdown'))
     else:
         # enable/disable
-        lockdown.enable_wifi_connections = state == 'on'
+        service_provider.enable_wifi_connections = state == 'on'
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/notification.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/notification.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,37 +21,37 @@
     """ notification options """
     pass
 
 
 @notification.command(cls=Command)
 @click.argument('names', nargs=-1)
 @click.option('--insecure', is_flag=True, help='use the insecure relay meant for untrusted clients instead')
-def post(lockdown: LockdownClient, names, insecure):
+def post(service_provider: LockdownClient, names, insecure):
     """ API for notify_post(). """
-    service = NotificationProxyService(lockdown=lockdown, insecure=insecure)
+    service = NotificationProxyService(lockdown=service_provider, insecure=insecure)
     for name in names:
         service.notify_post(name)
 
 
 @notification.command(cls=Command)
 @click.argument('names', nargs=-1)
 @click.option('--insecure', is_flag=True, help='use the insecure relay meant for untrusted clients instead')
-def observe(lockdown: LockdownClient, names, insecure):
+def observe(service_provider: LockdownClient, names, insecure):
     """ API for notify_register_dispatch(). """
-    service = NotificationProxyService(lockdown=lockdown, insecure=insecure)
+    service = NotificationProxyService(lockdown=service_provider, insecure=insecure)
     for name in names:
         service.notify_register_dispatch(name)
 
     for event in service.receive_notification():
         logger.info(event)
 
 
 @notification.command('observe-all', cls=Command)
 @click.option('--insecure', is_flag=True, help='use the insecure relay meant for untrusted clients instead')
-def observe_all(lockdown: LockdownClient, insecure):
+def observe_all(service_provider: LockdownClient, insecure):
     """ attempt to observe all builtin firmware notifications. """
-    service = NotificationProxyService(lockdown=lockdown, insecure=insecure)
+    service = NotificationProxyService(lockdown=service_provider, insecure=insecure)
     for notification in get_notifications():
         service.notify_register_dispatch(notification)
 
     for event in service.receive_notification():
         logger.info(event)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/pcap.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/pcap.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 
 
 @cli.command(cls=Command)
 @click.argument('out', type=click.File('wb'), required=False)
 @click.option('-c', '--count', type=click.INT, default=-1, help='Number of packets to sniff. Omit to endless sniff.')
 @click.option('--process', default=None, help='Process to filter. Omit for all.')
 @click.option('--color/--no-color', default=True)
-def pcap(lockdown: LockdownClient, out: IO, count: int, process: str, color: bool):
+def pcap(service_provider: LockdownClient, out: IO, count: int, process: str, color: bool):
     """ sniff device traffic """
-    service = PcapdService(lockdown=lockdown)
+    service = PcapdService(lockdown=service_provider)
     packets_generator = service.watch(packets_count=count, process=process)
 
     if out is not None:
         packets_generator_with_print = map(lambda p: print_packet(p, color), packets_generator)
         service.write_to_pcap(out, packets_generator_with_print)
         return
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/power_assertion.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/power_assertion.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 
 @cli.command('power-assertion', cls=Command)
 @click.argument('type', type=click.Choice(
     ['AMDPowerAssertionTypeWirelessSync', 'PreventUserIdleSystemSleep', 'PreventSystemSleep']))
 @click.argument('name')
 @click.argument('timeout', type=click.INT)
 @click.argument('details', required=False)
-def power_assertion(lockdown: LockdownClient, type, name, timeout, details):
+def power_assertion(service_provider: LockdownClient, type, name, timeout, details):
     """ Create a power assertion (wraps IOPMAssertionCreateWithName()) """
-    with PowerAssertionService(lockdown).create_power_assertion(type, name, timeout, details):
+    with PowerAssertionService(service_provider).create_power_assertion(type, name, timeout, details):
         print('> Hit Ctrl+C to exit')
         time.sleep(timeout)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/profile.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/profile.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,66 +18,66 @@
 @cli.group('profile')
 def profile_group():
     """ profile options """
     pass
 
 
 @profile_group.command('list', cls=Command)
-def profile_list(lockdown: LockdownClient):
+def profile_list(service_provider: LockdownClient):
     """ list installed profiles """
-    print_json(MobileConfigService(lockdown=lockdown).get_profile_list())
+    print_json(MobileConfigService(lockdown=service_provider).get_profile_list())
 
 
 @profile_group.command('install', cls=Command)
 @click.argument('profiles', nargs=-1, type=click.File('rb'))
-def profile_install(lockdown: LockdownClient, profiles):
+def profile_install(service_provider: LockdownClient, profiles):
     """ install given profiles """
-    service = MobileConfigService(lockdown=lockdown)
+    service = MobileConfigService(lockdown=service_provider)
     for profile in profiles:
         logger.info(f'installing {profile.name}')
         service.install_profile(profile.read())
 
 
 @profile_group.command('install-silent', cls=Command)
 @click.option('--keystore', type=click.File('rb'), required=True,
               help="A PKCS#12 keystore containing the certificate and private key which can supervise the device.")
 @click.option('--keystore-password', prompt=True, required=True, hide_input=True,
               help="The password for the PKCS#12 keystore.")
 @click.argument('profiles', nargs=-1, type=click.File('rb'))
-def profile_install_silent(lockdown: LockdownClient, profiles, keystore, keystore_password):
+def profile_install_silent(service_provider: LockdownClient, profiles, keystore, keystore_password):
     """ install given profiles without user interaction (requires the device to be supervised) """
-    service = MobileConfigService(lockdown=lockdown)
+    service = MobileConfigService(lockdown=service_provider)
     for profile in profiles:
         logger.info(f'installing {profile.name}')
         service.install_profile_silent(
             profile.read(), keystore.read(), keystore_password)
 
 
 @profile_group.command('cloud-configuration', cls=Command)
 @click.option('--color/--no-color', default=True)
-def profile_cloud_configuration(lockdown: LockdownClient, color):
+def profile_cloud_configuration(service_provider: LockdownClient, color):
     """ get cloud configuration """
-    print_json(MobileConfigService(lockdown=lockdown).get_cloud_configuration(), colored=color)
+    print_json(MobileConfigService(lockdown=service_provider).get_cloud_configuration(), colored=color)
 
 
 @profile_group.command('store', cls=Command)
 @click.argument('profiles', nargs=-1, type=click.File('rb'))
-def profile_store(lockdown: LockdownClient, profiles):
+def profile_store(service_provider: LockdownClient, profiles):
     """ store profile """
-    service = MobileConfigService(lockdown=lockdown)
+    service = MobileConfigService(lockdown=service_provider)
     for profile in profiles:
         logger.info(f'storing {profile.name}')
         service.store_profile(profile.read())
 
 
 @profile_group.command('remove', cls=Command)
 @click.argument('name')
-def profile_remove(lockdown: LockdownClient, name):
+def profile_remove(service_provider: LockdownClient, name):
     """ remove profile by name """
-    MobileConfigService(lockdown=lockdown).remove_profile(name)
+    MobileConfigService(lockdown=service_provider).remove_profile(name)
 
 
 @profile_group.command('set-wifi-power', cls=Command)
 @click.argument('state', type=click.Choice(['on', 'off']), required=False)
-def profile_set_wifi_power(lockdown: LockdownClient, state):
+def profile_set_wifi_power(service_provider: LockdownClient, state):
     """ change Wi-Fi power state """
-    MobileConfigService(lockdown=lockdown).set_wifi_power_state(state == 'on')
+    MobileConfigService(lockdown=service_provider).set_wifi_power_state(state == 'on')
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/provision.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/provision.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,41 +20,41 @@
 def provision():
     """ privision options """
     pass
 
 
 @provision.command('install', cls=Command)
 @click.argument('profile', type=click.File('rb'))
-def provision_install(lockdown: LockdownClient, profile):
+def provision_install(service_provider: LockdownClient, profile):
     """ install a provision profile (.mobileprovision file) """
-    MisagentService(lockdown=lockdown).install(profile)
+    MisagentService(lockdown=service_provider).install(profile)
 
 
 @provision.command('remove', cls=Command)
 @click.argument('profile_id')
-def provision_remove(lockdown: LockdownClient, profile_id):
+def provision_remove(service_provider: LockdownClient, profile_id):
     """ remove a provision profile """
-    MisagentService(lockdown=lockdown).remove(profile_id)
+    MisagentService(lockdown=service_provider).remove(profile_id)
 
 
 @provision.command('clear', cls=Command)
-def provision_clear(lockdown: LockdownClient):
+def provision_clear(service_provider: LockdownClient):
     """ remove all provision profiles """
-    for profile in MisagentService(lockdown=lockdown).copy_all():
-        MisagentService(lockdown=lockdown).remove(profile.plist['UUID'])
+    for profile in MisagentService(lockdown=service_provider).copy_all():
+        MisagentService(lockdown=service_provider).remove(profile.plist['UUID'])
 
 
 @provision.command('list', cls=Command)
 @click.option('--color/--no-color', default=True)
-def provision_list(lockdown: LockdownClient, color):
+def provision_list(service_provider: LockdownClient, color):
     """ list installed provision profiles """
-    print_json([p.plist for p in MisagentService(lockdown=lockdown).copy_all()], colored=color)
+    print_json([p.plist for p in MisagentService(lockdown=service_provider).copy_all()], colored=color)
 
 
 @provision.command('dump', cls=Command)
 @click.argument('out', type=click.Path(file_okay=False, dir_okay=True, exists=True))
-def provision_dump(lockdown: LockdownClient, out):
+def provision_dump(service_provider: LockdownClient, out):
     """ dump installed provision profiles to specified location """
-    for profile in MisagentService(lockdown=lockdown).copy_all():
+    for profile in MisagentService(lockdown=service_provider).copy_all():
         filename = f'{profile.plist["UUID"]}.mobileprovision'
         logger.info(f'downloading {filename}')
         (Path(out) / filename).write_bytes(profile.buf)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/restore.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/springboard.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/springboard.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,42 +26,42 @@
 def state():
     """ icons state options """
     pass
 
 
 @state.command('get', cls=Command)
 @click.option('--color/--no-color', default=True)
-def state_get(lockdown: LockdownClient, color):
+def state_get(service_provider: LockdownClient, color):
     """ get icon state """
-    print_json(SpringBoardServicesService(lockdown=lockdown).get_icon_state(), colored=color)
+    print_json(SpringBoardServicesService(lockdown=service_provider).get_icon_state(), colored=color)
 
 
 @springboard.command('shell', cls=Command)
-def springboard_shell(lockdown: LockdownClient):
+def springboard_shell(service_provider: LockdownClient):
     """ open a shell to communicate with SpringBoardServicesService """
-    service = SpringBoardServicesService(lockdown=lockdown)
+    service = SpringBoardServicesService(lockdown=service_provider)
     IPython.embed(
         header=SHELL_USAGE,
         user_ns={
             'service': service,
         })
 
 
 @springboard.command('icon', cls=Command)
 @click.argument('bundle_id')
 @click.argument('out', type=click.File('wb'))
-def springboard_icon(lockdown: LockdownClient, bundle_id, out):
+def springboard_icon(service_provider: LockdownClient, bundle_id, out):
     """ get application's icon """
-    out.write(SpringBoardServicesService(lockdown=lockdown).get_icon_pngdata(bundle_id))
+    out.write(SpringBoardServicesService(lockdown=service_provider).get_icon_pngdata(bundle_id))
 
 
 @springboard.command('orientation', cls=Command)
 def springboard_orientation(lockdown: LockdownClient):
     """ get screen orientation """
     print(SpringBoardServicesService(lockdown=lockdown).get_interface_orientation())
 
 
 @springboard.command('wallpaper', cls=Command)
 @click.argument('out', type=click.File('wb'))
-def springboard_wallpaper(lockdown: LockdownClient, out):
+def springboard_wallpaper(service_provider: LockdownClient, out):
     """ get wallpapaer """
-    out.write(SpringBoardServicesService(lockdown=lockdown).get_wallpaper_pngdata())
+    out.write(SpringBoardServicesService(lockdown=service_provider).get_wallpaper_pngdata())
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/syslog.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/syslog.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 @cli.group()
 def syslog():
     """ syslog options """
     pass
 
 
 @syslog.command('live-old', cls=Command)
-def syslog_live_old(lockdown: LockdownClient):
+def syslog_live_old(service_provider: LockdownClient):
     """ view live syslog lines in raw bytes form from old relay """
-    for line in SyslogService(lockdown=lockdown).watch():
+    for line in SyslogService(lockdown=service_provider).watch():
         print(line)
 
 
 def format_line(color, pid, syslog_entry, include_label):
     log_level_colors = {
         'Notice': 'white',
         'Error': 'red',
@@ -86,27 +86,28 @@
 @click.option('--pid', type=click.INT, default=-1, help='pid to filter. -1 for all')
 @click.option('-pn', '--process-name', help='process name to filter')
 @click.option('-m', '--match', multiple=True, help='match expression')
 @click.option('-mi', '--match-insensitive', multiple=True, help='insensitive match expression')
 @click.option('include_label', '--label', is_flag=True, help='should include label')
 @click.option('-e', '--regex', multiple=True, help='filter only lines matching given regex')
 @click.option('-ei', '--insensitive-regex', multiple=True, help='filter only lines matching given regex (insensitive)')
-def syslog_live(lockdown: LockdownClient, out, color, pid, process_name, match, match_insensitive, include_label, regex,
+def syslog_live(service_provider: LockdownClient, out, color, pid, process_name, match, match_insensitive,
+                include_label, regex,
                 insensitive_regex):
     """ view live syslog lines """
 
     match_regex = [re.compile(f'.*({r}).*') for r in regex]
     match_regex += [re.compile(f'.*({r}).*', re.IGNORECASE) for r in insensitive_regex]
 
     def replace(m):
         if len(m.groups()):
             return line.replace(m.group(1), colored(m.group(1), attrs=['bold', 'underline']))
         return None
 
-    for syslog_entry in OsTraceService(lockdown=lockdown).syslog(pid=pid):
+    for syslog_entry in OsTraceService(lockdown=service_provider).syslog(pid=pid):
         if process_name:
             if posixpath.basename(syslog_entry.filename) != process_name:
                 continue
 
         line = format_line(color, pid, syslog_entry, include_label)
 
         skip = False
@@ -153,15 +154,15 @@
 
 
 @syslog.command('collect', cls=Command)
 @click.argument('out', type=click.Path(exists=False, dir_okay=True, file_okay=True))
 @click.option('--size-limit', type=click.INT)
 @click.option('--age-limit', type=click.INT)
 @click.option('--start-time', type=click.INT)
-def syslog_collect(lockdown: LockdownClient, out, size_limit, age_limit, start_time):
+def syslog_collect(service_provider: LockdownClient, out, size_limit, age_limit, start_time):
     """
     Collect the system logs into a .logarchive that can be viewed later with tools such as log or Console.
     If the filename doesn't exist, system_logs.logarchive will be created in the given directory.
     """
 
     if os.path.isdir(out):
         out = os.path.join(out, 'system_logs.logarchive')
@@ -169,8 +170,9 @@
     if not os.path.exists(out):
         os.makedirs(out)
 
     if not out.endswith('.logarchive'):
         logger.warning('given out path doesn\'t end with a .logarchive - consider renaming to be able to view '
                        'the file with the likes of the Console.app and the `log show` utilities')
 
-    OsTraceService(lockdown=lockdown).collect(out, size_limit=size_limit, age_limit=age_limit, start_time=start_time)
+    OsTraceService(lockdown=service_provider).collect(out, size_limit=size_limit, age_limit=age_limit,
+                                                      start_time=start_time)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/usbmux.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/usbmux.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/cli/webinspector.py` & `pymobiledevice3-2.1.0/pymobiledevice3/cli/webinspector.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,23 +71,23 @@
     return inspector, application
 
 
 @webinspector.command(cls=Command)
 @click.option('-v', '--verbose', is_flag=True)
 @click.option('-t', '--timeout', default=3, show_default=True, type=float)
 @catch_errors
-def opened_tabs(lockdown: LockdownClient, verbose, timeout):
+def opened_tabs(service_provider: LockdownClient, verbose, timeout):
     """
     Show all currently opened tabs.
 
     \b
     Opt-in:
         Settings -> Safari -> Advanced -> Web Inspector
     """
-    inspector = WebinspectorService(lockdown=lockdown, loop=asyncio.get_event_loop())
+    inspector = WebinspectorService(lockdown=service_provider, loop=asyncio.get_event_loop())
     inspector.connect(timeout)
     while not inspector.connected_application:
         inspector.flush_input()
     reload_pages(inspector)
     for app_id, app_ in inspector.connected_application.items():
         if app_id not in inspector.application_pages:
             continue
@@ -103,24 +103,24 @@
     inspector.close()
 
 
 @webinspector.command(cls=Command)
 @click.argument('url')
 @click.option('-t', '--timeout', default=3, show_default=True, type=float)
 @catch_errors
-def launch(lockdown: LockdownClient, url, timeout):
+def launch(service_provider: LockdownClient, url, timeout):
     """
     Launch a specific URL in Safari.
 
     \b
     Opt-in:
         Settings -> Safari -> Advanced -> Web Inspector
         Settings -> Safari -> Advanced -> Remote Automation
     """
-    inspector, safari = create_webinspector_and_launch_app(lockdown, timeout, SAFARI)
+    inspector, safari = create_webinspector_and_launch_app(service_provider, timeout, SAFARI)
     session = inspector.automation_session(safari)
     driver = WebDriver(session)
     print('Starting session')
     driver.start_session()
     print('Getting URL')
     driver.get(url)
     wait_return()
@@ -148,24 +148,24 @@
 # See selenium api for more features.
 '''
 
 
 @webinspector.command(cls=Command)
 @click.option('-t', '--timeout', default=3, show_default=True, type=float)
 @catch_errors
-def shell(lockdown: LockdownClient, timeout):
+def shell(service_provider: LockdownClient, timeout):
     """
     Create an IPython shell for interacting with a WebView.
 
     \b
     Opt-in:
         Settings -> Safari -> Advanced -> Web Inspector
         Settings -> Safari -> Advanced -> Remote Automation
     """
-    inspector, safari = create_webinspector_and_launch_app(lockdown, timeout, SAFARI)
+    inspector, safari = create_webinspector_and_launch_app(service_provider, timeout, SAFARI)
     session = inspector.automation_session(safari)
     driver = WebDriver(session)
     try:
         IPython.embed(
             header=highlight(SHELL_USAGE, lexers.PythonLexer(), formatters.TerminalTrueColorFormatter(style='native')),
             user_ns={
                 'driver': driver,
@@ -178,54 +178,54 @@
 
 
 @webinspector.command(cls=Command)
 @click.option('-t', '--timeout', default=3, show_default=True, type=float)
 @click.option('--automation', is_flag=True, help='Use remote automation')
 @click.argument('url', required=False, default='')
 @catch_errors
-def js_shell(lockdown: LockdownClient, timeout, automation, url):
+def js_shell(service_provider: LockdownClient, timeout, automation, url):
     """
     Create a javascript shell. This interpreter runs on your local machine,
     but evaluates each expression on the remote
 
     \b
     Opt-in:
         Settings -> Safari -> Advanced -> Web Inspector
 
     \b
     for automation also enable:
         Settings -> Safari -> Advanced -> Remote Automation
     """
 
     js_shell_class = AutomationJsShell if automation else InspectorJsShell
-    asyncio.run(run_js_shell(js_shell_class, lockdown, timeout, url))
+    asyncio.run(run_js_shell(js_shell_class, service_provider, timeout, url))
 
 
 udid = ''
 
 
 def create_app():
     inspector = WebinspectorService(lockdown=create_using_usbmux(udid))
     app.state.inspector = inspector
     return app
 
 
 @webinspector.command(cls=Command)
 @click.option('--host', default='127.0.0.1')
 @click.option('--port', type=click.INT, default=9222)
-def cdp(lockdown: LockdownClient, host, port):
+def cdp(service_provider: LockdownClient, host, port):
     """
     Start a CDP server for debugging WebViews.
 
     \b
     In order to debug the WebView that way, open in Google Chrome:
         chrome://inspect/#devices
     """
     global udid
-    udid = lockdown.udid
+    udid = service_provider.udid
     uvicorn.run('pymobiledevice3.cli.webinspector:create_app', host=host, port=port, factory=True,
                 ws_ping_timeout=None, ws='wsproto', loop='asyncio')
 
 
 class JsShell(ABC):
     def __init__(self):
         super().__init__()
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/exceptions.py` & `pymobiledevice3-2.1.0/pymobiledevice3/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'NotMountedError', 'AlreadyMountedError', 'UnsupportedCommandError', 'ExtractingStackshotError',
     'ConnectionTerminatedError', 'WirError', 'WebInspectorNotEnabledError', 'RemoteAutomationNotEnabledError',
     'ArbitrationError', 'InternalError', 'DeveloperModeIsNotEnabledError', 'DeviceAlreadyInUseError', 'LockdownError',
     'PairingDialogResponsePendingError', 'UserDeniedPairingError', 'InvalidHostIDError', 'SetProhibitedError',
     'MissingValueError', 'PasscodeRequiredError', 'AmfiError', 'DeviceHasPasscodeSetError', 'NotificationTimeoutError',
     'DeveloperModeError', 'ProfileError', 'IRecvError', 'IRecvNoDeviceConnectedError',
     'NoDeviceSelectedError', 'MessageNotSupportedError', 'InvalidServiceError', 'InspectorEvaluateError',
-    'LaunchingApplicationError', 'BadCommandError', 'BadDevError', 'ConnectionFailedError',
+    'LaunchingApplicationError', 'BadCommandError', 'BadDevError', 'ConnectionFailedError', 'CoreDeviceError'
 ]
 
 
 class PyMobileDevice3Exception(Exception):
     pass
 
 
@@ -280,7 +280,11 @@
 
 class LaunchingApplicationError(PyMobileDevice3Exception):
     pass
 
 
 class AppInstallError(PyMobileDevice3Exception):
     pass
+
+
+class CoreDeviceError(PyMobileDevice3Exception):
+    pass
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/irecv.py` & `pymobiledevice3-2.1.0/pymobiledevice3/irecv.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/irecv_devices.py` & `pymobiledevice3-2.1.0/pymobiledevice3/irecv_devices.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/lockdown.py` & `pymobiledevice3-2.1.0/pymobiledevice3/lockdown.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 from pymobiledevice3 import usbmux
 from pymobiledevice3.ca import ca_do_everything
 from pymobiledevice3.exceptions import CannotStopSessionError, ConnectionTerminatedError, FatalPairingError, \
     IncorrectModeError, InvalidConnectionError, InvalidHostIDError, InvalidServiceError, LockdownError, \
     MissingValueError, NotPairedError, PairingDialogResponsePendingError, PairingError, PasswordRequiredError, \
     SetProhibitedError, StartServiceError, UserDeniedPairingError
 from pymobiledevice3.irecv_devices import IRECV_DEVICES
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
 from pymobiledevice3.pair_records import create_pairing_records_cache_folder, generate_host_id, \
     get_preferred_pair_record
-from pymobiledevice3.service_connection import ServiceConnection
+from pymobiledevice3.service_connection import LockdownServiceConnection
 from pymobiledevice3.usbmux import PlistMuxConnection
 from pymobiledevice3.utils import sanitize_ios_version
 
 SYSTEM_BUID = '30142955-444094379208051516'
 DOMAINS = ['com.apple.disk_usage',
            'com.apple.disk_usage.factory',
            'com.apple.mobile.battery',
@@ -96,16 +97,17 @@
             self.service = self._create_service_connection(self.port)
             self.validate_pairing()
             return f(*args, **kwargs)
 
     return _inner_reconnect_on_remote_close
 
 
-class LockdownClient(ABC):
-    def __init__(self, service: ServiceConnection, host_id: str, identifier: str = None, label: str = DEFAULT_LABEL,
+class LockdownClient(ABC, LockdownServiceProvider):
+    def __init__(self, service: LockdownServiceConnection, host_id: str, identifier: str = None,
+                 label: str = DEFAULT_LABEL,
                  system_buid: str = SYSTEM_BUID, pair_record: Mapping = None, pairing_records_cache_folder: Path = None,
                  port: int = SERVICE_PORT):
         """
         Create a LockdownClient instance
 
         :param service: lockdownd connection handler
         :param host_id: Used as the host identifier for the handshake
@@ -131,19 +133,18 @@
         if self.query_type() != 'com.apple.mobile.lockdown':
             raise IncorrectModeError()
 
         self.all_values = self.get_value()
         self.udid = self.all_values.get('UniqueDeviceID')
         self.unique_chip_id = self.all_values.get('UniqueChipID')
         self.device_public_key = self.all_values.get('DevicePublicKey')
-        self.product_version = self.all_values.get('ProductVersion')
         self.product_type = self.all_values.get('ProductType')
 
     @classmethod
-    def create(cls, service: ServiceConnection, identifier: str = None, system_buid: str = SYSTEM_BUID,
+    def create(cls, service: LockdownServiceConnection, identifier: str = None, system_buid: str = SYSTEM_BUID,
                label: str = DEFAULT_LABEL, autopair: bool = True, pair_timeout: int = None, local_hostname: str = None,
                pair_record: Mapping = None, pairing_records_cache_folder: Path = None, port: int = SERVICE_PORT,
                **cls_specific_args):
         """
         Create a LockdownClient instance
 
         :param service: lockdownd connection handler
@@ -177,14 +178,18 @@
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     @property
+    def product_version(self) -> str:
+        return self.all_values.get('ProductVersion')
+
+    @property
     def device_class(self) -> DeviceClass:
         try:
             return DeviceClass(self.all_values.get('DeviceClass'))
         except ValueError:
             return DeviceClass('Unknown')
 
     @property
@@ -442,42 +447,32 @@
             if response.get('Error', '') == 'PasswordProtected':
                 raise PasswordRequiredError(
                     'your device is protected with password, please enter password in device and try again')
             raise StartServiceError(response.get('Error'))
         return response
 
     @_reconnect_on_remote_close
-    def start_service(self, name: str, escrow_bag=None) -> ServiceConnection:
+    def start_lockdown_service(self, name: str, escrow_bag: bytes = None) -> LockdownServiceConnection:
         attr = self.get_service_connection_attributes(name, escrow_bag=escrow_bag)
         service_connection = self._create_service_connection(attr['Port'])
 
         if attr.get('EnableServiceSSL', False):
             with self.ssl_file() as f:
                 service_connection.ssl_start(f)
         return service_connection
 
-    async def aio_start_service(self, name: str, escrow_bag=None) -> ServiceConnection:
+    async def aio_start_lockdown_service(self, name: str, escrow_bag: bytes = None) -> LockdownServiceConnection:
         attr = self.get_service_connection_attributes(name, escrow_bag=escrow_bag)
         service_connection = self._create_service_connection(attr['Port'])
 
         if attr.get('EnableServiceSSL', False):
             with self.ssl_file() as f:
                 await service_connection.aio_ssl_start(f)
         return service_connection
 
-    def start_developer_service(self, name, escrow_bag=None) -> ServiceConnection:
-        try:
-            return self.start_service(name, escrow_bag)
-        except StartServiceError:
-            self.logger.error(
-                'Failed to connect to required service. Make sure DeveloperDiskImage.dmg has been mounted. '
-                'You can do so using: pymobiledevice3 mounter mount'
-            )
-            raise
-
     def close(self) -> None:
         self.service.close()
 
     @contextmanager
     def ssl_file(self) -> str:
         cert_pem = self.pair_record['HostCertificate']
         private_key_pem = self.pair_record['HostPrivateKey']
@@ -503,15 +498,15 @@
             return
         self.pair(timeout=timeout)
         # get session_id
         if not self.validate_pairing():
             raise FatalPairingError()
 
     @abstractmethod
-    def _create_service_connection(self, port: int) -> ServiceConnection:
+    def _create_service_connection(self, port: int) -> LockdownServiceConnection:
         """ Used to establish a new ServiceConnection to a given port """
         pass
 
     def _request(self, request: str, options: Mapping = None, verify_request: bool = True) -> Mapping:
         message = {'Label': self.label, 'Request': request}
         if options:
             message.update(options)
@@ -565,28 +560,29 @@
 class UsbmuxLockdownClient(LockdownClient):
     @property
     def short_info(self) -> Dict:
         short_info = super().short_info
         short_info['ConnectionType'] = self.service.mux_device.connection_type
         return short_info
 
-    def _create_service_connection(self, port: int) -> ServiceConnection:
-        return ServiceConnection.create_using_usbmux(self.identifier, port, self.service.mux_device.connection_type)
+    def _create_service_connection(self, port: int) -> LockdownServiceConnection:
+        return LockdownServiceConnection.create_using_usbmux(self.identifier, port,
+                                                             self.service.mux_device.connection_type)
 
 
 class PlistUsbmuxLockdownClient(UsbmuxLockdownClient):
     def save_pair_record(self) -> None:
         super().save_pair_record()
         record_data = plistlib.dumps(self.pair_record)
         with usbmux.create_mux() as client:
             client.save_pair_record(self.identifier, self.service.mux_device.devid, record_data)
 
 
 class TcpLockdownClient(LockdownClient):
-    def __init__(self, service: ServiceConnection, host_id: str, hostname: str, identifier: str = None,
+    def __init__(self, service: LockdownServiceConnection, host_id: str, hostname: str, identifier: str = None,
                  label: str = DEFAULT_LABEL, system_buid: str = SYSTEM_BUID, pair_record: Mapping = None,
                  pairing_records_cache_folder: Path = None, port: int = SERVICE_PORT):
         """
         Create a LockdownClient instance
 
         :param service: lockdownd connection handler
         :param host_id: Used as the host identifier for the handshake
@@ -598,16 +594,16 @@
         :param pairing_records_cache_folder: Use the following location to search and save pair records
         :param port: lockdownd service port
         """
         super().__init__(service, host_id, identifier, label, system_buid, pair_record, pairing_records_cache_folder,
                          port)
         self.hostname = hostname
 
-    def _create_service_connection(self, port: int) -> ServiceConnection:
-        return ServiceConnection.create_using_tcp(self.hostname, port)
+    def _create_service_connection(self, port: int) -> LockdownServiceConnection:
+        return LockdownServiceConnection.create_using_tcp(self.hostname, port)
 
 
 def create_using_usbmux(serial: str = None, identifier: str = None, label: str = DEFAULT_LABEL, autopair: bool = True,
                         connection_type: str = None, pair_timeout: int = None, local_hostname: str = None,
                         pair_record: Mapping = None, pairing_records_cache_folder: Path = None,
                         port: int = SERVICE_PORT) -> UsbmuxLockdownClient:
     """
@@ -621,15 +617,15 @@
     :param pair_timeout: Timeout for autopair
     :param local_hostname: Used as a seed to generate the HostID
     :param pair_record: Use this pair record instead of the default behavior (search in host/create our own)
     :param pairing_records_cache_folder: Use the following location to search and save pair records
     :param port: lockdownd service port
     :return: UsbmuxLockdownClient instance
     """
-    service = ServiceConnection.create_using_usbmux(serial, port, connection_type=connection_type)
+    service = LockdownServiceConnection.create_using_usbmux(serial, port, connection_type=connection_type)
     cls = UsbmuxLockdownClient
     with usbmux.create_mux() as client:
         if isinstance(client, PlistMuxConnection):
             # Only the Plist version of usbmuxd supports this message type
             system_buid = client.get_buid()
             cls = PlistUsbmuxLockdownClient
 
@@ -656,15 +652,15 @@
     :param pair_timeout: Timeout for autopair
     :param local_hostname: Used as a seed to generate the HostID
     :param pair_record: Use this pair record instead of the default behavior (search in host/create our own)
     :param pairing_records_cache_folder: Use the following location to search and save pair records
     :param port: lockdownd service port
     :return: TcpLockdownClient instance
     """
-    service = ServiceConnection.create_using_tcp(hostname, port)
+    service = LockdownServiceConnection.create_using_tcp(hostname, port)
     client = TcpLockdownClient.create(
         service, identifier=identifier, label=label, local_hostname=local_hostname, pair_record=pair_record,
         pairing_records_cache_folder=pairing_records_cache_folder, pair_timeout=pair_timeout, autopair=autopair,
         port=port, hostname=hostname)
     return client
 
 
@@ -682,15 +678,15 @@
     :param pair_timeout: Timeout for autopair
     :param local_hostname: Used as a seed to generate the HostID
     :param pair_record: Use this pair record instead of the default behavior (search in host/create our own)
     :param pairing_records_cache_folder: Use the following location to search and save pair records
     :param port: lockdownd service port
     :return: TcpLockdownClient instance
     """
-    service = ServiceConnection.create_using_tcp(hostname, port)
+    service = LockdownServiceConnection.create_using_tcp(hostname, port)
     service.send_plist({'Label': label, 'ProtocolVersion': '2', 'Request': 'RSDCheckin'})
 
     # we expect two responses after the first request
     service.recv_plist()
     service.recv_plist()
 
     client = TcpLockdownClient.create(
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/pair_records.py` & `pymobiledevice3-2.1.0/pymobiledevice3/pair_records.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/remote/bonjour.py` & `pymobiledevice3-2.1.0/pymobiledevice3/remote/bonjour.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/remote/core_device_tunnel_service.py` & `pymobiledevice3-2.1.0/pymobiledevice3/remote/core_device_tunnel_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         self.ed25519_private_key = Ed25519PrivateKey.generate()
         self.identifier = generate_host_id()
         self.srp_context = None
         self.encryption_key = None
         self.signature = None
 
     def connect(self, autopair: bool = True) -> None:
-        self.service = self.rsd.connect_to_service('com.apple.internal.dt.coredevice.untrusted.tunnelservice')
+        self.service = self.rsd.start_remote_service('com.apple.internal.dt.coredevice.untrusted.tunnelservice')
         self.version = self.service.receive_response()['ServiceVersion']
 
         self._attempt_pair_verify()
         if not self._validate_pairing():
             if autopair:
                 self._pair()
         self._init_client_server_main_encryption_keys()
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/remote/remote_service_discovery.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/companion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-from dataclasses import dataclass
-from typing import List, Tuple
+#!/usr/bin/env python3
+import typing
 
-from pymobiledevice3.exceptions import NoDeviceConnectedError
-from pymobiledevice3.remote.bonjour import DEFAULT_BONJOUR_TIMEOUT, get_remoted_addresses
-from pymobiledevice3.remote.remotexpc import RemoteXPCConnection
+from pymobiledevice3.exceptions import PyMobileDevice3Exception
+from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
-@dataclass
-class RSDDevice:
-    hostname: str
-    udid: str
-    product_type: str
-    os_version: str
+class CompanionProxyService(LockdownService):
+    SERVICE_NAME = 'com.apple.companion_proxy'
+    RSD_SERVICE_NAME = 'com.apple.companion_proxy.shim.remote'
 
+    def __init__(self, lockdown: LockdownServiceProvider):
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
 
-# from remoted ([RSDRemoteNCMDeviceDevice createPortListener])
-RSD_PORT = 58783
+    def list(self):
+        service = self.lockdown.start_lockdown_service(self.service_name)
+        return service.send_recv_plist({'Command': 'GetDeviceRegistry'}).get('PairedDevicesArray', [])
 
+    def listen_for_devices(self):
+        service = self.lockdown.start_lockdown_service(self.service_name)
+        service.send_plist({'Command': 'StartListeningForDevices'})
+        while True:
+            yield service.recv_plist()
 
-class RemoteServiceDiscoveryService:
-    def __init__(self, address: Tuple[str, int]):
-        self.service = RemoteXPCConnection(address)
-        self.peer_info = None
+    def get_value(self, udid: str, key: str):
+        service = self.lockdown.start_lockdown_service(self.service_name)
+        response = service.send_recv_plist({'Command': 'GetValueFromRegistry',
+                                            'GetValueGizmoUDIDKey': udid,
+                                            'GetValueKeyKey': key})
 
-    def connect(self) -> None:
-        self.service.connect()
-        self.peer_info = self.service.receive_response()
+        value = response.get('RetrievedValueDictionary')
+        if value is not None:
+            return value
 
-    def connect_to_service(self, name: str) -> RemoteXPCConnection:
-        service_port = int(self.peer_info['Services'][name]['Port'])
-        service = RemoteXPCConnection((self.service.address[0], service_port))
-        service.connect()
-        return service
+        error = response.get('Error')
+        raise PyMobileDevice3Exception(error)
 
-    def __enter__(self) -> 'RemoteServiceDiscoveryService':
-        self.connect()
-        return self
+    def start_forwarding_service_port(self, remote_port: int, service_name: str = None, options: typing.Mapping = None):
+        service = self.lockdown.start_lockdown_service(self.service_name)
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        self.service.close()
+        request = {'Command': 'StartForwardingServicePort',
+                   'GizmoRemotePortNumber': remote_port,
+                   'IsServiceLowPriority': False,
+                   'PreferWifi': False}
 
+        if service_name is not None:
+            request['ForwardedServiceName'] = service_name
 
-def get_remoted_devices(timeout: int = DEFAULT_BONJOUR_TIMEOUT) -> List[RSDDevice]:
-    result = []
-    for hostname in get_remoted_addresses(timeout):
-        with RemoteServiceDiscoveryService((hostname, RSD_PORT)) as rsd:
-            properties = rsd.peer_info['Properties']
-            result.append(RSDDevice(hostname=hostname, udid=properties['UniqueDeviceID'],
-                                    product_type=properties['ProductType'], os_version=properties['OSVersion']))
-    return result
+        if options is not None:
+            request.update(options)
 
+        return service.send_recv_plist(request).get('CompanionProxyServicePort')
 
-def get_remoted_device(udid: str, timeout: int = DEFAULT_BONJOUR_TIMEOUT) -> RSDDevice:
-    devices = get_remoted_devices(timeout=timeout)
-    for device in devices:
-        if device.udid == udid:
-            return device
-    raise NoDeviceConnectedError()
+    def stop_forwarding_service_port(self, remote_port: int):
+        service = self.lockdown.start_lockdown_service(self.service_name)
+
+        request = {'Command': 'StopForwardingServicePort',
+                   'GizmoRemotePortNumber': remote_port}
+
+        return service.send_recv_plist(request)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/remote/sniffer.py` & `pymobiledevice3-2.1.0/misc/remotexpc_sniffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from typing import List, MutableMapping, Optional
 
 import click
 import coloredlogs
 from construct import ConstError, StreamError
 from hexdump import hexdump
 from hyperframe.frame import DataFrame, Frame, GoAwayFrame, HeadersFrame
-from remotexpc import HTTP2_MAGIC
 from scapy.layers.inet import IP, TCP
 from scapy.layers.inet6 import IPv6
 from scapy.packet import Packet
 from scapy.sendrecv import sniff
 
 from pymobiledevice3.remote.core_device_tunnel_service import PairingDataComponentTLVBuf
-from pymobiledevice3.remote.xpc_message import get_object_from_xpc_wrapper
+from pymobiledevice3.remote.remotexpc import HTTP2_MAGIC
+from pymobiledevice3.remote.xpc_message import XpcWrapper, decode_xpc_object
 
 logger = logging.getLogger()
 
 coloredlogs.install(level=logging.DEBUG)
 
 FRAME_HEADER_SIZE = 9
 
@@ -126,15 +126,18 @@
         stream_finished_assembling = stream.add(tcp_pkt)
         if stream_finished_assembling:  # if we just added something in order
             self._process_stream(stream)
 
     def _handle_data_frame(self, stream: H2Stream, frame: DataFrame) -> None:
         previous_frame_data = self._previous_frame_data.get(stream.key, b'')
         try:
-            xpc_message = get_object_from_xpc_wrapper(previous_frame_data + frame.data)
+            payload = XpcWrapper.parse(previous_frame_data + frame.data).message.payload
+            if payload is None:
+                return None
+            xpc_message = decode_xpc_object(payload.obj)
         except ConstError:  # if we don't know what this payload is
             logger.debug(
                 f'New Data frame {stream.src}->{stream.dst} on HTTP/2 stream {frame.stream_id} TCP port {stream.dport}')
             hexdump(frame.data[:64])
             if len(frame.data) > 64:
                 logger.debug(f'... {len(frame.data)} bytes')
             return
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/remote/xpc_message.py` & `pymobiledevice3-2.1.0/pymobiledevice3/remote/xpc_message.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import dataclasses
 import uuid
+from datetime import datetime
 from typing import Any, List, Mapping
 
 from construct import Aligned, Array, Bytes, Const, CString, Default, Double, Enum, ExprAdapter, FlagsEnum, \
     GreedyBytes, Hex, If, Int32ul, Int64sl, Int64ul, LazyBound
 from construct import Optional as ConstructOptional
-from construct import Prefixed, Probe, Struct, Switch, this
+from construct import Pass, Prefixed, Probe, Struct, Switch, this
 
 XpcMessageType = Enum(Hex(Int32ul),
                       NULL=0x00001000,
                       BOOL=0x00002000,
                       INT64=0x00003000,
                       UINT64=0x00004000,
                       DOUBLE=0x00005000,
@@ -32,23 +34,24 @@
                       SERVICE=0x00017000,
                       SERVICE_INSTANCE=0x00018000,
                       ACTIVITY=0x00019000,
                       FILE_TRANSFER=0x0001a000,
                       )
 XpcFlags = FlagsEnum(Hex(Int32ul),
                      ALWAYS_SET=0x00000001,
+                     PING=0x00000002,
                      DATA_PRESENT=0x00000100,
-                     HEARTBEAT_REQUEST=0x00010000,
-                     HEARTBEAT_RESPONSE=0x00020000,
+                     WANTING_REPLY=0x00010000,
+                     REPLY=0x00020000,
                      FILE_TX_STREAM_REQUEST=0x00100000,
                      FILE_TX_STREAM_RESPONSE=0x00200000,
                      INIT_HANDSHAKE=0x00400000,
                      )
 AlignedString = Aligned(4, CString('utf8'))
-XpcNull = None
+XpcNull = Pass
 XpcBool = Int32ul
 XpcInt64 = Int64sl
 XpcUInt64 = Int64ul
 XpcDouble = Double
 XpcPointer = None
 XpcDate = Int64ul
 XpcData = Aligned(4, Prefixed(Int32ul, GreedyBytes))
@@ -63,14 +66,18 @@
     'key' / AlignedString,
     'value' / LazyBound(lambda: XpcObject),
 )
 XpcDictionary = Prefixed(Int32ul, Struct(
     'count' / Hex(Int32ul),
     'entries' / If(this.count > 0, Array(this.count, XpcDictionaryEntry)),
 ))
+XpcFileTransfer = Struct(
+    'msg_id' / Int64ul,
+    'data' / LazyBound(lambda: XpcObject),
+)
 XpcObject = Struct(
     'type' / XpcMessageType,
     'data' / Switch(this.type, {
         XpcMessageType.DICTIONARY: XpcDictionary,
         XpcMessageType.STRING: XpcString,
         XpcMessageType.INT64: XpcInt64,
         XpcMessageType.UINT64: XpcUInt64,
@@ -80,14 +87,15 @@
         XpcMessageType.UUID: XpcUuid,
         XpcMessageType.POINTER: XpcPointer,
         XpcMessageType.DATE: XpcDate,
         XpcMessageType.DATA: XpcData,
         XpcMessageType.FD: XpcFd,
         XpcMessageType.SHMEM: XpcShmem,
         XpcMessageType.ARRAY: XpcArray,
+        XpcMessageType.FILE_TRANSFER: XpcFileTransfer,
     }, default=Probe(lookahead=1000)),
 )
 XpcPayload = Struct(
     'magic' / Hex(Const(0x42133742, Int32ul)),
     'protocol_version' / Hex(Const(0x00000005, Int32ul)),
     'obj' / XpcObject,
 )
@@ -107,27 +115,32 @@
     pass
 
 
 class XpcUInt64Type(int):
     pass
 
 
+@dataclasses.dataclass
+class FileTransferType:
+    transfer_size: int
+
+
 def _decode_xpc_dictionary(xpc_object) -> Mapping:
     if xpc_object.data.count == 0:
         return {}
     result = {}
     for entry in xpc_object.data.entries:
-        result[entry.key] = _decode_xpc_object(entry.value)
+        result[entry.key] = decode_xpc_object(entry.value)
     return result
 
 
 def _decode_xpc_array(xpc_object) -> List:
     result = []
     for entry in xpc_object.data.entries:
-        result.append(_decode_xpc_object(entry))
+        result.append(decode_xpc_object(entry))
     return result
 
 
 def _decode_xpc_bool(xpc_object) -> bool:
     return bool(xpc_object.data)
 
 
@@ -147,46 +160,63 @@
     return xpc_object.data
 
 
 def _decode_xpc_data(xpc_object) -> bytes:
     return xpc_object.data
 
 
-def _decode_xpc_object(xpc_object) -> Any:
+def _decode_xpc_date(xpc_object) -> datetime:
+    # Convert from nanoseconds to seconds
+    return datetime.fromtimestamp(xpc_object.data / 1000000000)
+
+
+def _decode_xpc_file_transfer(xpc_object) -> FileTransferType:
+    return FileTransferType(transfer_size=_decode_xpc_dictionary(xpc_object.data.data)['s'])
+
+
+def _decode_xpc_double(xpc_object) -> float:
+    return xpc_object.data
+
+
+def _decode_xpc_null(xpc_object) -> None:
+    return None
+
+
+def decode_xpc_object(xpc_object) -> Any:
     decoders = {
         XpcMessageType.DICTIONARY: _decode_xpc_dictionary,
         XpcMessageType.ARRAY: _decode_xpc_array,
         XpcMessageType.BOOL: _decode_xpc_bool,
         XpcMessageType.INT64: _decode_xpc_int64,
         XpcMessageType.UINT64: _decode_xpc_uint64,
         XpcMessageType.UUID: _decode_xpc_uuid,
         XpcMessageType.STRING: _decode_xpc_string,
         XpcMessageType.DATA: _decode_xpc_data,
+        XpcMessageType.DATE: _decode_xpc_date,
+        XpcMessageType.FILE_TRANSFER: _decode_xpc_file_transfer,
+        XpcMessageType.DOUBLE: _decode_xpc_double,
+        XpcMessageType.NULL: _decode_xpc_null,
     }
     decoder = decoders.get(xpc_object.type)
     if decoder is None:
         raise TypeError(f'deserialize error: {xpc_object}')
     return decoder(xpc_object)
 
 
-def get_object_from_xpc_wrapper(payload: bytes):
-    payload = XpcWrapper.parse(payload).message.payload
-    if payload is None:
-        return None
-    return _decode_xpc_object(payload.obj)
-
-
 def _build_xpc_array(payload: List) -> Mapping:
     entries = []
     for entry in payload:
         entry = _build_xpc_object(entry)
         entries.append(entry)
     return {
         'type': XpcMessageType.ARRAY,
-        'data': entries
+        'data': {
+            'count': len(entries),
+            'entries': entries
+        }
     }
 
 
 def _build_xpc_dictionary(payload: Mapping) -> Mapping:
     entries = []
     for key, value in payload.items():
         entry = {'key': key, 'value': _build_xpc_object(value)}
@@ -217,14 +247,35 @@
 def _build_xpc_data(payload: bool) -> Mapping:
     return {
         'type': XpcMessageType.DATA,
         'data': payload,
     }
 
 
+def _build_xpc_double(payload: float) -> Mapping:
+    return {
+        'type': XpcMessageType.DOUBLE,
+        'data': payload,
+    }
+
+
+def _build_xpc_uuid(payload: uuid.UUID) -> Mapping:
+    return {
+        'type': XpcMessageType.UUID,
+        'data': payload.bytes,
+    }
+
+
+def _build_xpc_null(payload: None) -> Mapping:
+    return {
+        'type': XpcMessageType.NULL,
+        'data': None,
+    }
+
+
 def _build_xpc_uint64(payload: XpcUInt64Type) -> Mapping:
     return {
         'type': XpcMessageType.UINT64,
         'data': payload,
     }
 
 
@@ -232,34 +283,40 @@
     return {
         'type': XpcMessageType.INT64,
         'data': payload,
     }
 
 
 def _build_xpc_object(payload: Any) -> Mapping:
+    if payload is None:
+        return _build_xpc_null(payload)
     payload_builders = {
         list: _build_xpc_array,
         dict: _build_xpc_dictionary,
         bool: _build_xpc_bool,
         str: _build_xpc_string,
         bytes: _build_xpc_data,
         bytearray: _build_xpc_data,
+        float: _build_xpc_double,
+        uuid.UUID: _build_xpc_uuid,
         'XpcUInt64Type': _build_xpc_uint64,
         'XpcInt64Type': _build_xpc_int64,
     }
     builder = payload_builders.get(type(payload), payload_builders.get(type(payload).__name__))
     if builder is None:
         raise TypeError(f'unrecognized type for: {payload} {type(payload)}')
     return builder(payload)
 
 
-def create_xpc_wrapper(d: Mapping, message_id: int = 0) -> bytes:
+def create_xpc_wrapper(d: Mapping, message_id: int = 0, wanting_reply: bool = False) -> bytes:
     flags = XpcFlags.ALWAYS_SET
     if len(d.keys()) > 0:
         flags |= XpcFlags.DATA_PRESENT
+    if wanting_reply:
+        flags |= XpcFlags.WANTING_REPLY
 
     xpc_payload = {
         'message_id': message_id,
         'payload': {'obj': _build_xpc_object(d)}
     }
 
     xpc_wrapper = {
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/dsc_uuid_map.json` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/dsc_uuid_map.json`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/dsc_uuid_map.py` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/dsc_uuid_map.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/firmware_notifications.py` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/firmware_notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/notifications.txt` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/notifications.txt`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/element_clear.js` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/element_clear.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/enter_fullscreen.js` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/enter_fullscreen.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/find_nodes.js` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/find_nodes.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/get_attribute.js` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/get_attribute.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/is_displayed.js` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/is_displayed.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/is_editable.js` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/is_editable.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/resources/webinspector/is_enabled.js` & `pymobiledevice3-2.1.0/pymobiledevice3/resources/webinspector/is_enabled.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/asr.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/asr.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import plistlib
 import typing
 
 from tqdm import trange
 
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
-from pymobiledevice3.service_connection import ServiceConnection
+from pymobiledevice3.service_connection import LockdownServiceConnection
 
 ASR_VERSION = 1
 ASR_STREAM_ID = 1
 ASR_PORT = 12345
 ASR_FEC_SLICE_STRIDE = 40
 ASR_PACKETS_PER_FEC = 25
 ASR_PAYLOAD_PACKET_SIZE = 1450
@@ -25,15 +25,15 @@
     """
     ASR — Apple Software Restore
     """
 
     SERVICE_PORT = ASR_PORT
 
     def __init__(self, udid: str):
-        self.service = ServiceConnection.create_using_usbmux(udid, self.SERVICE_PORT)
+        self.service = LockdownServiceConnection.create_using_usbmux(udid, self.SERVICE_PORT)
 
         # receive Initiate command message
         data = self.recv_plist()
         logger.debug(f'got command: {data}')
 
         command = data.get('Command')
         if command != 'Initiate':
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/base_restore.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/base_restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/consts.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/consts.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/device.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/device.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/fdr.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/fdr.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import socket
 import struct
 import threading
 from enum import Enum
 
 from pymobiledevice3 import usbmux
 from pymobiledevice3.exceptions import ConnectionFailedError, NoDeviceConnectedError, PyMobileDevice3Exception
-from pymobiledevice3.service_connection import ServiceConnection
+from pymobiledevice3.service_connection import LockdownServiceConnection
 
 CTRL_PORT = 0x43a  # 1082
 CTRLCMD = b'BeginCtrl\0'
 HELLOCTRLCMD = b'HelloCtrl\0'
 HELLOCMD = b'HelloConn\0'
 
 FDR_SYNC_MSG = 0x1
@@ -44,18 +44,18 @@
                 raise ConnectionFailedError()
             else:
                 raise NoDeviceConnectedError()
 
         logger.debug('connecting to FDR')
 
         if type_ == fdr_type.FDR_CTRL:
-            self.service = ServiceConnection.create_using_usbmux(device.serial, self.SERVICE_PORT)
+            self.service = LockdownServiceConnection.create_using_usbmux(device.serial, self.SERVICE_PORT)
             self.ctrl_handshake()
         else:
-            self.service = ServiceConnection.create_using_usbmux(device.serial, conn_port)
+            self.service = LockdownServiceConnection.create_using_usbmux(device.serial, conn_port)
             self.sync_handshake()
 
         logger.debug('FDR connected')
 
     def recv_plist(self):
         return self.service.recv_plist(endianity='<')
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/ftab.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/ftab.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/recovery.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/recovery.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/restore.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pymobiledevice3.restore.device import Device
 from pymobiledevice3.restore.fdr import FDRClient, fdr_type, start_fdr_thread
 from pymobiledevice3.restore.ftab import Ftab
 from pymobiledevice3.restore.recovery import Behavior, Recovery
 from pymobiledevice3.restore.restore_options import RestoreOptions
 from pymobiledevice3.restore.restored_client import RestoredClient
 from pymobiledevice3.restore.tss import TSSRequest, TSSResponse
-from pymobiledevice3.service_connection import ServiceConnection
+from pymobiledevice3.service_connection import LockdownServiceConnection
 from pymobiledevice3.utils import plist_access_path
 
 known_errors = {
     0xFFFFFFFFFFFFFFFF: 'verification error',
     6: 'disk failure',
     14: 'fail',
     27: 'failed to mount filesystems',
@@ -44,15 +44,15 @@
         self.recovery = Recovery(ipsw, device, tss=tss, behavior=behavior)
         self.bbtss: Optional[TSSResponse] = None
         self._restored: Optional[RestoredClient] = None
         self._restore_finished = False
 
         # used when ignore_fdr=True, to store an active FDR connection just to make the device believe it can actually
         # perform an FDR communication, but without really establishing any
-        self._fdr: Optional[ServiceConnection] = None
+        self._fdr: Optional[LockdownServiceConnection] = None
         self._ignore_fdr = ignore_fdr
 
         # query preflight info while device may still be in normal mode
         self._preflight_info = self.device.preflight_info
 
         # prepare progress bar for OS component verify
         self._pb_verify_restore = None
@@ -629,15 +629,15 @@
     def send_bootability_bundle_data(self, message):
         self.logger.debug(f'send_bootability_bundle_data: {message}')
         data_port = message['DataPort']
         self.logger.info('Connecting to BootabilityBundle data port')
 
         while True:
             try:
-                client = ServiceConnection.create_using_usbmux(self._restored.udid, data_port)
+                client = LockdownServiceConnection.create_using_usbmux(self._restored.udid, data_port)
                 break
             except ConnectionFailedError:
                 self.logger.debug('Retrying connection...')
 
         if not client:
             raise ConnectionFailedError(f'failed to establish connection to {data_port}')
 
@@ -1149,15 +1149,15 @@
         self.logger.debug(f'restore_handle_baseband_updater_output_data: {message}')
         data_port = message['DataPort']
 
         self.logger.info('Connecting to baseband updater data port')
 
         while True:
             try:
-                client = ServiceConnection.create_using_usbmux(self._restored.udid, data_port)
+                client = LockdownServiceConnection.create_using_usbmux(self._restored.udid, data_port)
                 break
             except ConnectionFailedError:
                 self.logger.debug('Retrying connection...')
 
         if not client:
             raise ConnectionFailedError(f'failed to establish connection to {data_port}')
 
@@ -1194,15 +1194,15 @@
 
         if self.recovery.tss.bb_ticket is not None:
             # initial TSS response contains a baseband ticket
             self.bbtss = self.recovery.tss
 
         if self._ignore_fdr:
             self.logger.info('Establishing a mock FDR listener')
-            self._fdr = ServiceConnection.create_using_usbmux(self._restored.udid, FDRClient.SERVICE_PORT)
+            self._fdr = LockdownServiceConnection.create_using_usbmux(self._restored.udid, FDRClient.SERVICE_PORT)
         else:
             self.logger.info('Starting FDR listener thread')
             start_fdr_thread(fdr_type.FDR_CTRL)
 
         sep = self.build_identity['Manifest']['SEP'].get('Info')
         spp = self.build_identity['Info'].get('SystemPartitionPadding')
         opts = RestoreOptions(preflight_info=self._preflight_info, sep=sep, macos_variant=self.macos_variant,
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/restore_options.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/restore_options.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/restored_client.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/restored_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 from functools import cached_property
 
 from pymobiledevice3 import usbmux
 from pymobiledevice3.exceptions import ConnectionFailedError, NoDeviceConnectedError
 from pymobiledevice3.restore.restore_options import RestoreOptions
-from pymobiledevice3.service_connection import ServiceConnection
+from pymobiledevice3.service_connection import LockdownServiceConnection
 
 
 class RestoredClient(object):
     DEFAULT_CLIENT_NAME = 'pyMobileDevice'
     SERVICE_PORT = 62078
 
     def __init__(self, udid=None, client_name=DEFAULT_CLIENT_NAME):
         self.logger = logging.getLogger(__name__)
         self.udid = self._get_or_verify_udid(udid)
-        self.service = ServiceConnection.create_using_usbmux(self.udid, self.SERVICE_PORT)
+        self.service = LockdownServiceConnection.create_using_usbmux(self.udid, self.SERVICE_PORT)
         self.label = client_name
         self.query_type = self.service.send_recv_plist({'Request': 'QueryType'})
         self.version = self.query_type.get('RestoreProtocolVersion')
 
         assert self.query_type.get('Type') == 'com.apple.mobile.restored', f'wrong query type: {self.query_type}'
 
     @staticmethod
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/restore/tss.py` & `pymobiledevice3-2.1.0/pymobiledevice3/restore/tss.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/service_connection.py` & `pymobiledevice3-2.1.0/pymobiledevice3/service_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,48 +58,48 @@
 
 
 class Medium(Enum):
     TCP = auto()
     USBMUX = auto()
 
 
-class ServiceConnection:
+class LockdownServiceConnection:
     """ wrapper for usbmux tcp-relay connections """
 
     def __init__(self, sock: socket.socket, mux_device: MuxDevice = None):
         self.logger = logging.getLogger(__name__)
         self.socket = sock
 
         # usbmux connections contain additional information associated with the current connection
         self.mux_device = mux_device
 
         self._reader = None  # type: Optional[asyncio.StreamReader]
         self._writer = None  # type: Optional[asyncio.StreamWriter]
 
     @staticmethod
-    def create_using_tcp(hostname: str, port: int) -> 'ServiceConnection':
+    def create_using_tcp(hostname: str, port: int) -> 'LockdownServiceConnection':
         sock = socket.create_connection((hostname, port))
-        return ServiceConnection(sock)
+        return LockdownServiceConnection(sock)
 
     @staticmethod
-    def create_using_usbmux(udid: Optional[str], port: int, connection_type: str = None) -> 'ServiceConnection':
+    def create_using_usbmux(udid: Optional[str], port: int, connection_type: str = None) -> 'LockdownServiceConnection':
         target_device = select_device(udid, connection_type=connection_type)
         if target_device is None:
             if udid:
                 raise ConnectionFailedError()
             raise NoDeviceConnectedError()
         sock = target_device.connect(port)
-        return ServiceConnection(sock, mux_device=target_device)
+        return LockdownServiceConnection(sock, mux_device=target_device)
 
     @staticmethod
-    def create(medium: Medium, identifier: str, port: int, connection_type: str = None) -> 'ServiceConnection':
+    def create(medium: Medium, identifier: str, port: int, connection_type: str = None) -> 'LockdownServiceConnection':
         if medium == Medium.TCP:
-            return ServiceConnection.create_using_tcp(identifier, port)
+            return LockdownServiceConnection.create_using_tcp(identifier, port)
         else:
-            return ServiceConnection.create_using_usbmux(identifier, port, connection_type=connection_type)
+            return LockdownServiceConnection.create_using_usbmux(identifier, port, connection_type=connection_type)
 
     def setblocking(self, blocking: bool) -> None:
         self.socket.setblocking(blocking)
 
     def close(self) -> None:
         self.socket.close()
 
@@ -183,13 +183,16 @@
     async def aio_ssl_start(self, certfile, keyfile=None) -> None:
         self._reader, self._writer = await asyncio.open_connection(
             sock=self.socket,
             ssl=create_context(certfile, keyfile=keyfile),
             server_hostname=''
         )
 
+    async def aio_start(self) -> None:
+        self._reader, self._writer = await asyncio.open_connection(sock=self.socket)
+
     def shell(self) -> None:
         IPython.embed(
             header=highlight(SHELL_USAGE, lexers.PythonLexer(), formatters.TerminalTrueColorFormatter(style='native')),
             user_ns={
                 'client': self,
             })
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/accessibilityaudit.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/accessibilityaudit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typing
 from dataclasses import dataclass
 from enum import Enum
 
 from packaging.version import Version
 
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
 from pymobiledevice3.services.remote_server import MessageAux, RemoteServer
 
 
 class SerializedObject:
     def __init__(self, fields: typing.Mapping):
         self._fields = fields
 
@@ -111,17 +112,21 @@
         return deserialize_object(d['Value'])
     else:
         return SERIALIZABLE_OBJECTS[d['ObjectType']](deserialize_object(d['Value']))
 
 
 class AccessibilityAudit(RemoteServer):
     SERVICE_NAME = 'com.apple.accessibility.axAuditDaemon.remoteserver'
+    RSD_SERVICE_NAME = 'com.apple.accessibility.axAuditDaemon.remoteserver.shim.remote'
 
-    def __init__(self, lockdown: LockdownClient):
-        super().__init__(lockdown, self.SERVICE_NAME, remove_ssl_context=True)
+    def __init__(self, lockdown: LockdownServiceProvider):
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME, remove_ssl_context=True, is_developer_service=False)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME, remove_ssl_context=True, is_developer_service=False)
 
         # flush previously received messages
         self.recv_plist()
         if Version(lockdown.product_version) >= Version('15.0'):
             self.recv_plist()
 
     @property
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/afc.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/afc.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from construct import Const, Container, CString, Enum, GreedyRange, Int64ul, Struct, Tell
 from pygments import formatters, highlight, lexers
 from pygnuutils.cli.ls import ls as ls_cli
 from pygnuutils.ls import Ls, LsStub
 
 from pymobiledevice3.exceptions import AfcException, AfcFileNotFoundError, ArgumentError
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.lockdown_service import LockdownService
 from pymobiledevice3.utils import try_decode
 
 MAXIMUM_READ_SIZE = 1 * 1024 ** 2  # 1 MB
 MODE_MASK = 0o0000777
 
 StatResult = namedtuple('StatResult',
                         ['st_mode', 'st_ino', 'st_dev', 'st_nlink', 'st_uid', 'st_gid', 'st_size', 'st_atime',
@@ -199,16 +200,24 @@
     assert len(t) % 2 == 0
     res = {}
     for i in range(int(len(t) / 2)):
         res[t[i * 2]] = t[i * 2 + 1]
     return res
 
 
-class AfcService(BaseService):
-    def __init__(self, lockdown: LockdownClient, service_name='com.apple.afc'):
+class AfcService(LockdownService):
+    SERVICE_NAME = 'com.apple.afc'
+    RSD_SERVICE_NAME = 'com.apple.afc.shim.remote'
+
+    def __init__(self, lockdown: LockdownServiceProvider, service_name: str = None):
+        if service_name is None:
+            if isinstance(lockdown, LockdownClient):
+                service_name = self.SERVICE_NAME
+            else:
+                service_name = self.RSD_SERVICE_NAME
         super().__init__(lockdown, service_name)
         self.packet_num = 0
 
     def pull(self, relative_src, dst, callback=None, src_dir=''):
         src = posixpath.join(src_dir, relative_src)
         if callback is not None:
             callback(src, dst)
@@ -670,24 +679,25 @@
         return ''
 
     def print(self, *objects, sep=' ', end='\n', file=sys.stdout, flush=False):
         self.afc_shell.poutput(objects[0], end=end)
 
 
 class AfcShell(Cmd):
-    def __init__(self, lockdown: LockdownClient, service_name='com.apple.afc', completekey='tab', afc_service=None):
+    def __init__(self, lockdown: LockdownServiceProvider, service_name: str = None, completekey: str = 'tab',
+                 afc_service: LockdownService = None):
         # bugfix: prevent the Cmd instance from trying to parse click's arguments
         sys.argv = sys.argv[:1]
 
         Cmd.__init__(self,
                      completekey=completekey,
                      persistent_history_file=os.path.join(tempfile.gettempdir(), f'.{service_name}-history'))
+
         self.logger = logging.getLogger(__name__)
         self.lockdown = lockdown
-        self.service_name = service_name
         self.afc = afc_service or AfcService(self.lockdown, service_name=service_name)
         self.curdir = '/'
         self.complete_edit = self._complete_first_arg
         self.complete_cd = self._complete_first_arg
         self.complete_ls = self._complete
         self.complete_walk = self._complete_first_arg
         self.complete_cat = self._complete_first_arg
@@ -807,15 +817,15 @@
         for k, v in self.afc.stat(self.relative_path(args.filename)).items():
             self.poutput(f'{k}: {v}')
 
     def relative_path(self, filename):
         return posixpath.join(self.curdir, filename)
 
     def _update_prompt(self):
-        self.prompt = highlight(f'[{self.service_name}:{self.curdir}]$ ', lexers.BashSessionLexer(),
+        self.prompt = highlight(f'[{self.afc.service_name}:{self.curdir}]$ ', lexers.BashSessionLexer(),
                                 formatters.TerminalTrueColorFormatter(style='solarized-dark')).strip()
 
     def _complete(self, text, line, begidx, endidx):
         curdir_diff = posixpath.dirname(text)
         dirname = posixpath.join(self.curdir, curdir_diff)
         prefix = posixpath.basename(text)
         return [
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/amfi.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/amfi.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
     def __init__(self, lockdown: LockdownClient):
         self._lockdown = lockdown
         self._logger = logging.getLogger(self.__module__)
 
     def create_amfi_show_override_path_file(self):
         """ create an empty file at AMFIShowOverridePath """
-        service = self._lockdown.start_service(self.SERVICE_NAME)
+        service = self._lockdown.start_lockdown_service(self.SERVICE_NAME)
         resp = service.send_recv_plist({'action': 0})
         if not resp['status']:
             raise PyMobileDevice3Exception(f'create_AMFIShowOverridePath() failed with: {resp}')
 
     def enable_developer_mode(self, enable_post_restart=True):
         """
         enable developer-mode
         if enable_post_restart is True, then wait for device restart to answer the final prompt
         with "yes"
         """
-        service = self._lockdown.start_service(self.SERVICE_NAME)
+        service = self._lockdown.start_lockdown_service(self.SERVICE_NAME)
         resp = service.send_recv_plist({'action': 1})
         error = resp.get('Error')
 
         if error is not None:
             if error == 'Device has a passcode set':
                 raise DeviceHasPasscodeSetError()
             raise AmfiError(error)
@@ -56,11 +56,11 @@
             except (NoDeviceConnectedError, ConnectionFailedError, BadDevError, construct.core.StreamError):
                 pass
 
         self.enable_developer_mode_post_restart()
 
     def enable_developer_mode_post_restart(self):
         """ answer the prompt that appears after the restart with "yes" """
-        service = self._lockdown.start_service(self.SERVICE_NAME)
+        service = self._lockdown.start_lockdown_service(self.SERVICE_NAME)
         resp = service.send_recv_plist({'action': 2})
         if not resp.get('success'):
             raise DeveloperModeError(f'enable_developer_mode_post_restart() failed: {resp}')
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/base_service.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/heartbeat.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-import logging
+#!/usr/bin/env python3
+import time
 
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.service_connection import ServiceConnection
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
-class BaseService:
-    def __init__(self, lockdown: LockdownClient, service_name: str, is_developer_service=False,
-                 service: ServiceConnection = None):
-        """
-        :param lockdown: lockdown connection
-        :param service_name: wrapped service name - will attempt
-        :param is_developer_service: should DeveloperDiskImage be mounted before
-        :param service: an established service connection object. If none, will attempt connecting to service_name
-        """
-
-        if not service:
-            start_service = lockdown.start_developer_service if is_developer_service else lockdown.start_service
-            service = start_service(service_name)
-
-        self.service_name = service_name
-        self.lockdown = lockdown
-        self.service = service
-        self.logger = logging.getLogger(self.__module__)
+class HeartbeatService(LockdownService):
+    """
+    Use to keep an active connection with lockdowd
+    """
+    SERVICE_NAME = 'com.apple.mobile.heartbeat'
+    RSD_SERVICE_NAME = 'com.apple.mobile.heartbeat.shim.remote'
+
+    def __init__(self, lockdown: LockdownServiceProvider):
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
+
+    def start(self, interval=None):
+        start = time.time()
+        service = self.lockdown.start_lockdown_service(self.SERVICE_NAME)
+
+        while True:
+            response = service.recv_plist()
+            self.logger.debug(response)
+
+            if interval is not None:
+                if time.time() >= start + interval:
+                    break
 
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.close()
-
-    def close(self):
-        self.service.close()
+            service.send_plist({'Command': 'Polo'})
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/companion.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/springboard.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,55 @@
-#!/usr/bin/env python3
 import typing
+from enum import IntEnum
 
-from pymobiledevice3.exceptions import PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
-class CompanionProxyService(BaseService):
-    SERVICE_NAME = 'com.apple.companion_proxy'
+class InterfaceOrientation(IntEnum):
+    PORTRAIT = 1
+    PORTRAIT_UPSIDE_DOWN = 2
+    LANDSCAPE = 3
+    LANDSCAPE_HOME_TO_LEFT = 4
 
-    def __init__(self, lockdown: LockdownClient):
-        super().__init__(lockdown, self.SERVICE_NAME)
 
-    def list(self):
-        service = self.lockdown.start_service(self.SERVICE_NAME)
-        return service.send_recv_plist({'Command': 'GetDeviceRegistry'}).get('PairedDevicesArray', [])
+class SpringBoardServicesService(LockdownService):
+    RSD_SERVICE_NAME = 'com.apple.springboardservices.shim.remote'
+    SERVICE_NAME = 'com.apple.springboardservices'
 
-    def listen_for_devices(self):
-        service = self.lockdown.start_service(self.SERVICE_NAME)
-        service.send_plist({'Command': 'StartListeningForDevices'})
-        while True:
-            yield service.recv_plist()
+    def __init__(self, lockdown: LockdownServiceProvider):
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
 
-    def get_value(self, udid: str, key: str):
-        service = self.lockdown.start_service(self.SERVICE_NAME)
-        response = service.send_recv_plist({'Command': 'GetValueFromRegistry',
-                                            'GetValueGizmoUDIDKey': udid,
-                                            'GetValueKeyKey': key})
+    def get_icon_state(self, format_version: str = '2'):
+        cmd = {'command': 'getIconState'}
+        if format_version:
+            cmd['formatVersion'] = format_version
 
-        value = response.get('RetrievedValueDictionary')
-        if value is not None:
-            return value
+        return self.service.send_recv_plist(cmd)
 
-        error = response.get('Error')
-        raise PyMobileDevice3Exception(error)
+    def set_icon_state(self, newstate: typing.Mapping = None):
+        if newstate is None:
+            newstate = {}
+        cmd = {'command': 'setIconState',
+               'iconState': newstate}
 
-    def start_forwarding_service_port(self, remote_port: int, service_name: str = None, options: typing.Mapping = None):
-        service = self.lockdown.start_service(self.SERVICE_NAME)
+        self.service.send_recv_plist(cmd)
 
-        request = {'Command': 'StartForwardingServicePort',
-                   'GizmoRemotePortNumber': remote_port,
-                   'IsServiceLowPriority': False,
-                   'PreferWifi': False}
+    def get_icon_pngdata(self, bundle_id: str):
+        cmd = {'command': 'getIconPNGData',
+               'bundleId': bundle_id}
 
-        if service_name is not None:
-            request['ForwardedServiceName'] = service_name
+        return self.service.send_recv_plist(cmd).get('pngData')
 
-        if options is not None:
-            request.update(options)
+    def get_interface_orientation(self):
+        cmd = {'command': 'getInterfaceOrientation'}
+        self.service.send_plist(cmd)
+        res = self.service.recv_plist()
+        return InterfaceOrientation(res.get('interfaceOrientation'))
 
-        return service.send_recv_plist(request).get('CompanionProxyServicePort')
-
-    def stop_forwarding_service_port(self, remote_port: int):
-        service = self.lockdown.start_service(self.SERVICE_NAME)
-
-        request = {'Command': 'StopForwardingServicePort',
-                   'GizmoRemotePortNumber': remote_port}
-
-        return service.send_recv_plist(request)
+    def get_wallpaper_pngdata(self):
+        cmd = {'command': 'getHomeScreenWallpaperPNGData'}
+        return self.service.send_recv_plist(cmd).get('pngData')
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/device_arbitration.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/device_arbitration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Mapping
 
 from pymobiledevice3.exceptions import ArbitrationError, DeviceAlreadyInUseError
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
-class DtDeviceArbitration(BaseService):
+class DtDeviceArbitration(LockdownService):
     SERVICE_NAME = 'com.apple.dt.devicearbitration'
 
     def __init__(self, lockdown: LockdownClient):
         super().__init__(lockdown, self.SERVICE_NAME, is_developer_service=True)
 
     @property
     def version(self) -> Mapping:
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/device_link.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/device_link.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/diagnostics.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/diagnostics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Mapping, Optional
 
 from pymobiledevice3.exceptions import ConnectionFailedError, PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 MobileGestaltKeys = ['BasebandKeyHashInformation',
                      'BasebandFirmwareManifestData',
                      'DieId',
                      'SerialNumber',
                      'UniqueChipID',
                      'WifiAddress',
@@ -83,30 +84,35 @@
                      'RegionalBehaviorNoWiFi',
                      'RegionalBehaviorChinaBrick',
                      'RegionalBehaviorNoVOIP',
                      'RegionalBehaviorAll',
                      'ApNonce']
 
 
-class DiagnosticsService(BaseService):
+class DiagnosticsService(LockdownService):
     """
     Provides an API to:
     * Query MobileGestalt & IORegistry keys.
     * Reboot, shutdown or put the device in sleep mode.
     """
-    SERVICE_NAME_NEW = 'com.apple.mobile.diagnostics_relay'
-    SERVICE_NAME_OLD = 'com.apple.iosdiagnostics.relay'
-
-    def __init__(self, lockdown: LockdownClient):
-        try:
-            service = lockdown.start_service(self.SERVICE_NAME_NEW)
-            service_name = self.SERVICE_NAME_NEW
-        except ConnectionFailedError:
-            service = lockdown.start_service(self.SERVICE_NAME_OLD)
-            service_name = self.SERVICE_NAME_OLD
+    RSD_SERVICE_NAME = 'com.apple.mobile.diagnostics_relay.shim.remote'
+    SERVICE_NAME = 'com.apple.mobile.diagnostics_relay'
+    OLD_SERVICE_NAME = 'com.apple.iosdiagnostics.relay'
+
+    def __init__(self, lockdown: LockdownServiceProvider):
+        if isinstance(lockdown, LockdownClient):
+            try:
+                service = lockdown.start_lockdown_service(self.SERVICE_NAME)
+                service_name = self.SERVICE_NAME
+            except ConnectionFailedError:
+                service = lockdown.start_lockdown_service(self.OLD_SERVICE_NAME)
+                service_name = self.OLD_SERVICE_NAME
+        else:
+            service = None
+            service_name = self.RSD_SERVICE_NAME
 
         super().__init__(lockdown, service_name, service=service)
 
     def mobilegestalt(self, keys: List[str] = None) -> Mapping:
         if keys is None or len(keys) == 0:
             keys = MobileGestaltKeys
         resp = self.service.send_recv_plist({'Request': 'MobileGestalt', 'MobileGestaltKeys': keys})
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dtfetchsymbols.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dtfetchsymbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         received = 0
         while received < size:
             buf = service.recv(min(size - received, self.MAX_CHUNK))
             stream.write(buf)
             received += len(buf)
 
     def _start_command(self, cmd: bytes):
-        service = self.lockdown.start_developer_service(self.SERVICE_NAME)
+        service = self.lockdown.start_lockdown_developer_service(self.SERVICE_NAME)
         service.sendall(cmd)
 
         # receive same command as an ack
         if cmd != service.recvall(len(cmd)):
             raise PyMobileDevice3Exception('bad ack')
 
         return service
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+from typing import Union
+
 from packaging.version import Version
 
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.remote.remote_service_discovery import RemoteServiceDiscoveryService
 from pymobiledevice3.services.remote_server import RemoteServer
 
 
 class DvtSecureSocketProxyService(RemoteServer):
     SERVICE_NAME = 'com.apple.instruments.remoteserver.DVTSecureSocketProxy'
     OLD_SERVICE_NAME = 'com.apple.instruments.remoteserver'
+    RSD_SERVICE_NAME = 'com.apple.instruments.dtservicehub'
 
-    def __init__(self, lockdown: LockdownClient):
-        if Version(lockdown.product_version) >= Version('14.0'):
+    def __init__(self, lockdown: Union[RemoteServiceDiscoveryService, LockdownClient]):
+        if isinstance(lockdown, RemoteServiceDiscoveryService):
+            service_name = self.RSD_SERVICE_NAME
+            remove_ssl_context = False
+        elif Version(lockdown.product_version) >= Version('14.0'):
             service_name = self.SERVICE_NAME
             remove_ssl_context = False
         else:
             service_name = self.OLD_SERVICE_NAME
             remove_ssl_context = True
 
         super().__init__(lockdown, service_name, remove_ssl_context=remove_ssl_context)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/application_listing.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/application_listing.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/condition_inducer.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/condition_inducer.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from io import BytesIO
 
 from construct import Array, Byte, Bytes, Computed, CString, Enum, FixedSized, GreedyBytes, GreedyRange, GreedyString, \
     Int16ul, Int32ul, Int64ul, LazyBound, Padded, Padding, Pass, Struct, Switch, this
 from pykdebugparser.kd_buf_parser import RAW_VERSION2_BYTES
 
 from pymobiledevice3.exceptions import ExtractingStackshotError
+from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.resources.dsc_uuid_map import get_dsc_map
 from pymobiledevice3.services.dvt.dvt_secure_socket_proxy import DvtSecureSocketProxyService
 from pymobiledevice3.services.dvt.instruments.device_info import DeviceInfo
 from pymobiledevice3.services.remote_server import Tap
 
 kcdata_types = {
     'KCDATA_TYPE_INVALID': 0x0,
@@ -672,12 +673,18 @@
 
     @staticmethod
     def get_time_config(dvt):
         time_info = DeviceInfo(dvt).mach_time_info()
         mach_absolute_time = time_info[0]
         numer = time_info[1]
         denom = time_info[2]
-        usecs_since_epoch = dvt.lockdown.get_value(key='TimeIntervalSince1970') * 1000000
+
+        usecs_since_epoch = None
+        timezone_ = None
+        if isinstance(dvt.lockdown, LockdownClient):
+            usecs_since_epoch = dvt.lockdown.get_value(key='TimeIntervalSince1970') * 1000000
+            timezone_ = timezone(timedelta(seconds=dvt.lockdown.get_value(key='TimeZoneOffsetFromUTC')))
+
         return dict(
             numer=numer, denom=denom, mach_absolute_time=mach_absolute_time, usecs_since_epoch=usecs_since_epoch,
-            timezone=timezone(timedelta(seconds=dvt.lockdown.get_value(key='TimeZoneOffsetFromUTC')))
+            timezone=timezone_
         )
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/device_info.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/device_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,18 @@
 
     def mach_time_info(self):
         return self.request_information('machTimeInfo')
 
     def mach_kernel_name(self) -> str:
         return self.request_information('machKernelName')
 
-    def kpep_database(self) -> typing.Mapping:
-        return plistlib.loads(self.request_information('kpepDatabase'))
+    def kpep_database(self) -> typing.Optional[typing.Mapping]:
+        kpep_database = self.request_information('kpepDatabase')
+        if kpep_database is not None:
+            return plistlib.loads(kpep_database)
 
     def trace_codes(self):
         codes_file = self.request_information('traceCodesFile')
         return {int(k, 16): v for k, v in map(lambda line: line.split(), codes_file.splitlines())}
 
     def request_information(self, selector_name):
         self._channel[selector_name]()
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/energy_monitor.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/energy_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/graphics.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/graphics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/network_monitor.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/network_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/notifications.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/process_control.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/process_control.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/dvt/instruments/sysmontap.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/dvt/instruments/sysmontap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/file_relay.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/file_relay.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 SRCFILES = '''Baseband
 CrashReporter
 MobileAsset
 VARFS
 HFSMeta
 Lockdown
@@ -18,15 +18,15 @@
 NANDDebugInfo
 SystemConfiguration
 Ubiquity
 tmp
 WirelessAutomation'''
 
 
-class FileRelayService(BaseService):
+class FileRelayService(LockdownService):
     SERVICE_NAME = 'com.apple.mobile.file_relay'
 
     def __init__(self, lockdown: LockdownClient):
         super().__init__(lockdown, self.SERVICE_NAME)
         self.packet_num = 0
 
     def stop_session(self):
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/heartbeat.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/house_arrest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-#!/usr/bin/env python3
-import time
-
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
-
-
-class HeartbeatService(BaseService):
-    """
-    Use to keep an active connection with lockdowd
-    """
-    SERVICE_NAME = 'com.apple.mobile.heartbeat'
-
-    def __init__(self, lockdown: LockdownClient):
-        super().__init__(lockdown, self.SERVICE_NAME)
-
-    def start(self, interval=None):
-        start = time.time()
-        service = self.lockdown.start_service(self.SERVICE_NAME)
-
-        while True:
-            response = service.recv_plist()
-            self.logger.debug(response)
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.afc import AfcService, AfcShell
 
-            if interval is not None:
-                if time.time() >= start + interval:
-                    break
 
-            service.send_plist({'Command': 'Polo'})
+class HouseArrestService(AfcService):
+    SERVICE_NAME = 'com.apple.mobile.house_arrest'
+    RSD_SERVICE_NAME = 'com.apple.mobile.house_arrest.shim.remote'
+
+    def __init__(self, lockdown: LockdownServiceProvider):
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
+
+    def send_command(self, bundle_id, cmd='VendContainer'):
+        self.service.send_plist({'Command': cmd, 'Identifier': bundle_id})
+        res = self.service.recv_plist()
+        if res.get('Error'):
+            self.logger.error('%s: %s', bundle_id, res.get('Error'))
+            return False
+        else:
+            return True
+
+    def shell(self, application_id, cmd='VendContainer'):
+        res = self.send_command(application_id, cmd)
+        if res:
+            AfcShell(self.lockdown, afc_service=self).cmdloop()
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/house_arrest.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/preboard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-import logging
+#!/usr/bin/env python3
 
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.afc import AfcService, AfcShell
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
-class HouseArrestService(AfcService):
-    SERVICE_NAME = 'com.apple.mobile.house_arrest'
+class PreboardService(LockdownService):
+    RSD_SERVICE_NAME = 'com.apple.preboardservice_v2.shim.remote'
+    SERVICE_NAME = 'com.apple.preboardservice_v2'
 
-    def __init__(self, lockdown: LockdownClient):
-        self.logger = logging.getLogger(__name__)
-        self.lockdown = lockdown
-        service_name = self.SERVICE_NAME
-        super(HouseArrestService, self).__init__(self.lockdown, service_name)
-
-    def send_command(self, bundle_id, cmd='VendContainer'):
-        self.service.send_plist({'Command': cmd, 'Identifier': bundle_id})
-        res = self.service.recv_plist()
-        if res.get('Error'):
-            self.logger.error('%s: %s', bundle_id, res.get('Error'))
-            return False
+    def __init__(self, lockdown: LockdownServiceProvider):
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
         else:
-            return True
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
 
-    def shell(self, application_id, cmd='VendContainer'):
-        res = self.send_command(application_id, cmd)
-        if res:
-            AfcShell(self.lockdown, afc_service=self).cmdloop()
+    def create_stashbag(self, manifest):
+        return self.service.send_recv_plist({'Command': 'CreateStashbag', 'Manifest': manifest})
+
+    def commit(self, manifest):
+        return self.service.send_recv_plist({'Command': 'CommitStashbag', 'Manifest': manifest})
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/installation_proxy.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/installation_proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import os
 import posixpath
 from typing import Callable, List, Mapping
 
 from pymobiledevice3.exceptions import AppInstallError
 from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.services.afc import AfcService
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 GET_APPS_ADDITIONAL_INFO = {'ReturnAttributes': ['CFBundleIdentifier', 'StaticDiskUsage', 'DynamicDiskUsage']}
 
 
-class InstallationProxyService(BaseService):
+class InstallationProxyService(LockdownService):
     SERVICE_NAME = 'com.apple.mobile.installation_proxy'
+    RSD_SERVICE_NAME = 'com.apple.mobile.installation_proxy.shim.remote'
 
     def __init__(self, lockdown: LockdownClient):
-        super().__init__(lockdown, self.SERVICE_NAME)
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
 
     def _watch_completion(self, handler: Callable = None, *args) -> None:
         while True:
             response = self.service.recv_plist()
             if not response:
                 break
             error = response.get('Error')
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/misagent.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/misagent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import plistlib
 from io import BytesIO
-from typing import List
+from typing import List, Mapping
 
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
 class ProvisioningProfile:
     def __init__(self, buf: bytes):
         self.buf = buf
 
         xml = b'<?xml' + buf.split(b'<?xml', 1)[1]
         xml = xml.split(b'</plist>')[0] + b'</plist>'
         self.plist = plistlib.loads(xml)
 
     def __str__(self):
         return str(self.plist)
 
 
-class MisagentService(BaseService):
+class MisagentService(LockdownService):
     SERVICE_NAME = 'com.apple.misagent'
+    RSD_SERVICE_NAME = 'com.apple.misagent.shim.remote'
 
     def __init__(self, lockdown: LockdownClient):
-        super().__init__(lockdown, self.SERVICE_NAME)
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
 
-    def install(self, plist: BytesIO):
+    def install(self, plist: BytesIO) -> Mapping:
         response = self.service.send_recv_plist({'MessageType': 'Install',
                                                  'Profile': plist.read(),
                                                  'ProfileType': 'Provisioning'})
         if response['Status']:
             raise PyMobileDevice3Exception(f'invalid status: {response}')
 
         return response
 
-    def remove(self, profile_id):
+    def remove(self, profile_id: str) -> Mapping:
         response = self.service.send_recv_plist({'MessageType': 'Remove',
                                                  'ProfileID': profile_id,
                                                  'ProfileType': 'Provisioning'})
         if response['Status']:
             raise PyMobileDevice3Exception(f'invalid status: {response}')
 
         return response
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/mobile_activation.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/mobile_activation.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,22 +68,22 @@
     def activate_with_session(self, activation_record, headers):
         data = {
             'Command': 'HandleActivationInfoWithSessionRequest',
             'Value': activation_record,
         }
         if headers:
             data['ActivationResponseHeaders'] = dict(headers)
-        with closing(create_using_usbmux(self.lockdown.udid).start_service(self.SERVICE_NAME)) as service:
+        with closing(create_using_usbmux(self.lockdown.udid).start_lockdown_service(self.SERVICE_NAME)) as service:
             return service.send_recv_plist(data)
 
     def send_command(self, command, value=''):
         data = {'Command': command}
         if value:
             data['Value'] = value
-        with closing(create_using_usbmux(self.lockdown.udid).start_service(self.SERVICE_NAME)) as service:
+        with closing(create_using_usbmux(self.lockdown.udid).start_lockdown_service(self.SERVICE_NAME)) as service:
             return service.send_recv_plist(data)
 
     def post(self, url, data, headers=None):
         if headers is None:
             headers = DEFAULT_HEADERS
 
         resp = requests.post(url, data=data, headers=headers)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/mobile_config.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/mobile_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.serialization import Encoding
 from cryptography.hazmat.primitives.serialization.pkcs7 import PKCS7SignatureBuilder
 from cryptography.hazmat.primitives.serialization.pkcs12 import load_pkcs12
 
 from pymobiledevice3.exceptions import ProfileError
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
 class Purpose(Enum):
     PostSetupInstallation = 'PostSetupInstallation'
 
 
-class MobileConfigService(BaseService):
+class MobileConfigService(LockdownService):
     SERVICE_NAME = 'com.apple.mobile.MCInstall'
+    RSD_SERVICE_NAME = 'com.apple.mobile.MCInstall.shim.remote'
 
     def __init__(self, lockdown: LockdownClient):
-        super().__init__(lockdown, self.SERVICE_NAME)
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
 
     def hello(self) -> None:
         self._send_recv({'RequestType': 'HelloHostIdentifier'})
 
     def flush(self) -> None:
         self._send_recv({'RequestType': 'Flush'})
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/mobile_image_mounter.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/mobile_image_mounter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 
 from pymobiledevice3.common import get_home_folder
 from pymobiledevice3.exceptions import AlreadyMountedError, DeveloperDiskImageNotFoundError, \
     DeveloperModeIsNotEnabledError, InternalError, MessageNotSupportedError, MissingManifestError, NotMountedError, \
     PyMobileDevice3Exception, UnsupportedCommandError
 from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.restore.tss import TSSRequest
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
-class MobileImageMounterService(BaseService):
+class MobileImageMounterService(LockdownService):
     # implemented in /usr/libexec/mobile_storage_proxy
     SERVICE_NAME = 'com.apple.mobile.mobile_image_mounter'
+    RSD_SERVICE_NAME = 'com.apple.mobile.mobile_image_mounter.shim.remote'
 
     def __init__(self, lockdown: LockdownClient):
-        super().__init__(lockdown, self.SERVICE_NAME)
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
 
     def copy_devices(self) -> List[Mapping]:
         """ Copy mounted devices list. """
         try:
             return self.service.send_recv_plist({'Command': 'CopyDevices'})['EntryList']
         except KeyError as e:
             raise MessageNotSupportedError from e
@@ -193,15 +197,15 @@
 
         # try to fetch the personalization manifest if the device already has one
         # in case of failure, the service will close the socket, so we'll have to reestablish the connection
         # and query the manifest from Apple's ticket server instead
         try:
             manifest = self.query_personalization_manifest('DeveloperDiskImage', hashlib.sha384(image).digest())
         except MissingManifestError:
-            self.service = self.lockdown.start_service(self.SERVICE_NAME)
+            self.service = self.lockdown.start_lockdown_service(self.SERVICE_NAME)
             manifest = self.get_manifest_from_tss(plistlib.loads(build_manifest.read_bytes()))
 
         self.upload_image(self.IMAGE_TYPE, image, manifest)
 
         extras = {}
         if info_plist is not None:
             extras['ImageInfoPlist'] = info_plist
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/mobilebackup2.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/mobilebackup2.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from datetime import datetime
 from pathlib import Path
 
 from pymobiledevice3.exceptions import AfcException, AfcFileNotFoundError, ConnectionTerminatedError, LockdownError, \
     PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.services.afc import AFC_LOCK_EX, AFC_LOCK_UN, AfcService, afc_error_t
-from pymobiledevice3.services.base_service import BaseService
 from pymobiledevice3.services.device_link import DeviceLink
 from pymobiledevice3.services.installation_proxy import InstallationProxyService
+from pymobiledevice3.services.lockdown_service import LockdownService
 from pymobiledevice3.services.notification_proxy import NotificationProxyService
 from pymobiledevice3.services.springboard import SpringBoardServicesService
 
 SUPPORTED_VERSIONS = [2.0, 2.1]
 ITUNES_FILES = [
     'ApertureAlbumPrefs', 'IC-Info.sidb', 'IC-Info.sidv', 'PhotosFolderAlbums', 'PhotosFolderName',
     'PhotosFolderPrefs', 'VoiceMemos.plist', 'iPhotoAlbumPrefs', 'iTunesApplicationIDs', 'iTunesPrefs',
@@ -24,15 +24,15 @@
 ]
 NP_SYNC_WILL_START = 'com.apple.itunes-mobdev.syncWillStart'
 NP_SYNC_DID_START = 'com.apple.itunes-mobdev.syncDidStart'
 NP_SYNC_LOCK_REQUEST = 'com.apple.itunes-mobdev.syncLockRequest'
 NP_SYNC_DID_FINISH = 'com.apple.itunes-mobdev.syncDidFinish'
 
 
-class Mobilebackup2Service(BaseService):
+class Mobilebackup2Service(LockdownService):
     SERVICE_NAME = 'com.apple.mobilebackup2'
 
     def __init__(self, lockdown: LockdownClient):
         super().__init__(lockdown, self.SERVICE_NAME)
 
     @property
     def will_encrypt(self):
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/notification_proxy.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/notification_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 import socket
 from typing import Generator, Mapping, Union
 
 from pymobiledevice3.exceptions import NotificationTimeoutError
-from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.remote.remote_service_discovery import RemoteServiceDiscoveryService
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
-class NotificationProxyService(BaseService):
+class NotificationProxyService(LockdownService):
     SERVICE_NAME = 'com.apple.mobile.notification_proxy'
+    RSD_SERVICE_NAME = 'com.apple.mobile.notification_proxy.shim.remote'
+
     INSECURE_SERVICE_NAME = 'com.apple.mobile.insecure_notification_proxy'
+    RSD_INSECURE_SERVICE_NAME = 'com.apple.mobile.insecure_notification_proxy.shim.remote'
+
+    def __init__(self, lockdown: LockdownServiceProvider, insecure=False, timeout: Union[float, int] = None):
+        if isinstance(lockdown, RemoteServiceDiscoveryService):
+            secure_service_name = self.RSD_SERVICE_NAME
+            insecure_service_name = self.RSD_INSECURE_SERVICE_NAME
+        else:
+            secure_service_name = self.SERVICE_NAME
+            insecure_service_name = self.INSECURE_SERVICE_NAME
 
-    def __init__(self, lockdown: LockdownClient, insecure=False, timeout: Union[float, int] = None):
         if insecure:
-            super().__init__(lockdown, self.INSECURE_SERVICE_NAME)
+            super().__init__(lockdown, insecure_service_name)
         else:
-            super().__init__(lockdown, self.SERVICE_NAME)
+            super().__init__(lockdown, secure_service_name)
 
         if timeout is not None:
             self.service.socket.settimeout(timeout)
 
     def notify_post(self, name: str) -> None:
         """ Send notification to the device's notification_proxy. """
-        self.service.send_plist({'Command': 'PostNotification',
-                                 'Name': name})
+        self.service.send_plist({'Command': 'PostNotification', 'Name': name})
 
     def notify_register_dispatch(self, name: str) -> None:
         """ Tells the device to send a notification on the specified event. """
         self.logger.info(f'Observing {name}')
-        self.service.send_plist({'Command': 'ObserveNotification',
-                                 'Name': name})
+        self.service.send_plist({'Command': 'ObserveNotification', 'Name': name})
 
     def receive_notification(self) -> Generator[Mapping, None, None]:
         while True:
             try:
                 yield self.service.recv_plist()
             except socket.timeout as e:
                 raise NotificationTimeoutError from e
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/os_trace.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/os_trace.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
-import logging
 import plistlib
 import struct
 import tempfile
 import typing
 from datetime import datetime
 from tarfile import TarFile
 
 from construct import Adapter, Byte, Bytes, Computed, Enum, Int16ul, Int32ul, Optional, RepeatUntil, Struct, this
 
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.lockdown_service import LockdownService
 from pymobiledevice3.utils import try_decode
 
 CHUNK_SIZE = 4096
 TIME_FORMAT = '%H:%M:%S'
 SYSLOG_LINE_SPLITTER = '\n\x00'
 
 
@@ -58,27 +58,30 @@
         'subsystem' / Computed(lambda ctx: try_decode(ctx._subsystem[:-1])),
         '_category' / Bytes(this._._category_size),
         'category' / Computed(lambda ctx: try_decode(ctx._category[:-1])),
     )),
 )
 
 
-class OsTraceService(BaseService):
+class OsTraceService(LockdownService):
     """
     Provides API for the following operations:
     * Show process list (process name and pid)
     * Stream syslog lines in binary form with optional filtering by pid.
     * Get old stored syslog archive in PAX format (can be extracted using `pax -r < filename`).
         * Archive contain the contents are the `/var/db/diagnostics` directory
     """
     SERVICE_NAME = 'com.apple.os_trace_relay'
+    RSD_SERVICE_NAME = 'com.apple.os_trace_relay.shim.remote'
 
-    def __init__(self, lockdown: LockdownClient):
-        super().__init__(lockdown, self.SERVICE_NAME)
-        self.logger = logging.getLogger(__name__)
+    def __init__(self, lockdown: LockdownServiceProvider):
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
 
     def get_pid_list(self):
         self.service.send_plist({'Request': 'PidList'})
 
         # ignore first received unknown byte
         self.service.recvall(1)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/pcapd.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/pcapd.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import socket
 import struct
 from typing import Generator
 
 from construct import Byte, Bytes, Container, CString, Int16ub, Int32ub, Int32ul, Padded, Seek, Struct, this
 
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 INTERFACE_NAMES = enum.Enum('InterfaceNames', names={
     'other': 1,
     'regular1822': 2,
     'hdh1822': 3,
     'ddnX25': 4,
     'rfc877x25': 5,
@@ -316,24 +317,28 @@
     'seconds' / Int32ub,
     'microseconds' / Int32ub,
     Seek(this.header_length),
     'data' / Bytes(this.packet_length),
 )
 
 
-class PcapdService(BaseService):
+class PcapdService(LockdownService):
     """
     Starting iOS 5, apple added a remote virtual interface (RVI) facility that allows mirroring networks traffic from
     an iOS device. On macOS, the virtual interface can be enabled with the rvictl command. This script allows to use
     this service on other systems.
     """
+    RSD_SERVICE_NAME = 'com.apple.pcapd.shim.remote'
     SERVICE_NAME = 'com.apple.pcapd'
 
-    def __init__(self, lockdown: LockdownClient):
-        super().__init__(lockdown, self.SERVICE_NAME)
+    def __init__(self, lockdown: LockdownServiceProvider):
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
 
     def watch(self, packets_count: int = -1, process: str = None) -> Generator[Container, None, None]:
         packet_index = 0
         while packet_index != packets_count:
             d = self.service.recv_plist()
             if not d:
                 break
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/remote_server.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/remote_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import IPython
 from bpylist2 import archiver
 from construct import Adapter, Const, Default, GreedyBytes, GreedyRange, Int16ul, Int32sl, Int32ul, Int64ul, Prefixed, \
     Select, Struct, Switch, this
 from pygments import formatters, highlight, lexers
 
 from pymobiledevice3.exceptions import DvtException, UnrecognizedSelectorError
-from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 SHELL_USAGE = '''
 # This shell allows you to send messages to the DVTSecureSocketProxy and receive answers easily.
 # Generally speaking, each channel represents a group of actions.
 # Calling actions is done using a selector and auxiliary (parameters).
 # Receiving answers is done by getting a return value and seldom auxiliary (private / extra parameters).
 # To see the available channels, type the following:
@@ -183,15 +183,15 @@
             self._stream_packet_data += chunk
             if mheader.fragmentId == mheader.fragmentCount - 1:
                 # last message
                 self._messages.put(self._stream_packet_data)
                 self._stream_packet_data = b''
 
 
-class RemoteServer(BaseService):
+class RemoteServer(LockdownService):
     """
     Wrapper to Apple's RemoteServer.
     This server exports several ObjC objects allowing calling their respective selectors.
     The `/Developer/Library/PrivateFrameworks/DVTInstrumentsFoundation.framework/DTServiceHub` service reads the
     configuration stored from `[[NSUserDefaults standardUserDefaults] boolForKey:@"DTXConnectionTracer"]`
     If the value is true, then `/tmp/DTServiceHub[PID].DTXConnection.RANDOM.log` is created and can be used to debug the
     transport protocol.
@@ -227,21 +227,22 @@
         var protocol = ObjC.protocols[name]
         if ('DTXAllowedRPC' in protocol.protocols) {
             console.log('@protocol', name)
             console.log('  ' + Object.keys(protocol.methods).join('\n  '))
         }
     }
     ```
-    """
+    """  # noqa: E501
     BROADCAST_CHANNEL = 0
     INSTRUMENTS_MESSAGE_TYPE = 2
     EXPECTS_REPLY_MASK = 0x1000
 
-    def __init__(self, lockdown: LockdownClient, service_name, remove_ssl_context=True):
-        super().__init__(lockdown, service_name, is_developer_service=True)
+    def __init__(self, lockdown: LockdownServiceProvider, service_name, remove_ssl_context: bool = True,
+                 is_developer_service: bool = True):
+        super().__init__(lockdown, service_name, is_developer_service=is_developer_service)
 
         if remove_ssl_context and hasattr(self.service.socket, '_sslobj'):
             self.service.socket._sslobj = None
 
         self.supported_identifiers = {}
         self.last_channel_code = 0
         self.cur_message = 0
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/screenshot.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/screenshot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
-class ScreenshotService(BaseService):
+class ScreenshotService(LockdownService):
     SERVICE_NAME = 'com.apple.mobile.screenshotr'
 
     def __init__(self, lockdown: LockdownClient):
         super().__init__(lockdown, self.SERVICE_NAME, is_developer_service=True)
 
         dl_message_version_exchange = self.service.recv_plist()
         version_major = dl_message_version_exchange[1]
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/simulate_location.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/simulate_location.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import struct
 import time
 
 import gpxpy
 
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.services.lockdown_service import LockdownService
 
 
-class DtSimulateLocation(BaseService):
+class DtSimulateLocation(LockdownService):
     SERVICE_NAME = 'com.apple.dt.simulatelocation'
 
     def __init__(self, lockdown: LockdownClient):
         super().__init__(lockdown, self.SERVICE_NAME)
 
     def clear(self):
         """ stop simulation """
-        service = self.lockdown.start_developer_service(self.SERVICE_NAME)
+        service = self.lockdown.start_lockdown_developer_service(self.SERVICE_NAME)
         service.sendall(struct.pack('>I', 1))
 
     def set(self, latitude: float, longitude: float):
         """ stop simulation """
-        service = self.lockdown.start_developer_service(self.SERVICE_NAME)
+        service = self.lockdown.start_lockdown_developer_service(self.SERVICE_NAME)
         service.sendall(struct.pack('>I', 0))
         latitude = str(latitude).encode()
         longitude = str(longitude).encode()
         service.sendall(struct.pack('>I', len(latitude)) + latitude)
         service.sendall(struct.pack('>I', len(longitude)) + longitude)
 
     def play_gpx_file(self, filename: str, disable_sleep: bool = False):
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/syslog.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/syslog.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.services.lockdown_service import LockdownService
 from pymobiledevice3.utils import try_decode
 
 CHUNK_SIZE = 4096
 TIME_FORMAT = '%H:%M:%S'
 SYSLOG_LINE_SPLITTER = b'\n\x00'
 
 
-class SyslogService(BaseService):
+class SyslogService(LockdownService):
     """
     View system logs
     """
 
     SERVICE_NAME = 'com.apple.syslog_relay'
+    RSD_SERVICE_NAME = 'com.apple.syslog_relay.shim.remote'
 
-    def __init__(self, lockdown: LockdownClient):
-        super().__init__(lockdown, self.SERVICE_NAME)
+    def __init__(self, lockdown: LockdownServiceProvider):
+        if isinstance(lockdown, LockdownClient):
+            super().__init__(lockdown, self.SERVICE_NAME)
+        else:
+            super().__init__(lockdown, self.RSD_SERVICE_NAME)
 
     def watch(self):
         buf = b''
         while True:
             # read in chunks till we have at least one syslog line
             chunk = self.service.recv(CHUNK_SIZE)
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/alert.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/alert.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/automation_session.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/automation_session.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/cdp_screencast.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/cdp_screencast.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/cdp_server.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/cdp_server.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/cdp_target.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/cdp_target.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/driver.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/driver.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/element.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/element.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/inspector_session.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/inspector_session.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/selenium_api.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/selenium_api.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/session_protocol.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/session_protocol.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/web_protocol/switch_to.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/web_protocol/switch_to.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/services/webinspector.py` & `pymobiledevice3-2.1.0/pymobiledevice3/services/webinspector.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from typing import Mapping, Optional, Tuple, Union
 
 import nest_asyncio
 
 from pymobiledevice3.exceptions import LaunchingApplicationError, RemoteAutomationNotEnabledError, \
     WebInspectorNotEnabledError
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.service_connection import ServiceConnection
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
+from pymobiledevice3.service_connection import LockdownServiceConnection
 from pymobiledevice3.services.web_protocol.automation_session import AutomationSession
 from pymobiledevice3.services.web_protocol.inspector_session import InspectorSession
 from pymobiledevice3.services.web_protocol.session_protocol import SessionProtocol
 
 SAFARI = 'com.apple.mobilesafari'
 
 
@@ -101,27 +102,34 @@
             app_dict['WIRIsApplicationReadyKey'],
             app_dict.get('WIRHostApplicationIdentifierKey', ''),
         )
 
 
 class WebinspectorService:
     SERVICE_NAME = 'com.apple.webinspector'
+    RSD_SERVICE_NAME = 'com.apple.webinspector.shim.remote'
 
-    def __init__(self, lockdown: LockdownClient, loop=None):
+    def __init__(self, lockdown: LockdownServiceProvider, loop=None):
         if loop is None:
             try:
                 loop = asyncio.get_running_loop()
             except RuntimeError:
                 loop = asyncio.new_event_loop()
                 asyncio.set_event_loop(loop)
         nest_asyncio.apply(loop)
+
+        if isinstance(lockdown, LockdownClient):
+            self.service_name = self.SERVICE_NAME
+        else:
+            self.service_name = self.RSD_SERVICE_NAME
+
         self.loop = loop
         self.logger = logging.getLogger(__name__)
         self.lockdown = lockdown
-        self.service: Optional[ServiceConnection] = None
+        self.service: Optional[LockdownServiceConnection] = None
         self.connection_id = str(uuid.uuid4()).upper()
         self.state = None
         self.connected_application = {}
         self.application_pages = {}
         self.wir_message_results = {}
         self.wir_events = []
         self.receive_handlers = {
@@ -133,15 +141,15 @@
             '_rpc_applicationConnected:': self._handle_application_connected,
             '_rpc_applicationSentData:': self._handle_application_sent_data,
             '_rpc_applicationDisconnected:': self._handle_application_disconnected,
         }
         self._recv_task: Optional[asyncio.Task] = None
 
     def connect(self, timeout: Union[float, int] = None):
-        self.service = self.await_(self.lockdown.aio_start_service(self.SERVICE_NAME))
+        self.service = self.await_(self.lockdown.aio_start_lockdown_service(self.service_name))
         self.await_(self._report_identifier())
         try:
             self._handle_recv(self.await_(asyncio.wait_for(self._recv_message(), timeout)))
         except asyncio.TimeoutError as e:
             raise WebInspectorNotEnabledError from e
         self._recv_task = self.loop.create_task(self._receiving_task())
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/tcp_forwarder.py` & `pymobiledevice3-2.1.0/pymobiledevice3/tcp_forwarder.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import select
 import socket
 import threading
 
 from pymobiledevice3 import usbmux
 from pymobiledevice3.exceptions import ConnectionFailedError
 from pymobiledevice3.lockdown import create_using_usbmux
-from pymobiledevice3.service_connection import ServiceConnection
+from pymobiledevice3.service_connection import LockdownServiceConnection
 
 
 class TcpForwarder:
     """
     Allows forwarding local tcp connection into the device via a given lockdown connection
     """
 
@@ -116,15 +116,15 @@
         local_connection, client_address = self.server_socket.accept()
         local_connection.setblocking(False)
 
         try:
             if self.enable_ssl:
                 # use the lockdown pairing record
                 lockdown = create_using_usbmux(self.serial, connection_type=self.usbmux_connection_type)
-                service_connection = ServiceConnection.create_using_usbmux(
+                service_connection = LockdownServiceConnection.create_using_usbmux(
                     self.serial, self.dst_port, connection_type=self.usbmux_connection_type)
 
                 with lockdown.ssl_file() as ssl_file:
                     service_connection.ssl_start(ssl_file)
 
                 remote_connection = service_connection.socket
             else:
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/usbmux.py` & `pymobiledevice3-2.1.0/pymobiledevice3/usbmux.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3/utils.py` & `pymobiledevice3-2.1.0/pymobiledevice3/utils.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3.egg-info/PKG-INFO` & `pymobiledevice3-2.1.0/pymobiledevice3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymobiledevice3
-Version: 2.0.4
+Version: 2.1.0
 Summary: Pure python3 implementation for working with iDevices (iPhone, etc...)
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -872,26 +872,26 @@
 * The following will require Web Inspector feature to be turned on:
     * Get interactive JavaScript shell on any open tab:
         * `pymobiledevice3 webinspector js_shell`
     * List currently opened tabs is device's browser:
         * `pymobiledevice3 webinspector opened-tabs`
     * The following will require also the Remote Automation feature to be turned on:
         * Get interactive JavaScript shell on new remote automation tab:
-            * `pymobiledevice3 webinspector js_shell --automation` 
+            * `pymobiledevice3 webinspector js_shell --automation`
         * Launch an automation session to view a given URL:
             * `pymobiledevice3 webinspector launch URL`
         * Get a a selenium-like shell:
             * `pymobiledevice3 webinspector shell`
-* Mount DeveloperDiskImage:
-    * `pymobiledevice3 mounter mount`
+* Mount DeveloperDiskImage (On iOS>=17.0, each command will require an additional `--rsd` option):
+    * `pymobiledevice3 mounter auto-mount`
     * The following will assume the DeveloperDiskImage is already mounted:
         * Simulate an `x y` location:
             * `pymobiledevice3 developer simulate-location set x y`
         * Taking a screenshot from the device:
-            * `pymobiledevice3 developer screenshot /path/to/screen.png`
+            * `pymobiledevice3 developer dvt screenshot /path/to/screen.png`
         * View detailed process list (including ppid, uid, guid, sandboxed, etc...):
             * `pymobiledevice3 developer dvt sysmon process single`
         * Sniffing oslog:
             * `pymobiledevice3 developer dvt oslog`
         * Kill a process:
             * `pymobiledevice3 developer dvt kill PID`
         * List files in a given directory (un-chrooted):
```

### Comparing `pymobiledevice3-2.0.4/pymobiledevice3.egg-info/SOURCES.txt` & `pymobiledevice3-2.1.0/pymobiledevice3.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
+misc/extract_plist_from_pcaps.py
+misc/remotexpc_sniffer.py
 pymobiledevice3/__init__.py
 pymobiledevice3/__main__.py
 pymobiledevice3/bonjour.py
 pymobiledevice3/ca.py
 pymobiledevice3/common.py
 pymobiledevice3/exceptions.py
 pymobiledevice3/irecv.py
 pymobiledevice3/irecv_devices.py
 pymobiledevice3/lockdown.py
+pymobiledevice3/lockdown_service_provider.py
 pymobiledevice3/pair_records.py
 pymobiledevice3/service_connection.py
 pymobiledevice3/tcp_forwarder.py
 pymobiledevice3/usbmux.py
 pymobiledevice3/utils.py
 pymobiledevice3.egg-info/PKG-INFO
 pymobiledevice3.egg-info/SOURCES.txt
@@ -47,18 +50,23 @@
 pymobiledevice3/cli/springboard.py
 pymobiledevice3/cli/syslog.py
 pymobiledevice3/cli/usbmux.py
 pymobiledevice3/cli/webinspector.py
 pymobiledevice3/remote/__init__.py
 pymobiledevice3/remote/bonjour.py
 pymobiledevice3/remote/core_device_tunnel_service.py
+pymobiledevice3/remote/remote_service.py
 pymobiledevice3/remote/remote_service_discovery.py
 pymobiledevice3/remote/remotexpc.py
-pymobiledevice3/remote/sniffer.py
 pymobiledevice3/remote/xpc_message.py
+pymobiledevice3/remote/core_device/__init__.py
+pymobiledevice3/remote/core_device/app_service.py
+pymobiledevice3/remote/core_device/core_device_service.py
+pymobiledevice3/remote/core_device/device_info.py
+pymobiledevice3/remote/core_device/diagnostics_service.py
 pymobiledevice3/resources/__init__.py
 pymobiledevice3/resources/dsc_uuid_map.json
 pymobiledevice3/resources/dsc_uuid_map.py
 pymobiledevice3/resources/firmware_notifications.py
 pymobiledevice3/resources/notifications.txt
 pymobiledevice3/resources/webinspector/element_attribute.js
 pymobiledevice3/resources/webinspector/element_clear.js
@@ -81,37 +89,38 @@
 pymobiledevice3/restore/restore_options.py
 pymobiledevice3/restore/restored_client.py
 pymobiledevice3/restore/tss.py
 pymobiledevice3/services/__init__.py
 pymobiledevice3/services/accessibilityaudit.py
 pymobiledevice3/services/afc.py
 pymobiledevice3/services/amfi.py
-pymobiledevice3/services/base_service.py
 pymobiledevice3/services/companion.py
 pymobiledevice3/services/crash_reports.py
 pymobiledevice3/services/debugserver_applist.py
 pymobiledevice3/services/device_arbitration.py
 pymobiledevice3/services/device_link.py
 pymobiledevice3/services/diagnostics.py
 pymobiledevice3/services/dtfetchsymbols.py
 pymobiledevice3/services/file_relay.py
 pymobiledevice3/services/heartbeat.py
 pymobiledevice3/services/house_arrest.py
 pymobiledevice3/services/installation_proxy.py
+pymobiledevice3/services/lockdown_service.py
 pymobiledevice3/services/misagent.py
 pymobiledevice3/services/mobile_activation.py
 pymobiledevice3/services/mobile_config.py
 pymobiledevice3/services/mobile_image_mounter.py
 pymobiledevice3/services/mobilebackup2.py
 pymobiledevice3/services/notification_proxy.py
 pymobiledevice3/services/os_trace.py
 pymobiledevice3/services/pcapd.py
 pymobiledevice3/services/power_assertion.py
 pymobiledevice3/services/preboard.py
 pymobiledevice3/services/remote_server.py
+pymobiledevice3/services/restore_service.py
 pymobiledevice3/services/screenshot.py
 pymobiledevice3/services/simulate_location.py
 pymobiledevice3/services/springboard.py
 pymobiledevice3/services/syslog.py
 pymobiledevice3/services/webinspector.py
 pymobiledevice3/services/dvt/__init__.py
 pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
```

### Comparing `pymobiledevice3-2.0.4/pyproject.toml` & `pymobiledevice3-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymobiledevice3"
-version = "2.0.4"
+version = "2.1.0"
 description = "Pure python3 implementation for working with iDevices (iPhone, etc...)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "protocol", "lockdownd", "instruments", "automation", "cli", "afc"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" },
```

