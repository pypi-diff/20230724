# Comparing `tmp/arivo-settings_models-0.0.1rc4.tar.gz` & `tmp/arivo-settings_models-0.0.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arivo-settings_models-0.0.1rc4.tar", last modified: Fri Jun 30 09:21:26 2023, max compression
+gzip compressed data, was "dist/arivo-settings_models-0.0.1rc5.tar", last modified: Mon Jul 24 13:36:33 2023, max compression
```

## Comparing `arivo-settings_models-0.0.1rc4.tar` & `arivo-settings_models-0.0.1rc5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      922 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/settings_models/
--rw-rw-rw-   0 root         (0) root         (0)     6344 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/intercom.py
--rw-rw-rw-   0 root         (0) root         (0)    20317 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/gate_control.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/enforcement.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/device_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/doc.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/_combat.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/validators.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tox.ini
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/docs/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/docs/migrations.md
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/test-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/tests/
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11501 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)    37784 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tests/test_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     3417 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tests/test_serialization.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1371 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/ChangeLog
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/tools/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tools/pages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc5/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/AUTHORS
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/settings_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:35:40.000000 arivo-settings_models-0.0.1rc5/settings_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/gate_control.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/intercom.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:35:40.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/enforcement.py
+-rw-rw-rw-   0 root         (0) root         (0)    20512 2023-07-24 13:35:39.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/device_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/_combat.py
+-rw-rw-rw-   0 root         (0) root         (0)     6344 2023-06-28 13:41:28.000000 arivo-settings_models-0.0.1rc5/settings_models/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc5/tox.ini
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc5/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      707 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-06-22 11:55:45.000000 arivo-settings_models-0.0.1rc5/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc5/tools/pages.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/tests/test_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)    38906 2023-07-24 13:35:39.000000 arivo-settings_models-0.0.1rc5/tests/test_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)    11501 2023-06-28 13:41:28.000000 arivo-settings_models-0.0.1rc5/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc5/README.md
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc5/test-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc5/docs/migrations.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      707 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/top_level.txt
```

### Comparing `arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/PKG-INFO` & `arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings-models
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/SOURCES.txt` & `arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc4/setup.cfg` & `arivo-settings_models-0.0.1rc5/setup.cfg`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc4/settings_models/serialization.py` & `arivo-settings_models-0.0.1rc5/settings_models/serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc4/settings_models/settings/common.py` & `arivo-settings_models-0.0.1rc5/settings_models/settings/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,16 @@
     @root_validator(skip_on_failure=True)
     def validate_shortterm_gates_in_gates(cls, values):
         """
         check if all shortterm gates are in gates
         """
         if not all(gate in values["gates"] for gate in values["shortterm_gates"]):
             raise ValueError("All shortterm gates must be in gates")
+        if len(values["shortterm_gates"]) == 0 and len(values["default_cost_entries"]) > 0:
+            raise ValueError("If no shortterm gates are defined, no default cost entries are allowed")
         return values
 
 
 class Parksetting(SettingsModel):
     """
     Defines the terms and conditions for parking sessions of registered users. This is not used for registered
     shortterm parkers.
```

### Comparing `arivo-settings_models-0.0.1rc4/settings_models/settings/gate_control.py` & `arivo-settings_models-0.0.1rc5/settings_models/settings/gate_control.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc4/settings_models/settings/device_keys.py` & `arivo-settings_models-0.0.1rc5/settings_models/settings/device_keys.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc4/settings_models/validators.py` & `arivo-settings_models-0.0.1rc5/settings_models/validators.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc4/PKG-INFO` & `arivo-settings_models-0.0.1rc5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings_models
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-0.0.1rc4/.gitlab-ci.yml` & `arivo-settings_models-0.0.1rc5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc4/tests/utils.py` & `arivo-settings_models-0.0.1rc5/tests/utils.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc4/tests/test_models.py` & `arivo-settings_models-0.0.1rc5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc4/tests/test_validation.py` & `arivo-settings_models-0.0.1rc5/tests/test_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,20 +350,37 @@
         gt = dump_setting({"0eec2445-15c3-4af8-b362-aeb1f278e3ac": {
             "id": "0eec2445-15c3-4af8-b362-aeb1f278e3ac", "default_cost_entries":
                 [{"entry_type": "rate_change", "group": "parking_default",
                   "value": "7a50fafd-3426-42c8-bf3c-ca708638c327", "account_id": "0"}],
             "pay_per_use_cost_entries":
                 [{"entry_type": "rate_change", "group": "parking_default",
                   "value": "7a50fafd-3426-42c8-bf3c-ca708638c327", "account_id": "0"}],
-            "gates": ["gate1"], "name": "Gesamter Parkplatz", "shortterm_gates": [],
+            "gates": ["gate1"], "name": "Gesamter Parkplatz", "shortterm_gates": ["gate1"],
             "shortterm_limit_type": "no_limit", "shortterm_limit": 0}
         })
         res = parse_setting("common/parking_areas2", gt)
         self.assert_result(dump_setting(res), gt)
 
