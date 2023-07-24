# Comparing `tmp/djangoldp_profile-2.0.1.tar.gz` & `tmp/djangoldp_profile-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_profile-2.0.1.tar", last modified: Fri Mar 26 13:26:18 2021, max compression
+gzip compressed data, was "djangoldp_profile-3.0.0.tar", last modified: Mon Jul 24 21:38:37 2023, max compression
```

## Comparing `djangoldp_profile-2.0.1.tar` & `djangoldp_profile-3.0.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      589 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/djangoldp_profile/
--rw-rw-rw-   0 root         (0) root         (0)       34 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1408 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/models.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/djangoldp_profile/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      552 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/migrations/0006_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/migrations/0007_auto_20200617_1817.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/migrations/0004_auto_20200506_0838.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/migrations/0003_auto_20200416_1157.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/migrations/0005_auto_20200522_1516.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/migrations/0002_auto_20190917_1141.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/djangoldp_profile/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/djangoldp_profile/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      446 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/management/commands/mock_profile.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/djangoldp_profile/management/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2021-03-26 13:26:16.000000 djangoldp_profile-2.0.1/djangoldp_profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-03-26 13:26:03.000000 djangoldp_profile-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/djangoldp_profile.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/djangoldp_profile.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/djangoldp_profile.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/djangoldp_profile.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      961 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/djangoldp_profile.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      305 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/djangoldp_profile.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      305 2021-03-26 13:26:18.000000 djangoldp_profile-2.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:38:37.885522 djangoldp_profile-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-24 21:38:37.885522 djangoldp_profile-3.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:38:37.881521 djangoldp_profile-3.0.0/djangoldp_profile/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-24 21:38:35.000000 djangoldp_profile-3.0.0/djangoldp_profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:38:37.881521 djangoldp_profile-3.0.0/djangoldp_profile/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:38:37.881521 djangoldp_profile-3.0.0/djangoldp_profile/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/management/commands/mock_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:38:37.885522 djangoldp_profile-3.0.0/djangoldp_profile/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/migrations/0002_auto_20190917_1141.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/migrations/0003_auto_20200416_1157.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/migrations/0004_auto_20200506_0838.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/migrations/0005_auto_20200522_1516.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/migrations/0006_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/migrations/0007_auto_20200617_1817.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/migrations/0008_alter_profile_available.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/djangoldp_profile/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:38:37.881521 djangoldp_profile-3.0.0/djangoldp_profile.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-24 21:38:37.000000 djangoldp_profile-3.0.0/djangoldp_profile.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-24 21:38:37.000000 djangoldp_profile-3.0.0/djangoldp_profile.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:38:37.000000 djangoldp_profile-3.0.0/djangoldp_profile.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 21:38:37.000000 djangoldp_profile-3.0.0/djangoldp_profile.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-24 21:38:37.000000 djangoldp_profile-3.0.0/djangoldp_profile.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-24 21:38:37.885522 djangoldp_profile-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 21:38:17.000000 djangoldp_profile-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_profile-2.0.1/setup.cfg` & `djangoldp_profile-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 author_email = nicolas@happy-dev.fr
 description = djangoldp package for profile data models
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp~=2.0
-	djangoldp_account~=2.0
+	djangoldp~=3.0
+	djangoldp_account~=3.0
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
 
 [semantic_release]
 version_source = tag
```

### Comparing `djangoldp_profile-2.0.1/djangoldp_profile/models.py` & `djangoldp_profile-3.0.0/djangoldp_profile/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from djangoldp.models import Model
 
 
 class Profile(Model):
     user = models.OneToOneField(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, related_name="profile")
     slug = models.SlugField(unique=True, blank=True)
-    available = models.NullBooleanField(blank=True)
+    available = models.BooleanField(null=True, blank=True)
     job = models.CharField(max_length=150, blank=True)
     city = models.CharField(max_length=255, blank=True)
     phone = models.CharField(max_length=255, blank=True)
     website = models.URLField(blank=True)
 
     def jabberID(self):
         try:
```

### Comparing `djangoldp_profile-2.0.1/djangoldp_profile/factories.py` & `djangoldp_profile-3.0.0/djangoldp_profile/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_profile-2.0.1/djangoldp_profile/admin.py` & `djangoldp_profile-3.0.0/djangoldp_profile/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from django.contrib import admin
 from djangoldp.admin import DjangoLDPAdmin
 from djangoldp.models import Model
 from .models import Profile
 
 
+@admin.register(Profile)
 class ProfileAdmin(DjangoLDPAdmin):
     list_display = ('urlid', 'user')
     exclude = ('urlid', 'user', 'is_backlink', 'allow_create_backlink', 'slug')
     search_fields = ['urlid', 'user__urlid', 'available', 'job', 'city', 'phone', 'website']
     ordering = ['urlid']
 
     def get_queryset(self, request):
         # Hide distant profiles
         queryset = super(ProfileAdmin, self).get_queryset(request)
         internal_ids = [x.pk for x in queryset if not Model.is_external(x)]
         return queryset.filter(pk__in=internal_ids)
 
 
-admin.site.register(Profile, ProfileAdmin)
```

### Comparing `djangoldp_profile-2.0.1/djangoldp_profile/migrations/0006_auto_20200610_1323.py` & `djangoldp_profile-3.0.0/djangoldp_profile/migrations/0006_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_profile-2.0.1/djangoldp_profile/migrations/0007_auto_20200617_1817.py` & `djangoldp_profile-3.0.0/djangoldp_profile/migrations/0007_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp_profile-2.0.1/djangoldp_profile/migrations/0005_auto_20200522_1516.py` & `djangoldp_profile-3.0.0/djangoldp_profile/migrations/0005_auto_20200522_1516.py`

 * *Files identical despite different names*

### Comparing `djangoldp_profile-2.0.1/djangoldp_profile/migrations/0001_initial.py` & `djangoldp_profile-3.0.0/djangoldp_profile/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_profile-2.0.1/djangoldp_profile/migrations/0002_auto_20190917_1141.py` & `djangoldp_profile-3.0.0/djangoldp_profile/migrations/0002_auto_20190917_1141.py`

 * *Files identical despite different names*

### Comparing `djangoldp_profile-2.0.1/djangoldp_profile.egg-info/SOURCES.txt` & `djangoldp_profile-3.0.0/djangoldp_profile.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 djangoldp_profile/migrations/0001_initial.py
 djangoldp_profile/migrations/0002_auto_20190917_1141.py
 djangoldp_profile/migrations/0003_auto_20200416_1157.py
 djangoldp_profile/migrations/0004_auto_20200506_0838.py
 djangoldp_profile/migrations/0005_auto_20200522_1516.py
 djangoldp_profile/migrations/0006_auto_20200610_1323.py
 djangoldp_profile/migrations/0007_auto_20200617_1817.py
+djangoldp_profile/migrations/0008_alter_profile_available.py
 djangoldp_profile/migrations/__init__.py
```

