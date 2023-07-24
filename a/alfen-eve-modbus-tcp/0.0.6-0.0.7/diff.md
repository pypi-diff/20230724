# Comparing `tmp/alfen_eve_modbus_tcp-0.0.6.tar.gz` & `tmp/alfen_eve_modbus_tcp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfen_eve_modbus_tcp-0.0.6.tar", last modified: Sun Jul 23 13:18:43 2023, max compression
+gzip compressed data, was "alfen_eve_modbus_tcp-0.0.7.tar", last modified: Mon Jul 24 09:58:26 2023, max compression
```

## Comparing `alfen_eve_modbus_tcp-0.0.6.tar` & `alfen_eve_modbus_tcp-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-23 13:18:43.593149 alfen_eve_modbus_tcp-0.0.6/
--rw-rw-r--   0 luc       (1000) luc       (1000)     1063 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.6/LICENSE
--rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-23 13:18:43.593149 alfen_eve_modbus_tcp-0.0.6/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)    11717 2023-07-16 19:44:24.000000 alfen_eve_modbus_tcp-0.0.6/README.md
--rw-rw-r--   0 luc       (1000) luc       (1000)      861 2023-07-23 13:18:43.593149 alfen_eve_modbus_tcp-0.0.6/setup.cfg
--rwxrwxr-x   0 luc       (1000) luc       (1000)       38 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.6/setup.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-23 13:18:43.589149 alfen_eve_modbus_tcp-0.0.6/src/
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-23 13:18:43.593149 alfen_eve_modbus_tcp-0.0.6/src/alfen_eve_modbus_tcp/
--rw-rw-r--   0 luc       (1000) luc       (1000)    24382 2023-07-23 13:12:31.000000 alfen_eve_modbus_tcp-0.0.6/src/alfen_eve_modbus_tcp/__init__.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-23 13:18:43.593149 alfen_eve_modbus_tcp-0.0.6/src/alfen_eve_modbus_tcp.egg-info/
--rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-23 13:18:43.000000 alfen_eve_modbus_tcp-0.0.6/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)      312 2023-07-23 13:18:43.000000 alfen_eve_modbus_tcp-0.0.6/src/alfen_eve_modbus_tcp.egg-info/SOURCES.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-23 13:18:43.000000 alfen_eve_modbus_tcp-0.0.6/src/alfen_eve_modbus_tcp.egg-info/dependency_links.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       40 2023-07-23 13:18:43.000000 alfen_eve_modbus_tcp-0.0.6/src/alfen_eve_modbus_tcp.egg-info/requires.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       21 2023-07-23 13:18:43.000000 alfen_eve_modbus_tcp-0.0.6/src/alfen_eve_modbus_tcp.egg-info/top_level.txt
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 09:58:26.919999 alfen_eve_modbus_tcp-0.0.7/
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1063 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.7/LICENSE
+-rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-24 09:58:26.919999 alfen_eve_modbus_tcp-0.0.7/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)    11717 2023-07-16 19:44:24.000000 alfen_eve_modbus_tcp-0.0.7/README.md
+-rw-rw-r--   0 luc       (1000) luc       (1000)      861 2023-07-24 09:58:26.919999 alfen_eve_modbus_tcp-0.0.7/setup.cfg
+-rwxrwxr-x   0 luc       (1000) luc       (1000)       38 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.7/setup.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 09:58:26.915998 alfen_eve_modbus_tcp-0.0.7/src/
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 09:58:26.915998 alfen_eve_modbus_tcp-0.0.7/src/alfen_eve_modbus_tcp/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    25465 2023-07-24 08:58:45.000000 alfen_eve_modbus_tcp-0.0.7/src/alfen_eve_modbus_tcp/__init__.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-24 09:58:26.915998 alfen_eve_modbus_tcp-0.0.7/src/alfen_eve_modbus_tcp.egg-info/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-24 09:58:26.000000 alfen_eve_modbus_tcp-0.0.7/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)      312 2023-07-24 09:58:26.000000 alfen_eve_modbus_tcp-0.0.7/src/alfen_eve_modbus_tcp.egg-info/SOURCES.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-24 09:58:26.000000 alfen_eve_modbus_tcp-0.0.7/src/alfen_eve_modbus_tcp.egg-info/dependency_links.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       40 2023-07-24 09:58:26.000000 alfen_eve_modbus_tcp-0.0.7/src/alfen_eve_modbus_tcp.egg-info/requires.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       21 2023-07-24 09:58:26.000000 alfen_eve_modbus_tcp-0.0.7/src/alfen_eve_modbus_tcp.egg-info/top_level.txt
```

### Comparing `alfen_eve_modbus_tcp-0.0.6/LICENSE` & `alfen_eve_modbus_tcp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alfen_eve_modbus_tcp-0.0.6/PKG-INFO` & `alfen_eve_modbus_tcp-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfen_eve_modbus_tcp
-Version: 0.0.6
+Version: 0.0.7
 Summary: Alfen Eve Car Charger parser library
 Home-page: https://github.com/nessnaj/alfen_eve_modbus_tcp
 Author: nessnaj
 License: MIT License
 Project-URL: Issue Tracker, https://github.com/nessnaj/alfen_eve_modbus_tcp/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `alfen_eve_modbus_tcp-0.0.6/README.md` & `alfen_eve_modbus_tcp-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alfen_eve_modbus_tcp-0.0.6/setup.cfg` & `alfen_eve_modbus_tcp-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alfen_eve_modbus_tcp