+    def test_parking_areas_no_cost_entries_without_shortterm(self):
+        self.maxDiff = None
+        with self.assertRaises(ValidationError) as e:
+            gt = dump_setting({"0eec2445-15c3-4af8-b362-aeb1f278e3ac": {
+                "id": "0eec2445-15c3-4af8-b362-aeb1f278e3ac", "default_cost_entries":
+                    [{"entry_type": "rate_change", "group": "parking_default",
+                      "value": "7a50fafd-3426-42c8-bf3c-ca708638c327", "account_id": "0"}],
+                "pay_per_use_cost_entries":
+                    [{"entry_type": "rate_change", "group": "parking_default",
+                      "value": "7a50fafd-3426-42c8-bf3c-ca708638c327", "account_id": "0"}],
+                "gates": ["gate1"], "name": "Gesamter Parkplatz", "shortterm_gates": [],
+                "shortterm_limit_type": "no_limit", "shortterm_limit": 0}
+            })
+            parse_setting("common/parking_areas2", gt)
+        self.assertEqual(str(e.exception).count("\n"), 2)
+        self.assertIn("If no shortterm gates are defined, no default cost entries are allowed", str(e.exception))
+
     def test_parking_areas_gates_no_empty_list(self):
         with self.assertRaises(ValidationError) as e:
             parse_setting("common/parking_areas2", dump_setting({
                 "0eec2445-15c3-4af8-b362-aeb1f278e3ac": {
                     "id": "0eec2445-15c3-4af8-b362-aeb1f278e3ac", "default_cost_entries":
                         [{"entry_type": "rate_change", "group": "parking_default",
                           "value": "7a50fafd-3426-42c8-bf3c-ca708638c327", "account_id": "0"}],
@@ -389,27 +406,27 @@
     def test_parking_areas_id_does_not_match_field(self):
         with self.assertRaises(ValueError) as e:
             parse_setting("common/parking_areas2", dump_setting({
                 "7a50fafd-3426-42c8-bf3c-ca708638c327": {
                     "id": "0eec2445-15c3-4af8-b362-aeb1f278e3ac", "default_cost_entries":
                         [{"entry_type": "rate_change", "group": "parking_default",
                           "value": "7a50fafd-3426-42c8-bf3c-ca708638c327", "account_id": "0"}],
-                    "gates": ["gate1"], "name": "Gesamter Parkplatz", "shortterm_gates": [],
+                    "gates": ["gate1"], "name": "Gesamter Parkplatz", "shortterm_gates": ["gate1"],
                     "shortterm_limit_type": "no_limit", "shortterm_limit": 0}
             }))
         self.assertEqual(str(e.exception).count("\n"), 0)
         self.assertEqual("key must match field id", str(e.exception))
 
         with self.assertRaises(ValueError) as e:
             parse_setting("common/parking_areas2", dump_setting({
                 "123": {
                     "id": "0eec2445-15c3-4af8-b362-aeb1f278e3ac", "default_cost_entries":
                         [{"entry_type": "rate_change", "group": "parking_default",
                           "value": "7a50fafd-3426-42c8-bf3c-ca708638c327", "account_id": "0"}],
-                    "gates": ["gate1"], "name": "Gesamter Parkplatz", "shortterm_gates": [],
+                    "gates": ["gate1"], "name": "Gesamter Parkplatz", "shortterm_gates": ["gate1"],
                     "shortterm_limit_type": "no_limit", "shortterm_limit": 0}
             }))
         self.assertEqual(str(e.exception).count("\n"), 0)
         self.assertIn("key must match field id", str(e.exception))
 
     def test_parking_areas_invalid_default_cost_entry_type(self):
         with self.assertRaises(ValidationError) as e:
```

### Comparing `arivo-settings_models-0.0.1rc4/tests/test_serialization.py` & `arivo-settings_models-0.0.1rc5/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc4/ChangeLog` & `arivo-settings_models-0.0.1rc5/ChangeLog`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v0.0.1rc5
+---------
+
+* parking areas: default cost entries requires shortterm gates
+
 v0.0.1rc4
 ---------
 
 * parksettings must have gates specified (again) changed comments for gate types
 * renamed GateType enums
 
 v0.0.1rc3
@@ -59,8 +64,7 @@
 ---------
 
 * added testcase for refs
 * coverage fix
 * removing pages stage because no documentation yet
 * settings models and parsing/serializing
 * committing before weekend [skip ci]
-* test something
```

