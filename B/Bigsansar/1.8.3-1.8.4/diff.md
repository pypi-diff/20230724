# Comparing `tmp/Bigsansar-1.8.3.tar.gz` & `tmp/Bigsansar-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.8.3.tar", last modified: Mon Jul 17 14:36:45 2023, max compression
+gzip compressed data, was "Bigsansar-1.8.4.tar", last modified: Mon Jul 24 11:36:02 2023, max compression
```

## Comparing `Bigsansar-1.8.3.tar` & `Bigsansar-1.8.4.tar`

### file list

```diff
@@ -1,161 +1,163 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.255632 Bigsansar-1.8.3/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.175632 Bigsansar-1.8.3/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4943 2023-07-17 14:36:45.000000 Bigsansar-1.8.3/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5561 2023-07-17 14:36:45.000000 Bigsansar-1.8.3/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-07-17 14:36:45.000000 Bigsansar-1.8.3/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-07-17 14:36:45.000000 Bigsansar-1.8.3/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-07-17 14:36:45.000000 Bigsansar-1.8.3/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-07-17 14:36:45.000000 Bigsansar-1.8.3/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.8.3/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4943 2023-07-17 14:36:45.255632 Bigsansar-1.8.3/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4383 2023-06-27 11:34:16.000000 Bigsansar-1.8.3/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.175632 Bigsansar-1.8.3/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.175632 Bigsansar-1.8.3/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.175632 Bigsansar-1.8.3/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.175632 Bigsansar-1.8.3/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.175632 Bigsansar-1.8.3/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.175632 Bigsansar-1.8.3/bigsansar/contrib/advance/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-06-25 11:54:17.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3004 2023-07-03 12:30:41.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.185632 Bigsansar-1.8.3/bigsansar/contrib/advance/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/migrations/0003_javascript.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      296 2023-06-18 11:06:29.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/migrations/0005_delete_css.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      289 2023-06-25 11:55:08.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/migrations/0006_delete_javascript.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      154 2023-06-25 11:53:50.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      589 2023-07-04 13:05:58.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4022 2023-07-04 13:12:10.000000 Bigsansar-1.8.3/bigsansar/contrib/advance/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.185632 Bigsansar-1.8.3/bigsansar/contrib/blogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2302 2023-07-06 13:11:19.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      261 2023-06-05 06:44:01.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.185632 Bigsansar-1.8.3/bigsansar/contrib/blogs/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-06-02 13:13:53.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2095 2023-07-15 13:50:00.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.185632 Bigsansar-1.8.3/bigsansar/contrib/blogs/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1525 2023-06-05 06:21:13.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/templatetags/blogs.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.185632 Bigsansar-1.8.3/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2462 2023-06-09 12:43:48.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4277 2023-07-17 14:19:50.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.195632 Bigsansar-1.8.3/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2225 2023-06-25 11:45:49.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.195632 Bigsansar-1.8.3/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      548 2023-07-17 14:17:50.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4447 2023-07-17 14:28:05.000000 Bigsansar-1.8.3/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.195632 Bigsansar-1.8.3/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.8.3/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.195632 Bigsansar-1.8.3/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.195632 Bigsansar-1.8.3/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.8.3/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.195632 Bigsansar-1.8.3/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.195632 Bigsansar-1.8.3/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/static/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.165632 Bigsansar-1.8.3/bigsansar/static/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.165632 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.165632 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.195632 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.195632 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.235632 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.245632 Bigsansar-1.8.3/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/templates/acc_active_email.html
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-17 14:36:45.255632 Bigsansar-1.8.3/bigsansar/templates/admin/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      558 2023-06-28 10:56:41.000000 Bigsansar-1.8.3/bigsansar/templates/admin/chpass.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      558 2023-06-27 11:25:11.000000 Bigsansar-1.8.3/bigsansar/templates/admin/chuname.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10741 2023-07-04 12:57:32.000000 Bigsansar-1.8.3/bigsansar/templates/admin/dashboard.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8901 2023-07-17 14:01:12.000000 Bigsansar-1.8.3/bigsansar/templates/admin/domain_manage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1019 2023-07-15 13:47:11.000000 Bigsansar-1.8.3/bigsansar/templates/admin/edit_domain.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      566 2023-07-03 12:32:25.000000 Bigsansar-1.8.3/bigsansar/templates/admin/editprofile.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1142 2023-06-26 11:40:15.000000 Bigsansar-1.8.3/bigsansar/templates/admin/login.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2137 2023-06-27 11:14:29.000000 Bigsansar-1.8.3/bigsansar/templates/admin/nav.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      947 2023-07-17 14:30:13.000000 Bigsansar-1.8.3/bigsansar/templates/admin/page_create.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.8.3/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1931 2023-06-05 06:55:58.000000 Bigsansar-1.8.3/bigsansar/templates/blog_preview.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      101 2023-06-25 11:39:45.000000 Bigsansar-1.8.3/bigsansar/templates/script.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-06-06 04:42:17.000000 Bigsansar-1.8.3/bigsansar/templates/sitemap.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      101 2023-06-18 11:01:43.000000 Bigsansar-1.8.3/bigsansar/templates/styles.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.8.3/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1241 2023-07-04 13:08:29.000000 Bigsansar-1.8.3/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4734 2023-06-25 11:54:54.000000 Bigsansar-1.8.3/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-07-17 14:36:45.255632 Bigsansar-1.8.3/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1753 2023-07-17 13:57:46.000000 Bigsansar-1.8.3/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:02.010188 Bigsansar-1.8.4/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.900188 Bigsansar-1.8.4/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4943 2023-07-24 11:36:01.000000 Bigsansar-1.8.4/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5645 2023-07-24 11:36:01.000000 Bigsansar-1.8.4/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-07-24 11:36:01.000000 Bigsansar-1.8.4/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-07-24 11:36:01.000000 Bigsansar-1.8.4/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-07-24 11:36:01.000000 Bigsansar-1.8.4/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-07-24 11:36:01.000000 Bigsansar-1.8.4/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.8.4/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4943 2023-07-24 11:36:02.010188 Bigsansar-1.8.4/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4383 2023-06-27 11:34:16.000000 Bigsansar-1.8.4/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.910188 Bigsansar-1.8.4/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.910188 Bigsansar-1.8.4/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.910188 Bigsansar-1.8.4/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.910188 Bigsansar-1.8.4/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.920188 Bigsansar-1.8.4/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.920188 Bigsansar-1.8.4/bigsansar/contrib/advance/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-06-25 11:54:17.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3004 2023-07-03 12:30:41.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.920188 Bigsansar-1.8.4/bigsansar/contrib/advance/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/migrations/0003_javascript.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      296 2023-06-18 11:06:29.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/migrations/0005_delete_css.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      289 2023-06-25 11:55:08.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/migrations/0006_delete_javascript.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      154 2023-06-25 11:53:50.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      589 2023-07-04 13:05:58.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4022 2023-07-04 13:12:10.000000 Bigsansar-1.8.4/bigsansar/contrib/advance/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.920188 Bigsansar-1.8.4/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2302 2023-07-06 13:11:19.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      261 2023-06-05 06:44:01.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.920188 Bigsansar-1.8.4/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-06-02 13:13:53.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2095 2023-07-15 13:50:00.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.920188 Bigsansar-1.8.4/bigsansar/contrib/blogs/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1525 2023-06-05 06:21:13.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/templatetags/blogs.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.930188 Bigsansar-1.8.4/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2462 2023-06-09 12:43:48.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4670 2023-07-24 10:35:46.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.930188 Bigsansar-1.8.4/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2225 2023-06-25 11:45:49.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.930188 Bigsansar-1.8.4/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      544 2023-07-24 10:44:02.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     6822 2023-07-24 10:46:01.000000 Bigsansar-1.8.4/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.930188 Bigsansar-1.8.4/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.8.4/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.940188 Bigsansar-1.8.4/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.940188 Bigsansar-1.8.4/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.8.4/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.940188 Bigsansar-1.8.4/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.940188 Bigsansar-1.8.4/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/static/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.890188 Bigsansar-1.8.4/bigsansar/static/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.890188 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.890188 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.940188 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.940188 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.980188 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:01.990188 Bigsansar-1.8.4/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/templates/acc_active_email.html
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-07-24 11:36:02.010188 Bigsansar-1.8.4/bigsansar/templates/admin/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      558 2023-06-28 10:56:41.000000 Bigsansar-1.8.4/bigsansar/templates/admin/chpass.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      558 2023-06-27 11:25:11.000000 Bigsansar-1.8.4/bigsansar/templates/admin/chuname.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10741 2023-07-04 12:57:32.000000 Bigsansar-1.8.4/bigsansar/templates/admin/dashboard.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8871 2023-07-24 10:43:29.000000 Bigsansar-1.8.4/bigsansar/templates/admin/domain_manage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1019 2023-07-15 13:47:11.000000 Bigsansar-1.8.4/bigsansar/templates/admin/edit_domain.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      566 2023-07-03 12:32:25.000000 Bigsansar-1.8.4/bigsansar/templates/admin/editprofile.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1142 2023-06-26 11:40:15.000000 Bigsansar-1.8.4/bigsansar/templates/admin/login.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2137 2023-06-27 11:14:29.000000 Bigsansar-1.8.4/bigsansar/templates/admin/nav.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      947 2023-07-17 14:30:13.000000 Bigsansar-1.8.4/bigsansar/templates/admin/page_create.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      948 2023-07-24 10:47:59.000000 Bigsansar-1.8.4/bigsansar/templates/admin/page_delete.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      717 2023-07-24 10:40:01.000000 Bigsansar-1.8.4/bigsansar/templates/admin/page_edit.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.8.4/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1931 2023-06-05 06:55:58.000000 Bigsansar-1.8.4/bigsansar/templates/blog_preview.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      101 2023-06-25 11:39:45.000000 Bigsansar-1.8.4/bigsansar/templates/script.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-06-06 04:42:17.000000 Bigsansar-1.8.4/bigsansar/templates/sitemap.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      101 2023-06-18 11:01:43.000000 Bigsansar-1.8.4/bigsansar/templates/styles.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.8.4/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1241 2023-07-04 13:08:29.000000 Bigsansar-1.8.4/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4734 2023-06-25 11:54:54.000000 Bigsansar-1.8.4/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-07-24 11:36:02.010188 Bigsansar-1.8.4/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1753 2023-07-24 10:23:46.000000 Bigsansar-1.8.4/setup.py
```

### Comparing `Bigsansar-1.8.3/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.8.4/Bigsansar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.8.3
+Version: 1.8.4
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.8.3 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.8.4 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `Bigsansar-1.8.3/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.8.4/Bigsansar.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -124,8 +124,10 @@
 bigsansar/templates/admin/chuname.html
 bigsansar/templates/admin/dashboard.html
 bigsansar/templates/admin/domain_manage.html
 bigsansar/templates/admin/edit_domain.html
 bigsansar/templates/admin/editprofile.html
 bigsansar/templates/admin/login.html
 bigsansar/templates/admin/nav.html
-bigsansar/templates/admin/page_create.html
+bigsansar/templates/admin/page_create.html
+bigsansar/templates/admin/page_delete.html
+bigsansar/templates/admin/page_edit.html
```

