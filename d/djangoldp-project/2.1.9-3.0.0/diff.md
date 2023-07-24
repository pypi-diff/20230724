# Comparing `tmp/djangoldp_project-2.1.9.tar.gz` & `tmp/djangoldp_project-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_project-2.1.9.tar", last modified: Thu May 20 18:08:25 2021, max compression
+gzip compressed data, was "djangoldp_project-3.0.0.tar", last modified: Mon Jul 24 20:43:36 2023, max compression
```

## Comparing `djangoldp_project-2.1.9.tar` & `djangoldp_project-3.0.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/
--rw-rw-rw-   0 root         (0) root         (0)      565 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2016 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      305 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project/
--rw-rw-rw-   0 root         (0) root         (0)       33 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     8687 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/models.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4263 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/views.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/xmpp.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     2908 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6738 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/tests/tests_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      672 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0018_auto_20210504_1748.py
--rw-rw-rw-   0 root         (0) root         (0)      546 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0020_auto_20210520_2005.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0015_auto_20200926_0911.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0009_project_status.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0016_remove_project_team.py
--rw-rw-rw-   0 root         (0) root         (0)     2195 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0010_auto_20200522_1516.py
--rw-rw-rw-   0 root         (0) root         (0)     1290 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0012_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0013_auto_20200619_0808.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0005_auto_20191217_1301.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0007_customer_owner.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0014_auto_20200903_1051.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0011_remove_member_name.py
--rw-rw-rw-   0 root         (0) root         (0)     2410 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0003_auto_20191209_1712.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0017_auto_20210125_1847.py
--rw-rw-rw-   0 root         (0) root         (0)     4645 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0004_auto_20191211_1552.py
--rw-rw-rw-   0 root         (0) root         (0)      451 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0002_member_is_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0006_auto_20200114_1547.py
--rw-rw-rw-   0 root         (0) root         (0)      937 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0019_auto_20210519_1349.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/migrations/0008_auto_20200326_2132.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/djangoldp_project/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      901 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/management/commands/mock_project.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/management/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/djangoldp_project/filters.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2021-05-20 18:08:23.000000 djangoldp_project-2.1.9/djangoldp_project/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-05-20 18:08:11.000000 djangoldp_project-2.1.9/setup.py
--rw-r--r--   0 root         (0) root         (0)      305 2021-05-20 18:08:25.000000 djangoldp_project-2.1.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:43:36.474758 djangoldp_project-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-24 20:43:36.474758 djangoldp_project-3.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:43:36.470758 djangoldp_project-3.0.0/djangoldp_project/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-24 20:43:33.000000 djangoldp_project-3.0.0/djangoldp_project/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2908 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:43:36.470758 djangoldp_project-3.0.0/djangoldp_project/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:43:36.470758 djangoldp_project-3.0.0/djangoldp_project/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/management/commands/mock_project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:43:36.474758 djangoldp_project-3.0.0/djangoldp_project/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     4645 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      451 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0002_member_is_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0003_auto_20191209_1712.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0004_auto_20191211_1552.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0005_auto_20191217_1301.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0006_auto_20200114_1547.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0007_customer_owner.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0008_auto_20200326_2132.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0009_project_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0010_auto_20200522_1516.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0011_remove_member_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0012_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0013_auto_20200619_0808.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0014_auto_20200903_1051.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0015_auto_20200926_0911.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0016_remove_project_team.py
+-rw-rw-rw-   0 root         (0) root         (0)      926 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0017_auto_20210125_1847.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0018_auto_20210504_1748.py
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0019_auto_20210519_1349.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0020_auto_20210520_2005.py
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0021_auto_20210521_1202.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/0022_alter_customer_options_alter_project_options.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8721 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4263 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:43:36.474758 djangoldp_project-3.0.0/djangoldp_project/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     6738 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/tests/tests_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/djangoldp_project/xmpp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:43:36.470758 djangoldp_project-3.0.0/djangoldp_project.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-24 20:43:36.000000 djangoldp_project-3.0.0/djangoldp_project.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-07-24 20:43:36.000000 djangoldp_project-3.0.0/djangoldp_project.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:43:36.000000 djangoldp_project-3.0.0/djangoldp_project.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-24 20:43:36.000000 djangoldp_project-3.0.0/djangoldp_project.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-24 20:43:36.000000 djangoldp_project-3.0.0/djangoldp_project.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-24 20:43:36.478758 djangoldp_project-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 20:43:16.000000 djangoldp_project-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_project-2.1.9/setup.cfg` & `djangoldp_project-3.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 author_email = nicolas@happy-dev.fr
 description = djangoldp package for project data models
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp>=2.1
+	djangoldp~=3.0
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
 
 [semantic_release]
 version_source = tag
