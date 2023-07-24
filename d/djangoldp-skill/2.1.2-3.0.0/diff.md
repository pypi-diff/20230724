# Comparing `tmp/djangoldp_skill-2.1.2.tar.gz` & `tmp/djangoldp_skill-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_skill-2.1.2.tar", last modified: Fri Mar 26 13:26:17 2021, max compression
+gzip compressed data, was "djangoldp_skill-3.0.0.tar", last modified: Mon Jul 24 21:23:43 2023, max compression
```

## Comparing `djangoldp_skill-2.1.2.tar` & `djangoldp_skill-3.0.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/djangoldp_skill.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/djangoldp_skill.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/djangoldp_skill.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/djangoldp_skill.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      939 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/djangoldp_skill.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      299 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/djangoldp_skill.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      571 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/djangoldp_skill/
--rw-rw-rw-   0 root         (0) root         (0)       31 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      610 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/models.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/djangoldp_skill/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      534 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/migrations/0005_auto_20200619_0813.py
--rw-rw-rw-   0 root         (0) root         (0)    16572 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/migrations/0006_auto_20201130_1147.py
--rw-rw-rw-   0 root         (0) root         (0)    17483 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/migrations/0007_auto_20210223_2254.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/migrations/0002_skill_urlid.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/migrations/0004_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/migrations/0003_auto_20200522_1516.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/djangoldp_skill/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/djangoldp_skill/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      888 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/management/commands/mock_skill.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/management/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/djangoldp_skill/translation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2021-03-26 13:26:15.000000 djangoldp_skill-2.1.2/djangoldp_skill/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-03-26 13:26:02.000000 djangoldp_skill-2.1.2/setup.py
--rw-r--r--   0 root         (0) root         (0)      299 2021-03-26 13:26:17.000000 djangoldp_skill-2.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:23:43.606097 djangoldp_skill-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-07-24 21:23:43.606097 djangoldp_skill-3.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:23:43.602096 djangoldp_skill-3.0.0/djangoldp_skill/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-24 21:23:40.000000 djangoldp_skill-3.0.0/djangoldp_skill/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:23:43.606097 djangoldp_skill-3.0.0/djangoldp_skill/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:23:43.606097 djangoldp_skill-3.0.0/djangoldp_skill/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/management/commands/mock_skill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:23:43.606097 djangoldp_skill-3.0.0/djangoldp_skill/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/migrations/0002_skill_urlid.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/migrations/0003_auto_20200522_1516.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/migrations/0004_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      534 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/migrations/0005_auto_20200619_0813.py
+-rw-rw-rw-   0 root         (0) root         (0)    16572 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/migrations/0006_auto_20201130_1147.py
+-rw-rw-rw-   0 root         (0) root         (0)    17483 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/migrations/0007_auto_20210223_2254.py
+-rw-rw-rw-   0 root         (0) root         (0)     1741 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/migrations/0008_skill_name_ar_dz_skill_name_ckb_skill_name_ig_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/djangoldp_skill/translation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:23:43.602096 djangoldp_skill-3.0.0/djangoldp_skill.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-07-24 21:23:43.000000 djangoldp_skill-3.0.0/djangoldp_skill.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-07-24 21:23:43.000000 djangoldp_skill-3.0.0/djangoldp_skill.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:23:43.000000 djangoldp_skill-3.0.0/djangoldp_skill.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-24 21:23:43.000000 djangoldp_skill-3.0.0/djangoldp_skill.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-24 21:23:43.000000 djangoldp_skill-3.0.0/djangoldp_skill.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-07-24 21:23:43.606097 djangoldp_skill-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 21:23:23.000000 djangoldp_skill-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_skill-2.1.2/djangoldp_skill.egg-info/SOURCES.txt` & `djangoldp_skill-3.0.0/djangoldp_skill.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 djangoldp_skill/migrations/0001_initial.py
 djangoldp_skill/migrations/0002_skill_urlid.py
 djangoldp_skill/migrations/0003_auto_20200522_1516.py
 djangoldp_skill/migrations/0004_auto_20200610_1323.py
 djangoldp_skill/migrations/0005_auto_20200619_0813.py
 djangoldp_skill/migrations/0006_auto_20201130_1147.py
 djangoldp_skill/migrations/0007_auto_20210223_2254.py
+djangoldp_skill/migrations/0008_skill_name_ar_dz_skill_name_ckb_skill_name_ig_and_more.py
 djangoldp_skill/migrations/__init__.py
```

### Comparing `djangoldp_skill-2.1.2/setup.cfg` & `djangoldp_skill-3.0.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 author_email = nicolas@happy-dev.fr
 description = djangoldp package for skill data models
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp~=2.1
+	djangoldp~=3.0
 	djangoldp_i18n
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
 
 [semantic_release]
```

### Comparing `djangoldp_skill-2.1.2/djangoldp_skill/models.py` & `djangoldp_skill-3.0.0/djangoldp_skill/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_skill-2.1.2/djangoldp_skill/admin.py` & `djangoldp_skill-3.0.0/djangoldp_skill/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from django.db.models import Count
 from djangoldp.admin import DjangoLDPAdmin
 from djangoldp_i18n.admin import DjangoLDPI18nAdmin
 from djangoldp.models import Model
 from djangoldp_skill.models import Skill
 
 
+@admin.register(Skill)
 class SkillAdmin(DjangoLDPI18nAdmin, DjangoLDPAdmin):
     list_display = ('urlid', 'name', 'users__count')
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
     search_fields = ['urlid', 'name']
     ordering = ['urlid']
 
     def users__count(self, obj):
@@ -18,8 +19,7 @@
     def get_queryset(self, request):
         # Hide distant skills
         queryset = super(SkillAdmin, self).get_queryset(request)
         internal_ids = [x.pk for x in queryset if not Model.is_external(x)]
         queryset = queryset.annotate(users_count=Count("users"))
         return queryset.filter(pk__in=internal_ids)
 
-admin.site.register(Skill, SkillAdmin)
```

### Comparing `djangoldp_skill-2.1.2/djangoldp_skill/migrations/0005_auto_20200619_0813.py` & `djangoldp_skill-3.0.0/djangoldp_skill/migrations/0005_auto_20200619_0813.py`

 * *Files identical despite different names*

### Comparing `djangoldp_skill-2.1.2/djangoldp_skill/migrations/0006_auto_20201130_1147.py` & `djangoldp_skill-3.0.0/djangoldp_skill/migrations/0006_auto_20201130_1147.py`

 * *Files identical despite different names*

### Comparing `djangoldp_skill-2.1.2/djangoldp_skill/migrations/0007_auto_20210223_2254.py` & `djangoldp_skill-3.0.0/djangoldp_skill/migrations/0007_auto_20210223_2254.py`

 * *Files identical despite different names*

### Comparing `djangoldp_skill-2.1.2/djangoldp_skill/migrations/0004_auto_20200610_1323.py` & `djangoldp_skill-3.0.0/djangoldp_skill/migrations/0004_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_skill-2.1.2/djangoldp_skill/migrations/0001_initial.py` & `djangoldp_skill-3.0.0/djangoldp_skill/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_skill-2.1.2/djangoldp_skill/migrations/0003_auto_20200522_1516.py` & `djangoldp_skill-3.0.0/djangoldp_skill/migrations/0003_auto_20200522_1516.py`

 * *Files identical despite different names*

### Comparing `djangoldp_skill-2.1.2/djangoldp_skill/management/commands/mock_skill.py` & `djangoldp_skill-3.0.0/djangoldp_skill/management/commands/mock_skill.py`

 * *Files identical despite different names*