### Comparing `Bigsansar-1.8.3/LICENSE` & `Bigsansar-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/PKG-INFO` & `Bigsansar-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.8.3
+Version: 1.8.4
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.8.3 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.8.4 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `Bigsansar-1.8.3/README.md` & `Bigsansar-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/account/forms.py` & `Bigsansar-1.8.4/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.8.4/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/account/models.py` & `Bigsansar-1.8.4/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/advance/forms.py` & `Bigsansar-1.8.4/bigsansar/contrib/advance/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/advance/migrations/0001_initial.py` & `Bigsansar-1.8.4/bigsansar/contrib/advance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/advance/migrations/0003_javascript.py` & `Bigsansar-1.8.4/bigsansar/contrib/advance/migrations/0003_javascript.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/advance/urls.py` & `Bigsansar-1.8.4/bigsansar/contrib/advance/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/advance/views.py` & `Bigsansar-1.8.4/bigsansar/contrib/advance/views.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/blogs/admin.py` & `Bigsansar-1.8.4/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.8.4/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.8.4/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/blogs/templatetags/blogs.py` & `Bigsansar-1.8.4/bigsansar/contrib/blogs/templatetags/blogs.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.8.4/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.8.4/bigsansar/contrib/sites/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,7 +111,18 @@
 class customviewspageform(forms.ModelForm):
     title = forms.CharField(max_length=50, required=True,
                             widget=forms.TextInput(attrs={'class': 'form-control', 'autofocus': True}))
 
     class Meta:
         model = pages
         fields = ('title',)
+
+
+
+class customviewseditpage(forms.ModelForm):
+    title = forms.CharField(max_length=50, required=True,
+                            widget=forms.TextInput(attrs={'class': 'form-control', 'autofocus': True}))
+
+    class Meta:
+        model = pages
+        fields = ('title', 'body',)
+        widgets = {'body': forms.Textarea(attrs={'class': 'form-control', 'cols': 90, 'rows': 20})}
```

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.8.4/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/sites/models.py` & `Bigsansar-1.8.4/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/sites/urls.py` & `Bigsansar-1.8.4/bigsansar/contrib/sites/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 urlpatterns = [
     path('manage/<id>', views.manage_domain, name='manage doamin'),
 #     path('create', views.create_domain, name='create domain'),
     path('manage/<id>/edit', views.edit_host, name='edit domain'),
     path('manage/<id>/pages/create', views.page_create, name='pages add'),
-#     path('manage/<id>/pages/<pagesid>/edit', views.pages_edit, name='pages edit panel'),
-#     path('manage/<id>/pages/<pagesid>/delete', views.page_delete, name='page delete'),
+    path('manage/<id>/pages/<pagesid>/edit', views.pages_edit, name='pages edit panel'),
+    path('manage/<id>/pages/<pagesid>/delete', views.page_delete, name='page delete'),
  ]
