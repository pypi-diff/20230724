# Comparing `tmp/netbox_powerdns_sync-0.0.3.tar.gz` & `tmp/netbox_powerdns_sync-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_powerdns_sync-0.0.3.tar", max compression
+gzip compressed data, was "netbox_powerdns_sync-0.0.4.tar", max compression
```

## Comparing `netbox_powerdns_sync-0.0.3.tar` & `netbox_powerdns_sync-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1062 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/LICENSE
--rw-r--r--   0        0        0     4971 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/README.md
--rw-r--r--   0        0        0      707 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/api/__init__.py
--rw-r--r--   0        0        0      808 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/api/nested_serializers.py
--rw-r--r--   0        0        0     1934 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/api/serializers.py
--rw-r--r--   0        0        0      251 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/api/urls.py
--rw-r--r--   0        0        0      734 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/api/views.py
--rw-r--r--   0        0        0      925 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/choices.py
--rw-r--r--   0        0        0      334 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/constants.py
--rw-r--r--   0        0        0      295 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/exceptions.py
--rw-r--r--   0        0        0      705 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/fields.py
--rw-r--r--   0        0        0     2620 2023-07-24 15:41:19.927946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/filtersets.py
--rw-r--r--   0        0        0       73 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/forms/__init__.py
--rw-r--r--   0        0        0     2288 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/forms/filtersets.py
--rw-r--r--   0        0        0     3654 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/forms/model_forms.py
--rw-r--r--   0        0        0      719 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/forms/sync.py
--rw-r--r--   0        0        0    15260 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/jobs.py
--rw-r--r--   0        0        0     4094 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/migrations/__init__.py
--rw-r--r--   0        0        0    10073 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/models.py
--rw-r--r--   0        0        0     4065 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/naming.py
--rw-r--r--   0        0        0     1113 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/navigation.py
--rw-r--r--   0        0        0      533 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/querysets.py
--rw-r--r--   0        0        0     1654 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/record.py
--rw-r--r--   0        0        0     4855 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/signals.py
--rw-r--r--   0        0        0     3881 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/tables.py
--rw-r--r--   0        0        0     2060 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html
--rw-r--r--   0        0        0     2047 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html
--rw-r--r--   0        0        0     1531 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html
--rw-r--r--   0        0        0     1378 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html
--rw-r--r--   0        0        0     1147 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html
--rw-r--r--   0        0        0     5565 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html
--rw-r--r--   0        0        0     1449 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/urls.py
--rw-r--r--   0        0        0     3312 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/utils.py
--rw-r--r--   0        0        0      280 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/validators.py
--rw-r--r--   0        0        0       22 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/version.py
--rw-r--r--   0        0        0       69 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/views/__init__.py
--rw-r--r--   0        0        0     2166 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/views/api_servers.py
--rw-r--r--   0        0        0     5085 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/views/syncs.py
--rw-r--r--   0        0        0     1546 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/views/zones.py
--rw-r--r--   0        0        0      653 2023-07-24 15:41:19.931946 netbox_powerdns_sync-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 netbox_powerdns_sync-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-24 17:31:08.060448 netbox_powerdns_sync-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4971 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/README.md
+-rw-r--r--   0        0        0      707 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/__init__.py
+-rw-r--r--   0        0        0      808 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/nested_serializers.py
+-rw-r--r--   0        0        0     1934 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/serializers.py
+-rw-r--r--   0        0        0      251 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/urls.py
+-rw-r--r--   0        0        0      739 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/views.py
+-rw-r--r--   0        0        0      925 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/choices.py
+-rw-r--r--   0        0        0      334 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/constants.py
+-rw-r--r--   0        0        0      295 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/exceptions.py
+-rw-r--r--   0        0        0      705 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/fields.py
+-rw-r--r--   0        0        0     2620 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/filtersets.py
+-rw-r--r--   0        0        0       73 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/__init__.py
+-rw-r--r--   0        0        0     2288 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/filtersets.py
+-rw-r--r--   0        0        0     3654 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/model_forms.py
+-rw-r--r--   0        0        0      719 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/sync.py
+-rw-r--r--   0        0        0    15260 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/jobs.py
+-rw-r--r--   0        0        0     4094 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/migrations/__init__.py
+-rw-r--r--   0        0        0    10555 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/models.py
+-rw-r--r--   0        0        0     4065 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/naming.py
+-rw-r--r--   0        0        0     1113 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/navigation.py
+-rw-r--r--   0        0        0      533 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/querysets.py
+-rw-r--r--   0        0        0     1654 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/record.py
+-rw-r--r--   0        0        0     4855 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/signals.py
+-rw-r--r--   0        0        0     3881 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/tables.py
+-rw-r--r--   0        0        0     2060 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html
+-rw-r--r--   0        0        0     2047 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html
+-rw-r--r--   0        0        0     1531 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html
+-rw-r--r--   0        0        0     1378 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html
+-rw-r--r--   0        0        0     1147 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html
+-rw-r--r--   0        0        0     5565 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html
+-rw-r--r--   0        0        0     1449 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/urls.py
+-rw-r--r--   0        0        0     3312 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/utils.py
+-rw-r--r--   0        0        0      280 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/validators.py
+-rw-r--r--   0        0        0       22 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/version.py
+-rw-r--r--   0        0        0       69 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/__init__.py
+-rw-r--r--   0        0        0     2166 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/api_servers.py
+-rw-r--r--   0        0        0     5085 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/syncs.py
+-rw-r--r--   0        0        0     1546 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/zones.py
+-rw-r--r--   0        0        0      653 2023-07-24 17:31:08.068448 netbox_powerdns_sync-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 netbox_powerdns_sync-0.0.4/PKG-INFO
```

### Comparing `netbox_powerdns_sync-0.0.3/LICENSE` & `netbox_powerdns_sync-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/README.md` & `netbox_powerdns_sync-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/__init__.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/api/nested_serializers.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/api/serializers.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/api/views.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 
 class ZoneViewSet(NetBoxModelViewSet):
     queryset = models.Zone.objects.prefetch_related(
         "api_servers",
         "match_ipaddress_tags",
         "match_interface_tags",
         "match_device_tags",
-        "match_fhrp_tags",
+        "match_fhrpgroup_tags",
         "match_device_roles",
         "tags"
     )
     serializer_class = ZoneSerializer
     filterset_class = filtersets.ZoneFilterSet
