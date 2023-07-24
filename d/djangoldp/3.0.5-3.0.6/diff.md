# Comparing `tmp/djangoldp-3.0.5.tar.gz` & `tmp/djangoldp-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp-3.0.5.tar", last modified: Mon Jul 24 18:36:35 2023, max compression
+gzip compressed data, was "djangoldp-3.0.6.tar", last modified: Mon Jul 24 20:29:58 2023, max compression
```

## Comparing `djangoldp-3.0.5.tar` & `djangoldp-3.0.6.tar`

### file list

```diff
@@ -1,144 +1,141 @@
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.910802 djangoldp-3.0.5/
--rw-r--r--   0 balessan  (1001) balessan  (1001)     1069 2019-09-08 17:46:45.000000 djangoldp-3.0.5/LICENSE
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      102 2022-10-18 19:19:34.000000 djangoldp-3.0.5/MANIFEST.in
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      322 2023-07-24 18:36:35.910802 djangoldp-3.0.5/PKG-INFO
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     3694 2023-07-24 18:36:11.000000 djangoldp-3.0.5/README.md
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.866802 djangoldp-3.0.5/commit_parser/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)       73 2023-07-24 18:18:30.000000 djangoldp-3.0.5/commit_parser/__init__.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     2599 2023-07-24 18:29:57.000000 djangoldp-3.0.5/commit_parser/parser.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.874802 djangoldp-3.0.5/djangoldp/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      468 2023-07-24 18:36:33.000000 djangoldp-3.0.5/djangoldp/__init__.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.878802 djangoldp-3.0.5/djangoldp/activities/
--rw-r--r--   0 balessan  (1001) balessan  (1001)       68 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/activities/__init__.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      165 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/activities/errors.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)     5050 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/activities/objects.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    30916 2022-12-12 13:19:59.000000 djangoldp-3.0.5/djangoldp/activities/services.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     3584 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/activities/verbs.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     2631 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/admin.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     2075 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/apps.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     5144 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/check_integrity.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     4621 2022-12-19 14:36:33.000000 djangoldp-3.0.5/djangoldp/cli.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.882802 djangoldp-3.0.5/djangoldp/conf/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)        1 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/__init__.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     5269 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/conf/default_settings.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     5272 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/conf/ldpsettings.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.882802 djangoldp-3.0.5/djangoldp/conf/package_template/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)       17 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/README.md
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.882802 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)       22 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/__init__.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)       33 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/admin.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      114 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/apps.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      262 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/djangoldp_settings.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      179 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/djangoldp_urls.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      249 2022-01-21 13:05:33.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/models.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)       60 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/tests.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      143 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/views.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      374 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/setup.cfg
--rw-rw-r--   0 balessan  (1001) balessan  (1001)       81 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/setup.py-tpl
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.882802 djangoldp-3.0.5/djangoldp/conf/server_template/
--rwxrwxr-x   0 balessan  (1001) balessan  (1001)      816 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/server_template/manage.py-tpl
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.886802 djangoldp-3.0.5/djangoldp/conf/server_template/server/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/server_template/server/__init__.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      996 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/conf/server_template/server/urls.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      598 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/server_template/server/wsgi.py-tpl
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      367 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/server_template/settings.yml
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.886802 djangoldp-3.0.5/djangoldp/endpoints/
--rw-r--r--   0 balessan  (1001) balessan  (1001)        0 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/endpoints/__init__.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)     3043 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/endpoints/webfinger.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      490 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/factories.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      449 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/fields.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     6264 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/filters.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.886802 djangoldp-3.0.5/djangoldp/management/
--rw-r--r--   0 balessan  (1001) balessan  (1001)        0 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/management/__init__.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.886802 djangoldp-3.0.5/djangoldp/management/commands/
--rw-r--r--   0 balessan  (1001) balessan  (1001)        0 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/management/commands/__init__.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     1178 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/management/commands/check_integrity.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     2139 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/management/commands/configure.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     2524 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/management/commands/federate.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      468 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/management/commands/mock_user.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     1790 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/middleware.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.890802 djangoldp-3.0.5/djangoldp/migrations/
--rw-r--r--   0 balessan  (1001) balessan  (1001)      790 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/migrations/0001_initial.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      586 2020-02-04 17:17:22.000000 djangoldp-3.0.5/djangoldp/migrations/0002_auto_20190906_0642.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      502 2020-02-04 17:17:22.000000 djangoldp-3.0.5/djangoldp/migrations/0003_auto_20190911_0931.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      420 2020-05-21 09:21:47.000000 djangoldp-3.0.5/djangoldp/migrations/0004_auto_20200221_1118.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      491 2020-05-21 09:21:47.000000 djangoldp-3.0.5/djangoldp/migrations/0005_auto_20200221_1127.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)     1045 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/migrations/0006_activity.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      773 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/migrations/0007_auto_20200429_1346.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      765 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/migrations/0008_auto_20200501_1207.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      601 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/migrations/0009_auto_20200505_1733.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)     1176 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/migrations/0010_follower.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)     1024 2020-07-09 13:56:25.000000 djangoldp-3.0.5/djangoldp/migrations/0011_auto_20200610_1323.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      992 2020-07-09 13:56:25.000000 djangoldp-3.0.5/djangoldp/migrations/0012_auto_20200617_1817.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      876 2020-07-09 13:56:25.000000 djangoldp-3.0.5/djangoldp/migrations/0013_auto_20200624_1709.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     3177 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/migrations/0014_auto_20200909_2206.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      951 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/migrations/0015_auto_20210125_1847.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)        0 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/migrations/__init__.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    21294 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/models.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     1188 2023-07-12 07:41:51.000000 djangoldp-3.0.5/djangoldp/pagination.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     7718 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/permissions.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     2594 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/related.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    43569 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/serializers.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.890802 djangoldp-3.0.5/djangoldp/templates/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      895 2022-10-18 19:19:34.000000 djangoldp-3.0.5/djangoldp/templates/swagger-ui.html
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.902802 djangoldp-3.0.5/djangoldp/tests/
--rw-r--r--   0 balessan  (1001) balessan  (1001)        0 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/tests/__init__.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      505 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/djangoldp_settings.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     1160 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/djangoldp_urls.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.902802 djangoldp-3.0.5/djangoldp/tests/dummy/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/dummy/__init__.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      241 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/dummy/apps.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      256 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/dummy/middleware.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    13968 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/models.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      778 2021-09-24 10:25:18.000000 djangoldp-3.0.5/djangoldp/tests/performance_runner.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     1179 2023-07-20 09:07:09.000000 djangoldp-3.0.5/djangoldp/tests/runner.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.902802 djangoldp-3.0.5/djangoldp/tests/scripts/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/scripts/__init__.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     2209 2023-07-12 07:41:51.000000 djangoldp-3.0.5/djangoldp/tests/scripts/prod_data_generator.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     1324 2022-11-07 09:45:03.000000 djangoldp-3.0.5/djangoldp/tests/scripts/test_data_generator.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     5102 2023-07-12 07:41:51.000000 djangoldp-3.0.5/djangoldp/tests/scripts/utils.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      770 2022-08-01 12:45:48.000000 djangoldp-3.0.5/djangoldp/tests/server_settings.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     1528 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/tests_anonymous_permissions.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)     1385 2020-07-09 13:56:25.000000 djangoldp-3.0.5/djangoldp/tests/tests_auto_author.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    18371 2022-08-01 12:45:48.000000 djangoldp-3.0.5/djangoldp/tests/tests_backlinks_service.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    14619 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/tests_cache.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)      610 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/tests/tests_delete.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    12402 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_get.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     7640 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/tests_guardian.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    28857 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_inbox.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     2811 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_ldp_model.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     6037 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_ldp_viewset.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    36663 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_model_serializer.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     1070 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_pagination.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     6074 2021-09-24 10:25:18.000000 djangoldp-3.0.5/djangoldp/tests/tests_perf_get.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     1625 2021-09-24 10:25:18.000000 djangoldp-3.0.5/djangoldp/tests/tests_performance.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    12660 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_post.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     2031 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/tests_settings.py
--rw-r--r--   0 balessan  (1001) balessan  (1001)     1079 2020-05-22 09:18:07.000000 djangoldp-3.0.5/djangoldp/tests/tests_sources.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    28385 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_update.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    23475 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_user_permissions.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     3571 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/urls.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      586 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/utils.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)    31406 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/views.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.878802 djangoldp-3.0.5/djangoldp.egg-info/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      322 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/PKG-INFO
--rw-rw-r--   0 balessan  (1001) balessan  (1001)     4321 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/SOURCES.txt
--rw-rw-r--   0 balessan  (1001) balessan  (1001)        1 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/dependency_links.txt
--rw-rw-r--   0 balessan  (1001) balessan  (1001)       49 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/entry_points.txt
--rw-rw-r--   0 balessan  (1001) balessan  (1001)        1 2023-07-24 18:12:54.000000 djangoldp-3.0.5/djangoldp.egg-info/not-zip-safe
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      283 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/requires.txt
--rw-rw-r--   0 balessan  (1001) balessan  (1001)       41 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/top_level.txt
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.906802 djangoldp-3.0.5/djangoldp_crypto/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/__init__.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      331 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/admin.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.906802 djangoldp-3.0.5/djangoldp_crypto/management/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/management/__init__.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.906802 djangoldp-3.0.5/djangoldp_crypto/management/commands/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/management/commands/__init__.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      804 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/management/commands/creatersakey.py
-drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.910802 djangoldp-3.0.5/djangoldp_crypto/migrations/
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      685 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/migrations/0001_initial.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/migrations/__init__.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      900 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp_crypto/models.py
--rw-rw-r--   0 balessan  (1001) balessan  (1001)      990 2023-07-24 18:36:35.910802 djangoldp-3.0.5/setup.cfg
--rw-r--r--   0 balessan  (1001) balessan  (1001)       61 2019-09-08 17:46:45.000000 djangoldp-3.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-24 20:29:34.000000 djangoldp-3.0.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-24 20:29:34.000000 djangoldp-3.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-24 20:29:58.734598 djangoldp-3.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3694 2023-07-24 20:29:34.000000 djangoldp-3.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.722597 djangoldp-3.0.6/djangoldp/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-24 20:29:51.000000 djangoldp-3.0.6/djangoldp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/activities/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/activities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/activities/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5050 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/activities/objects.py
+-rw-rw-rw-   0 root         (0) root         (0)    30916 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/activities/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/activities/verbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     5144 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4621 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/conf/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5269 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/ldpsettings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/conf/package_template/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/__init__.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/admin.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/apps.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/djangoldp_settings.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/djangoldp_urls.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/models.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/tests.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/views.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/setup.py-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/conf/server_template/
+-rwxrwxrwx   0 root         (0) root         (0)      816 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/server_template/manage.py-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/conf/server_template/server/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/server_template/server/__init__.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/server_template/server/urls.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/server_template/server/wsgi.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      367 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/server_template/settings.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/endpoints/webfinger.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     6264 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/commands/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/commands/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/commands/federate.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/commands/mock_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.730598 djangoldp-3.0.6/djangoldp/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0002_auto_20190906_0642.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0003_auto_20190911_0931.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0004_auto_20200221_1118.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0005_auto_20200221_1127.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0006_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0007_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0008_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)      601 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0009_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0010_follower.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0011_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0012_auto_20200617_1817.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0013_auto_20200624_1709.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0014_auto_20200909_2206.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0015_auto_20210125_1847.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21294 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2594 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/related.py
+-rw-rw-rw-   0 root         (0) root         (0)    43569 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.730598 djangoldp-3.0.6/djangoldp/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/templates/swagger-ui.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/djangoldp_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp/tests/dummy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/dummy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/dummy/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/dummy/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)    13968 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/performance_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp/tests/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2209 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/scripts/prod_data_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1324 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/scripts/test_data_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5102 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/scripts/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/server_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_anonymous_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_auto_author.py
+-rw-rw-rw-   0 root         (0) root         (0)    18371 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_backlinks_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    14619 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12402 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     7640 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_guardian.py
+-rw-rw-rw-   0 root         (0) root         (0)    28857 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_inbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     2811 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_ldp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     6134 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_ldp_viewset.py
+-rw-rw-rw-   0 root         (0) root         (0)    36663 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_model_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     6074 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_perf_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_performance.py
+-rw-rw-rw-   0 root         (0) root         (0)    12660 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_sources.py
+-rw-rw-rw-   0 root         (0) root         (0)    28385 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_update.py
+-rw-rw-rw-   0 root         (0) root         (0)    23475 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_user_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31406 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      283 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp_crypto/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp_crypto/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp_crypto/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/management/commands/creatersakey.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp_crypto/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-07-24 20:29:58.734598 djangoldp-3.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 20:29:34.000000 djangoldp-3.0.6/setup.py
```

### Comparing `djangoldp-3.0.5/LICENSE` & `djangoldp-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/README.md` & `djangoldp-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/activities/objects.py` & `djangoldp-3.0.6/djangoldp/activities/objects.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/activities/services.py` & `djangoldp-3.0.6/djangoldp/activities/services.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/activities/verbs.py` & `djangoldp-3.0.6/djangoldp/activities/verbs.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/admin.py` & `djangoldp-3.0.6/djangoldp/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/apps.py` & `djangoldp-3.0.6/djangoldp/apps.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/check_integrity.py` & `djangoldp-3.0.6/djangoldp/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/cli.py` & `djangoldp-3.0.6/djangoldp/cli.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/conf/default_settings.py` & `djangoldp-3.0.6/djangoldp/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/conf/ldpsettings.py` & `djangoldp-3.0.6/djangoldp/conf/ldpsettings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/conf/server_template/manage.py-tpl` & `djangoldp-3.0.6/djangoldp/conf/server_template/manage.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/conf/server_template/server/urls.py-tpl` & `djangoldp-3.0.6/djangoldp/conf/server_template/server/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/conf/server_template/server/wsgi.py-tpl` & `djangoldp-3.0.6/djangoldp/conf/server_template/server/wsgi.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/endpoints/webfinger.py` & `djangoldp-3.0.6/djangoldp/endpoints/webfinger.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/filters.py` & `djangoldp-3.0.6/djangoldp/filters.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/management/commands/check_integrity.py` & `djangoldp-3.0.6/djangoldp/management/commands/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/management/commands/configure.py` & `djangoldp-3.0.6/djangoldp/management/commands/configure.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/management/commands/federate.py` & `djangoldp-3.0.6/djangoldp/management/commands/federate.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/middleware.py` & `djangoldp-3.0.6/djangoldp/middleware.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0001_initial.py` & `djangoldp-3.0.6/djangoldp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0002_auto_20190906_0642.py` & `djangoldp-3.0.6/djangoldp/migrations/0002_auto_20190906_0642.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0006_activity.py` & `djangoldp-3.0.6/djangoldp/migrations/0006_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0007_auto_20200429_1346.py` & `djangoldp-3.0.6/djangoldp/migrations/0007_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0008_auto_20200501_1207.py` & `djangoldp-3.0.6/djangoldp/migrations/0008_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0009_auto_20200505_1733.py` & `djangoldp-3.0.6/djangoldp/migrations/0009_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0010_follower.py` & `djangoldp-3.0.6/djangoldp/migrations/0010_follower.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0011_auto_20200610_1323.py` & `djangoldp-3.0.6/djangoldp/migrations/0011_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0012_auto_20200617_1817.py` & `djangoldp-3.0.6/djangoldp/migrations/0012_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0013_auto_20200624_1709.py` & `djangoldp-3.0.6/djangoldp/migrations/0013_auto_20200624_1709.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0014_auto_20200909_2206.py` & `djangoldp-3.0.6/djangoldp/migrations/0014_auto_20200909_2206.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/migrations/0015_auto_20210125_1847.py` & `djangoldp-3.0.6/djangoldp/migrations/0015_auto_20210125_1847.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/models.py` & `djangoldp-3.0.6/djangoldp/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/pagination.py` & `djangoldp-3.0.6/djangoldp/pagination.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/permissions.py` & `djangoldp-3.0.6/djangoldp/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/related.py` & `djangoldp-3.0.6/djangoldp/related.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/serializers.py` & `djangoldp-3.0.6/djangoldp/serializers.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/templates/swagger-ui.html` & `djangoldp-3.0.6/djangoldp/templates/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/djangoldp_urls.py` & `djangoldp-3.0.6/djangoldp/tests/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/models.py` & `djangoldp-3.0.6/djangoldp/tests/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/performance_runner.py` & `djangoldp-3.0.6/djangoldp/tests/performance_runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/runner.py` & `djangoldp-3.0.6/djangoldp/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/scripts/prod_data_generator.py` & `djangoldp-3.0.6/djangoldp/tests/scripts/prod_data_generator.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/scripts/test_data_generator.py` & `djangoldp-3.0.6/djangoldp/tests/scripts/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/scripts/utils.py` & `djangoldp-3.0.6/djangoldp/tests/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/server_settings.py` & `djangoldp-3.0.6/djangoldp/tests/server_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_anonymous_permissions.py` & `djangoldp-3.0.6/djangoldp/tests/tests_anonymous_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_auto_author.py` & `djangoldp-3.0.6/djangoldp/tests/tests_auto_author.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_backlinks_service.py` & `djangoldp-3.0.6/djangoldp/tests/tests_backlinks_service.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_cache.py` & `djangoldp-3.0.6/djangoldp/tests/tests_cache.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_delete.py` & `djangoldp-3.0.6/djangoldp/tests/tests_delete.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_get.py` & `djangoldp-3.0.6/djangoldp/tests/tests_get.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_guardian.py` & `djangoldp-3.0.6/djangoldp/tests/tests_guardian.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_inbox.py` & `djangoldp-3.0.6/djangoldp/tests/tests_inbox.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_ldp_model.py` & `djangoldp-3.0.6/djangoldp/tests/tests_ldp_model.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_ldp_viewset.py` & `djangoldp-3.0.6/djangoldp/tests/tests_ldp_viewset.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,18 +73,20 @@
 
         # request id and name only
         fields_shape = '["@id", "name"]'
 
         response = self.client.get('/circles/', HTTP_ACCEPT_MODEL_FIELDS=fields_shape)
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         response_data_keys = response.data['ldp:contains'][0].keys()
-        self.assertEqual(len(response_data_keys), 3)
+        self.assertIn(len(response_data_keys), (3,4))
         self.assertIn('@id', response_data_keys)
         self.assertIn('name', response_data_keys)
         self.assertIn('@type', response_data_keys)