```

### Comparing `Bigsansar-1.8.3/bigsansar/contrib/sites/views.py` & `Bigsansar-1.8.4/bigsansar/contrib/sites/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 from django.shortcuts import redirect, render
 from django.core.paginator import Paginator
 import requests
-from bigsansar.contrib.sites.forms import create_domainform, customviewspageform
+from bigsansar.contrib.sites.forms import create_domainform, customviewseditpage, customviewspageform
 from django.contrib import messages
 from bigsansar.contrib.sites.models import domains, pages
 from django.utils.text import slugify
 from django.core.exceptions import ValidationError
 
 from www.settings import BASE_DIR
 
@@ -121,7 +121,79 @@
         else:
             form = customviewspageform
         return render(request, 'admin/page_create.html', {'form': form})
 
     else:
         return redirect('/admin')
 
+
+
+def pages_edit(request, id, pagesid):
+    if request.user.is_authenticated:
+        getdir = 'templates'
+
+        try:
+            user = request.user
+            get_host = domains.objects.get(pk=id, user=user)
+            query = pages.objects.get(domain=id, id=pagesid)
+
+        except:
+            return render(request, '404.html')
+
+        else:
+            if request.method == 'POST':
+                form = customviewseditpage(request.POST, instance=query)
+                if form.is_valid():
+                    db = form.save(commit=False)
+                    db.domain = get_host
+
+                    mkdir = getdir + '/' + str(get_host.domain)
+                    full_path = os.path.join(BASE_DIR, mkdir)
+                    createfile = full_path + '/' + query.slug + '.html'
+                    get_content = form.cleaned_data.get('body')
+
+                    f = open(createfile, "w", encoding="utf-8")
+                    f.write(get_content)
+                    f.close()
+                    db.save()
+                    messages.success(request, 'pages Successfully Updated')
+                    return redirect('/admin/domain/manage/' + id)
+
+            else:
+                form = customviewseditpage(instance=query)
+
+            return render(request, 'admin/page_edit.html', {'form': form})
+
+    else:
+
+        return redirect('/admin')
+
+
+
+def page_delete(request, id, pagesid):
+    if request.user.is_authenticated:
+        getdir = 'templates'
+
+        try:
+            user = request.user
+            getdomain = domains.objects.get(pk=id, user=user)
+            query = pages.objects.get(domain=id, id=pagesid)
+
+        except:
+            return render(request, '404.html')
+
+        if request.method == 'POST':
+            mkdir = getdir + '/' + str(getdomain.domain)
+            createfile = mkdir + '/' + query.slug + '.html'
+
+            if os.path.exists(createfile):
+                os.remove(createfile)
+                query.delete()
+            else:
+                query.delete()
+
+            messages.success(request, 'Pages Successfully Deleted')
+            return redirect('/admin/domain/manage/' + id)
+        return render(request, 'admin/page_delete.html', {'path': query, 'domain': getdomain})
+
+    else:
+        redirect('/admin')
```

### Comparing `Bigsansar-1.8.3/bigsansar/core/__init__.py` & `Bigsansar-1.8.4/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/core/init.py` & `Bigsansar-1.8.4/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/management/commands/createuser.py` & `Bigsansar-1.8.4/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js` & `Bigsansar-1.8.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/logo.png` & `Bigsansar-1.8.4/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/static/style.css` & `Bigsansar-1.8.4/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/404.html` & `Bigsansar-1.8.4/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/admin/chpass.html` & `Bigsansar-1.8.4/bigsansar/templates/admin/chpass.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/admin/chuname.html` & `Bigsansar-1.8.4/bigsansar/templates/admin/chuname.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/admin/dashboard.html` & `Bigsansar-1.8.4/bigsansar/templates/admin/dashboard.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/admin/domain_manage.html` & `Bigsansar-1.8.4/bigsansar/templates/admin/domain_manage.html`

 * *Files 1% similar despite different names*

```diff
@@ -199,19 +199,19 @@
 								</table>
 								<hr/>
 								{% for page in pages %}
 									<table class='table table-borderless'>
 
 										<tr>
 											<th style="text-align:left">