```

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/choices.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/fields.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/fields.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/filtersets.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/forms/filtersets.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/forms/model_forms.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/model_forms.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/forms/sync.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/sync.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/jobs.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/jobs.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/migrations/0001_initial.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/models.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.contrib.contenttypes.models import ContentType
 from django.core.validators import MinLengthValidator
 from django.db import models
 from django.forms import ValidationError
 from django.urls import reverse
+from taggit.managers import TaggableManager
 from core.models import Job
 from dcim.models import DeviceRole, Interface
 from ipam.models import IPAddress, FHRPGroup
 from netbox.models import NetBoxModel
 from extras.models import Tag
 from virtualization.models import VMInterface
 
@@ -158,14 +159,24 @@
         max_length=200,
         help_text="How to construct DNS name from FHRP Group IP is assigned to",
         verbose_name="FHRP Group naming method",
         choices=NamingFgrpGroupChoices,
         default=None,
         null=True,
     )
+    # netbox-plugin-dns also has Zone model
+    # if both plugins are installed, django complains:
+    #   netbox_dns.Zone.tags: (fields.E304) Reverse accessor 'Tag.zone_set'
+    #   for 'netbox_dns.Zone.tags' clashes with reverse accessor for
+    #   'netbox_powerdns_sync.Zone.tags'
+    # So let's disable generating reverse relation here.
+    tags = TaggableManager(
+        through="extras.TaggedItem",
+        related_name="+"
+    )
 
     @property
     def is_reverse(self) -> bool:
         if not self.name:
             return False
         return is_reverse(self.name)
```

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/naming.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/naming.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/navigation.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/querysets.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/querysets.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/record.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/record.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/signals.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/signals.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/tables.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/urls.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/utils.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/utils.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/views/api_servers.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/api_servers.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/views/syncs.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/syncs.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/netbox_powerdns_sync/views/zones.py` & `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/zones.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.3/pyproject.toml` & `netbox_powerdns_sync-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netbox-powerdns-sync"
-version = "0.0.3"
+version = "0.0.4"
 description = "Sync DNS records in PowerDNS with NetBox"
 authors = ["Matej Vadnjal <matej.vadnjal@arnes.si>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ArnesSI/netbox-powerdns-sync/"
 keywords = ["netbox", "netbox-plugin", "powerdns"]
 packages = [{include = "netbox_powerdns_sync"}]
```

### Comparing `netbox_powerdns_sync-0.0.3/PKG-INFO` & `netbox_powerdns_sync-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-powerdns-sync
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sync DNS records in PowerDNS with NetBox
 Home-page: https://github.com/ArnesSI/netbox-powerdns-sync/
 License: MIT
 Keywords: netbox,netbox-plugin,powerdns
 Author: Matej Vadnjal
 Author-email: matej.vadnjal@arnes.si
 Requires-Python: >=3.9
```

