# Comparing `tmp/djangoldp-2.1.9.tar.gz` & `tmp/djangoldp-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp-2.1.9.tar", last modified: Fri Apr 23 15:12:59 2021, max compression
+gzip compressed data, was "djangoldp-3.0.5.tar", last modified: Mon Jul 24 18:36:35 2023, max compression
```

## Comparing `djangoldp-2.1.9.tar` & `djangoldp-3.0.5.tar`

### file list

```diff
@@ -1,138 +1,144 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/
--rw-rw-rw-   0 root         (0) root         (0)     1011 2021-04-23 15:12:59.000000 djangoldp-2.1.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2277 2021-04-23 15:12:39.000000 djangoldp-2.1.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)       75 2021-04-23 15:12:39.000000 djangoldp-2.1.9/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp_crypto/
--rw-rw-rw-   0 root         (0) root         (0)      902 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/models.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp_crypto/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      685 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp_crypto/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp_crypto/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      804 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/management/commands/creatersakey.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/management/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-04-23 15:12:39.000000 djangoldp-2.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/
--rw-rw-rw-   0 root         (0) root         (0)    39434 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)    18319 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/models.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/conf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/conf/package_template/
--rw-rw-rw-   0 root         (0) root         (0)      374 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       17 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/
--rw-rw-rw-   0 root         (0) root         (0)      114 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/apps.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      220 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/models.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      143 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/views.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       60 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/tests.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       33 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/admin.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      262 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/djangoldp_settings.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      184 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/djangoldp_urls.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       22 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/__init__.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       81 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/setup.py-tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/conf/server_template/
--rwxrwxrwx   0 root         (0) root         (0)      816 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/server_template/manage.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      367 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/server_template/settings.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/conf/server_template/server/
--rw-rw-rw-   0 root         (0) root         (0)      598 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/server_template/server/wsgi.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)     1002 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/server_template/server/urls.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/server_template/server/__init__.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)     4311 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     4839 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/ldpsettings.py
--rw-rw-rw-   0 root         (0) root         (0)        1 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/activities/
--rw-rw-rw-   0 root         (0) root         (0)     5050 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/activities/objects.py
--rw-rw-rw-   0 root         (0) root         (0)    28065 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/activities/services.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/activities/verbs.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/activities/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/activities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8560 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)     3043 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/endpoints/webfinger.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30033 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/views.py
--rw-rw-rw-   0 root         (0) root         (0)     2594 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/related.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     5144 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     2327 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_sources.py
--rw-rw-rw-   0 root         (0) root         (0)    11559 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)    28591 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_update.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/performance_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     7962 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_guardian.py
--rw-rw-rw-   0 root         (0) root         (0)    18514 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_user_permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/tests/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1753 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/scripts/prod_data_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2153 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/scripts/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1098 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/scripts/test_data_generator.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/tests/dummy/
--rw-rw-rw-   0 root         (0) root         (0)      241 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/dummy/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/dummy/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/dummy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      610 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_delete.py
--rw-rw-rw-   0 root         (0) root         (0)     2940 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_ldp_viewset.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_auto_author.py
--rw-rw-rw-   0 root         (0) root         (0)     1635 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_performance.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)    11970 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_get.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     1528 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_anonymous_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     5796 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_perf_get.py
--rw-rw-rw-   0 root         (0) root         (0)    18691 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_backlinks_service.py
--rw-rw-rw-   0 root         (0) root         (0)    11634 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/settings_default.py
--rw-rw-rw-   0 root         (0) root         (0)    28823 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_inbox.py
--rw-rw-rw-   0 root         (0) root         (0)    36950 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_model_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2821 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_ldp_model.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/djangoldp_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3097 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     4621 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      773 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0007_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0011_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0003_auto_20190911_0931.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0012_auto_20200617_1817.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0008_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)     1176 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0010_follower.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0002_auto_20190906_0642.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0005_auto_20200221_1127.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0006_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0004_auto_20200221_1118.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0015_auto_20210125_1847.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0013_auto_20200624_1709.py
--rw-rw-rw-   0 root         (0) root         (0)     3177 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0014_auto_20200909_2206.py
--rw-rw-rw-   0 root         (0) root         (0)      601 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0009_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/pagination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     2474 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/commands/federate.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/commands/mock_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/commands/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/commands/configure.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2933 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2021-04-23 15:12:52.000000 djangoldp-2.1.9/djangoldp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      339 2021-04-23 15:12:59.000000 djangoldp-2.1.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      304 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       50 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     4228 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      339 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/PKG-INFO
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.910802 djangoldp-3.0.5/
+-rw-r--r--   0 balessan  (1001) balessan  (1001)     1069 2019-09-08 17:46:45.000000 djangoldp-3.0.5/LICENSE
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      102 2022-10-18 19:19:34.000000 djangoldp-3.0.5/MANIFEST.in
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      322 2023-07-24 18:36:35.910802 djangoldp-3.0.5/PKG-INFO
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     3694 2023-07-24 18:36:11.000000 djangoldp-3.0.5/README.md
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.866802 djangoldp-3.0.5/commit_parser/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       73 2023-07-24 18:18:30.000000 djangoldp-3.0.5/commit_parser/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     2599 2023-07-24 18:29:57.000000 djangoldp-3.0.5/commit_parser/parser.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.874802 djangoldp-3.0.5/djangoldp/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      468 2023-07-24 18:36:33.000000 djangoldp-3.0.5/djangoldp/__init__.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.878802 djangoldp-3.0.5/djangoldp/activities/
+-rw-r--r--   0 balessan  (1001) balessan  (1001)       68 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/activities/__init__.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      165 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/activities/errors.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)     5050 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/activities/objects.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    30916 2022-12-12 13:19:59.000000 djangoldp-3.0.5/djangoldp/activities/services.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     3584 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/activities/verbs.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     2631 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/admin.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     2075 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/apps.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     5144 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/check_integrity.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     4621 2022-12-19 14:36:33.000000 djangoldp-3.0.5/djangoldp/cli.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.882802 djangoldp-3.0.5/djangoldp/conf/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        1 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     5269 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/conf/default_settings.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     5272 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/conf/ldpsettings.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.882802 djangoldp-3.0.5/djangoldp/conf/package_template/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       17 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/README.md
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.882802 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       22 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/__init__.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       33 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/admin.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      114 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/apps.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      262 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/djangoldp_settings.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      179 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/djangoldp_urls.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      249 2022-01-21 13:05:33.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/models.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       60 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/tests.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      143 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/app_name/views.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      374 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/setup.cfg
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       81 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/package_template/setup.py-tpl
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.882802 djangoldp-3.0.5/djangoldp/conf/server_template/
+-rwxrwxr-x   0 balessan  (1001) balessan  (1001)      816 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/server_template/manage.py-tpl
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.886802 djangoldp-3.0.5/djangoldp/conf/server_template/server/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/server_template/server/__init__.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      996 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/conf/server_template/server/urls.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      598 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/server_template/server/wsgi.py-tpl
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      367 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/conf/server_template/settings.yml
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.886802 djangoldp-3.0.5/djangoldp/endpoints/
+-rw-r--r--   0 balessan  (1001) balessan  (1001)        0 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/endpoints/__init__.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)     3043 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/endpoints/webfinger.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      490 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/factories.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      449 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/fields.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     6264 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/filters.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.886802 djangoldp-3.0.5/djangoldp/management/
+-rw-r--r--   0 balessan  (1001) balessan  (1001)        0 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/management/__init__.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.886802 djangoldp-3.0.5/djangoldp/management/commands/
+-rw-r--r--   0 balessan  (1001) balessan  (1001)        0 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/management/commands/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1178 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/management/commands/check_integrity.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     2139 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/management/commands/configure.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     2524 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/management/commands/federate.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      468 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/management/commands/mock_user.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1790 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/middleware.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.890802 djangoldp-3.0.5/djangoldp/migrations/
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      790 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/migrations/0001_initial.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      586 2020-02-04 17:17:22.000000 djangoldp-3.0.5/djangoldp/migrations/0002_auto_20190906_0642.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      502 2020-02-04 17:17:22.000000 djangoldp-3.0.5/djangoldp/migrations/0003_auto_20190911_0931.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      420 2020-05-21 09:21:47.000000 djangoldp-3.0.5/djangoldp/migrations/0004_auto_20200221_1118.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      491 2020-05-21 09:21:47.000000 djangoldp-3.0.5/djangoldp/migrations/0005_auto_20200221_1127.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)     1045 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/migrations/0006_activity.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      773 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/migrations/0007_auto_20200429_1346.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      765 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/migrations/0008_auto_20200501_1207.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      601 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/migrations/0009_auto_20200505_1733.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)     1176 2020-05-26 20:42:38.000000 djangoldp-3.0.5/djangoldp/migrations/0010_follower.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)     1024 2020-07-09 13:56:25.000000 djangoldp-3.0.5/djangoldp/migrations/0011_auto_20200610_1323.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      992 2020-07-09 13:56:25.000000 djangoldp-3.0.5/djangoldp/migrations/0012_auto_20200617_1817.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      876 2020-07-09 13:56:25.000000 djangoldp-3.0.5/djangoldp/migrations/0013_auto_20200624_1709.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     3177 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/migrations/0014_auto_20200909_2206.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      951 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/migrations/0015_auto_20210125_1847.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)        0 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/migrations/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    21294 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/models.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1188 2023-07-12 07:41:51.000000 djangoldp-3.0.5/djangoldp/pagination.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     7718 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/permissions.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     2594 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/related.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    43569 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/serializers.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.890802 djangoldp-3.0.5/djangoldp/templates/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      895 2022-10-18 19:19:34.000000 djangoldp-3.0.5/djangoldp/templates/swagger-ui.html
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.902802 djangoldp-3.0.5/djangoldp/tests/
+-rw-r--r--   0 balessan  (1001) balessan  (1001)        0 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/tests/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      505 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/djangoldp_settings.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1160 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/djangoldp_urls.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.902802 djangoldp-3.0.5/djangoldp/tests/dummy/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/dummy/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      241 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/dummy/apps.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      256 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/dummy/middleware.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    13968 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/models.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      778 2021-09-24 10:25:18.000000 djangoldp-3.0.5/djangoldp/tests/performance_runner.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1179 2023-07-20 09:07:09.000000 djangoldp-3.0.5/djangoldp/tests/runner.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.902802 djangoldp-3.0.5/djangoldp/tests/scripts/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/scripts/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     2209 2023-07-12 07:41:51.000000 djangoldp-3.0.5/djangoldp/tests/scripts/prod_data_generator.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1324 2022-11-07 09:45:03.000000 djangoldp-3.0.5/djangoldp/tests/scripts/test_data_generator.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     5102 2023-07-12 07:41:51.000000 djangoldp-3.0.5/djangoldp/tests/scripts/utils.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      770 2022-08-01 12:45:48.000000 djangoldp-3.0.5/djangoldp/tests/server_settings.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1528 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/tests_anonymous_permissions.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)     1385 2020-07-09 13:56:25.000000 djangoldp-3.0.5/djangoldp/tests/tests_auto_author.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    18371 2022-08-01 12:45:48.000000 djangoldp-3.0.5/djangoldp/tests/tests_backlinks_service.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    14619 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/tests_cache.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)      610 2019-09-08 17:46:45.000000 djangoldp-3.0.5/djangoldp/tests/tests_delete.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    12402 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_get.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     7640 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/tests_guardian.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    28857 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_inbox.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     2811 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_ldp_model.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     6037 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_ldp_viewset.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    36663 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_model_serializer.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1070 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_pagination.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     6074 2021-09-24 10:25:18.000000 djangoldp-3.0.5/djangoldp/tests/tests_perf_get.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1625 2021-09-24 10:25:18.000000 djangoldp-3.0.5/djangoldp/tests/tests_performance.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    12660 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_post.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     2031 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/tests/tests_settings.py
+-rw-r--r--   0 balessan  (1001) balessan  (1001)     1079 2020-05-22 09:18:07.000000 djangoldp-3.0.5/djangoldp/tests/tests_sources.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    28385 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_update.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    23475 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/tests/tests_user_permissions.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     3571 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/urls.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      586 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp/utils.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)    31406 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp/views.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.878802 djangoldp-3.0.5/djangoldp.egg-info/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      322 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/PKG-INFO
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     4321 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/SOURCES.txt
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        1 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/dependency_links.txt
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       49 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/entry_points.txt
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        1 2023-07-24 18:12:54.000000 djangoldp-3.0.5/djangoldp.egg-info/not-zip-safe
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      283 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/requires.txt
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       41 2023-07-24 18:36:35.000000 djangoldp-3.0.5/djangoldp.egg-info/top_level.txt
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.906802 djangoldp-3.0.5/djangoldp_crypto/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      331 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/admin.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.906802 djangoldp-3.0.5/djangoldp_crypto/management/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/management/__init__.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.906802 djangoldp-3.0.5/djangoldp_crypto/management/commands/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/management/commands/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      804 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/management/commands/creatersakey.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:36:35.910802 djangoldp-3.0.5/djangoldp_crypto/migrations/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      685 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/migrations/0001_initial.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        0 2021-08-25 08:46:23.000000 djangoldp-3.0.5/djangoldp_crypto/migrations/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      900 2023-07-24 17:56:19.000000 djangoldp-3.0.5/djangoldp_crypto/models.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      990 2023-07-24 18:36:35.910802 djangoldp-3.0.5/setup.cfg
+-rw-r--r--   0 balessan  (1001) balessan  (1001)       61 2019-09-08 17:46:45.000000 djangoldp-3.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp-2.1.9/setup.cfg` & `djangoldp-3.0.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 universal = 1
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 setup_requires = 
-	django~=2.2
+	django~=4.2
 install_requires = 
-	django~=2.2
+	django~=4.2
 	validators~=0.12
-	pyld==1.0.5
-	django-guardian==2.3.0
-	django-cookies-samesite~=0.8.0
-	djangorestframework~=3.12
-	requests==2.23.0
-	pyyaml==5.3.1
-	pyyaml==5.3.1
-	click==7.1.1
+	pyld~=1.0
+	django-guardian~=2.4
+	djangorestframework~=3.14
+	drf-spectacular~=0.24
+	requests~=2.31
+	pyyaml~=6.0
+	click~=8.1
 	django-brotli~=0.2.0
 	djangorestframework-guardian~=0.3.0
+	Faker~=14.2
 
 [options.entry_points]
 console_scripts = 
 	djangoldp = djangoldp.cli:main
 
 [options.extras_require]
 dev =
```

### Comparing `djangoldp-2.1.9/djangoldp_crypto/models.py` & `djangoldp-3.0.5/djangoldp_crypto/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from hashlib import md5
 
 from Cryptodome.PublicKey import RSA
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
-
+from django.utils.translation import gettext_lazy as _
 
 class RSAKey(models.Model):
 
     priv_key = models.TextField(
         verbose_name=_(u'Key'), unique=True,
         help_text=_(u'Paste your private RSA Key here.'))
```

### Comparing `djangoldp-2.1.9/djangoldp_crypto/migrations/0001_initial.py` & `djangoldp-3.0.5/djangoldp_crypto/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp_crypto/management/commands/creatersakey.py` & `djangoldp-3.0.5/djangoldp_crypto/management/commands/creatersakey.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/serializers.py` & `djangoldp-3.0.5/djangoldp/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,73 +1,91 @@
 import uuid
-from collections import OrderedDict, Mapping, Iterable
+import json
+from collections import OrderedDict
+from collections.abc import Mapping, Iterable
 from typing import Any
 from urllib import parse
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ImproperlyConfigured
 from django.core.exceptions import ValidationError as DjangoValidationError
 from django.db import transaction
 from django.db.models import QuerySet
 from django.urls import resolve, Resolver404, get_script_prefix
 from django.urls.resolvers import get_resolver
 from django.utils.datastructures import MultiValueDictKeyError
 from django.utils.encoding import uri_to_iri
+from django.utils.functional import cached_property
 from rest_framework.exceptions import ValidationError
 from rest_framework.fields import SkipField, empty, ReadOnlyField
 from rest_framework.fields import get_error_detail, set_value
 from rest_framework.relations import HyperlinkedRelatedField, ManyRelatedField, MANY_RELATION_KWARGS, Hyperlink
 from rest_framework.serializers import HyperlinkedModelSerializer, ListSerializer, ModelSerializer, \
     LIST_SERIALIZER_KWARGS
 from rest_framework.settings import api_settings
 from rest_framework.utils import model_meta
 from rest_framework.utils.field_mapping import get_nested_relation_kwargs
-from rest_framework.utils.serializer_helpers import ReturnDict
+from rest_framework.utils.serializer_helpers import ReturnDict, BindingDict
 
 from djangoldp.fields import LDPUrlField, IdURLField
 from djangoldp.models import Model
 from djangoldp.permissions import LDPPermissions
 
 
 # defaults for various DjangoLDP settings (see documentation)
 SERIALIZE_EXCLUDE_PERMISSIONS_DEFAULT = ['inherit']
 SERIALIZE_EXCLUDE_CONTAINER_PERMISSIONS_DEFAULT = ['delete']
 SERIALIZE_EXCLUDE_OBJECT_PERMISSIONS_DEFAULT = []
+MAX_RECORDS_SERIALIZER_CACHE = getattr(settings, 'MAX_RECORDS_SERIALIZER_CACHE', 10000)
 
 
 class InMemoryCache:
 
     def __init__(self):
         self.cache = {
         }
 
     def reset(self):
         self.cache = {
         }
 
-    def has(self, cache_key, vary):
-        return cache_key in self.cache and vary in self.cache[cache_key]
-
-    def get(self, cache_key, vary):
-        if self.has(cache_key, vary):
-            return self.cache[cache_key][vary]['value']
+    def has(self, cache_key, container_urlid=None, vary=None):
+        return cache_key in self.cache and \
+               (container_urlid is None or container_urlid in self.cache[cache_key]) and \
+               (vary is None or vary in self.cache[cache_key][container_urlid])
+
+    def get(self, cache_key, container_urlid, vary):
+        if self.has(cache_key, container_urlid, vary):
+            return self.cache[cache_key][container_urlid][vary]['value']
         else:
             return None
 
-    def set(self, cache_key, vary, value):
+    def set(self, cache_key, container_urlid, vary, value):
+        if len(self.cache.keys()) > MAX_RECORDS_SERIALIZER_CACHE:
+            self.reset()
+        
         if cache_key not in self.cache:
             self.cache[cache_key] = {}
-        self.cache[cache_key][vary] = {'value': value}
-
-    def invalidate(self, cache_key, vary=None):
-        if vary is None:
-            self.cache.pop(cache_key, None)
+        if container_urlid not in self.cache[cache_key]:
+            self.cache[cache_key][container_urlid] = {}
+        self.cache[cache_key][container_urlid][vary] = {'value': value}
+
+    def invalidate(self, cache_key, container_urlid=None, vary=None):
+        # can clear cache_key -> container_urlid -> vary, cache_key -> container_urlid or cache_key
+        if container_urlid is not None:
+            if vary is not None:
+                self.cache[cache_key][container_urlid].pop(vary, None)
+            else:
+                self.cache[cache_key].pop(container_urlid, None)
         else:
-            self.cache[cache_key].pop(vary, None)
+            self.cache.pop(cache_key, None)
+
+
+GLOBAL_SERIALIZER_CACHE = InMemoryCache()
 
 
 def _serialize_permissions(permissions, exclude_perms):
     '''takes a set or list of permissions and returns them in the JSON-LD format'''
     exclude_perms = set(exclude_perms).union(
         getattr(settings, 'SERIALIZE_EXCLUDE_PERMISSIONS', SERIALIZE_EXCLUDE_PERMISSIONS_DEFAULT))
 
@@ -109,16 +127,14 @@
 
 class LDListMixin:
     '''A Mixin for serializing containers into JSONLD format'''
     child_attr = 'child'
 
     with_cache = getattr(settings, 'SERIALIZER_CACHE', True)
 
-    to_representation_cache = InMemoryCache()
-
     # converts primitive data representation to the representation used within our application
     def to_internal_value(self, data):
         try:
             # if this is a container, the data will be stored in ldp:contains
             data = data['ldp:contains']
         except (TypeError, KeyError):
             pass
@@ -136,22 +152,26 @@
         '''
         Converts internal representation to primitive data representation
         Filters objects out which I don't have permission to view
         Permission on container :
          - Can Add if add permission on contained object's type
          - Can view the container is view permission on container model : container obj are filtered by view permission
         '''
-        def check_cache():
+        def check_cache(model):
             '''Auxiliary function to avoid code duplication - checks cache and returns from it if it has entry'''
-            if not self.id.startswith('http'):
-                self.id = '{}{}{}'.format(settings.BASE_URL, Model.resource(parent_model), self.id)
-
-            cache_key = self.id
-            if self.with_cache and self.to_representation_cache.has(cache_key, cache_vary):
-                return self.to_representation_cache.get(cache_key, cache_vary)
+            cache_key = Model.get_meta(model, 'label')
+            if self.with_cache and GLOBAL_SERIALIZER_CACHE.has(cache_key, self.id, cache_vary):
+                cache_value = GLOBAL_SERIALIZER_CACHE.get(cache_key, self.id, cache_vary)
+                # this check is to handle the situation where the cache has been invalidated by something we don't check
+                # namely if my permissions are upgraded then I may have access to view more objects
+                cache_under_value = cache_value['ldp:contains'] if 'ldp:contains' in cache_value else cache_value
+                if not hasattr(cache_under_value, '__len__') or not hasattr(value, '__len__') \
+                    or (len(cache_under_value) == len(value)):
+                    return cache_value
+            return False
 
         # if this field is listed as an "empty_container" it means that it should only be serialized with @id
         if getattr(self, 'parent', None) is not None and getattr(self, 'field_name', None) is not None:
             empty_containers = getattr(self.parent.Meta.model._meta, 'empty_containers', None)
 
             if empty_containers is not None and self.field_name in empty_containers:
                 return _ldp_container_representation(self.id)
@@ -159,44 +179,59 @@
         try:
             child_model = getattr(self, self.child_attr).Meta.model
         except AttributeError:
             child_model = value.model
 
         parent_model = None
 
+        # if the depth is greater than 0, we don't hit the cache, because a nested container might be outdated
+        # this Mixin may not have access to the depth of the parent serializer, e.g. if it's a ManyRelatedField
+        # in these cases we assume the depth is 0 and so we hit the cache
+        parent_meta = getattr(getattr(self, self.child_attr), 'Meta', getattr(self.parent, 'Meta', None))
+        depth = max(getattr(parent_meta, "depth", 0), 0) if parent_meta else 1
+
         cache_vary = str(self.context['request'].user)
 
         if not isinstance(value, Iterable) and not isinstance(value, QuerySet):
-            check_cache()
+            if not self.id.startswith('http'):
+                self.id = '{}{}{}'.format(settings.BASE_URL, Model.resource(parent_model), self.id)
+
+            cache_result = check_cache(child_model) if depth == 0 else False
+            if cache_result:
+                return cache_result
+
+            setattr(self.context['request'], "parent_id", self.id)
             container_permissions = _serialize_container_permissions(
                 Model.get_container_permissions(child_model, self.context['request'], self.context['view']))
 
         else:
-            try:
-                parent_model = Model.resolve_parent(self.context['request'].path)
-            except:
-                parent_model = child_model
+            parent_model = self.context['request'].parent_model if self.context['request'].parent_model is not None else child_model
 
-            check_cache()
+            if not self.id.startswith('http'):
+                self.id = '{}{}{}'.format(settings.BASE_URL, Model.resource(parent_model), self.id)
+
+            cache_result = check_cache(child_model) if depth == 0 else False
+            if cache_result:
+                return cache_result
 
             # optimize: filter the queryset automatically based on child model permissions classes (filter_backends)
             if isinstance(value, QuerySet) and hasattr(child_model, 'get_queryset'):
                 value = child_model.get_queryset(self.context['request'], self.context['view'], queryset=value,
                                                  model=child_model)
 
             container_permissions = Model.get_container_permissions(child_model, self.context['request'], self.context['view'])
             container_permissions = _serialize_container_permissions(container_permissions.union(
                 Model.get_container_permissions(parent_model, self.context['request'], self.context['view'])))
 
-        self.to_representation_cache.set(self.id, cache_vary,
-                                         _ldp_container_representation(self.id,
-                                                                       container_permissions=container_permissions,
-                                                                       value=super().to_representation(value)))
+        GLOBAL_SERIALIZER_CACHE.set(Model.get_meta(child_model, 'label'), self.id, cache_vary,
+                                    _ldp_container_representation(self.id,
+                                                                  container_permissions=container_permissions,
+                                                                  value=super().to_representation(value)))
 
-        return self.to_representation_cache.get(self.id, cache_vary)
+        return GLOBAL_SERIALIZER_CACHE.get(Model.get_meta(child_model, 'label'), self.id, cache_vary)
 
     def get_attribute(self, instance):
         parent_id_field = self.parent.fields[self.parent.url_field_name]
         context = self.parent.context
         parent_id = parent_id_field.get_url(instance, parent_id_field.view_name, context['request'], context['format'])
         self.id = parent_id + self.field_name + "/"
         return super().get_attribute(instance)
@@ -315,15 +350,15 @@
         try:
             return super().to_internal_value(data[self.parent.url_field_name])
         except (KeyError, TypeError):
             return super().to_internal_value(data)
 
     @classmethod
     def many_init(cls, *args, **kwargs):
-        list_kwargs = {'child_relation': cls(*args, **kwargs)}
+        list_kwargs = {'child_relation': cls(*args, **kwargs),}
         for key in kwargs:
             if key in MANY_RELATION_KWARGS:
                 list_kwargs[key] = kwargs[key]
         return ManyJsonLdRelatedField(**list_kwargs)
 
 
 class JsonLdIdentityField(JsonLdField):
@@ -366,40 +401,58 @@
 
 class LDPSerializer(HyperlinkedModelSerializer):
     url_field_name = "@id"
     serializer_related_field = JsonLdRelatedField
     serializer_url_field = JsonLdIdentityField
     ModelSerializer.serializer_field_mapping[LDPUrlField] = IdURLField
 
-    with_cache = getattr(settings, 'SERIALIZER_CACHE', True)
-
-    to_representation_cache = InMemoryCache()
+    def __init__(self, *args, **kwargs):
+        # for performance reasons, we don't serialize permissions on a resource if we're in a larger container
+        self.in_container = kwargs.pop('in_container', False)
+        super().__init__(*args, **kwargs)
+
+
+    @cached_property
+    def fields(self):
+        """
+        A dictionary of {field_name: field_instance}.
+        """
+        # `fields` is evaluated lazily. We do this to ensure that we don't
+        # have issues importing modules that use ModelSerializers as fields,
+        # even if Django's app-loading stage has not yet run.
+        fields = BindingDict(self)
+
+        # we allow the request object to specify a subset of fields which should be serialized
+        model_fields = self.get_fields()
+        req_header_accept_shape = self.context['request'].META.get('HTTP_ACCEPT_MODEL_FIELDS') if 'request' in self.context else None
+        try:
+            allowed_fields = list(set(json.loads(req_header_accept_shape)).intersection(model_fields.keys())) if req_header_accept_shape is not None else model_fields.keys()
+        except json.decoder.JSONDecodeError:
+            raise ValidationError("Please send the HTTP header Accept-Model-Fields as an array of strings")
+
+        for key, value in model_fields.items():
+            if key in allowed_fields:
+                fields[key] = value
+        
+        return fields
 
     def get_default_field_names(self, declared_fields, model_info):
         try:
             fields = list(self.Meta.model._meta.serializer_fields)
         except AttributeError:
             fields = super().get_default_field_names(declared_fields, model_info)
         return fields + list(getattr(self.Meta, 'extra_fields', []))
 
     def to_representation(self, obj):
         # external Models should only be returned with rdf values
         if Model.is_external(obj):
             data = {'@id': obj.urlid}
             return _serialize_rdf_fields(obj, data)
 
-        cache_vary = str(self.context['request'].user)
-        if self.with_cache and hasattr(obj, 'urlid'):
-            if self.to_representation_cache.has(obj.urlid, cache_vary):
-                data = self.to_representation_cache.get(obj.urlid, cache_vary)
-            else:
-                data = super().to_representation(obj)
-                self.to_representation_cache.set(obj.urlid, cache_vary, data)
-        else:
-            data = super().to_representation(obj)
+        data = super().to_representation(obj)
 
         slug_field = Model.slug_field(obj)
         for field in data:
             if isinstance(data[field], dict) and '@id' in data[field]:
                 data[field]['@id'] = data[field]['@id'].format(Model.container_id(obj), str(getattr(obj, slug_field)))
         # prioritise urlid field over generated @id
         if 'urlid' in data and data['urlid'] is not None:
@@ -408,16 +461,17 @@
             data['@id'] = '{}{}'.format(settings.SITE_URL, Model.resource(obj))
 
         data = _serialize_rdf_fields(obj, data, include_context=True)
         if hasattr(obj, 'get_model_class'):
             model_class = obj.get_model_class()
         else:
             model_class = type(obj)
-        data['permissions'] = _serialize_object_permissions(
-            Model.get_permissions(model_class, self.context['request'], self.context['view'], obj))
+        if not self.in_container:
+            data['permissions'] = _serialize_object_permissions(
+                Model.get_permissions(model_class, self.context['request'], self.context['view'], obj))
 
         return data
 
     def build_property_field(self, field_name, model_class):
         class JSonLDPropertyField(ReadOnlyField):
             def to_representation(self, instance):
                 from djangoldp.views import LDPViewSet
@@ -433,15 +487,15 @@
                                                                                         'permission_classes',
                                                                                         [LDPPermissions]),
                                                       fields=Model.get_meta(model_class, 'serializer_fields', []),
                                                       nested_fields=model_class.nested.nested_fields())
                     parent_depth = max(getattr(self.parent.Meta, "depth", 0) - 1, 0)
                     serializer_generator.depth = parent_depth
                     serializer = serializer_generator.build_read_serializer()(context=self.parent.context)