-												<a href="/domain/manage/{{ host.id }}/pages/{{ page.id }}/edit" style="text-decoration:none;">{{ page.title }}</a>
+												<a href="{{ host.id }}/pages/{{ page.id }}/edit" style="text-decoration:none;">{{ page.title }}</a>
 											</th>
 											<th style="text-align:right">
 												<a href="http://{{ host.domain }}/{{ page.slug }}" target="_blank"><i class="fa fa-eye" aria-hidden="true"></i></a>
-												<a href="/domain/manage/{{ host.id }}/pages/{{ page.id }}/delete"> <i class="fa fa-trash" aria-hidden="true"></i> </a>
+												<a href="{{ host.id }}/pages/{{ page.id }}/delete"> <i class="fa fa-trash" aria-hidden="true"></i> </a>
 											</th>
 
 										</tr>
 
 									</table>
 									<hr/>
 								{% endfor %}
```

### Comparing `Bigsansar-1.8.3/bigsansar/templates/admin/edit_domain.html` & `Bigsansar-1.8.4/bigsansar/templates/admin/edit_domain.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/admin/editprofile.html` & `Bigsansar-1.8.4/bigsansar/templates/admin/editprofile.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/admin/login.html` & `Bigsansar-1.8.4/bigsansar/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/admin/nav.html` & `Bigsansar-1.8.4/bigsansar/templates/admin/nav.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/admin/page_create.html` & `Bigsansar-1.8.4/bigsansar/templates/admin/page_create.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/base.html` & `Bigsansar-1.8.4/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/blog_preview.html` & `Bigsansar-1.8.4/bigsansar/templates/blog_preview.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/default.html` & `Bigsansar-1.8.4/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/defaultpage.html` & `Bigsansar-1.8.4/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/templates/parking.html` & `Bigsansar-1.8.4/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/urls.py` & `Bigsansar-1.8.4/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/bigsansar/views.py` & `Bigsansar-1.8.4/bigsansar/views.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.8.3/setup.py` & `Bigsansar-1.8.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.8.3",
+    version="1.8.4",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