-version = 0.0.6
+version = 0.0.7
 author = nessnaj
 description = Alfen Eve Car Charger parser library
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 url = https://github.com/nessnaj/alfen_eve_modbus_tcp
 project_urls =
```

### Comparing `alfen_eve_modbus_tcp-0.0.6/src/alfen_eve_modbus_tcp/__init__.py` & `alfen_eve_modbus_tcp-0.0.7/src/alfen_eve_modbus_tcp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -509,7 +509,27 @@
                     current_phases = self.read('charge_using_1_or_3_phases')['charge_using_1_or_3_phases']
                     syslog.syslog(f"Current phase(s): {current_phases}")
         else:
             syslog.syslog(f"Invalid # of phases: {phases}...")
 
     def set_current(self, current):
         self.write('modbus_slave_max_current', current)
+
+    def set_charge_profile(self, phases, current):
+        mode_3_state = self.read('mode_3_state')
+        status = MODE_3_STATE_MAP[mode_3_state['mode_3_state']]
+        if (status == "Charging" or status == "Connected"):
+            current_phases = int(self.read('charge_using_1_or_3_phases')['charge_using_1_or_3_phases'])
+            syslog.syslog(f"Current Phase(s): {current_phases} versus Requested Phase(s): {phases}")
+            if current_phases != phases:
+                if status == "Charging":
+                    self.pause_charging()
+                    time.sleep(1)
+                self.switch_phase(phases)
+            self.set_current(current)
+            time.sleep(1)
+            phases = self.read('charge_using_1_or_3_phases')['charge_using_1_or_3_phases']
+            current = self.read('modbus_slave_max_current')['modbus_slave_max_current']
+            syslog.syslog(f"Charge Profile Set: Phase(s): {phases}; Current: {current} A.")
+        else:
+            syslog.syslog(f"Car is not connected: {status}, so no changes in charge profile applied.")
+
```

### Comparing `alfen_eve_modbus_tcp-0.0.6/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO` & `alfen_eve_modbus_tcp-0.0.7/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfen-eve-modbus-tcp
-Version: 0.0.6
+Version: 0.0.7
 Summary: Alfen Eve Car Charger parser library
 Home-page: https://github.com/nessnaj/alfen_eve_modbus_tcp
 Author: nessnaj
 License: MIT License
 Project-URL: Issue Tracker, https://github.com/nessnaj/alfen_eve_modbus_tcp/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
```