-                    if parent_depth is 0:
+                    if parent_depth == 0:
                         serializer.Meta.fields = ["@id"]
 
                     if isinstance(instance, QuerySet):
                         data = list(instance)
                         id = '{}{}{}/'.format(settings.SITE_URL, '{}{}/', self.source)
                         permissions = _serialize_container_permissions(Model.get_permissions(self.parent.Meta.model,
                                                                                     self.parent.context['request'],
@@ -524,15 +578,15 @@
                 depth = nested_depth - 1
                 try:
                     fields = ['@id'] + list(model._meta.serializer_fields)
                 except AttributeError:
                     fields = '__all__'
 
             def to_internal_value(self, data):
-                if data is '':
+                if data == '':
                     return ''
                 # workaround for Hubl app - 293
                 if 'username' in data and not self.url_field_name in data:
                     data[self.url_field_name] = './'
                 if self.url_field_name in data:
                     if not isinstance(data, Mapping):
                         message = self.error_messages['invalid'].format(
@@ -601,37 +655,43 @@
         kwargs['read_only'] = False
         kwargs['required'] = False
         return NestedLDPSerializer, kwargs
 
     @classmethod
     def many_init(cls, *args, **kwargs):
         allow_empty = kwargs.pop('allow_empty', None)
+        # we pass in_container to tell the child that they're in a container
+        #  then in the child we optimize the permissions serialization based on this
+        kwargs['in_container'] = True
         child_serializer = cls(*args, **kwargs)
         list_kwargs = {
             'child': child_serializer,
         }
         if allow_empty is not None:
             list_kwargs['allow_empty'] = allow_empty
         list_kwargs.update({
             key: value for key, value in kwargs.items()
             if key in LIST_SERIALIZER_KWARGS
         })
         meta = getattr(cls, 'Meta', None)
         list_serializer_class = getattr(meta, 'list_serializer_class', ContainerSerializer)
         serializer = list_serializer_class(*args, **list_kwargs)
 
+        # if the child serializer has disabled the cache, really it means disable it on the container
+        if hasattr(child_serializer, 'with_cache'):
+            serializer.with_cache = child_serializer.with_cache
+
         if 'context' in kwargs and getattr(kwargs['context']['view'], 'nested_field', None) is not None:
             serializer.id = '{}{}/'.format(serializer.id, kwargs['context']['view'].nested_field)
         elif 'context' in kwargs:
             serializer.id = '{}{}'.format(settings.BASE_URL, kwargs['context']['view'].request.path)
         return serializer
 
     def to_internal_value(self, data):
-        is_user_and_external = self.Meta.model is get_user_model() and '@id' in data and not data['@id'].startswith(
-            settings.BASE_URL)
+        is_user_and_external = self.Meta.model is get_user_model() and '@id' in data and Model.is_external(data['@id'])
         if is_user_and_external:
             data['username'] = 'external'
         ret = super().to_internal_value(data)
         if is_user_and_external:
             ret['urlid'] = data['@id']
             ret.pop('username')
         return ret
@@ -691,50 +751,57 @@
         nested_fields = []
         nested_list_fields_name = list(filter(lambda key: isinstance(validated_data[key], list), validated_data))
         for field_name in nested_list_fields_name:
             nested_fields.append((field_name, validated_data.pop(field_name)))
 
         info = model_meta.get_field_info(model)
         many_to_many = []
+        one_to_one = {}
         for field_name, relation_info in info.relations.items():
             if relation_info.to_many and relation_info.reverse and (
                     field_name in validated_data) and not field_name is None:
                 many_to_many.append((field_name, validated_data.pop(field_name)))
+            elif relation_info.reverse and (field_name in validated_data) and not field_name is None:
+                one_to_one[field_name] = validated_data[field_name]
         validated_data = self.remove_empty_value(validated_data)
 
         if model is get_user_model() and not 'username' in validated_data:
             validated_data['username'] = str(uuid.uuid4())
         instance = model.objects.create(**validated_data)
 
         for field_name, value in many_to_many:
             validated_data[field_name] = value
 
+        if one_to_one:
+             for field_name, value in one_to_one.items():
+                 setattr(instance, field_name, value)
+                 value.save()
+
         self.save_or_update_nested_list(instance, nested_fields)
 
         return instance
 
     def remove_empty_value(self, validated_data):
         '''sets any empty strings in the validated_data to None'''
         for attr, value in validated_data.items():
-            if value is '':
+            if value == '':
                 validated_data[attr] = None
         return validated_data
 
     def update(self, instance, validated_data):
         model = self.Meta.model
-
         nested_fields = []
         nested_fields_name = list(filter(lambda key: isinstance(validated_data[key], list), validated_data))
         for field_name in nested_fields_name:
             nested_fields.append((field_name, validated_data.pop(field_name)))
 
         for attr, value in validated_data.items():
             if isinstance(value, dict):
                 value = self.update_dict_value(attr, instance, value)
-            if value is '' and not isinstance(getattr(instance, attr), str):
+            if value == '' and not isinstance(getattr(instance, attr), str):
                 setattr(instance, attr, None)
             else:
                 setattr(instance, attr, value)
 
         self.save_or_update_nested_list(instance, nested_fields)
         instance.save()
```

### Comparing `djangoldp-2.1.9/djangoldp/models.py` & `djangoldp-3.0.5/djangoldp/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import json
 import logging
 import uuid
 import copy
-from urllib.parse import urlparse
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
-from django.core.exceptions import ObjectDoesNotExist, ValidationError
+from django.core.exceptions import ObjectDoesNotExist, ValidationError, FieldDoesNotExist
 from django.db import models
 from django.db.models import BinaryField, DateTimeField
 from django.db.models.base import ModelBase
 from django.db.models.signals import post_save, pre_save, pre_delete, m2m_changed
 from django.dispatch import receiver
-from django.urls import reverse_lazy, get_resolver, NoReverseMatch
+from django.urls import get_resolver
 from urllib import parse
 from django.utils.datastructures import MultiValueDictKeyError
 from django.utils.decorators import classonlymethod
 from rest_framework.utils import model_meta
 
 from djangoldp.fields import LDPUrlField
-from djangoldp.permissions import LDPPermissions, DEFAULT_DJANGOLDP_PERMISSIONS
+from djangoldp.permissions import LDPPermissions, select_container_permissions, DEFAULT_DJANGOLDP_PERMISSIONS
 
 logger = logging.getLogger('djangoldp')
 
 
 class LDPModelManager(models.Manager):
     def local(self):
         '''an alternative to all() which exlcudes external resources'''
@@ -36,17 +35,17 @@
         nested_fields = set()
         # include all many-to-many relations
         for field_name, relation_info in model_meta.get_field_info(self.model).relations.items():
             if relation_info.to_many:
                 if field_name is not None:
                     nested_fields.add(field_name)
         # include all nested fields explicitly included on the model
-        nested_fields.update(set(Model.get_meta(self.model, 'nested_fields', set())))
+        nested_fields.update(set(getattr(self.model._meta, 'nested_fields', set())))
         # exclude anything marked explicitly to be excluded
-        nested_fields = nested_fields.difference(set(Model.get_meta(self.model, 'nested_fields_exclude', set())))
+        nested_fields = nested_fields.difference(set(getattr(self.model._meta, 'nested_fields_exclude', set())))
         return list(nested_fields)
 
     def fields(self):
         return self.nested_fields()
 
 
 class Model(models.Model):
@@ -59,15 +58,15 @@
 
     def __init__(self, *args, **kwargs):
         super(Model, self).__init__(*args, **kwargs)
 
     @classmethod
     def filter_backends(cls):
         '''constructs a list of filter_backends configured on the permissions classes applied to this model'''
-        filtered_classes = [p for p in cls.get_permission_classes(cls, [LDPPermissions]) if
+        filtered_classes = [p for p in getattr(cls._meta, 'permission_classes', [LDPPermissions]) if
                             hasattr(p, 'filter_backends') and p.filter_backends is not None]
         filter_backends = list()
         for p in filtered_classes:
             filter_backends = list(set(filter_backends).union(set(p.filter_backends)))
         return filter_backends
 
     @classmethod
@@ -90,14 +89,19 @@
     def get_view_set(cls):
         '''returns the view_set defined in the model Meta or the LDPViewSet class'''
         view_set = getattr(cls._meta, 'view_set', getattr(cls.Meta, 'view_set', None))
         if view_set is None:
             from djangoldp.views import LDPViewSet
             view_set = LDPViewSet
         return view_set
+    
+    @classmethod
+    def get_serializer_class(cls):
+        from djangoldp.serializers import LDPSerializer
+        return LDPSerializer
 
     @classmethod
     def get_container_path(cls):
         '''returns the url path which is used to access actions on this model (e.g. /users/)'''
         path = getattr(cls._meta, 'container_path', getattr(cls.Meta, 'container_path', None))
         if path is None:
             path = "{}s".format(cls._meta.object_name.lower())
@@ -128,24 +132,32 @@
     def resource_id(cls, instance):
         r_id = "{}{}".format(cls.container_id(instance), getattr(instance, cls.slug_field(instance), ""))
         return cls.__clean_path(r_id)
 
     @classonlymethod
     def slug_field(cls, instance_or_model):
         if isinstance(instance_or_model, ModelBase):
-            object_name = instance_or_model.__name__.lower()
+            model = instance_or_model
         else:
-            object_name = instance_or_model._meta.object_name.lower()
+            model = type(instance_or_model)
+        
+        # Use cached value if present
+        if hasattr(model, "_slug_field"):
+            return model._slug_field
+        object_name = model.__name__.lower()
         view_name = '{}-detail'.format(object_name)
+
         try:
             slug_field = '/{}'.format(get_resolver().reverse_dict[view_name][0][0][1][0])
         except MultiValueDictKeyError:
-            slug_field = Model.get_meta(instance_or_model, 'lookup_field', 'pk')
+            slug_field = getattr(model._meta, 'lookup_field', 'pk')
         if slug_field.startswith('/'):
             slug_field = slug_field[1:]
+        
+        model._slug_field = slug_field
         return slug_field
 
     @classonlymethod
     def container_id(cls, instance):
         if isinstance(instance, cls):
             path = instance.get_container_path()
         else:
@@ -248,104 +260,150 @@
         return Model.get_or_create(model, urlid, **kwargs)
 
     @classonlymethod
     def get_model_rdf_type(cls, model):
         if model is get_user_model():
             return "foaf:user"
         else:
-            return Model.get_meta(model, "rdf_type")
+            return getattr(model._meta, "rdf_type", None)
 
     @classonlymethod
     def get_subclass_with_rdf_type(cls, type):
+        #TODO: deprecate
         '''returns Model subclass with Meta.rdf_type matching parameterised type, or None'''
         if type == 'foaf:user':
             return get_user_model()
 
         for subcls in Model.__subclasses__():
-            if Model.get_meta(subcls, 'rdf_type') == type:
+            if getattr(subcls._meta, "rdf_type", None) == type:
                 return subcls
 
         return None
 
     @classonlymethod
-    def get_permission_classes(cls, related_model, default_permissions_classes):
-        '''returns the permission_classes set in the models Meta class'''
-        return cls.get_meta(related_model, 'permission_classes', default_permissions_classes)
-
-    @classonlymethod
+    #TODO: deprecate
     def get_meta(cls, model_class, meta_name, default=None):
         '''returns the models Meta class'''
         if hasattr(model_class, 'Meta'):
             meta = getattr(model_class.Meta, meta_name, default)
         elif hasattr(model_class, '_meta'):
             meta = default
         else:
             return default
         return getattr(model_class._meta, meta_name, meta)
 
     @classmethod
     def get_model_class(cls):
         return cls
-
+    
     @classonlymethod
-    def get_container_permissions(cls, model_class, request, view, obj=None):
-        '''outputs the permissions given by all permissions_classes on the model_class on the model-level'''
-        perms = set()
-        view = copy.copy(view)
-        view.model = model_class
-        for permission_class in Model.get_permission_classes(model_class, [LDPPermissions]):
-            if hasattr(permission_class, 'get_container_permissions'):
-                perms = perms.union(permission_class().get_container_permissions(request, view, obj))
+    def _get_permissions_setting(cls, model, perm_name, inherit_perms=None):
+        '''Auxiliary function returns the configured permissions given to parameterised setting, or default'''
+        # gets the model-configured setting or default if it exists
+        if not model:
+            model = cls
+        perms = getattr(model._meta, perm_name, None)
+        if perms is None:
+            # If no specific permission is set on the Model, take the ones on all Permission classes
+            perms = []
+            #TODO: there should be a default meta param, instead of passing the default here?
+            for permission_class in getattr(model._meta, 'permission_classes', [LDPPermissions]):
+                perms = perms + getattr(permission_class, perm_name, [])
+
+        if inherit_perms is not None and 'inherit' in perms:
+            perms += set(inherit_perms) - set(perms)
+        
         return perms
+    
+    @classonlymethod
+    def get_permission_settings(cls, model=None):
+        '''returns a tuple of (Auth, Anon, Owner) settings for a given model'''
+        # takes a model so that it can be called on Django native models
+        if not model:
+            model = cls
+        anonymous_perms = cls._get_permissions_setting(model, 'anonymous_perms')
+        authenticated_perms = cls._get_permissions_setting(model, 'authenticated_perms', anonymous_perms)
+        owner_perms = cls._get_permissions_setting(model, 'owner_perms', authenticated_perms)
+        superuser_perms = cls._get_permissions_setting(model, 'superuser_perms', owner_perms)
+
+        return anonymous_perms, authenticated_perms, owner_perms, superuser_perms
+    
+    #TODO review architecture of permissions
+    @classonlymethod
+    def get_container_permissions(cls, model, request, view, obj=None):
+        '''outputs the permissions given by all permissions_classes on the model on the model-level'''
+        anonymous_perms, authenticated_perms, owner_perms, superuser_perms = cls.get_permission_settings(model)
+        return select_container_permissions(request, obj, model, anonymous_perms, authenticated_perms, owner_perms, superuser_perms)
 
     @classonlymethod
-    def get_object_permissions(cls, model_class, request, view, obj):
-        '''outputs the permissions given by all permissions_classes on the model_class on the object-level'''
+    def get_object_permissions(cls, model, request, view, obj):
+        '''outputs the permissions given by all permissions_classes on the model on the object-level'''
         perms = set()
-        for permission_class in Model.get_permission_classes(model_class, [LDPPermissions]):
+        for permission_class in getattr(model._meta, 'permission_classes', [LDPPermissions]):
             if hasattr(permission_class, 'get_object_permissions'):
                 perms = perms.union(permission_class().get_object_permissions(request, view, obj))
         return perms
 
     @classonlymethod
-    def get_permissions(cls, model_class, request, view, obj=None):
-        '''outputs the permissions given by all permissions_classes on the model_class on both the model and the object level'''
-        perms = Model.get_container_permissions(model_class, request, view, obj)
+    def get_permissions(cls, model, request, view, obj=None):
+        '''outputs the permissions given by all permissions_classes on the model on both the model and the object level'''
+        perms = Model.get_container_permissions(model, request, view, obj)
         if obj is not None:
-            perms = perms.union(Model.get_object_permissions(model_class, request, view, obj))
+            perms = perms.union(Model.get_object_permissions(model, request, view, obj))
         return perms
 
     @classmethod
-    def is_owner(cls, model_class, user, obj):
+    def is_owner(cls, model, user, obj):
         '''returns True if I given user is the owner of given object instance, otherwise False'''
-        owner_field = Model.get_meta(model_class, 'owner_field')
+        owner_field = getattr(model._meta, 'owner_field', None)
+        owner_urlid_field = getattr(model._meta, 'owner_urlid_field', None)
 
+        if owner_field is not None and owner_urlid_field is not None:
+            raise AttributeError("you can not set both owner_field and owner_urlid_field")
         if owner_field is None:
-            return False
+            if owner_urlid_field is None:
+                return False
+            else:
+                # use the one that is set, the check with urlid is done at the end
+                owner_field = owner_urlid_field
 
-        return (getattr(obj, owner_field) == user
-                or (hasattr(user, 'urlid') and getattr(obj, owner_field) == user.urlid)
-                or getattr(obj, owner_field) == user.id)
+        try:
+            # owner fields might be nested (e.g. "collection__author")
+            owner_field_nesting = owner_field.split("__")
+            if len(owner_field_nesting) > 1:
+                obj_copy = obj
+
+                for level in owner_field_nesting:
+                    owner_value = getattr(obj_copy, level)
+                    obj_copy = owner_value
+
+            # or they might not be (e.g. "author")
+            else:
+                owner_value = getattr(obj, owner_field)
+        except AttributeError:
+            raise FieldDoesNotExist(f"the owner_field setting {owner_field} contains field(s) which do not exist on model {model.__name__}")
+        
+        return (owner_value == user
+                or (hasattr(user, 'urlid') and owner_value == user.urlid)
+                or owner_value == user.id)
 
     @classmethod
     def is_external(cls, value):
         '''
         :param value: string urlid or an instance with urlid field
         :return: True if the urlid is external to the server, False otherwise
         '''
         try:
+            if not value:
+                return False
             if not isinstance(value, str):
                 value = value.urlid
 
-            if value is not None:
-                value_netloc = parse.urlparse(value).netloc
-
-                return value_netloc is not None and value_netloc != '' and\
-                       value_netloc != parse.urlparse(settings.SITE_URL).netloc
-            return False
+            # This expects all @ids to start with http which mlight not be universal. Maybe needs a fix.
+            return value.startswith('http') and not value.startswith(settings.SITE_URL)
         except:
             return False
 
 
 class LDPSource(Model):
     federation = models.CharField(max_length=255)
 
@@ -423,27 +481,40 @@
 
 
 #if not hasattr(get_user_model(), 'webid'):
 #    def webid(self):
 #        # an external user should have urlid set
 #        webid = getattr(self, 'urlid', None)
 #        if webid is not None and urlparse(settings.BASE_URL).netloc != urlparse(webid).netloc:
-#            webid = self.urlid
+#            webid = self.urlid`
 #        # local user use user-detail URL with primary key
 #        else:
 #            base_url = settings.BASE_URL
 #            if base_url.endswith('/'):
 #                base_url = base_url[:len(base_url) - 1]
 #            webid = '{0}{1}'.format(base_url, reverse_lazy('user-detail', kwargs={'pk': self.pk}))
 #        return webid
 #
 #
 #    get_user_model().webid = webid
 
 
-@receiver([pre_save, pre_delete, m2m_changed])
-def invalidate_caches(instance, **kwargs):
-    from djangoldp.serializers import LDListMixin, LDPSerializer
-    LDListMixin.to_representation_cache.reset()
+def invalidate_cache_if_has_entry(entry):
+    from djangoldp.serializers import GLOBAL_SERIALIZER_CACHE
+
+    if GLOBAL_SERIALIZER_CACHE.has(entry):
+        GLOBAL_SERIALIZER_CACHE.invalidate(entry)
+
+
+def invalidate_model_cache_if_has_entry(model):
+    entry = getattr(model._meta, 'label', None)
+    invalidate_cache_if_has_entry(entry)
+
+
+@receiver([pre_save, pre_delete])
+def invalidate_caches(sender, instance, **kwargs):
+    invalidate_model_cache_if_has_entry(sender)
+
 
-    if hasattr(instance, 'urlid'):
-        LDPSerializer.to_representation_cache.invalidate(instance.urlid)
+@receiver([m2m_changed])
+def invalidate_caches_m2m(sender, instance, action, *args, **kwargs):
+    invalidate_model_cache_if_has_entry(kwargs['model'])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `djangoldp-2.1.9/djangoldp/utils.py` & `djangoldp-3.0.5/djangoldp/utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/conf/server_template/manage.py-tpl` & `djangoldp-3.0.5/djangoldp/conf/server_template/manage.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/conf/server_template/server/wsgi.py-tpl` & `djangoldp-3.0.5/djangoldp/conf/server_template/server/wsgi.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/conf/server_template/server/urls.py-tpl` & `djangoldp-3.0.5/djangoldp/conf/server_template/server/urls.py-tpl`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 Class-based views
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  url(r'^$', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.conf.urls import url, include
     2. Add a URL to urlpatterns:  url(r'^blog/', include('blog.urls'))
 """
-from django.conf.urls import url, include
+from django.urls import include, path
 from django.contrib import admin
 from django.conf import settings
 from django.conf.urls.static import static
 
 urlpatterns = [
-    url(r'^', include('djangoldp.urls')),
-    url(r'^admin/', admin.site.urls),
+    path('', include('djangoldp.urls')),
+    path('admin/', admin.site.urls),
 ]
 
 if settings.DEBUG:
   urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
```

### Comparing `djangoldp-2.1.9/djangoldp/conf/default_settings.py` & `djangoldp-3.0.5/djangoldp/conf/default_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -105,26 +105,48 @@
 # MIDDLEWARE #
 ##############
 
 # List of middleware to use. Order is important; in the request phase, these
 # middleware will be applied in the order given, and in the response
 # phase the middleware will be applied in reverse order.
 MIDDLEWARE = [
-    'django_cookies_samesite.middleware.CookiesSameSite',
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
+    'djangoldp.middleware.AllowRequestedCORSMiddleware',
+    'djangoldp.middleware.PrefetchParentModel',
     'django.middleware.gzip.GZipMiddleware',
     'django_brotli.middleware.BrotliMiddleware'
 ]
 
+##################
+# REST FRAMEWORK #
+##################
+REST_FRAMEWORK = {
+    'DEFAULT_SCHEMA_CLASS': 'drf_spectacular.openapi.AutoSchema',
+    'DEFAULT_PAGINATION_CLASS': 'djangoldp.pagination.LDPPagination'
+}
+
+###################
+# DRF SPECTACULAR #
+###################
+ENABLE_SWAGGER_DOCUMENTATION = False
+SPECTACULAR_SETTINGS = {
+    'TITLE': 'DjangoLDP Based API Description',
+    'DESCRIPTION': 'Here you will find the list of all endpoints available on your Djangoldp-based server instance and\
+         the available methods, needed parameters and requests examples. The list of available endpoints depend on your instance configuration\
+             especially the list of bloxes and associated django models activated.',
+    'VERSION': '2.1.37',
+    'SERVE_INCLUDE_SCHEMA': False
+}
+
 ############
 # SESSIONS #
 ############
 
 # Same site policy
 DCS_SESSION_COOKIE_SAMESITE = 'none'
 
@@ -135,7 +157,11 @@
 AUTHENTICATION_BACKENDS = ['django.contrib.auth.backends.ModelBackend', 'guardian.backends.ObjectPermissionBackend']
 
 OIDC_ACCESS_CONTROL_ALLOW_HEADERS = 'Content-Type, if-match, accept, authorization, DPoP'
 
 # The minimum number of seconds a password reset link is valid for
 PASSWORD_RESET_TIMEOUT = 60 * 60 * 24 * 3
 
+DISABLE_LOCAL_OBJECT_FILTER = False
+
+GUARDIAN_AUTO_PREFETCH = True
+DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
```

### Comparing `djangoldp-2.1.9/djangoldp/conf/ldpsettings.py` & `djangoldp-3.0.5/djangoldp/conf/ldpsettings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import os
 import sys
 import yaml
 import logging
 from django.core.exceptions import ImproperlyConfigured
 from django.conf import settings as django_settings
 from pathlib import Path
+from collections import OrderedDict
 from typing import Iterable
+from importlib import import_module
 from . import default_settings
 
-try:
-    from importlib import import_module
-except ImportError:
-    from django.utils.importlib import import_module
-
 
 logger = logging.getLogger(__name__)
 
 
 def configure(filename='settings.yml'):
     """Helper function to configure django from LDPSettings."""
 
@@ -41,14 +38,15 @@
 
         """Build a Django Setting object from a dict."""
 
         if django_settings.configured:
             raise ImproperlyConfigured('Settings have been configured already')
 
         self._config = config
+        self._explicit_settings = set(default_settings.__dict__.keys()) #default settings are explicit
         self._settings = self.build_settings()
 
     def build_settings(self, extend=['INSTALLED_APPS', 'MIDDLEWARE']):
         """
         Look for the parameters in multiple places.
         Each step overrides the value of the previous key found. Except for "extend" list. Those value must be lists and all values found are added to these lists without managing duplications.
 
@@ -57,32 +55,33 @@
           2. Packages settings
           3. Code from a local settings.py file
           4. YAML config file
         """
 
         # helper loop
         def update_with(config):
-            for k, v in config.items():
-
-                if k in extend:
-                    settings[k].extend(v)
+            for setting, value in config.items():
+                self._explicit_settings.add(setting)
+                if setting in extend:
+                    settings[setting].extend(value)
 
-                elif not k.startswith('_'):
-                    settings.update({k: v})
+                elif not setting.startswith('_'):
+                    settings.update({setting: value})
 
         # start from default core settings
         settings = default_settings.__dict__.copy()
         logger.debug(f'Building settings from core defaults')
 
         # INSTALLED_APPS starts empty
         settings['INSTALLED_APPS'] = []
 
         # look settings from packages in the order they are given (local overrides installed)
         for pkg in self.DJANGOLDP_PACKAGES:
 
+            # FIXME: There is something better to do here with the sys.modules path
             try:
                 # override with values from installed package
                 mod = import_module(f'{pkg}.djangoldp_settings')
                 update_with(mod.__dict__)
                 logger.debug(f'Updating settings from installed package {pkg}')
             except ModuleNotFoundError:
                 pass
@@ -131,20 +130,23 @@
 
         # get ldp packages (they are django apps)
         apps = self.DJANGOLDP_PACKAGES.copy()
 
         # add the default apps
         apps.extend(self._settings['INSTALLED_APPS'])
 
-        return apps
+        # As settings come from different origins duplicuation is likeliy to happen
+        return list(OrderedDict.fromkeys(apps))
 
     def __getattr__(self, param):
         """Return the requested parameter from cached settings."""
         if param.startswith('_') or param.islower():
             # raise the django exception for inexistent parameter
             raise AttributeError(f'"{param}" is not compliant to django settings format')
         try:
             return self._settings[param]
         except KeyError:
             # raise the django exception for inexistent parameter
             raise AttributeError(f'no "{param}" parameter found in settings')
 
+    def is_overridden(self, setting):
+        return setting in self._explicit_settings
```

### Comparing `djangoldp-2.1.9/djangoldp/activities/objects.py` & `djangoldp-3.0.5/djangoldp/activities/objects.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/activities/services.py` & `djangoldp-3.0.5/djangoldp/activities/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import threading
 import json
 import time
+import copy
 import requests
 from queue import Queue
 from requests.exceptions import Timeout, ConnectionError
 from urllib.parse import urlparse
 from django.contrib.auth import get_user_model
 from django.db.models.signals import post_save, post_delete, m2m_changed
 from django.dispatch import receiver, Signal
@@ -27,19 +28,98 @@
     'apscheduler.timezone': getattr(settings, 'TIME_ZONE', 'UTC'),
 }
 
 MAX_ACTIVITY_RESCHEDULES = getattr(settings, 'MAX_ACTIVITY_RESCHEDULES', 3)
 DEFAULT_BACKOFF_FACTOR = getattr(settings, 'DEFAULT_BACKOFF_FACTOR', 1)
 DEFAULT_ACTIVITY_DELAY = getattr(settings, 'DEFAULT_ACTIVITY_DELAY', 0.1)
 DEFAULT_REQUEST_TIMEOUT = getattr(settings, 'DEFAULT_REQUEST_TIMEOUT', 10)
+MAX_RECORDS_ACTIVITY_CACHE = getattr(settings, 'MAX_RECORDS_ACTIVITY_CACHE', 10000)
 
 
 activity_sending_finished = Signal()
 
 
+class ActivityInMemoryCache:
+    '''
+    {
+        'urlid': {
+            # if an object is sent without a urlid it is not cached
+            'object_urlid': {
+                # for create/update, just interested in the most recent activity on this external id
+                './': ACTIVITY
+
+                # for add/remove, we're interested also in the target (container_id)
+                'circles': ACTIVITY
+                'circle-members': ACTIVITY
+            }
+        }
+    }
+    '''
+
+    def __init__(self):
+        self.cache = {
+        }
+
+    def reset(self):
+        self.cache = {
+        }
+
+    def has(self, urlid, object_id, target_id=None):
+        if urlid not in self.cache or object_id not in self.cache[urlid]:
+            return False
+    
+        if target_id is None:
+            target_id = './'
+        
+        return target_id in self.cache[urlid][object_id]
+
+    def get(self, urlid, object_id, target_id=None):
+        if target_id is None:
+            target_id = './'
+
+        if self.has(urlid, object_id, target_id):
+            return self.cache[urlid][object_id][target_id]
+        else:
+            return None
+
+    def set(self, urlid, object_id, target_id=None, value=None):
+        if MAX_RECORDS_ACTIVITY_CACHE == 0:
+            return
+
+        if len(self.cache.keys()) > MAX_RECORDS_ACTIVITY_CACHE:
+            self.reset()
+
+        if target_id is None:
+            target_id = './'
+
+        if urlid not in self.cache:
+            self.cache[urlid] = {}
+        
+        if object_id not in self.cache[urlid]:
+            self.cache[urlid][object_id] = {}
+        
+        self.cache[urlid][object_id][target_id] = copy.deepcopy(value)
+
+    def invalidate(self, urlid, object_id=None, target_id=None):
+        # can clear the cache for an entire record or at any level in the cache
+        if object_id is not None:
+            if target_id is not None:
+                self.cache[urlid][object_id].pop(target_id, None)
+            else:
+                self.cache[urlid].pop(object_id, None)
+        else:
+            self.cache.pop(urlid, None)
+
+
+# used to minimise the activity traffic to necessary activities,
+# preferred over a database solution which is slower
+ACTIVITY_CACHE = ActivityInMemoryCache()
+ACTIVITY_SAVING_SETTING = getattr(settings, 'STORE_ACTIVITIES', 'ERROR')
+
+
 class ActivityQueueService:
     '''Manages an asynchronous queue for Activity format messages'''
     initialized = False
     queue = None
 
     @classmethod
     def revive_activities(cls):
@@ -91,31 +171,52 @@
         logger.debug('[Sender] sending Activity... ' + str(activity))
 
         if getattr(settings, 'DISABLE_OUTBOX', False) == 'DEBUG':
             return {'data': {}}
         return requests.post(url, data=json.dumps(activity), headers=headers, timeout=timeout)
 
     @classmethod
+    def _get_str_urlid(cls, obj):
+        if obj is None:
+            return None
+
+        return obj if isinstance(obj, str) else obj['@id'] if '@id' in obj else None
+
+    @classmethod
     def _save_activity_from_response(cls, response, url, scheduled_activity):
         '''
         wrapper to save a finished Activity based on the parameterised response
         :return: saved Activity object
         '''
         response_body = None
 
         if hasattr(response, 'text'):
             response_body = response.text
         response_location = getattr(response, "Location", None)
-        status_code = getattr(response, "status_code", None)
-        success = str(status_code).startswith("2")
-
-        return cls._save_sent_activity(scheduled_activity.to_activitystream(), ActivityModel, success=success,
-                                       external_id=url, type=scheduled_activity.type,
-                                       response_location=response_location, response_code=str(status_code),
-                                       response_body=response_body)
+        status_code = getattr(response, "status_code", response['status_code'] if 'status_code' in response else None)
+        success = str(status_code).startswith("2") if status_code is not None else False
+        
+        # strip some key info from the activity (standardise the datatype)
+        activity_json = scheduled_activity.to_activitystream() if isinstance(scheduled_activity, ScheduledActivity) else scheduled_activity
+        activity_type = scheduled_activity.type if hasattr(scheduled_activity, 'type') else scheduled_activity['type']
+
+        # set the activity cache
+        if 'object' in activity_json:
+            object_id = cls._get_str_urlid(activity_json['object'])
+            
+            if object_id is not None:
+                target_origin = cls._get_str_urlid(activity_json.get('target', activity_json.get('origin', None)))
+                ACTIVITY_CACHE.set(url, object_id, target_origin, activity_json)
+
+        # save the activity if instructed to do so
+        if ACTIVITY_SAVING_SETTING == 'VERBOSE' or (not success and ACTIVITY_SAVING_SETTING == 'ERROR'):
+            return cls._save_sent_activity(activity_json, ActivityModel, success=success,
+                                           external_id=url, type=activity_type,
+                                           response_location=response_location, response_code=str(status_code),
+                                           response_body=response_body)
 
     @classmethod
     def _attempt_failed_reschedule(cls, url, scheduled_activity, backoff_factor):
         '''
         either re-schedules a failed activity or saves its failure state, depending on the number of fails and the
         fail policy (MAX_ACTIVITY_RESCHEDULES)
         :return: True if it was able to reschedule
@@ -173,15 +274,15 @@
         '''
 
         def get_related_activities(type):
             '''returns a list of activity types which should be considered a "match" with the parameterised type'''
             if type is None:
                 return []
             type = type.lower()
-            group_a = ['create', 'update', 'delete']
+            group_a = ['create', 'update', 'delete', 'creation', 'deletion']
             groub_b = ['add', 'remove']
 
             if type in group_a:
                 return group_a
             if type in groub_b:
                 return groub_b
             return []
@@ -235,69 +336,56 @@
             else:
                 return obj
 
         def no_new_changes(old_activity, new_activity):
             '''returns False if the two activities are equivalent'''
             return ordered(old_activity['object']) == ordered(new_activity['object'])
 
-        def get_most_recent_sent_activity(external_id):
-            '''returns the most recently sent activity which meets the specification'''
-            activities = ActivityModel.objects.filter(external_id=external_id, is_finished=True,
-                                                      type__in=['create', 'update']).order_by('-created_at')[:10]
-            for a in activities.all():
-                a = a.to_activitystream()
-                if 'object' in a:
-                    return a
-            return None
+        def get_most_recent_sent_activity(external_id, object_id):
+            return ACTIVITY_CACHE.get(external_id, object_id)
 
         # str objects will have to be checked manually by the receiver
         new_activity = scheduled_activity.to_activitystream()
-        if 'object' not in new_activity or isinstance(new_activity['object'], str):
+        if 'object' not in new_activity or isinstance(new_activity['object'], str) or \
+             '@id' not in new_activity['object']:
+        
             return True
 
-        old_activity = get_most_recent_sent_activity(url)
+        old_activity = get_most_recent_sent_activity(url, new_activity['object']['@id'])
 
         if old_activity is None:
             return True
 
         if no_new_changes(old_activity, new_activity):
             return False
         return True
 
     @classmethod
     def _add_remove_is_new(cls, url, scheduled_activity):
         '''auxiliary function validates if the receiver does not know about this Add/Remove activity'''
         def get_most_recent_sent_activity(source_obj, source_target_origin):
-            # get a list of activities with the right type
-            activities = ActivityModel.objects.filter(external_id=url, is_finished=True,
-                                                      type__in=['add', 'remove']).order_by('-created_at')[:10]
-
-            # we are searching for the most recent Add/Remove activity which shares inbox, object and target/origin
-            for a in activities.all():
-                astream = a.to_activitystream()
-                obj = astream.get('object', None)
-                target_origin = astream.get('target', astream.get('origin', None))
-                if obj is None or target_origin is None:
-                    continue
+            obj_id = cls._get_str_urlid(source_obj)
+            target_id = cls._get_str_urlid(source_target_origin)
 
-                if source_obj == obj and source_target_origin == target_origin:
-                    return a
-            return None
+            return ACTIVITY_CACHE.get(url, obj_id, target_id)
 
         new_activity = scheduled_activity.to_activitystream()
         new_obj = new_activity.get('object', None)
         new_target_origin = new_activity.get('target', new_activity.get('origin', None))
 
         # bounds checking
-        if new_obj is None or new_target_origin is None:
+        if new_obj is None or new_target_origin is None or \
+            (not isinstance(new_obj, str) and '@id' not in new_obj) or \
+            (not isinstance(new_target_origin, str) and '@id' not in new_target_origin):
             return True
 
         #  if most recent is the same type of activity as me, it's not new
         old_activity = get_most_recent_sent_activity(new_obj, new_target_origin)
-        if old_activity is not None and old_activity.type == scheduled_activity.type:
+
+        if old_activity is not None and old_activity['type'].lower() == scheduled_activity.type.lower():
             return False
         return True
 
     @classmethod
     def _push_to_queue(cls, url, scheduled_activity, delay=DEFAULT_ACTIVITY_DELAY):
         '''wrapper to check for singleton initialization before pushing'''
         if not cls.initialized:
```

### Comparing `djangoldp-2.1.9/djangoldp/activities/verbs.py` & `djangoldp-3.0.5/djangoldp/activities/verbs.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/permissions.py` & `djangoldp-3.0.5/djangoldp/permissions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from django.conf import settings
-from django.contrib.auth.models import _user_get_all_permissions
 from django.contrib.auth import _get_backends
 from rest_framework.permissions import DjangoObjectPermissions
 from djangoldp.utils import is_anonymous_user
 from djangoldp.filters import LDPPermissionsFilterBackend
 
 
 DEFAULT_DJANGOLDP_PERMISSIONS = ['add', 'change', 'delete', 'view', 'control']
@@ -72,75 +71,58 @@
     def compare_permissions(self, required_perms, user_perms):
         '''returns True if all user_perms are in required_perms'''
         for perm in required_perms:
             if not perm.split('.')[-1].split('_')[0] in user_perms:
                 return False
         return True
 
+def select_container_permissions(request, obj, model, anonymous_perms, authenticated_perms, owner_perms, superuser_perms):
+    from djangoldp.models import Model
+    
+    if is_anonymous_user(request.user):
+        return set(anonymous_perms)
+    else:
+        if obj is not None and Model.is_owner(model, request.user, obj):
+            perms = set(owner_perms)
+        else:
+            perms = set(authenticated_perms)
+        if request.user.is_superuser:
+            perms = perms.union(set(superuser_perms))
+    return perms
 
 class ModelConfiguredPermissions(LDPBasePermission):
     # *DEFAULT* model-level permissions for anon, auth and owner statuses
     anonymous_perms = ['view']
     authenticated_perms = ['inherit']
     owner_perms = ['inherit']
     # superuser has all permissions by default
     superuser_perms = getattr(settings, 'DEFAULT_SUPERUSER_PERMS', DEFAULT_DJANGOLDP_PERMISSIONS)
 
-    def _get_permissions_setting(self, model, setting, parent_perms=None):
-        '''Auxiliary function returns the configured permissions given to parameterised setting, or default'''
-        from djangoldp.models import Model
-
-        # gets the model-configured setting or default if it exists
-        return_perms = Model.get_meta(model, setting, getattr(self, setting))
-
-        if parent_perms is not None and 'inherit' in return_perms:
-            return_perms = return_perms + list(set(parent_perms) - set(return_perms))
-
-        return return_perms
-
-    def get_permission_settings(self, model):
-        '''returns a tuple of (Auth, Anon, Owner) settings for a given model'''
-        anonymous_perms = self._get_permissions_setting(model, 'anonymous_perms')
-        authenticated_perms = self._get_permissions_setting(model, 'authenticated_perms', anonymous_perms)
-        owner_perms = self._get_permissions_setting(model, 'owner_perms', authenticated_perms)
-        superuser_perms = self._get_permissions_setting(model, 'superuser_perms', owner_perms)
-
-        return anonymous_perms, authenticated_perms, owner_perms, superuser_perms
-
     def get_container_permissions(self, request, view, obj=None):
         '''analyses the Model's set anonymous, authenticated and owner_permissions and returns these'''
+        perms = super().get_container_permissions(request, view, obj=obj)
         from djangoldp.models import Model
-
-        model = view.model
-        anonymous_perms, authenticated_perms, owner_perms, superuser_perms = self.get_permission_settings(model)
-
-        perms = super().get_container_permissions(request, view, obj)
-        if is_anonymous_user(request.user):
-            perms = perms.union(set(anonymous_perms))
+        if isinstance(view.model, Model):
+            anonymous_perms, authenticated_perms, owner_perms, superuser_perms = view.model.get_permission_settings()
         else:
-            if obj is not None and Model.is_owner(view.model, request.user, obj):
-                perms = perms.union(set(owner_perms))
-            else:
-                perms = perms.union(set(authenticated_perms))
-
-            if request.user.is_superuser:
-                perms = perms.union(set(superuser_perms))
-        return perms
+            anonymous_perms, authenticated_perms, owner_perms, superuser_perms = Model.get_permission_settings(view.model)
+        return select_container_permissions(request, obj, view.model, anonymous_perms, authenticated_perms, owner_perms, superuser_perms)
 
     def has_permission(self, request, view):
         """concerned with the permissions to access the _view_"""
         if is_anonymous_user(request.user):
             if not self.has_container_permission(request, view):
                 return False
         return True
 
 
 class LDPObjectLevelPermissions(LDPBasePermission):
     def get_all_user_object_permissions(self, user, obj):
-        return _user_get_all_permissions(user, obj)
+        return user.get_all_permissions(obj)
+
 
     def get_object_permissions(self, request, view, obj):
         '''overridden to append permissions from all backends given to the user (e.g. Groups and object-level perms)'''
         from djangoldp.models import Model
 
         model_name = Model.get_meta(view.model, 'model_name')
```

### Comparing `djangoldp-2.1.9/djangoldp/endpoints/webfinger.py` & `djangoldp-3.0.5/djangoldp/endpoints/webfinger.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/views.py` & `djangoldp-3.0.5/djangoldp/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import validators
 from collections import OrderedDict
 from django.apps import apps
 from django.conf import settings
-from django.conf.urls import include, re_path
 from django.contrib.auth import get_user_model
 from django.core.exceptions import FieldDoesNotExist, ObjectDoesNotExist
 from django.db import IntegrityError, transaction
 from django.http import JsonResponse, Http404
 from django.shortcuts import get_object_or_404
+from django.urls import include, re_path, path
 from django.urls.resolvers import get_resolver
 from django.utils.decorators import classonlymethod
 from django.views import View
 from pyld import jsonld
 from rest_framework import status
 from rest_framework.authentication import SessionAuthentication
 from rest_framework.exceptions import ParseError
@@ -23,19 +23,18 @@
 from rest_framework.utils import model_meta
 from rest_framework.views import APIView
 from rest_framework.viewsets import ModelViewSet
 
 from djangoldp.endpoints.webfinger import WebFingerEndpoint, WebFingerError
 from djangoldp.models import LDPSource, Model, Follower
 from djangoldp.permissions import LDPPermissions
-from djangoldp.filters import LocalObjectOnContainerPathBackend
+from djangoldp.filters import LocalObjectOnContainerPathBackend, SearchByQueryParamFilterBackend
 from djangoldp.related import get_prefetch_fields
 from djangoldp.utils import is_authenticated_user
-from djangoldp.activities import ActivityQueueService, as_activitystream
-from djangoldp.activities import ActivityPubService
+from djangoldp.activities import ActivityQueueService, as_activitystream, ACTIVITY_SAVING_SETTING, ActivityPubService
 from djangoldp.activities.errors import ActivityStreamDecodeError, ActivityStreamValidationError
 import logging
 
 logger = logging.getLogger('djangoldp')
 get_user_model()._meta.rdf_context = {"get_full_name": "rdfs:label"}
 
 
@@ -87,14 +86,15 @@
         data_ordered = reorder_data(data)
 
         return super(JSONLDRenderer, self).render(data, accepted_media_type, renderer_context)
 
 
 # https://github.com/digitalbazaar/pyld
 class JSONLDParser(JSONParser):
+    #TODO: It current only works with pyld 1.0. We need to check our support of JSON-LD
     media_type = 'application/ld+json'
 
     def parse(self, stream, media_type=None, parser_context=None):
         data = super(JSONLDParser, self).parse(stream, media_type, parser_context)
         # compact applies the context to the data and makes it a format which is easier to work with
         # see: http://json-ld.org/spec/latest/json-ld/#compacted-document-form
         try:
@@ -134,19 +134,23 @@
         except IntegrityError:
             return Response({'Unable to save due to an IntegrityError in the receiver model'},
                             status=status.HTTP_200_OK)
         except ValueError as e:
             return Response(str(e), status=status.HTTP_400_BAD_REQUEST)
 
         # save the activity and return 201
-        obj = ActivityQueueService._save_sent_activity(activity.to_json(), local_id=request.path_info, success=True,
-                                                       type=activity.type)
+        if ACTIVITY_SAVING_SETTING == 'VERBOSE':
+            obj = ActivityQueueService._save_sent_activity(activity.to_json(), local_id=request.path_info, success=True,
+                                                           type=activity.type)
 
-        response = Response({}, status=status.HTTP_201_CREATED)
-        response['Location'] = obj.urlid
+            response = Response({}, status=status.HTTP_201_CREATED)
+            response['Location'] = obj.urlid
+        
+        else:
+            response = Response({}, status=status.HTTP_200_OK)
 
         return response
 
     def _handle_activity(self, activity, **kwargs):
         if activity.type == 'Add':
             self.handle_add_activity(activity, **kwargs)
         elif activity.type == 'Remove':
@@ -218,15 +222,15 @@
                     if not Model.is_external(urlid):
                         ActivityPubService.save_follower_for_target(external.urlid, urlid)
 
             return external
 
         # this will be raised when the object was local, but it didn't exist
         except ObjectDoesNotExist:
-            raise Http404()
+            raise Http404(Model.get_meta(object_model, 'label', 'Unknown Model') + ' ' + str(obj['@id']) + ' does not exist')
 
     # TODO: a fallback here? Saving the backlink as Object or similar
     def _get_subclass_with_rdf_type_or_404(self, rdf_type):
         model = Model.get_subclass_with_rdf_type(rdf_type)
         if model is None:
             raise Http404('unable to store type ' + rdf_type + ', model not found')
         return model
@@ -267,15 +271,15 @@
         origin_model = self._get_subclass_with_rdf_type_or_404(activity.origin['@type'])
 
         # get the model reference to saved object
         try:
             origin = origin_model.objects.get(urlid=activity.origin['@id'])
             object_instance = object_model.objects.get(urlid=activity.object['@id'])
         except origin_model.DoesNotExist:
-            raise Http404()
+            raise Http404(activity.origin['@id'] + ' did not exist')
         except object_model.DoesNotExist:
             return
 
         # remove object from origin
         origin_info = model_meta.get_field_info(origin_model)
 
         for field_name, relation_info in origin_info.relations.items():
@@ -321,17 +325,17 @@
         '''
         object_model = self._get_subclass_with_rdf_type_or_404(activity.object['@type'])
 
         # get the model reference to saved object
         try:
             object_instance = object_model.objects.get(urlid=activity.object['@id'])
         except object_model.DoesNotExist:
-            raise Http404()
+            raise Http404(activity.object['@id'] + ' did not exist')
         if Model.is_external(object_instance):
-            raise Http404()
+            raise Http404(activity.object['@id'] + ' is not local to this server')
 
         # get the inbox field from the actor
         if isinstance(activity.actor, str):
             inbox = activity.actor
         else:
             inbox = getattr(activity.actor, 'inbox', None)
             if inbox is None:
@@ -390,15 +394,15 @@
         kwargs['model'] = cls.get_model(**kwargs)
         model_name = kwargs['model']._meta.object_name.lower()
         if kwargs.get('model_prefix'):
             model_name = '{}-{}'.format(kwargs['model_prefix'], model_name)
         detail_expr = cls.get_detail_expr(**kwargs)
 
         urls = [
-            re_path('^$', cls.as_view(cls.list_actions, **kwargs), name='{}-list'.format(model_name)),
+            path('', cls.as_view(cls.list_actions, **kwargs), name='{}-list'.format(model_name)),
             re_path('^' + detail_expr + '$', cls.as_view(cls.detail_actions, **kwargs),
                     name='{}-detail'.format(model_name)),
         ]
 
         # append nested fields to the urls list
         for field in kwargs.get('nested_fields') or cls.nested_fields:
             # the nested property may have a custom viewset defined
@@ -443,68 +447,87 @@
 class LDPViewSet(LDPViewSetGenerator):
     """An automatically generated viewset that serves models following the Linked Data Platform convention"""
     fields = None
     exclude = None
     renderer_classes = (JSONLDRenderer,)
     parser_classes = (JSONLDParser,)
     authentication_classes = (NoCSRFAuthentication,)
-    filter_backends = [LocalObjectOnContainerPathBackend]
+
+    filter_backends = [SearchByQueryParamFilterBackend, LocalObjectOnContainerPathBackend]
     prefetch_fields = None
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         # attach filter backends based on permissions classes, to reduce the queryset based on these permissions
         # https://www.django-rest-framework.org/api-guide/filtering/#generic-filtering
         if self.permission_classes:
             filtered_classes = [p for p in self.permission_classes if hasattr(p, 'filter_backends') and p.filter_backends is not None]
             for p in filtered_classes:
                 self.filter_backends = list(set(self.filter_backends).union(set(p.filter_backends)))
 
+        # Workaround: Push the costly filter activation as a setting
+        if getattr(settings, "DISABLE_LOCAL_OBJECT_FILTER", False):
+            if(LocalObjectOnContainerPathBackend in self.filter_backends):
+                self.filter_backends.remove(LocalObjectOnContainerPathBackend)
+
         self.serializer_class = self.build_read_serializer()
         self.write_serializer_class = self.build_write_serializer()
 
     def build_read_serializer(self):
         model_name = self.model._meta.object_name.lower()
-        lookup_field = get_resolver().reverse_dict[model_name + '-detail'][0][0][1][0]
+        try:
+            lookup_field = get_resolver().reverse_dict[model_name + '-detail'][0][0][1][0]
+        except:
+            lookup_field = 'urlid'
+            pass
+        
         meta_args = {'model': self.model, 'extra_kwargs': {
             '@id': {'lookup_field': lookup_field}},
                      'depth': getattr(self, 'depth', Model.get_meta(self.model, 'depth', 0)),
                      # 'depth': getattr(self, 'depth', 4),
                      'extra_fields': self.nested_fields}
+
         if self.fields:
             meta_args['fields'] = self.fields
         else:
             meta_args['exclude'] = Model.get_meta(self.model, 'serializer_fields_exclude') or ()
-        
+
         return self.build_serializer(meta_args, 'Read')
 
     def build_write_serializer(self):
         model_name = self.model._meta.object_name.lower()
-        lookup_field = get_resolver().reverse_dict[model_name + '-detail'][0][0][1][0]
+
+        try:
+            lookup_field = get_resolver().reverse_dict[model_name + '-detail'][0][0][1][0]
+        except:
+            lookup_field = 'urlid'
+            pass
+        
         meta_args = {'model': self.model, 'extra_kwargs': {
             '@id': {'lookup_field': lookup_field}},
                      'depth': 10,
                      'extra_fields': self.nested_fields}
+
         if self.fields:
             meta_args['fields'] = self.fields
         else:
             meta_args['exclude'] = self.exclude or Model.get_meta(self.model, 'serializer_fields_exclude') or ()
 
         return self.build_serializer(meta_args, 'Write')
 
     def build_serializer(self, meta_args, name_prefix):
         # create the Meta class to associate to LDPSerializer, using meta_args param
         meta_class = type('Meta', (), meta_args)
 
         from djangoldp.serializers import LDPSerializer
 
         if self.serializer_class is None:
-            self.serializer_class = LDPSerializer
+            self.serializer_class = self.model.get_serializer_class() if issubclass(self.model, Model) else LDPSerializer
 
-        return type(LDPSerializer)(self.model._meta.object_name.lower() + name_prefix + 'Serializer',
+        return type(self.serializer_class)(self.model._meta.object_name.lower() + name_prefix + 'Serializer',
                                    (self.serializer_class,),
                                    {'Meta': meta_class})
 
     def is_safe_create(self, user, validated_data, *args, **kwargs):
         '''
         A function which is checked before the create operation to confirm the validated data is safe to add
         returns True by default
@@ -585,42 +608,39 @@
         if hasattr(self.model._meta, 'auto_author') and isinstance(self.request.user, get_user_model()):
             # auto_author_field may be set (a field on user which should be made author - e.g. profile)
             auto_author_field = getattr(self.model._meta, 'auto_author_field', None)
             if auto_author_field is not None:
                 kwargs[self.model._meta.auto_author] = getattr(self.request.user, auto_author_field, None)
             else:
                 kwargs[self.model._meta.auto_author] = get_user_model().objects.get(pk=self.request.user.pk)
-        serializer.save(**kwargs)
+        return serializer.save(**kwargs)
+
+    def perform_update(self, serializer):
+        return serializer.save()
 
     def get_queryset(self, *args, **kwargs):
         if self.model:
             queryset = self.model.objects.all()
         else:
             queryset = super(LDPViewSet, self).get_queryset(*args, **kwargs)
         if self.prefetch_fields is None:
             depth = getattr(self, 'depth', Model.get_meta(self.model, 'depth', 0))
             self.prefetch_fields = get_prefetch_fields(self.model, self.get_serializer(), depth)
         return queryset.prefetch_related(*self.prefetch_fields)
 
     def dispatch(self, request, *args, **kwargs):
         '''overriden dispatch method to append some custom headers'''
         response = super(LDPViewSet, self).dispatch(request, *args, **kwargs)
-        response["Access-Control-Allow-Origin"] = request.META.get('HTTP_ORIGIN')
-        response["Access-Control-Allow-Methods"] = "GET,POST,PUT,PATCH,DELETE"
-        response["Access-Control-Allow-Headers"] = \
-            getattr(settings, 'OIDC_ACCESS_CONTROL_ALLOW_HEADERS',
-                    "authorization, Content-Type, if-match, accept, DPoP")
-        response["Access-Control-Expose-Headers"] = "Location, User"
-        response["Access-Control-Allow-Credentials"] = 'true'
         response["Accept-Post"] = "application/ld+json"
+
         if response.status_code in [201, 200] and '@id' in response.data:
             response["Location"] = str(response.data['@id'])
         else:
             pass
-        response["Accept-Post"] = "application/ld+json"
+
         if is_authenticated_user(request.user):
             try:
                 response['User'] = request.user.webid()
             except AttributeError:
                 pass
         return response
 
@@ -646,14 +666,35 @@
     def get_queryset(self, *args, **kwargs):
         if self.related_field.many_to_many or self.related_field.one_to_many:
             return getattr(self.get_parent(), self.nested_field).all()
         if self.related_field.many_to_one or self.related_field.one_to_one:
             return [getattr(self.get_parent(), self.nested_field)]
 
 
+class LDPAPIView(APIView):
+    '''extends rest framework APIView to support Solid standards'''
+    authentication_classes = (NoCSRFAuthentication,)
+
+    def dispatch(self, request, *args, **kwargs):
+        '''overriden dispatch method to append some custom headers'''
+        response = super().dispatch(request, *args, **kwargs)
+        
+        if response.status_code in [201, 200] and isinstance(response.data, dict) and '@id' in response.data:
+            response["Location"] = str(response.data['@id'])
+        else:
+            pass
+
+        if is_authenticated_user(request.user):
+            try:
+                response['User'] = request.user.webid()
+            except AttributeError:
+                pass
+        return response
+
+
 class LDPSourceViewSet(LDPViewSet):
     model = LDPSource
     federation = None
     filter_backends = []
 
     def get_queryset(self, *args, **kwargs):
         return super().get_queryset(*args, **kwargs).filter(federation=self.kwargs['federation'])
```

### Comparing `djangoldp-2.1.9/djangoldp/related.py` & `djangoldp-3.0.5/djangoldp/related.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/check_integrity.py` & `djangoldp-3.0.5/djangoldp/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/admin.py` & `djangoldp-3.0.5/djangoldp/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.contrib import admin
 from guardian.admin import GuardedModelAdmin
 from django.contrib.auth.admin import UserAdmin
 from djangoldp.models import Activity, ScheduledActivity, Follower
+from djangoldp.activities.services import ActivityQueueService
 
 
 class DjangoLDPAdmin(GuardedModelAdmin):
     '''
     An admin model representing a federated object. Inherits from GuardedModelAdmin to provide Django-Guardian
     object-level permissions
     '''
@@ -13,14 +14,15 @@
 
 
 class DjangoLDPUserAdmin(UserAdmin, GuardedModelAdmin):
     '''An extension of UserAdmin providing the functionality of DjangoLDPAdmin'''
 
     list_display = ('urlid', 'email', 'first_name', 'last_name', 'date_joined', 'last_login', 'is_staff')
     search_fields = ['urlid', 'email', 'first_name', 'last_name']
+    ordering = ['urlid']
 
     def get_fieldsets(self, request, obj=None):
         fieldsets = super().get_fieldsets(request, obj)
         
         federated_fields = ['urlid', 'allow_create_backlink']
         if self.exclude is not None:
             federated_fields = list(set(federated_fields) - set(self.exclude))
@@ -32,30 +34,37 @@
             return fieldsets
 
         fieldsets = [('Federation', {'fields': federated_fields})] + list(fieldsets)
 
         return fieldsets
 
 
+@admin.action(description='Resend activity')
+def resend_activity(modeladmin, request, queryset):
+    for a in queryset:
+        ActivityQueueService.send_activity(a.external_id, a.to_activitystream())
+resend_activity.short_description = 'Resend activity'
+
+
+@admin.register(Activity, ScheduledActivity)
 class ActivityAdmin(DjangoLDPAdmin):
     fields = ['urlid', 'type', 'local_id', 'external_id', 'created_at', 'success', 'payload_view', 'response_code',
               'response_location', 'response_body_view']
     list_display = ['created_at', 'type', 'local_id', 'external_id', 'success', 'response_code']
     readonly_fields = ['created_at', 'payload_view', 'response_location', 'response_code', 'response_body_view']
     search_fields = ['urlid', 'type', 'local_id', 'external_id', 'response_code']
+    actions = [resend_activity]
 
     def payload_view(self, obj):
         return str(obj.to_activitystream())
 
     def response_body_view(self, obj):
         return str(obj.response_to_json())
 
 
+@admin.register(Follower)
 class FollowerAdmin(DjangoLDPAdmin):
     fields = ['urlid', 'object', 'inbox', 'follower']
     list_display = ['urlid', 'object', 'inbox', 'follower']
     search_fields = ['object', 'inbox', 'follower']
 
 
-admin.site.register(Activity, ActivityAdmin)
-admin.site.register(ScheduledActivity, ActivityAdmin)
-admin.site.register(Follower, FollowerAdmin)
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_sources.py` & `djangoldp-3.0.5/djangoldp/tests/tests_sources.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/tests/models.py` & `djangoldp-3.0.5/djangoldp/tests/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from djangoldp.models import Model
 from djangoldp.permissions import LDPPermissions, SuperUserPermission
 
 
 class User(AbstractUser, Model):
 
     class Meta(AbstractUser.Meta, Model.Meta):
+        ordering = ['pk']
         serializer_fields = ['@id', 'username', 'first_name', 'last_name', 'email', 'userprofile',
                              'conversation_set', 'circle_set', 'projects']
         anonymous_perms = ['view', 'add']
         authenticated_perms = ['inherit', 'change']
         owner_perms = ['inherit']
         rdf_type = 'foaf:user'
 
@@ -24,14 +25,15 @@
     slug = models.SlugField(blank=True, null=True, unique=True)
     date = models.DateTimeField(auto_now_add=True, blank=True)
 
     def recent_jobs(self):
         return self.joboffer_set.filter(date__gte=date.today())
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'add', 'change']
         owner_perms = ['inherit', 'delete', 'control']
         serializer_fields = ["@id", "title", "recent_jobs", "slug", "obligatoire"]
         lookup_field = 'slug'
         rdf_type = 'hd:skill'
 
@@ -45,14 +47,15 @@
     def recent_skills(self):
         return self.skills.filter(date__gte=date.today())
 
     def some_skill(self):
         return self.skills.all().first()
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'change', 'add']
         owner_perms = ['inherit', 'delete', 'control']
         serializer_fields = ["@id", "title", "skills", "recent_skills", "resources", "slug", "some_skill", "urlid"]
         container_path = "job-offers/"
         lookup_field = 'slug'
         rdf_type = 'hd:joboffer'
@@ -62,25 +65,27 @@
     description = models.CharField(max_length=255, blank=True, null=True)
     author_user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.DO_NOTHING)
     peer_user = models.ForeignKey(settings.AUTH_USER_MODEL, blank=True, null=True, related_name="peers_conv",
                                   on_delete=models.DO_NOTHING)
     observers = models.ManyToManyField(settings.AUTH_USER_MODEL, blank=True, related_name='observed_conversations')
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'add']
         owner_perms = ['inherit', 'change', 'delete', 'control']
         owner_field = 'author_user'
 
 
 class Resource(Model):
     joboffers = models.ManyToManyField(JobOffer, blank=True, related_name='resources')
     description = models.CharField(max_length=255)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view', 'add', 'delete', 'change', 'control']
         authenticated_perms = ['inherit']
         owner_perms = ['inherit']
         serializer_fields = ["@id", "joboffers"]
         depth = 1
         rdf_type = 'hd:Resource'
 
@@ -88,98 +93,136 @@
 # a resource in which only the owner has permissions (for testing owner permissions)
 class OwnedResource(Model):
     description = models.CharField(max_length=255, blank=True, null=True)
     user = models.ForeignKey(settings.AUTH_USER_MODEL, blank=True, null=True, related_name="owned_resources",
                              on_delete=models.CASCADE)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = []
         authenticated_perms = []
         owner_perms = ['view', 'delete', 'add', 'change', 'control']
         owner_field = 'user'
         serializer_fields = ['@id', 'description', 'user']
         depth = 1
 
 
 class OwnedResourceVariant(Model):
     description = models.CharField(max_length=255, blank=True, null=True)
     user = models.ForeignKey(settings.AUTH_USER_MODEL, blank=True, null=True, related_name="owned_variant_resources",
                              on_delete=models.CASCADE)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = []
         authenticated_perms = ['view', 'change']
         owner_perms = ['view', 'delete', 'add', 'change', 'control']
         owner_field = 'user'
         serializer_fields = ['@id', 'description', 'user']
         depth = 1
 
 
+class OwnedResourceNestedOwnership(Model):
+    description = models.CharField(max_length=255, blank=True, null=True)
+    parent = models.ForeignKey(OwnedResource, blank=True, null=True, related_name="owned_resources",
+                               on_delete=models.CASCADE)
+
+    class Meta(Model.Meta):
+        ordering = ['pk']
+        anonymous_perms = []
+        authenticated_perms = []
+        owner_perms = ['view', 'delete', 'add', 'change', 'control']
+        owner_field = 'parent__user'
+        serializer_fields = ['@id', 'description', 'parent']
+        depth = 1
+
+
+class OwnedResourceTwiceNestedOwnership(Model):
+    description = models.CharField(max_length=255, blank=True, null=True)
+    parent = models.ForeignKey(OwnedResourceNestedOwnership, blank=True, null=True, related_name="owned_resources",
+                               on_delete=models.CASCADE)
+
+    class Meta(Model.Meta):
+        ordering = ['pk']
+        anonymous_perms = []
+        authenticated_perms = []
+        owner_perms = ['view', 'delete', 'add', 'change', 'control']
+        owner_field = 'parent__parent__user'
+        serializer_fields = ['@id', 'description', 'parent']
+        depth = 1
+
+
 class UserProfile(Model):
     description = models.CharField(max_length=255, blank=True, null=True)
     user = models.OneToOneField(settings.AUTH_USER_MODEL, related_name='userprofile', on_delete=models.CASCADE)
     slug = models.SlugField(blank=True, null=True, unique=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view']
         authenticated_perms = ['inherit']
         owner_perms = ['inherit', 'change', 'control']
         owner_field = 'user'
         lookup_field = 'slug'
         serializer_fields = ['@id', 'description', 'settings', 'user', 'post_set']
         depth = 1
 
 
 class NotificationSetting(Model):
     user = models.OneToOneField(UserProfile, on_delete=models.CASCADE, related_name="settings")
     receiveMail = models.BooleanField(default=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view', 'change']
         authenticated_perms = ['inherit']
         owner_perms = ['inherit', 'change', 'control']
 
 
 class Message(models.Model):
     text = models.CharField(max_length=255, blank=True, null=True)
     conversation = models.ForeignKey(Conversation, on_delete=models.DO_NOTHING)
     author_user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.DO_NOTHING)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'add']
         owner_perms = ['inherit', 'change', 'delete', 'control']
 
 
 class Dummy(models.Model):
     some = models.CharField(max_length=255, blank=True, null=True)
     slug = models.SlugField(blank=True, null=True, unique=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'add']
         owner_perms = ['inherit', 'change', 'delete', 'control']
 
 
 class LDPDummy(Model):
     some = models.CharField(max_length=255, blank=True, null=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'add']
         owner_perms = ['inherit', 'change', 'delete', 'control']
 
 
 # model used in django-guardian permission tests (no anonymous etc permissions set)
 class PermissionlessDummy(Model):
     some = models.CharField(max_length=255, blank=True, null=True)
     slug = models.SlugField(blank=True, null=True, unique=True)
     parent = models.ForeignKey(LDPDummy, on_delete=models.DO_NOTHING, related_name="anons", blank=True, null=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = []
         authenticated_perms = []
         owner_perms = []
         permissions = (
             ('custom_permission_permissionlessdummy', 'Custom Permission'),
         )
 
@@ -187,128 +230,155 @@
 class Post(Model):
     content = models.CharField(max_length=255)
     author = models.ForeignKey(UserProfile, blank=True, null=True, on_delete=models.SET_NULL)
     peer_user = models.ForeignKey(settings.AUTH_USER_MODEL, blank=True, null=True, related_name="peers_post",
                                   on_delete=models.SET_NULL)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         auto_author = 'author'
         auto_author_field = 'userprofile'
         anonymous_perms = ['view', 'add', 'delete', 'add', 'change', 'control']
         authenticated_perms = ['inherit']
         owner_perms = ['inherit']
         rdf_type = 'hd:post'
 
 
 class Invoice(Model):
     title = models.CharField(max_length=255, blank=True, null=True)
     date = models.DateField(blank=True, null=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         depth = 2
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'add', 'change']
         owner_perms = ['inherit', 'delete', 'control']
 
 
 class Circle(Model):
     name = models.CharField(max_length=255, blank=True)
     description = models.CharField(max_length=255, blank=True)
     team = models.ManyToManyField(settings.AUTH_USER_MODEL, through="CircleMember", blank=True)
     owner = models.ForeignKey(settings.AUTH_USER_MODEL, related_name="owned_circles", on_delete=models.DO_NOTHING, null=True, blank=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view', 'add', 'delete', 'add', 'change', 'control']
         authenticated_perms = ["inherit"]
+        serializer_fields = ['@id', 'name', 'description', 'members', 'team', 'owner', 'space']
         rdf_type = 'hd:circle'
 
 
+class Space(Model):
+    name = models.CharField(max_length=255, blank=True)
+    circle = models.OneToOneField(to=Circle, null=True, blank=True, on_delete=models.CASCADE, related_name='space')
+
+    class Meta(Model.Meta):
+        ordering = ['pk']
+
+
 class Batch(Model):
     invoice = models.ForeignKey(Invoice, on_delete=models.CASCADE, related_name='batches')
     title = models.CharField(max_length=255, blank=True, null=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         serializer_fields = ['@id', 'title', 'invoice', 'tasks']
         anonymous_perms = ['view', 'add']
         authenticated_perms = ['inherit', 'add']
         owner_perms = ['inherit', 'change', 'delete', 'control']
         depth = 1
         rdf_type = 'hd:batch'
 
 
 class CircleMember(Model):
     circle = models.ForeignKey(Circle, on_delete=models.CASCADE, related_name='members')
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, related_name="circles")
     is_admin = models.BooleanField(default=False)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         container_path = "circle-members/"
         anonymous_perms = ['view', 'add', 'delete', 'add', 'change', 'control']
         authenticated_perms = ['inherit']
         unique_together = ['user', 'circle']
         rdf_type = 'hd:circlemember'
 
 
 class Task(models.Model):
     batch = models.ForeignKey(Batch, on_delete=models.CASCADE, related_name='tasks')
     title = models.CharField(max_length=255)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         serializer_fields = ['@id', 'title', 'batch']
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'add']
         owner_perms = ['inherit', 'change', 'delete', 'control']
 
 
 class ModelTask(Model, Task):
     class Meta(Model.Meta):
-        pass
+        ordering = ['pk']
 
+STATUS_CHOICES = [
+    ('Public', 'Public'),
+    ('Private', 'Private'),
+    ('Archived', 'Archived'),
+]
 
 class Project(Model):
     description = models.CharField(max_length=255, null=True, blank=False)
+    status = models.CharField(max_length=8, choices=STATUS_CHOICES, default='Private', null=True, blank=True)
     members = models.ManyToManyField(settings.AUTH_USER_MODEL, blank=True, related_name='projects')
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view', 'add', 'delete', 'add', 'change', 'control']
         authenticated_perms = ["inherit"]
         rdf_type = 'hd:project'
 
 
 class DateModel(Model):
     excluded = models.CharField(max_length=255, null=True, default='test')
     value = models.DateField()
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         rdf_type = "hd:date"
         serializer_fields_exclude = ['excluded']
 
 
 class DateChild(Model):
     parent = models.ForeignKey(DateModel, on_delete=models.CASCADE, related_name='children')
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         rdf_type = 'hd:datechild'
 
 
 class MyAbstractModel(Model):
     defaultsomething = models.CharField(max_length=255, blank=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         permission_classes = [LDPPermissions]
         abstract = True
         rdf_type = "wow:defaultrdftype"
 
 
 class NoSuperUsersAllowedModel(Model):
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = []
         authenticated_perms = []
         owner_perms = []
         superuser_perms = []
         permission_classes = [LDPPermissions]
 
 
 class ComplexPermissionClassesModel(Model):
     class Meta(Model.Meta):
+        ordering = ['pk']
         permission_classes = [LDPPermissions, SuperUserPermission]
         superuser_perms = []
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_update.py` & `djangoldp-3.0.5/djangoldp/tests/tests_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import uuid
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.test import TestCase
 from rest_framework.test import APIRequestFactory, APIClient
 from rest_framework.utils import json
 
-from djangoldp.serializers import LDPSerializer, LDListMixin
-from djangoldp.tests.models import Post, UserProfile, Resource, Circle, CircleMember, Invoice, Batch, Task, Skill, JobOffer, \
-    Conversation, Message, Project, NotificationSetting
+from djangoldp.tests.models import UserProfile, Resource, Invoice, Batch, Task, Skill, JobOffer, Conversation, Project,\
+    NotificationSetting
 
 
 class Update(TestCase):
 
     def setUp(self):
         self.factory = APIRequestFactory()
         self.client = APIClient()
         self.user = get_user_model().objects.create_user(username='john', email='jlennon@beatles.com',
                                                          password='glass onion')
         self.client.force_authenticate(user=self.user)
-        LDListMixin.to_representation_cache.reset()
-        LDPSerializer.to_representation_cache.reset()
 
     # TODO: https://git.startinblox.com/djangoldp-packages/djangoldp/issues/326
     '''
     def test_update_container_append_resource(self):
         pre_existing_skill_a = Skill.objects.create(title="to keep", obligatoire="obligatoire", slug="slug1")
         pre_existing_skill_b = Skill.objects.create(title="to keep", obligatoire="obligatoire", slug="slug2")
         job = JobOffer.objects.create(title="job test")
@@ -58,15 +55,15 @@
             '@id': '{}/skills/{}/'.format(settings.BASE_URL, skill.slug),
             'http://happy-dev.fr/owl/#title': "new", 'http://happy-dev.fr/owl/#obligatoire': "new"}]
         response = self.client.put('/skills/{}/'.format(skill.slug), data=json.dumps(body),
                                    content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
         self.assertEquals(response.data['title'], "new")
         self.assertEquals(response.data['obligatoire'], "new")
-        self.assertIn('location', response._headers)
+        self.assertIn('location', response.headers)
 
     def test_patch_resource(self):
         skill = Skill.objects.create(title='original', obligatoire='original', slug='skill1')
         body = {
             '@id': '{}/skills/{}'.format(settings.BASE_URL, skill.slug),
             'http://happy-dev.fr/owl/#title': 'new'
         }
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_settings.py` & `djangoldp-3.0.5/djangoldp/tests/tests_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,40 +13,38 @@
 
     def test_only_in_package(self):
         """Asserts default settings defined in the package."""
         assert settings.MYPACKAGEVAR == "ok"
 
     def test_only_in_user_config(self):
         """Asserts LDP packages are loaded from YAML file."""
-        assert settings.DJANGOLDP_PACKAGES == ['djangoldp.tests']
+        assert 'djangoldp.tests' in settings.DJANGOLDP_PACKAGES
 
     def test_overrided_core_by_package_config(self):
         assert settings.USE_I18N == False
 
     def test_overrided_package_by_user_config(self):
         assert settings.USE_TZ == False
 
     def test_overrided_core_by_user_config(self):
         """Asserts values overrided from user configuration."""
         assert settings.EMAIL_HOST == 'somewhere'
 
     def test_installed_apps_resolution(self):
         """Asserts LDP packages are referenced along with default installed apps."""
-        assert settings.INSTALLED_APPS == [
-            'djangoldp.tests',
-            'djangoldp.tests.dummy.apps.DummyConfig',
-            'django.contrib.admin',
-            'django.contrib.auth',
-            'django.contrib.contenttypes',
-            'django.contrib.sessions',
-            'django.contrib.messages',
-            'django.contrib.staticfiles',
-            'djangoldp',
-            'guardian',
-        ]
+        # test inclusion from server YAML settings
+        assert 'djangoldp.tests' in settings.INSTALLED_APPS
+        # test inclusion from ldppackage settings
+        assert 'djangoldp.tests.dummy.apps.DummyConfig' in settings.INSTALLED_APPS
+        # test inclusion from default core settings
+        assert 'djangoldp' in settings.INSTALLED_APPS
+        # test deduplication of dummy app
+        assert settings.INSTALLED_APPS.count('djangoldp.tests.dummy.apps.DummyConfig') == 1
+
+        # FIXME: We should check the order
 
     def test_reference_middleware(self):
         """Asserts middlewares added in packages are added to the settings."""
         assert 'djangoldp.tests.dummy.middleware.DummyMiddleware' in settings.MIDDLEWARE
 
     def test_extra_module(self):
         #FIXME
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/runner.py` & `djangoldp-3.0.5/djangoldp/tests/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import yaml
 
 import django
 from django.conf import settings as django_settings
 from djangoldp.conf.ldpsettings import LDPSettings
-from djangoldp.tests.settings_default import yaml_config
+from djangoldp.tests.server_settings import yaml_config
 
 # load test config
 config = yaml.safe_load(yaml_config)
 ldpsettings = LDPSettings(config)
 django_settings.configure(ldpsettings)
 
 django.setup()
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/performance_runner.py` & `djangoldp-3.0.5/djangoldp/tests/performance_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import sys
+import yaml
 
 import django
-from djangoldp.tests import settings_default
-from django.conf import settings
+from django.conf import settings as django_settings
+from djangoldp.conf.ldpsettings import LDPSettings
+from djangoldp.tests.server_settings import yaml_config
 
-# configure settings not to use pagination
-settings.configure(default_settings=settings_default,
-                   REST_FRAMEWORK = {
-                       'DEFAULT_PAGINATION_CLASS': None
-                   })
+# load test config
+config = yaml.safe_load(yaml_config)
+ldpsettings = LDPSettings(config)
+django_settings.configure(ldpsettings,
+                          REST_FRAMEWORK = {
+                                'DEFAULT_PAGINATION_CLASS': None
+                          },
+                          ANONYMOUS_USER_NAME=None)
 
 django.setup()
 from django.test.runner import DiscoverRunner
 
 test_runner = DiscoverRunner(verbosity=1)
 
 failures = test_runner.run_tests([
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_guardian.py` & `djangoldp-3.0.5/djangoldp/tests/tests_guardian.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 import json
 import uuid
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group
-from djangoldp.serializers import LDListMixin, LDPSerializer
 from rest_framework.test import APIClient, APITestCase
 from guardian.shortcuts import assign_perm
 
 from .models import PermissionlessDummy, Dummy, LDPDummy
-from djangoldp.permissions import LDPPermissions
 
 
 class TestsGuardian(APITestCase):
 
     def setUp(self):
         self.client = APIClient(enforce_csrf_checks=True)
-        LDListMixin.to_representation_cache.reset()
-        LDPSerializer.to_representation_cache.reset()
 
     def setUpLoggedInUser(self):
         self.user = get_user_model().objects.create_user(username='john', email='jlennon@beatles.com',
                                                          password='glass onion')
         self.group = Group.objects.create(name='Test')
         self.user.groups.add(self.group)
         self.user.save()
         self.client.force_authenticate(user=self.user)
-        LDListMixin.to_representation_cache.reset()
-        LDPSerializer.to_representation_cache.reset()
 
     def _get_dummy_with_perms(self, perms=None, parent=None, group=False):
         if perms is None:
             perms = []
         dummy = PermissionlessDummy.objects.create(some='test', slug=uuid.uuid4(), parent=parent)
         model_name = PermissionlessDummy._meta.model_name
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/scripts/prod_data_generator.py` & `djangoldp-3.0.5/djangoldp/tests/scripts/prod_data_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 import json
 import argparse
 from pathlib import Path
 from datetime import datetime
-from utils import generate_users, generate_projects
+from utils import generate_users, generate_projects, generate_skills
 
 '''
-A script which generates and outputs random production data, into a parameterised file (csv), which can be used as
+A script which generates and outputs random production data, into a parameterised file (json), which can be used as
 a Django fixture or imported into a live database
 e.g. python manage.py loaddata fixture.json
 for help run python prod_data_generator.py -h
 '''
 
 # starting from offset ensures that existing users etc are not disturbed
 parser = argparse.ArgumentParser(description='generates and outputs random test data, into a file used by the performance unit tests')
 parser.add_argument(dest='count', metavar='N', type=int, help='the number of users (and projects) to generate')
 parser.add_argument('--offset', dest='offset', type=int, default=100, help='an offset to start primary keys at (should be larger than the largest pre-existing project/user primary key)')
 parser.add_argument('-f', dest='file_dest', type=str, default="../fixtures/live.json", help='the file destination to write to')
+parser.add_argument('-s', dest='generate_skills', type=bool, default=False, help='Do you want to generate skills too ?')
 
 args = parser.parse_args()
 count = args.count
 OFFSET = args.offset
 
 user_template = {
     'model': 'djangoldp_account.ldpuser',
     'pk': 0,
     'fields': {
         'username': 'john',
         'email': 'jlennon@c.coop',
-        'password':'glass onion'
+        'password':'glassonion',
+        'first_name': 'John',
+        'last_name': 'Lennon'
     }
 }
 
 project_template = {
     'model': 'djangoldp_project.project',
     'pk': 0,
     'fields': {
         'description': 'Test',
+        'status': 'Public',
         'creationDate': str(datetime.date(datetime.now()))
     }
 }
 
+skill_template = {
+    'model': 'djangoldp_skill.skill',
+    'pk': 0,
+    'fields': {
+        'name': 'PHP',
+    }
+}
+
 fixture = generate_users(count, user_template, offset=OFFSET)
 fixture = generate_projects(count, project_template, fixture=fixture, offset=OFFSET)
 
+if args.generate_skills:
+    fixture = generate_skills(count, skill_template, fixture=fixture, offset=OFFSET)
+
 with open(Path(__file__).parent / args.file_dest, 'w') as output:
     json.dump(fixture, output)
 
 print(str(count))
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/scripts/test_data_generator.py` & `djangoldp-3.0.5/djangoldp/tests/scripts/test_data_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,36 +6,40 @@
 '''
 A script which generates and outputs random test data, into a file used by the performance unit tests
 for help run python test_data_generator.py -h
 '''
 
 parser = argparse.ArgumentParser(description='generates and outputs random test data, into a file used by the performance unit tests')
 parser.add_argument(dest='count', metavar='N', type=int, help='the number of users (and projects) to generate')
+parser.add_argument('-f', dest='file_dest', type=str, default="../fixtures/test.json", help='the file destination to write to')
 
 args = parser.parse_args()
 count = args.count
 
 user_template = {
     'model': 'tests.user',
     'pk': 0,
     'fields': {
         'username': 'john',
         'email': 'jlennon@c.coop',
-        'password':'glass onion'
+        'password':'glassonion',
+        'first_name': 'John',
+        'last_name': 'Lennon'
     }
 }
 
 project_template = {
     'model': 'tests.project',
     'pk': 0,
     'fields': {
+        'status': 'Public',
         'description': 'Test'
     }
 }
 
 fixture = generate_users(count, user_template)
-fixtue = generate_projects(count, project_template, fixture=fixture)
+fixture = generate_projects(count, project_template, fixture=fixture, production=False)
 
-with open(Path(__file__).parent / "../fixtures/test.json", 'w') as output:
+with open(Path(__file__).parent / args.file_dest, 'w') as output:
     json.dump(fixture, output)
 
 print(str(count))
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_delete.py` & `djangoldp-3.0.5/djangoldp/tests/tests_delete.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_auto_author.py` & `djangoldp-3.0.5/djangoldp/tests/tests_auto_author.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_performance.py` & `djangoldp-3.0.5/djangoldp/tests/tests_performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
     def _enable_new_profiler(self):
         pr = cProfile.Profile()
         pr.enable()
         return pr
 
     def test_get_container(self):
-        # pr = self._enable_new_profiler()
+        pr = self._enable_new_profiler()
         response = self.client.get('/projects/', content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
         print('counted ' + str(len(response.data['ldp:contains'])) + ' projects')
-        # pr.disable()
-        #self._print_stats(pr)
+        pr.disable()
+        self._print_stats(pr)
 
-        # pr = self._enable_new_profiler()
+        pr = self._enable_new_profiler()
         response = self.client.get('/users/', content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
         print('counted ' + str(len(response.data['ldp:contains'])) + ' users')
-        # pr.disable()
-        #self._print_stats(pr)
+        pr.disable()
+        self._print_stats(pr)
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/djangoldp_urls.py` & `djangoldp-3.0.5/djangoldp/tests/djangoldp_urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.conf.urls import re_path
+from django.urls import re_path
 
 from djangoldp.permissions import LDPPermissions
 from djangoldp.tests.models import Skill, JobOffer, Message, Conversation, Dummy, PermissionlessDummy, Task, DateModel, LDPDummy
 from djangoldp.views import LDPViewSet
 
 urlpatterns = [
     re_path(r'^messages/', LDPViewSet.urls(model=Message, permission_classes=[LDPPermissions], fields=["@id", "text", "conversation"], nested_fields=['conversation'])),
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_post.py` & `djangoldp-3.0.5/djangoldp/tests/tests_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-from django.conf import settings
 from django.contrib.auth import get_user_model
-from django.test import TestCase, override_settings
+from django.test import TestCase
 from rest_framework.test import APIRequestFactory, APIClient
 from rest_framework.utils import json
 
 from djangoldp.models import Model
-from djangoldp.serializers import LDPSerializer, LDListMixin
-from djangoldp.tests.models import Skill, JobOffer, Invoice, LDPDummy, Resource, Post, Circle, Project, \
-    UserProfile, NotificationSetting
+from djangoldp.tests.models import Invoice, LDPDummy, Resource, Post, Circle, Project, Space
 
 
 class PostTestCase(TestCase):
 
     def setUp(self):
         self.factory = APIRequestFactory()
         self.client = APIClient()
         self.user = get_user_model().objects.create_user(username='john', email='jlennon@beatles.com',
                                                          password='glass onion')
         self.client.force_authenticate(self.user)
-        LDListMixin.to_representation_cache.reset()
-        LDPSerializer.to_representation_cache.reset()
 
     def test_save_fk_graph_with_nested(self):
         post = {
             '@graph': [
                 {
                     'http://happy-dev.fr/owl/#title': "title",
                     'http://happy-dev.fr/owl/#invoice': {
@@ -46,15 +41,15 @@
     def test_save_fk_graph_with_existing_nested(self):
         invoice = Invoice.objects.create(title="title 3")
         post = {
             '@graph': [
                 {
                     'http://happy-dev.fr/owl/#title': "title",
                     'http://happy-dev.fr/owl/#invoice': {
-                        '@id': "https://happy-dev.fr{}{}/".format(Model.container_id(invoice), invoice.id)
+                        '@id': "http://happy-dev.fr{}{}/".format(Model.container_id(invoice), invoice.id)
                     }
                 }
             ]
         }
 
         response = self.client.post('/batchs/', data=json.dumps(post), content_type='application/ld+json')
         self.assertEqual(response.status_code, 201)
@@ -91,15 +86,15 @@
         dummy = LDPDummy.objects.create(some="foo")
 
         body = [
             {
                 '@id': "_:b216",
                 'http://happy-dev.fr/owl/#description': "user update",
                 'http://happy-dev.fr/owl/#ddummy': {
-                    "@id": "https://happy-dev.fr{}{}/".format(Model.container_id(dummy), dummy.id)
+                    "@id": "http://happy-dev.fr{}{}/".format(Model.container_id(dummy), dummy.id)
                 }
             },
             {
                 '@id': './',
                 "http://happy-dev.fr/owl/#first_name": "Alexandre",
                 "http://happy-dev.fr/owl/#last_name": "Bourlier",
                 "http://happy-dev.fr/owl/#username": "alex",
@@ -263,27 +258,50 @@
 
     # from JSON-LD spec: "The value associated with the @value key MUST be either a string, a number, true, false or null"
     def test_save_field_with_invalid_value_object(self):
         invoice = Invoice.objects.create(title="title 3")
         post = {
             'http://happy-dev.fr/owl/#invoice': {
                 '@value': {'title': 'title',
-                           '@id': "https://happy-dev.fr{}{}/".format(Model.container_id(invoice), invoice.id)}
+                           '@id': "http://happy-dev.fr{}{}/".format(Model.container_id(invoice), invoice.id)}
             }
         }
         response = self.client.post('/batchs/', data=json.dumps(post), content_type='application/ld+json')
         self.assertEqual(response.status_code, 400)
 
     # TODO: bug with PyLD: https://github.com/digitalbazaar/pyld/issues/142
     # from JSON-LD spec: "If the value associated with the @type key is @json, the value MAY be either an array or an object"
     '''
     def test_save_field_with_object_value_object(self):
         invoice = Invoice.objects.create(title="title 3")
         post = {
             'http://happy-dev.fr/owl/#invoice': {
-                '@value': {'title': 'title', '@id': "https://happy-dev.fr{}{}/".format(Model.container_id(invoice), invoice.id)},
+                '@value': {'title': 'title', '@id': "http://happy-dev.fr{}{}/".format(Model.container_id(invoice), invoice.id)},
                 '@type': '@json'
             }
         }
         response = self.client.post('/batchs/', data=json.dumps(post), content_type='application/ld+json')
         self.assertEqual(response.status_code, 201)
-    '''
+    '''
+
+    # the below test is necessary because of an obscure bug where the OneToOne field is successfully applied
+    # during the life of the serializer (and response) but is not persisted in the database,
+    # when it is posted onto the reverse relation
+    def test_one_to_one_field_reverse_post(self):
+        self.assertEqual(Circle.objects.count(), 0)
+        self.assertEqual(Space.objects.count(), 0)
+
+        body = {
+            '@context': {'@vocab': "http://happy-dev.fr/owl/#" },
+            'space': {'name': "Etablissement"}
+        }
+
+        response = self.client.post('/circles/', data=json.dumps(body), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 201)
+        self.assertEqual(Circle.objects.count(), 1)
+        self.assertEqual(Space.objects.count(), 1)
+
+        circle = Circle.objects.all()[0]
+        space = circle.space
+
+        self.assertIsNotNone(space)
+        self.assertIsNotNone(space.circle)
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_get.py` & `djangoldp-3.0.5/djangoldp/tests/tests_get.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 from datetime import datetime
 from django.contrib.auth import get_user_model
-from djangoldp.serializers import LDListMixin, LDPSerializer
 from rest_framework.test import APIRequestFactory, APIClient, APITestCase
 
 from djangoldp.tests.models import Post, Invoice, JobOffer, Skill, Batch, DateModel, Circle, CircleMember, UserProfile
-
+from djangoldp.serializers import GLOBAL_SERIALIZER_CACHE
 
 class TestGET(APITestCase):
 
     def setUp(self):
         self.factory = APIRequestFactory()
         self.client = APIClient()
         self.ordered_fields = ['@context', '@type', '@id']
-        LDListMixin.to_representation_cache.reset()
-        LDPSerializer.to_representation_cache.reset()
         setattr(Circle._meta, 'depth', 0)
         setattr(Circle._meta, 'empty_containers', [])
 
     def tearDown(self):
-        pass
+        GLOBAL_SERIALIZER_CACHE.reset()
 
     def test_get_resource(self):
         post = Post.objects.create(content="content")
-        response = self.client.get('/posts/{}/'.format(post.pk), content_type='application/ld+json')
+        response = self.client.get('/posts/{}/'.format(post.pk), content_type='application/ld+json', HTTP_ORIGIN='http://localhost:8080/test/')
         self.assertEqual(response.status_code, 200)
         self.assertEquals(response.data['content'], "content")
         self.assertIn('author', response.data)
         self.assertIn('@type', response.data)
+        self.assertIn('permissions', response.data)
+
+
+        # test headers returned
+        self.assertEqual(response['Content-Type'], 'application/ld+json') 
+        self.assertEqual(response['Accept-Post'], 'application/ld+json')
+        self.assertEqual(response['Allow'], 'GET, PUT, PATCH, DELETE, HEAD, OPTIONS')
+        self.assertEqual(response['Access-Control-Allow-Origin'], 'http://localhost:8080/test/')
+        self.assertIn('DPoP', response['Access-Control-Allow-Headers'])
 
     def test_get_resource_urlid(self):
         user = get_user_model().objects.create_user(username='john', email='jlennon@beatles.com',
                                                     password='glass onion')
         UserProfile.objects.create(user=user)
         post = Post.objects.create(content="content", author=user.userprofile)
         response = self.client.get('/posts/{}/'.format(post.pk), content_type='application/ld+json')
@@ -43,24 +49,24 @@
         # federated object - should not be returned in the container view
         Post.objects.create(content="federated", urlid="https://external.com/posts/1/")
         response = self.client.get('/posts/', content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
         self.assertEquals(1, len(response.data['ldp:contains']))
         self.assertIn('@type', response.data)
         self.assertIn('@type', response.data['ldp:contains'][0])
+        self.assertNotIn('permissions', response.data['ldp:contains'][0])
         self.assertEquals(4, len(response.data['permissions'])) # configured anonymous permissions to give all
 
         Invoice.objects.create(title="content")
         response = self.client.get('/invoices/', content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
         self.assertIn('permissions', response.data)
         self.assertEquals(1, len(response.data['permissions']))  # read only
 
     def test_get_empty_container(self):
-        Post.objects.all().delete()
         response = self.client.get('/posts/', content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
         self.assertEquals(0, len(response.data['ldp:contains']))
 
     def test_get_filtered_fields(self):
         skill = Skill.objects.create(title="Java", obligatoire="ok", slug="1")
         skill2 = Skill.objects.create(title="Java", obligatoire="ok", slug="2")
@@ -105,17 +111,20 @@
     def test_get_nested(self):
         invoice = Invoice.objects.create(title="invoice")
         batch = Batch.objects.create(invoice=invoice, title="batch")
         distant_batch = Batch.objects.create(invoice=invoice, title="distant", urlid="https://external.com/batch/1/")
         response = self.client.get('/invoices/{}/batches/'.format(invoice.pk), content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
         self.assertEquals(response.data['@id'], 'http://happy-dev.fr/invoices/{}/batches/'.format(invoice.pk))
+        self.assertIn('permissions', response.data)
         self.assertEquals(len(response.data['ldp:contains']), 2)
         self.assertIn('@type', response.data['ldp:contains'][0])
         self.assertIn('@type', response.data['ldp:contains'][1])
+        self.assertNotIn('permissions', response.data['ldp:contains'][0])
+        self.assertNotIn('permissions', response.data['ldp:contains'][1])
         self.assertEquals(response.data['ldp:contains'][0]['invoice']['@id'], invoice.urlid)
         self.assertEqual(response.data['ldp:contains'][1]['@id'], distant_batch.urlid)
 
     # TODO: https://git.startinblox.com/djangoldp-packages/djangoldp/issues/335
     #  test getting a route with multiple nested fields (/job-offers/X/skills/Y/)
     '''def test_get_twice_nested(self):
         job = JobOffer.objects.create(title="job", slug="slug1")
@@ -209,9 +218,8 @@
             response.data['ldp:contains'][-1],
             response.data['ldp:contains'][-1]['circle_set']
         ]
 
         for test_fields in fields_to_test:
             test_fields = list(test_fields)
             o_f = [field for field in self.ordered_fields if field in test_fields]
-            self.assertEquals(o_f, test_fields[:len(o_f)])  
-    
+            self.assertEquals(o_f, test_fields[:len(o_f)])
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_pagination.py` & `djangoldp-3.0.5/djangoldp/tests/tests_pagination.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 
 class TestPagination(APITestCase):
 
     def setUp(self):
         self.factory = APIRequestFactory()
         self.client = APIClient()
-        for i in range(0, 10):
+        for i in range(0, 30):
             Post.objects.create(content="content {}".format(i))
 
     def tearDown(self):
         pass
 
     def test_next(self):
         response = self.client.get('/posts/', content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
-        self.assertIn('link', response._headers)
-        self.assertEquals(response._headers['link'][1], '<http://testserver/posts/?limit=5&offset=5>; rel="next"')
+        self.assertIn('link', response.headers)
+        self.assertEquals(response.headers['link'], '<http://testserver/posts/?p=2>; rel="next"')
 
     def test_previous(self):
-        response = self.client.get('/posts/?offset=2&limit=2', content_type='application/ld+json')
+        response = self.client.get('/posts/?p=2', content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
-        self.assertIn('link', response._headers)
-        self.assertEquals(response._headers['link'][1],
-                          '<http://testserver/posts/?limit=2>; rel="prev", <http://testserver/posts/?limit=2&offset=4>; rel="next"')
+        self.assertIn('link', response.headers)
+        self.assertEquals(response.headers['link'],
+                          '<http://testserver/posts/>; rel="prev", <http://testserver/posts/?p=3>; rel="next"')
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_anonymous_permissions.py` & `djangoldp-3.0.5/djangoldp/tests/tests_anonymous_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_perf_get.py` & `djangoldp-3.0.5/djangoldp/tests/tests_perf_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import datetime
 import platform
 
 import time
 from django.contrib.auth import get_user_model
 from rest_framework.test import APIRequestFactory, APIClient, APITestCase
 from statistics import mean, variance
+import cProfile, io, pstats
 
 from djangoldp.permissions import LDPPermissions
-from djangoldp.tests.models import Post, Invoice, JobOffer, Skill, Batch, DateModel, Project, User
+from djangoldp.tests.models import Post, JobOffer, Skill, Project, User
 
 
 class TestPerformanceGET(APITestCase):
     posts = []
     skills = []
     jobs = []
     test_volume = 100
     result_line = []
     withAuth = True
     withPermsCache = True
-    # fixtures = ['test.json',]
+    fixtures = ['test.json']
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         print("Init", end='', flush=True)
 
         LDPPermissions.with_cache = cls.withPermsCache
@@ -57,15 +58,15 @@
         cls.result_line.append("N/A")
         cls.result_line.append("N/A")
         cls.result_line.append("N/A")
 
     def setUp(self):
         self.client = APIClient()
         self.user = get_user_model().objects.create_user(username='john', email='jlennon@beatles.com',
-                                                         password='glass onion')
+                                                         password='glass onion', is_active=True)
         self.client.force_authenticate(user=self.user)
         print('there are ' + str(Project.objects.count()) + ' projects in the database')
         print('there are ' + str(User.objects.count()) + ' users in the database')
 
     @classmethod
     def tearDownClass(cls):
         import csv
@@ -131,25 +132,36 @@
             response = self.client.get('/jobs/{}/skills'.format(job.slug), content_type='application/ld+json')
             end_time = time.time()
             times.append(end_time - start_time)
 
         self.result_line[9] = str(mean(times))
         print("Variance execution time :" + str(variance(times)))
 
+    def _print_stats(self, pr):
+        s = io.StringIO()
+        ps = pstats.Stats(pr, stream=s)
+        ps.sort_stats('time').print_stats(50)
+        print(s.getvalue())
+
+    def _enable_new_profiler(self):
+        pr = cProfile.Profile()
+        pr.enable()
+        return pr
+
     def test_get_users_container(self):
-        # pr = self._enable_new_profiler()
-        # response = self.client.get('/projects/', content_type='application/ld+json')
-        # self.assertEqual(response.status_code, 200)
-        # print('counted ' + str(len(response.data['ldp:contains'])) + ' projects')
-        # pr.disable()
-        #self._print_stats(pr)
+        pr = self._enable_new_profiler()
+        response = self.client.get('/projects/', content_type='application/ld+json')
+        self.assertEqual(response.status_code, 200)
+        print('counted ' + str(len(response.data['ldp:contains'])) + ' projects')
+        pr.disable()
+        self._print_stats(pr)
 
-        # pr = self._enable_new_profiler()
+        pr = self._enable_new_profiler()
         start_time = time.time()
         response = self.client.get('/users/', content_type='application/ld+json')
         end_time = time.time()
         self.assertEqual(response.status_code, 200)
         print('counted ' + str(len(response.data['ldp:contains'])) + ' users')
         self.result_line[10] = str(end_time-start_time)
-        # pr.disable()
-        #self._print_stats(pr)
+        pr.disable()
+        self._print_stats(pr)
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_backlinks_service.py` & `djangoldp-3.0.5/djangoldp/tests/tests_backlinks_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import uuid
 import time
+import copy
 from django.contrib.auth import get_user_model
 from django.test import override_settings
 from rest_framework.test import APIClient, APITestCase
 from djangoldp.tests.models import Circle, Project
 from djangoldp.models import Activity, ScheduledActivity
 from djangoldp.activities.services import BACKLINKS_ACTOR, ActivityPubService, ActivityQueueService
 
@@ -193,16 +194,15 @@
 
     @override_settings(SEND_BACKLINKS=True, DISABLE_OUTBOX='DEBUG')
     def test_unnecessary_add_not_sent(self):
         # an add activity was sent previously
         a = {'type': 'Add', 'actor': {'type': 'Service', 'name': 'Backlinks Service'},
              'object': {'@type': 'foaf:user', '@id': 'https://api.test2.startinblox.com/users/calum/'},
              'target': {'@type': 'hd:skill', '@id': 'https://api.test1.startinblox.com/skills/3/'}}
-        ActivityQueueService._save_sent_activity(a, Activity, success=True, type='add',
-                                                 external_id='https://distant.com/inbox/')
+        ActivityQueueService._save_activity_from_response({'status_code': '201'}, 'https://distant.com/inbox/', a)
 
         # no remove has since been sent, but a new Add is scheduled
         scheduled_b = ActivityQueueService._save_sent_activity(a, ScheduledActivity, success=False, type='add',
                                                                external_id='https://distant.com/inbox/')
         ActivityQueueService._activity_queue_worker('https://distant.com/inbox/', scheduled_b)
 
         # assert that only the previous activity was sent, and the scheduled activites cleaned up
@@ -211,16 +211,15 @@
 
     @override_settings(SEND_BACKLINKS=True, DISABLE_OUTBOX='DEBUG')
     def test_unnecessary_remove_not_sent(self):
         # an remove activity was sent previously
         a = {'type': 'Remove', 'actor': {'type': 'Service', 'name': 'Backlinks Service'},
              'object': {'@type': 'foaf:user', '@id': 'https://api.test2.startinblox.com/users/calum/'},
              'target': {'@type': 'hd:skill', '@id': 'https://api.test1.startinblox.com/skills/3/'}}
-        ActivityQueueService._save_sent_activity(a, Activity, success=True, type='remove',
-                                                 external_id='https://distant.com/inbox/')
+        ActivityQueueService._save_activity_from_response({'status_code': '201'}, 'https://distant.com/inbox/', a)
 
         # no add has since been sent, but a new Remove is scheduled
         scheduled_b = ActivityQueueService._save_sent_activity(a, ScheduledActivity, success=False, type='remove',
                                                                external_id='https://distant.com/inbox/')
         ActivityQueueService._activity_queue_worker('https://distant.com/inbox/', scheduled_b)
 
         # assert that only the previous activity was sent, and the scheduled activites cleaned up
@@ -229,16 +228,15 @@
 
     @override_settings(SEND_BACKLINKS=True, DISABLE_OUTBOX='DEBUG')
     def test_necessary_add_sent(self):
         # a remove activity was sent previously
         a = {'type': 'Remove', 'actor': {'type': 'Service', 'name': 'Backlinks Service'},
              'object': {'@type': 'foaf:user', '@id': 'https://api.test2.startinblox.com/users/calum/'},
              'target': {'@type': 'hd:skill', '@id': 'https://api.test1.startinblox.com/skills/3/'}}
-        ActivityQueueService._save_sent_activity(a, Activity, success=True, type='remove',
-                                                 external_id='https://distant.com/inbox/')
+        ActivityQueueService._save_activity_from_response({'status_code': '201'}, 'https://distant.com/inbox/', a)
 
         # an add is now being sent
         scheduled_b = ActivityQueueService._save_sent_activity(a, ScheduledActivity, type='add',
                                                                external_id='https://distant.com/inbox/')
         ActivityQueueService._activity_queue_worker('https://distant.com/inbox/', scheduled_b)
 
         # assert that both activities sent, and the scheduled activites cleaned up
@@ -266,16 +264,15 @@
         obj = {
             '@type': 'hd:circle',
             '@id': 'https://test.com/circles/8/',
             'owner': {'@id': 'https://distant.com/users/john/',
                       '@type': 'foaf:user'}
         }
         activity_a = ActivityPubService.build_activity(BACKLINKS_ACTOR, obj, activity_type='Create', summary='A')
-        ActivityQueueService._save_sent_activity(activity_a, Activity, success=True, type='create',
-                                                 external_id='https://distant.com/inbox/')
+        ActivityQueueService._save_activity_from_response({'status_code': '201'}, 'https://distant.com/inbox/', activity_a)
 
         # now I'm sending an update, which doesn't change anything about the object
         activity_b = ActivityPubService.build_activity(BACKLINKS_ACTOR, obj, activity_type='Create', summary='B')
         scheduled_b = ActivityQueueService._save_sent_activity(activity_b, ScheduledActivity, type='update',
                                                                external_id='https://distant.com/inbox/')
 
         ActivityQueueService._activity_queue_worker('https://distant.com/inbox/', scheduled_b)
@@ -290,16 +287,15 @@
         obj = {
             '@type': 'hd:circle',
             '@id': 'https://test.com/circles/8/',
             'owner': {'@id': 'https://distant.com/users/john/',
                       '@type': 'foaf:user'}
         }
         activity_a = ActivityPubService.build_activity(BACKLINKS_ACTOR, obj, activity_type='Create', summary='A')
-        ActivityQueueService._save_sent_activity(activity_a, Activity, success=True, type='create',
-                                                 external_id='https://distant.com/inbox/')
+        ActivityQueueService._save_activity_from_response({'status_code': '201'}, 'https://distant.com/inbox/', activity_a)
 
         # now I'm sending an update, which changes the owner of the circle
         obj['owner']['@id'] = 'https://distant.com/users/mark/'
         activity_b = ActivityPubService.build_activity(BACKLINKS_ACTOR, obj, activity_type='Create', summary='B')
         scheduled_b = ActivityQueueService._save_sent_activity(activity_b, ScheduledActivity, type='update',
                                                                external_id='https://distant.com/inbox/')
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_cache.py` & `djangoldp-3.0.5/djangoldp/tests/tests_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from django.contrib.auth import get_user_model
 from django.test import TestCase, override_settings
 from rest_framework.test import APIRequestFactory, APIClient
 from rest_framework.utils import json
 
-from djangoldp.serializers import LDPSerializer, LDListMixin
-from djangoldp.tests.models import Conversation, Project, Circle, CircleMember
+from djangoldp.tests.models import Conversation, Project, Circle, CircleMember, User
 
 
 class TestCache(TestCase):
 
     def setUp(self):
         self.factory = APIRequestFactory()
         self.client = APIClient()
         self.user = get_user_model().objects.create_user(username='john', email='jlennon@beatles.com',
-                                                         password='glass onion')
+                                                         password='glass onion', first_name='John')
         self.client.force_authenticate(self.user)
-        LDListMixin.to_representation_cache.reset()
-        LDPSerializer.to_representation_cache.reset()
 
     def tearDown(self):
         setattr(Circle._meta, 'depth', 0)
         setattr(Circle._meta, 'empty_containers', [])
 
     # test container cache after new resource added
     @override_settings(SERIALIZER_CACHE=True)
@@ -189,14 +186,69 @@
 
         conversation.observers.add(self.user)
         conversation.observers.clear()
         response = self.client.get('/conversations/{}/observers/'.format(conversation.pk), content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
         self.assertEqual(len(response.data['ldp:contains']), 0)
 
+    # test cache working inside of the nested field (serializer) of another object
+    @override_settings(SERIALIZER_CACHE=True)
+    def test_cached_container_serializer_nested_field(self):
+        project = Project.objects.create(description='Test')
+        response = self.client.get('/projects/{}/'.format(project.pk), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(len(response.data['members']['ldp:contains']), 0)
+
+        project.members.add(self.user)
+        response = self.client.get('/projects/{}/'.format(project.pk), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(len(response.data['members']['ldp:contains']), 1)
+
+        project.members.remove(self.user)
+        response = self.client.get('/projects/{}/'.format(project.pk), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(len(response.data['members']['ldp:contains']), 0)
+
+        project.members.add(self.user)
+        project.members.clear()
+        response = self.client.get('/projects/{}/'.format(project.pk), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(len(response.data['members']['ldp:contains']), 0)
+
+    # test cache working on a serialized nested field at higher depth
+    @override_settings(SERIALIZER_CACHE=True)
+    def test_cache_depth_2(self):
+        setattr(Circle._meta, 'depth', 2)
+
+        circle = Circle.objects.create(description='Test')
+        response = self.client.get('/circles/{}/'.format(circle.pk), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(len(response.data['members']['ldp:contains']), 0)
+
+        CircleMember.objects.create(user=self.user, circle=circle)
+        response = self.client.get('/circles/{}/'.format(circle.pk), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(len(response.data['members']['ldp:contains']), 1)
+        # assert the depth is applied
+        self.assertIn('user', response.data['members']['ldp:contains'][0])
+        self.assertIn('first_name', response.data['members']['ldp:contains'][0]['user'])
+        self.assertEqual(response.data['members']['ldp:contains'][0]['user']['first_name'], self.user.first_name)
+
+        # make a change to the _user_
+        self.user.first_name = "Alan"
+        self.user.save()
+
+        # assert that the use under the circles members has been updated
+        response = self.client.get('/circles/{}/'.format(circle.pk), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(len(response.data['members']['ldp:contains']), 1)
+        self.assertIn('user', response.data['members']['ldp:contains'][0])
+        self.assertIn('first_name', response.data['members']['ldp:contains'][0]['user'])
+        self.assertEqual(response.data['members']['ldp:contains'][0]['user']['first_name'], self.user.first_name)
+
     # test the cache behaviour when empty_containers is an active setting
     @override_settings(SERIALIZER_CACHE=True)
     def test_cache_empty_container(self):
         setattr(Circle._meta, 'depth', 1)
         setattr(Circle._meta, 'empty_containers', ['members'])
 
         circle = Circle.objects.create(name='test', description='test')
@@ -214,10 +266,7 @@
         # and a second on the child
         response = self.client.get('/circles/1/members/', content_type='application/ld+json')
         self.assertEqual(response.data['@type'], 'ldp:Container')
         self.assertIn('@id', response.data)
         self.assertIn('ldp:contains', response.data)
         self.assertIn('permissions', response.data)
         self.assertIn('circle', response.data['ldp:contains'][0])
-
-
-
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/settings_default.py` & `djangoldp-3.0.5/djangoldp/tests/server_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-"""This module contains YAML configurations for djangoldp testing."""
+"""
+This module contains the YAML configuration for a testing djangoldp server.
+"""
 
 yaml_config = """
 dependencies:
 
 ldppackages:
-  - djangoldp.tests
+  - djangoldp.tests                         # fetch 'djangoldp.tests.djangoldp_settings'
+  - djangoldp.tests.dummy.apps.DummyConfig  # already declared in 'djangoldp.tests'
 
 server:
   ALLOWED_HOSTS:
     - '*'
   AUTH_USER_MODEL: tests.User
   EMAIL_HOST: somewhere
   ANONYMOUS_USER_NAME: None
@@ -19,8 +22,9 @@
   REST_FRAMEWORK:
     DEFAULT_PAGINATION_CLASS: djangoldp.pagination.LDPPagination
     PAGE_SIZE: 5
   USE_TZ: false
   SEND_BACKLINKS: false
   GUARDIAN_AUTO_PREFETCH: true
   SERIALIZER_CACHE: false
+  STORE_ACTIVITIES: VERBOSE
 """
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_inbox.py` & `djangoldp-3.0.5/djangoldp/tests/tests_inbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,14 +444,15 @@
         self.assertIn("https://distant.com/projects/1/", projects.values_list('urlid', flat=True))
         self.assertIn("https://distant.com/projects/1/", user_projects.values_list('urlid', flat=True))
         self._assert_activity_created(response)
         backlink = Project.objects.get(urlid="https://distant.com/projects/1/")
         self.assertNotEqual(backlink.pk, 100)
 
     def test_missing_not_null_field_activity(self):
+        # TODO: catch the warning
         # DateChild must not have a null reference to parent
         # and parent must not have a null field 'date', which here is missing
         obj = {
             "@type": "hd:datechild",
             "@id": "https://distant.com/datechilds/1/",
             "parent": {
                 "@type": "hd:date",
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_model_serializer.py` & `djangoldp-3.0.5/djangoldp/tests/tests_model_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-import uuid
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.test import TestCase, override_settings
 from rest_framework.test import APIRequestFactory, APIClient
 
-from djangoldp.serializers import LDPSerializer, LDListMixin
-from djangoldp.tests.models import Post, UserProfile, Resource, Circle, CircleMember, Invoice, Batch, Task, ModelTask
-from djangoldp.tests.models import Skill, JobOffer, Conversation, Message, Project
+from djangoldp.serializers import LDPSerializer
+from djangoldp.tests.models import Invoice, Batch, ModelTask
+from djangoldp.tests.models import Skill, JobOffer, Conversation, Message
 
 
 class LDPModelSerializerTestCase(TestCase):
     def setUp(self):
         self.factory = APIRequestFactory()
-        self.client = APIClient()
         self.user = get_user_model().objects.create_user(username='john', email='jlennon@beatles.com',
                                                          password='glass onion')
-        self.client.force_authenticate(user=self.user)
-        LDListMixin.to_representation_cache.reset()
-        LDPSerializer.to_representation_cache.reset()
 
     def _get_serializer_class(self, model, depth, fields):
         meta_args = {'model': model, 'depth': depth, 'fields': fields}
 
         meta_class = type('Meta', (), meta_args)
         return type(LDPSerializer)('TestSerializer', (LDPSerializer,), {'Meta': meta_class})
 
@@ -720,15 +715,15 @@
     def test_save_m2m_switch_base_url_prefix(self):
         skill1 = Skill.objects.create(title="skill1", obligatoire="obligatoire", slug="slug1")
 
         job = {"title": "job test",
                "slug": "slug1",
                "skills": {
                    "ldp:contains": [
-                       {"@id": "https://happy-dev.fr/skills/{}/".format(skill1.slug)},
+                       {"@id": "http://happy-dev.fr/skills/{}/".format(skill1.slug)},
                    ]}
                }
 
         meta_args = {'model': JobOffer, 'depth': 2, 'fields': ("@id", "title", "skills", "slug")}
 
         meta_class = type('Meta', (), meta_args)
         serializer_class = type(LDPSerializer)('JobOfferSerializer', (LDPSerializer,), {'Meta': meta_class})
```

### Comparing `djangoldp-2.1.9/djangoldp/tests/tests_ldp_model.py` & `djangoldp-3.0.5/djangoldp/tests/tests_ldp_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,11 +52,11 @@
             self.assertIn(expected, nested_fields)
 
         nested_fields = CircleMember.objects.nested_fields()
         expected_nested_fields = []
         self.assertEqual(nested_fields, expected_nested_fields)
 
     def test_ldp_manager_nested_fields_exclude(self):
-        setattr(Circle.Meta, 'nested_fields_exclude', ['team'])
+        Circle._meta.nested_fields_exclude = ['team']
         nested_fields = Circle.objects.nested_fields()
         expected_nested_fields = ['members']
         self.assertEqual(nested_fields, expected_nested_fields)
```

### Comparing `djangoldp-2.1.9/djangoldp/urls.py` & `djangoldp-3.0.5/djangoldp/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from importlib import import_module
 
 from django.conf import settings
-from django.conf.urls import re_path, include
+from django.urls import path, re_path, include
 
 from djangoldp.models import LDPSource, Model
 from djangoldp.permissions import LDPPermissions
 from djangoldp.views import LDPSourceViewSet, WebFingerView, InboxView
 from djangoldp.views import LDPViewSet
 
-
 def __clean_path(path):
     '''ensures path is Django-friendly'''
     if path.startswith("/"):
         path = path[1:]
     if not path.endswith("/"):
         path = "{}/".format(path)
     return path
@@ -36,37 +35,53 @@
     return {cls.__name__: cls for cls in get_all_non_abstract_subclasses(cls)}
 
 
 urlpatterns = [
     re_path(r'^sources/(?P<federation>\w+)/', LDPSourceViewSet.urls(model=LDPSource, fields=['federation', 'urlid'],
                                                                     permission_classes=[LDPPermissions], )),
     re_path(r'^\.well-known/webfinger/?$', WebFingerView.as_view()),
-    re_path(r'^inbox/$', InboxView.as_view()),
+    path('inbox/', InboxView.as_view())
 ]
 
+if settings.ENABLE_SWAGGER_DOCUMENTATION:
+    from drf_spectacular.views import SpectacularAPIView, SpectacularSwaggerView
+    urlpatterns.extend([
+        path("schema/", SpectacularAPIView.as_view(), name="schema"),
+        path(
+            "docs/",
+            SpectacularSwaggerView.as_view(
+                template_name="swagger-ui.html", url_name="schema"
+            ),
+            name="swagger-ui",
+        )
+    ])
+
 for package in settings.DJANGOLDP_PACKAGES:
     try:
         import_module('{}.models'.format(package))
-        urlpatterns.append(re_path(r'^', include('{}.djangoldp_urls'.format(package))))
+    except ModuleNotFoundError:
+        pass
+    try:
+        urlpatterns.append(path('', include('{}.djangoldp_urls'.format(package))))
     except ModuleNotFoundError:
         pass
 
 # fetch a list of all models which subclass DjangoLDP Model
 model_classes = get_all_non_abstract_subclasses_dict(Model)
 
 # append urls for all DjangoLDP Model subclasses
 for class_name in model_classes:
     model_class = model_classes[class_name]
     # the path is the url for this model
-    path = __clean_path(model_class.get_container_path())
+    model_path = __clean_path(model_class.get_container_path())
     # urls_fct will be a method which generates urls for a ViewSet (defined in LDPViewSetGenerator)
     urls_fct = model_class.get_view_set().urls
-    urlpatterns.append(re_path(r'^' + path,
+    urlpatterns.append(path('' + model_path,
         urls_fct(model=model_class,
                  lookup_field=Model.get_meta(model_class, 'lookup_field', 'pk'),
                  permission_classes=Model.get_meta(model_class, 'permission_classes', [LDPPermissions]),
                  fields=Model.get_meta(model_class, 'serializer_fields', []),
                  nested_fields=model_class.nested.fields())))
 
 # NOTE: this route will be ignored if a custom (subclass of Model) user model is used, or it is registered by a package
 # Django matches the first url it finds for a given path
-urlpatterns.append(re_path(r'^users/', LDPViewSet.urls(model=settings.AUTH_USER_MODEL, permission_classes=[])))
+urlpatterns.append(re_path('users/', LDPViewSet.urls(model=settings.AUTH_USER_MODEL, permission_classes=[])))
```

### Comparing `djangoldp-2.1.9/djangoldp/cli.py` & `djangoldp-3.0.5/djangoldp/cli.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0007_auto_20200429_1346.py` & `djangoldp-3.0.5/djangoldp/migrations/0007_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0011_auto_20200610_1323.py` & `djangoldp-3.0.5/djangoldp/migrations/0011_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0012_auto_20200617_1817.py` & `djangoldp-3.0.5/djangoldp/migrations/0012_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0008_auto_20200501_1207.py` & `djangoldp-3.0.5/djangoldp/migrations/0008_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0010_follower.py` & `djangoldp-3.0.5/djangoldp/migrations/0010_follower.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0002_auto_20190906_0642.py` & `djangoldp-3.0.5/djangoldp/migrations/0002_auto_20190906_0642.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0006_activity.py` & `djangoldp-3.0.5/djangoldp/migrations/0006_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0015_auto_20210125_1847.py` & `djangoldp-3.0.5/djangoldp/migrations/0015_auto_20210125_1847.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0001_initial.py` & `djangoldp-3.0.5/djangoldp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0013_auto_20200624_1709.py` & `djangoldp-3.0.5/djangoldp/migrations/0013_auto_20200624_1709.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0014_auto_20200909_2206.py` & `djangoldp-3.0.5/djangoldp/migrations/0014_auto_20200909_2206.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/migrations/0009_auto_20200505_1733.py` & `djangoldp-3.0.5/djangoldp/migrations/0009_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/management/commands/federate.py` & `djangoldp-3.0.5/djangoldp/management/commands/federate.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,18 @@
     "eventsfuture": "/events/future/",
     "eventspast": "/events/past/",
     "typeevents": "/typeevents/",
     "resources": "/resources/",
     "keywords": "/keywords/",
     "types": "/types/",
     "joboffers": "/job-offers/current/",
+    "polls": "/polls/",
     "projects": "/projects/",
     "projectsjoinable": "/projects/joinable/",
+    "skills": "/skills/",
     "users": "/users/"
   }
 
 class Command(BaseCommand):
   help = 'Add another server to this one sources'
 
   def add_arguments(self, parser):
```

### Comparing `djangoldp-2.1.9/djangoldp/management/commands/check_integrity.py` & `djangoldp-3.0.5/djangoldp/management/commands/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp/management/commands/configure.py` & `djangoldp-3.0.5/djangoldp/management/commands/configure.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.9/djangoldp.egg-info/SOURCES.txt` & `djangoldp-3.0.5/djangoldp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+commit_parser/__init__.py
+commit_parser/parser.py
 djangoldp/__init__.py
 djangoldp/admin.py
 djangoldp/apps.py
 djangoldp/check_integrity.py
 djangoldp/cli.py
 djangoldp/factories.py
 djangoldp/fields.py
@@ -70,21 +73,22 @@
 djangoldp/migrations/0010_follower.py
 djangoldp/migrations/0011_auto_20200610_1323.py
 djangoldp/migrations/0012_auto_20200617_1817.py
 djangoldp/migrations/0013_auto_20200624_1709.py
 djangoldp/migrations/0014_auto_20200909_2206.py
 djangoldp/migrations/0015_auto_20210125_1847.py
 djangoldp/migrations/__init__.py
+djangoldp/templates/swagger-ui.html
 djangoldp/tests/__init__.py
 djangoldp/tests/djangoldp_settings.py
 djangoldp/tests/djangoldp_urls.py
 djangoldp/tests/models.py
 djangoldp/tests/performance_runner.py
 djangoldp/tests/runner.py
-djangoldp/tests/settings_default.py
+djangoldp/tests/server_settings.py
 djangoldp/tests/tests_anonymous_permissions.py
 djangoldp/tests/tests_auto_author.py
 djangoldp/tests/tests_backlinks_service.py
 djangoldp/tests/tests_cache.py
 djangoldp/tests/tests_delete.py
 djangoldp/tests/tests_get.py
 djangoldp/tests/tests_guardian.py
```