+        if len(response_data_keys)>3:
+            self.assertIn('@context', response_data_keys)
 
     def test_search_fields_basic(self):
         self.setUpLoggedInUser()
         lowercase_circle = Circle.objects.create(name='test circle')
         uppercase_circle = Circle.objects.create(name='hello world', description='test')
 
         response = self.client.get('/circles/?search-fields=name&search-terms=test&search-method=basic')
```

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_model_serializer.py` & `djangoldp-3.0.6/djangoldp/tests/tests_model_serializer.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_pagination.py` & `djangoldp-3.0.6/djangoldp/tests/tests_pagination.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_perf_get.py` & `djangoldp-3.0.6/djangoldp/tests/tests_perf_get.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_performance.py` & `djangoldp-3.0.6/djangoldp/tests/tests_performance.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_post.py` & `djangoldp-3.0.6/djangoldp/tests/tests_post.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_settings.py` & `djangoldp-3.0.6/djangoldp/tests/tests_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_sources.py` & `djangoldp-3.0.6/djangoldp/tests/tests_sources.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_update.py` & `djangoldp-3.0.6/djangoldp/tests/tests_update.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/tests/tests_user_permissions.py` & `djangoldp-3.0.6/djangoldp/tests/tests_user_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/urls.py` & `djangoldp-3.0.6/djangoldp/urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/utils.py` & `djangoldp-3.0.6/djangoldp/utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp/views.py` & `djangoldp-3.0.6/djangoldp/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp.egg-info/SOURCES.txt` & `djangoldp-3.0.6/djangoldp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-commit_parser/__init__.py
-commit_parser/parser.py
 djangoldp/__init__.py
 djangoldp/admin.py
 djangoldp/apps.py
 djangoldp/check_integrity.py
 djangoldp/cli.py
 djangoldp/factories.py
 djangoldp/fields.py
```

### Comparing `djangoldp-3.0.5/djangoldp_crypto/management/commands/creatersakey.py` & `djangoldp-3.0.6/djangoldp_crypto/management/commands/creatersakey.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp_crypto/migrations/0001_initial.py` & `djangoldp-3.0.6/djangoldp_crypto/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/djangoldp_crypto/models.py` & `djangoldp-3.0.6/djangoldp_crypto/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.5/setup.cfg` & `djangoldp-3.0.6/setup.cfg`

 * *Files identical despite different names*

