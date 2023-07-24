# Comparing `tmp/netbox_powerdns_sync-0.0.1.tar.gz` & `tmp/netbox_powerdns_sync-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_powerdns_sync-0.0.1.tar", max compression
+gzip compressed data, was "netbox_powerdns_sync-0.0.2.tar", max compression
```

## Comparing `netbox_powerdns_sync-0.0.1.tar` & `netbox_powerdns_sync-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1062 2023-06-16 16:20:28.327727 netbox_powerdns_sync-0.0.1/LICENSE
--rw-r--r--   0        0        0     4971 2023-07-24 12:00:36.790485 netbox_powerdns_sync-0.0.1/README.md
--rw-r--r--   0        0        0      707 2023-07-24 12:01:54.379841 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 09:39:42.586125 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/api/__init__.py
--rw-r--r--   0        0        0      808 2023-07-14 14:51:54.445561 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/api/nested_serializers.py
--rw-r--r--   0        0        0     1934 2023-07-24 10:38:29.112831 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/api/serializers.py
--rw-r--r--   0        0        0      251 2023-07-14 10:29:50.069380 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/api/urls.py
--rw-r--r--   0        0        0      734 2023-07-14 13:44:48.625591 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/api/views.py
--rw-r--r--   0        0        0      925 2023-07-19 09:48:22.646046 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/choices.py
--rw-r--r--   0        0        0      334 2023-07-24 09:57:50.846535 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/constants.py
--rw-r--r--   0        0        0      295 2023-07-21 12:56:21.382815 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/exceptions.py
--rw-r--r--   0        0        0      705 2023-07-21 11:17:45.310170 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/fields.py
--rw-r--r--   0        0        0     2620 2023-07-21 11:55:36.052188 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/filtersets.py
--rw-r--r--   0        0        0       73 2023-07-21 06:28:25.567195 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/forms/__init__.py
--rw-r--r--   0        0        0     2288 2023-07-21 11:54:49.515344 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/forms/filtersets.py
--rw-r--r--   0        0        0     3654 2023-07-24 10:25:42.915513 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/forms/model_forms.py
--rw-r--r--   0        0        0      719 2023-07-21 12:15:27.719704 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/forms/sync.py
--rw-r--r--   0        0        0    14872 2023-07-24 13:13:28.700733 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/jobs.py
--rw-r--r--   0        0        0     4094 2023-07-24 10:08:04.774247 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-14 09:22:39.629613 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/migrations/__init__.py
--rw-r--r--   0        0        0    10073 2023-07-24 10:38:42.525070 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/models.py
--rw-r--r--   0        0        0     4065 2023-07-21 12:46:19.280127 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/naming.py
--rw-r--r--   0        0        0     1113 2023-07-20 12:00:46.377066 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/navigation.py
--rw-r--r--   0        0        0      533 2023-07-21 11:44:51.208438 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/querysets.py
--rw-r--r--   0        0        0     1654 2023-07-14 13:32:48.730194 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/record.py
--rw-r--r--   0        0        0     4855 2023-07-24 13:11:37.593814 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/signals.py
--rw-r--r--   0        0        0     3843 2023-07-24 10:33:51.167916 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/tables.py
--rw-r--r--   0        0        0     2060 2023-07-14 14:59:40.742225 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html
--rw-r--r--   0        0        0     2047 2023-07-21 05:32:00.064298 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html
--rw-r--r--   0        0        0     1531 2023-07-20 13:25:16.258268 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html
--rw-r--r--   0        0        0     1378 2023-07-24 09:54:22.598492 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html
--rw-r--r--   0        0        0     1147 2023-07-21 08:49:12.068124 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html
--rw-r--r--   0        0        0     5565 2023-07-24 10:31:28.605424 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html
--rw-r--r--   0        0        0     1449 2023-07-21 12:18:17.038546 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/urls.py
--rw-r--r--   0        0        0     3312 2023-07-24 12:42:41.239436 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/utils.py
--rw-r--r--   0        0        0      280 2023-07-14 11:47:50.874790 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/validators.py
--rw-r--r--   0        0        0       22 2023-06-16 18:10:31.188405 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/version.py
--rw-r--r--   0        0        0       69 2023-07-20 07:26:23.220242 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/views/__init__.py
--rw-r--r--   0        0        0     2166 2023-07-14 11:23:44.770023 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/views/api_servers.py
--rw-r--r--   0        0        0     5085 2023-07-21 12:17:45.106008 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/views/syncs.py
--rw-r--r--   0        0        0     1546 2023-07-14 11:01:27.912653 netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/views/zones.py
--rw-r--r--   0        0        0      653 2023-07-24 14:04:59.117397 netbox_powerdns_sync-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 netbox_powerdns_sync-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4971 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/README.md
+-rw-r--r--   0        0        0      707 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/api/__init__.py
+-rw-r--r--   0        0        0      808 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/api/nested_serializers.py
+-rw-r--r--   0        0        0     1934 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/api/serializers.py
+-rw-r--r--   0        0        0      251 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/api/urls.py
+-rw-r--r--   0        0        0      734 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/api/views.py
+-rw-r--r--   0        0        0      925 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/choices.py
+-rw-r--r--   0        0        0      334 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/constants.py
+-rw-r--r--   0        0        0      295 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/exceptions.py
+-rw-r--r--   0        0        0      705 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/fields.py
+-rw-r--r--   0        0        0     2620 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/filtersets.py
+-rw-r--r--   0        0        0       73 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/forms/__init__.py
+-rw-r--r--   0        0        0     2288 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/forms/filtersets.py
+-rw-r--r--   0        0        0     3654 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/forms/model_forms.py
+-rw-r--r--   0        0        0      719 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/forms/sync.py
+-rw-r--r--   0        0        0    14872 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/jobs.py
+-rw-r--r--   0        0        0     4094 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/migrations/__init__.py
+-rw-r--r--   0        0        0    10073 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/models.py
+-rw-r--r--   0        0        0     4065 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/naming.py
+-rw-r--r--   0        0        0     1113 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/navigation.py
+-rw-r--r--   0        0        0      533 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/querysets.py
+-rw-r--r--   0        0        0     1654 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/record.py
+-rw-r--r--   0        0        0     4855 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/signals.py
+-rw-r--r--   0        0        0     3843 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/tables.py
+-rw-r--r--   0        0        0     2060 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html
+-rw-r--r--   0        0        0     2047 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html
+-rw-r--r--   0        0        0     1531 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html
+-rw-r--r--   0        0        0     1378 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html
+-rw-r--r--   0        0        0     1147 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html
+-rw-r--r--   0        0        0     5565 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html
+-rw-r--r--   0        0        0     1449 2023-07-24 14:33:47.727230 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/urls.py
+-rw-r--r--   0        0        0     3312 2023-07-24 14:33:47.731231 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/utils.py
+-rw-r--r--   0        0        0      280 2023-07-24 14:33:47.731231 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/validators.py
+-rw-r--r--   0        0        0       22 2023-07-24 14:33:47.731231 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/version.py
+-rw-r--r--   0        0        0       69 2023-07-24 14:33:47.731231 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/views/__init__.py
+-rw-r--r--   0        0        0     2166 2023-07-24 14:33:47.731231 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/views/api_servers.py
+-rw-r--r--   0        0        0     5085 2023-07-24 14:33:47.731231 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/views/syncs.py
+-rw-r--r--   0        0        0     1546 2023-07-24 14:33:47.731231 netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/views/zones.py
+-rw-r--r--   0        0        0      653 2023-07-24 14:33:47.731231 netbox_powerdns_sync-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 netbox_powerdns_sync-0.0.2/PKG-INFO
```

### Comparing `netbox_powerdns_sync-0.0.1/LICENSE` & `netbox_powerdns_sync-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/README.md` & `netbox_powerdns_sync-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/__init__.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/api/nested_serializers.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/api/serializers.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/api/views.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/choices.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/fields.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/fields.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/filtersets.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/forms/filtersets.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/forms/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/forms/model_forms.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/forms/model_forms.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/forms/sync.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/forms/sync.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/jobs.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/jobs.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/migrations/0001_initial.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/models.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/models.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/naming.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/naming.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/navigation.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/querysets.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/querysets.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/record.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/record.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/signals.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/signals.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/tables.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/urls.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/utils.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/utils.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/views/api_servers.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/views/api_servers.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/views/syncs.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/views/syncs.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/netbox_powerdns_sync/views/zones.py` & `netbox_powerdns_sync-0.0.2/netbox_powerdns_sync/views/zones.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.1/pyproject.toml` & `netbox_powerdns_sync-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netbox-powerdns-sync"
-version = "0.0.1"
+version = "0.0.2"
 description = "Sync DNS records in PowerDNS with NetBox"
 authors = ["Matej Vadnjal <matej.vadnjal@arnes.si>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ArnesSI/netbox-powerdns-sync/"
 keywords = ["netbox", "netbox-plugin", "powerdns"]
 packages = [{include = "netbox_powerdns_sync"}]
```

### Comparing `netbox_powerdns_sync-0.0.1/PKG-INFO` & `netbox_powerdns_sync-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-powerdns-sync
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sync DNS records in PowerDNS with NetBox
 Home-page: https://github.com/ArnesSI/netbox-powerdns-sync/
 License: MIT
 Keywords: netbox,netbox-plugin,powerdns
 Author: Matej Vadnjal
 Author-email: matej.vadnjal@arnes.si
 Requires-Python: >=3.9
```