```

### Comparing `djangoldp_project-2.1.9/djangoldp_project.egg-info/SOURCES.txt` & `djangoldp_project-3.0.0/djangoldp_project.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -36,12 +36,14 @@
 djangoldp_project/migrations/0014_auto_20200903_1051.py
 djangoldp_project/migrations/0015_auto_20200926_0911.py
 djangoldp_project/migrations/0016_remove_project_team.py
 djangoldp_project/migrations/0017_auto_20210125_1847.py
 djangoldp_project/migrations/0018_auto_20210504_1748.py
 djangoldp_project/migrations/0019_auto_20210519_1349.py
 djangoldp_project/migrations/0020_auto_20210520_2005.py
+djangoldp_project/migrations/0021_auto_20210521_1202.py
+djangoldp_project/migrations/0022_alter_customer_options_alter_project_options.py
 djangoldp_project/migrations/__init__.py
 djangoldp_project/tests/__init__.py
 djangoldp_project/tests/models.py
 djangoldp_project/tests/runner.py
 djangoldp_project/tests/tests_permissions.py
```

### Comparing `djangoldp_project-2.1.9/djangoldp_project/models.py` & `djangoldp_project-3.0.0/djangoldp_project/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,21 @@
     postcode = models.CharField(max_length=10, null=True, blank=True)
     city = models.CharField(max_length=50, null=True, blank=True)
     country = models.CharField(max_length=50, null=True, blank=True)
     logo = models.URLField(blank=True, null=True)
     companyRegister = models.CharField(max_length=255, null=True, blank=True)
     first_name = models.CharField(max_length=255, null=True, blank=True)
     last_name = models.CharField(max_length=255, null=True, blank=True)
