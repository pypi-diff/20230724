# Comparing `tmp/djangoldp_dashboard-2.3.2.tar.gz` & `tmp/djangoldp_dashboard-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_dashboard-2.3.2.tar", last modified: Fri Mar 26 13:26:18 2021, max compression
+gzip compressed data, was "djangoldp_dashboard-3.0.0.tar", last modified: Mon Jul 24 21:32:37 2023, max compression
```

## Comparing `djangoldp_dashboard-2.3.2.tar` & `djangoldp_dashboard-3.0.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/
--rw-rw-rw-   0 root         (0) root         (0)      553 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      852 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      483 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      138 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/
--rw-rw-rw-   0 root         (0) root         (0)      381 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/models.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      579 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0006_auto_20210219_1255.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0007_auto_20210223_2254.py
--rw-rw-rw-   0 root         (0) root         (0)      542 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0005_auto_20200619_1102.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0004_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0002_auto_20200330_1531.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0003_auto_20200522_1516.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)    12851 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/fixtures/sample.json
--rw-rw-rw-   0 root         (0) root         (0)       51 2021-03-26 13:26:16.000000 djangoldp_dashboard-2.3.2/djangoldp_dashboard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-03-26 13:26:03.000000 djangoldp_dashboard-2.3.2/setup.py
--rw-r--r--   0 root         (0) root         (0)      483 2021-03-26 13:26:18.000000 djangoldp_dashboard-2.3.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:32:37.031246 djangoldp_dashboard-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      380 2023-07-24 21:32:37.031246 djangoldp_dashboard-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:32:37.031246 djangoldp_dashboard-3.0.0/djangoldp_dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-24 21:32:34.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:32:37.031246 djangoldp_dashboard-3.0.0/djangoldp_dashboard/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)    12851 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/fixtures/sample.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:32:37.031246 djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0002_auto_20200330_1531.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0003_auto_20200522_1516.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0004_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0005_auto_20200619_1102.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0006_auto_20210219_1255.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0007_auto_20210223_2254.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:32:37.031246 djangoldp_dashboard-3.0.0/djangoldp_dashboard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      380 2023-07-24 21:32:36.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      860 2023-07-24 21:32:36.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:32:36.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-24 21:32:36.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-24 21:32:36.000000 djangoldp_dashboard-3.0.0/djangoldp_dashboard.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      553 2023-07-24 21:32:37.031246 djangoldp_dashboard-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 21:32:17.000000 djangoldp_dashboard-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_dashboard-2.3.2/setup.cfg` & `djangoldp_dashboard-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 include_package_data = True
 packages = find:
 install_requires = 
-	djangoldp~=2.1
+	djangoldp~=3.0
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_dashboard/__init__.py:__version__
 commit_parser = commit_parser.parse
 
 [egg_info]
```

### Comparing `djangoldp_dashboard-2.3.2/djangoldp_dashboard.egg-info/SOURCES.txt` & `djangoldp_dashboard-3.0.0/djangoldp_dashboard.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 djangoldp_dashboard/__init__.py
 djangoldp_dashboard/admin.py
 djangoldp_dashboard/apps.py
```

### Comparing `djangoldp_dashboard-2.3.2/djangoldp_dashboard/admin.py` & `djangoldp_dashboard-3.0.0/djangoldp_dashboard/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from django.contrib import admin
 from djangoldp.admin import DjangoLDPAdmin
 from djangoldp.models import Model
 from .models import Dashboard
 
 
+@admin.register(Dashboard)
 class DashboardAdmin(DjangoLDPAdmin):
     list_display = ('urlid', 'target', 'size', 'background')
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
     search_fields = ['urlid', 'target', 'size', 'background', 'content']
     ordering = ['urlid']
 
     def get_queryset(self, request):
         # Hide distant dashboard cards
         queryset = super(DashboardAdmin, self).get_queryset(request)
         internal_ids = [x.pk for x in queryset if not Model.is_external(x)]
         return queryset.filter(pk__in=internal_ids)
 
-admin.site.register(Dashboard, DashboardAdmin)
```

### Comparing `djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0006_auto_20210219_1255.py` & `djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0006_auto_20210219_1255.py`

 * *Files identical despite different names*

### Comparing `djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0005_auto_20200619_1102.py` & `djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0005_auto_20200619_1102.py`

 * *Files identical despite different names*

### Comparing `djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0004_auto_20200610_1323.py` & `djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0004_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0001_initial.py` & `djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_dashboard-2.3.2/djangoldp_dashboard/migrations/0003_auto_20200522_1516.py` & `djangoldp_dashboard-3.0.0/djangoldp_dashboard/migrations/0003_auto_20200522_1516.py`

 * *Files identical despite different names*

### Comparing `djangoldp_dashboard-2.3.2/djangoldp_dashboard/fixtures/sample.json` & `djangoldp_dashboard-3.0.0/djangoldp_dashboard/fixtures/sample.json`

 * *Files identical despite different names*