-    owner = models.ForeignKey(settings.AUTH_USER_MODEL, related_name="owned_customers", on_delete=models.SET_NULL,
-                              null=True)
+    owner = models.ForeignKey(settings.AUTH_USER_MODEL, related_name="owned_customers", null=True, blank=True, on_delete=models.SET_NULL)
     role = models.CharField(max_length=255, null=True, blank=True)
     email = models.EmailField(null=True, blank=True)
     phone = models.CharField(max_length=255, null=True, blank=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         auto_author = 'owner'
         owner_field = 'owner'
         anonymous_perms = []
         authenticated_perms = ['add']
         owner_perms = ['inherit', 'view', 'change', 'delete']
         permission_classes = [CustomerPermissions]
 
@@ -76,14 +76,15 @@
     captain = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.SET_NULL, blank=True, null=True,
                                 related_name='+')
     driveID = models.TextField(null=True, blank=True)
     jabberID = models.CharField(max_length=255, blank=True, null=True)
     jabberRoom = models.BooleanField(default=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         empty_containers = ["captain"]
 #        depth = 1 # Disabled due to captain being serialized
         permission_classes = [ProjectPermissions]
         anonymous_perms = []
         authenticated_perms = []
         owner_perms = []
         rdf_type = 'hd:project'
```

### Comparing `djangoldp_project-2.1.9/djangoldp_project/permissions.py` & `djangoldp_project-3.0.0/djangoldp_project/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/djangoldp_urls.py` & `djangoldp_project-3.0.0/djangoldp_project/djangoldp_urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from django.conf.urls import url
+from django.urls import path
 from .views import ProjectsJoinableViewset
 from .models import Project
 from djangoldp.models import Model
 
 
 urlpatterns = [
-    url(r'^projects/joinable/', ProjectsJoinableViewset.urls(model_prefix="projects-joinable",
+    path('projects/joinable/', ProjectsJoinableViewset.urls(model_prefix="projects-joinable",
         model=Project,
         lookup_field=Model.get_meta(Project, 'lookup_field', 'pk'),
         permission_classes=Model.get_meta(Project, 'permission_classes', []),
         fields=Model.get_meta(Project, 'serializer_fields', []),
         nested_fields=Model.get_meta(Project, 'nested_fields', [])))
 ]
```

### Comparing `djangoldp_project-2.1.9/djangoldp_project/views.py` & `djangoldp_project-3.0.0/djangoldp_project/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/factories.py` & `djangoldp_project-3.0.0/djangoldp_project/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/check_integrity.py` & `djangoldp_project-3.0.0/djangoldp_project/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/admin.py` & `djangoldp_project-3.0.0/djangoldp_project/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.contrib import admin
 from djangoldp.admin import DjangoLDPAdmin
 from djangoldp.models import Model
 from .models import Project, Member, Customer, BusinessProvider
 
 
+@admin.register(BusinessProvider, Customer, Member)
 class EmptyAdmin(admin.ModelAdmin):
     def get_model_perms(self, request):
         return {}
 
 
 class TeamInline(admin.TabularInline):
     model = Member
@@ -17,14 +18,15 @@
 
 class BusinessProviderInline(admin.TabularInline):
     model = BusinessProvider
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
     extra = 0
 
 
+@admin.register(Project)
 class ProjectAdmin(DjangoLDPAdmin):
     list_display = ('urlid', 'customer', 'name', 'captain', 'status', 'jabberID')
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink', 'jabberID', 'jabberRoom')
     search_fields = ['urlid', 'name', 'members__user__urlid', 'number', 'description',\
         'status', 'captain__urlid', 'customer__urlid', 'customer__name',\
         'businessProvider__urlid', 'businessProvider__name']
     ordering = ['urlid']
@@ -33,11 +35,7 @@
     def get_queryset(self, request):
         # Hide distant projects
         queryset = super(ProjectAdmin, self).get_queryset(request)
         internal_ids = [x.pk for x in queryset if not Model.is_external(x)]
         return queryset.filter(pk__in=internal_ids)
 
 
-admin.site.register(Project, ProjectAdmin)
-admin.site.register(Member, EmptyAdmin)
-admin.site.register(Customer, EmptyAdmin)
-admin.site.register(BusinessProvider, EmptyAdmin)
```

### Comparing `djangoldp_project-2.1.9/djangoldp_project/tests/tests_permissions.py` & `djangoldp_project-3.0.0/djangoldp_project/tests/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/tests/runner.py` & `djangoldp_project-3.0.0/djangoldp_project/tests/runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import sys
 import yaml
 
 import django
 from django.conf import settings as django_settings
 from djangoldp.conf.ldpsettings import LDPSettings
-from djangoldp.tests.settings_default import yaml_config
+from djangoldp.tests.server_settings import yaml_config
 
 # override config loading
 config = {
     # add the packages to the reference list
     'ldppackages': ['djangoldp_project', 'djangoldp_project.tests'],
 
     # required values for server
     'server': {
+        'SECRET_KEY': "$r&)p-4k@h5b!1yrft6&q%j)_p$lxqh6#)jeeu0z1iag&y&wdu",
         'AUTH_USER_MODEL': 'tests.User',
         'REST_FRAMEWORK': {
             'DEFAULT_PAGINATION_CLASS': 'djangoldp.pagination.LDPPagination',
             'PAGE_SIZE': 5
         },
         # map the config of the core settings (avoid asserts to fail)
         'SITE_URL': 'http://happy-dev.fr',
```

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0018_auto_20210504_1748.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0018_auto_20210504_1748.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0020_auto_20210520_2005.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0020_auto_20210520_2005.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0015_auto_20200926_0911.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0015_auto_20200926_0911.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0009_project_status.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0009_project_status.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0010_auto_20200522_1516.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0010_auto_20200522_1516.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0012_auto_20200610_1323.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0012_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0013_auto_20200619_0808.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0013_auto_20200619_0808.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0005_auto_20191217_1301.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0005_auto_20191217_1301.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0007_customer_owner.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0007_customer_owner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0014_auto_20200903_1051.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0014_auto_20200903_1051.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0003_auto_20191209_1712.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0003_auto_20191209_1712.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0017_auto_20210125_1847.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0017_auto_20210125_1847.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0001_initial.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0004_auto_20191211_1552.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0004_auto_20191211_1552.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0019_auto_20210519_1349.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0019_auto_20210519_1349.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/migrations/0008_auto_20200326_2132.py` & `djangoldp_project-3.0.0/djangoldp_project/migrations/0008_auto_20200326_2132.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/management/commands/mock_project.py` & `djangoldp_project-3.0.0/djangoldp_project/management/commands/mock_project.py`

 * *Files identical despite different names*

### Comparing `djangoldp_project-2.1.9/djangoldp_project/filters.py` & `djangoldp_project-3.0.0/djangoldp_project/filters.py`

 * *Files identical despite different names*

