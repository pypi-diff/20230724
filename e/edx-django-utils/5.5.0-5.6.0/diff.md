# Comparing `tmp/edx-django-utils-5.5.0.tar.gz` & `tmp/edx-django-utils-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-django-utils-5.5.0.tar", last modified: Thu Jun  1 18:11:23 2023, max compression
+gzip compressed data, was "edx-django-utils-5.6.0.tar", last modified: Mon Jul 24 08:05:36 2023, max compression
```

## Comparing `edx-django-utils-5.5.0.tar` & `edx-django-utils-5.6.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)    13109 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    20617 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6848 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.278468 edx-django-utils-5.5.0/edx_django_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils/admin/
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/admin/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils/admin/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/admin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/admin/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/admin/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils/cache/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1400 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils/cache/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    12463 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils/db/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/queryset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4834 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/read_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/db/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/tests/test_queryset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/tests/test_read_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/ip/
--rw-r--r--   0 runner    (1001) docker     (122)     7936 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/ip/internal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/ip/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10730 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/ip/internal/ip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/ip/internal/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/ip/internal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13591 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/ip/internal/tests/test_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/logging/internal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/internal/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     7961 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/internal/log_sensitive.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/logging/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/tests/test_log_sensitive.py
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.290468 edx-django-utils-5.5.0/edx_django_utils/monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.290468 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.290468 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5260 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    10474 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    22556 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3895 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.290468 edx-django-utils-5.5.0/edx_django_utils/monitoring/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/scripts/new_relic_nrql_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     8178 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.290468 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/mock_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    12959 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6238 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    13475 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3016 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/plugins/
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     3200 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/pluggable_override.py
--rw-r--r--   0 runner    (1001) docker     (122)      794 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_contexts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.278468 edx-django-utils-5.5.0/edx_django_utils/security/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/security/csp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/security/csp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5753 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/security/csp/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/security/csp/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4974 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/security/csp/tests/test_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/tests/test_pluggable_override.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/user/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/edx_django_utils/user/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/edx_django_utils/user/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/commands/manage_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     6487 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/commands/manage_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/edx_django_utils/user/management/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7382 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/tests/test_manage_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     7796 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/tests/test_manage_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/edx_django_utils/user/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/tests/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    20617 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3840 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    13302 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6848 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.598981 edx-django-utils-5.6.0/edx_django_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.598981 edx-django-utils-5.6.0/edx_django_utils/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/admin/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.598981 edx-django-utils-5.6.0/edx_django_utils/admin/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/admin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/admin/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/admin/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.598981 edx-django-utils-5.6.0/edx_django_utils/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1400 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/cache/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.598981 edx-django-utils-5.6.0/edx_django_utils/cache/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/cache/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3191 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/cache/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12463 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/cache/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/cache/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.598981 edx-django-utils-5.6.0/edx_django_utils/db/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/db/queryset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4834 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/db/read_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.598981 edx-django-utils-5.6.0/edx_django_utils/db/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/db/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/db/tests/test_queryset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/db/tests/test_read_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.598981 edx-django-utils-5.6.0/edx_django_utils/ip/
+-rw-r--r--   0 runner    (1001) docker     (122)     7936 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/ip/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/ip/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10730 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/ip/internal/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/ip/internal/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/ip/internal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13591 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/ip/internal/tests/test_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/logging/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/logging/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/logging/internal/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7961 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/logging/internal/log_sensitive.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/logging/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/logging/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/logging/tests/test_log_sensitive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/logging/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/code_owner/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/code_owner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5260 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/code_owner/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10474 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/code_owner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22556 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3895 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/monitoring/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)    13423 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/scripts/new_relic_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8178 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.602981 edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/code_owner/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/code_owner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/code_owner/mock_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12959 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6352 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13563 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3016 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/monitoring/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/edx_django_utils/plugins/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3200 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/pluggable_override.py
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.594981 edx-django-utils-5.6.0/edx_django_utils/security/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/edx_django_utils/security/csp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/security/csp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5753 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/security/csp/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/edx_django_utils/security/csp/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4974 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/security/csp/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/edx_django_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/tests/test_pluggable_override.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/edx_django_utils/user/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/edx_django_utils/user/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/user/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/edx_django_utils/user/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/user/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/user/management/commands/manage_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6487 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/user/management/commands/manage_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/edx_django_utils/user/management/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/user/management/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7382 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/user/management/tests/test_manage_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7796 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/user/management/tests/test_manage_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/edx_django_utils/user/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/user/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/edx_django_utils/user/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.598981 edx-django-utils-5.6.0/edx_django_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-07-24 08:05:36.000000 edx-django-utils-5.6.0/edx_django_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-07-24 08:05:36.000000 edx-django-utils-5.6.0/edx_django_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 08:05:36.000000 edx-django-utils-5.6.0/edx_django_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-07-24 08:05:36.000000 edx-django-utils-5.6.0/edx_django_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 08:05:36.000000 edx-django-utils-5.6.0/edx_django_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-24 08:05:36.000000 edx-django-utils-5.6.0/edx_django_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-24 08:05:36.000000 edx-django-utils-5.6.0/edx_django_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5537 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:05:36.606981 edx-django-utils-5.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-24 08:05:32.000000 edx-django-utils-5.6.0/tests/test_models.py
```

### Comparing `edx-django-utils-5.5.0/CHANGELOG.rst` & `edx-django-utils-5.6.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,25 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+Added
+
+* Support added for Django 4.2
+
+[5.6.0] - 2023-07-24
+--------------------
+
+Changed
+~~~~~~~
+* Updated and renamed new_relic_nrql_search to search in text widgets as well as NRQL queries
+
 [5.5.0] - 2023-06-01
 --------------------
 
 Changed
 ~~~~~~~
 * Switched to ``sphinx-book-theme`` as the new standard theme across all Open
   edX repos.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
```

### Comparing `edx-django-utils-5.5.0/LICENSE.txt` & `edx-django-utils-5.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/PKG-INFO` & `edx-django-utils-5.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: edx-django-utils
-Version: 5.5.0
+Version: 5.6.0
 Summary: EdX utilities for Django Application development.
 Home-page: https://github.com/openedx/edx-django-utils
 Author: edX
 Author-email: oscm@edx.org
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -230,14 +231,25 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+Added
+
+* Support added for Django 4.2
+
+[5.6.0] - 2023-07-24
+--------------------
+
+Changed
+~~~~~~~
+* Updated and renamed new_relic_nrql_search to search in text widgets as well as NRQL queries
+
 [5.5.0] - 2023-06-01
 --------------------
 
 Changed
 ~~~~~~~
 * Switched to ``sphinx-book-theme`` as the new standard theme across all Open
   edX repos.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
```

### Comparing `edx-django-utils-5.5.0/README.rst` & `edx-django-utils-5.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/admin/mixins.py` & `edx-django-utils-5.6.0/edx_django_utils/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/admin/tests/test_mixins.py` & `edx-django-utils-5.6.0/edx_django_utils/admin/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/cache/middleware.py` & `edx-django-utils-5.6.0/edx_django_utils/cache/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/cache/tests/test_middleware.py` & `edx-django-utils-5.6.0/edx_django_utils/cache/tests/test_middleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Tests for the RequestCacheMiddleware.
 """
-from unittest.mock import MagicMock
+from unittest.mock import MagicMock, Mock
 
 from django.test import RequestFactory, TestCase
 
 from edx_django_utils.cache import middleware
 from edx_django_utils.cache.utils import FORCE_CACHE_MISS_PARAM, SHOULD_FORCE_CACHE_MISS_KEY, RequestCache
 
 TEST_KEY = "clobert"
@@ -13,15 +13,16 @@
 TEST_NAMESPACE = "test_namespace"
 
 
 class TestRequestCacheMiddleware(TestCase):  # pylint: disable=missing-class-docstring
 
     def setUp(self):
         super().setUp()
-        self.middleware = middleware.RequestCacheMiddleware()
+        self.mock_response = Mock()
+        self.middleware = middleware.RequestCacheMiddleware(self.mock_response)
         self.request = RequestFactory().get('/')
 
         self.request_cache = RequestCache()
         self.other_request_cache = RequestCache(TEST_NAMESPACE)
         self._dirty_request_cache()
 
     def test_process_request(self):
@@ -46,15 +47,16 @@
         self.other_request_cache.set(TEST_KEY, EXPECTED_VALUE)
 
 
 class TestTieredCacheMiddleware(TestCase):  # pylint: disable=missing-class-docstring
 
     def setUp(self):
         super().setUp()
-        self.middleware = middleware.TieredCacheMiddleware()
+        self.mock_response = Mock()
+        self.middleware = middleware.TieredCacheMiddleware(self.mock_response)
         self.request = RequestFactory().get('/')
         self.request.user = self._mock_user(is_staff=True)
 
         self.request_cache = RequestCache()
         self.request_cache.clear_all_namespaces()
 
     def test_process_request(self):
```

### Comparing `edx-django-utils-5.5.0/edx_django_utils/cache/tests/test_utils.py` & `edx-django-utils-5.6.0/edx_django_utils/cache/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/cache/utils.py` & `edx-django-utils-5.6.0/edx_django_utils/cache/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/db/queryset_utils.py` & `edx-django-utils-5.6.0/edx_django_utils/db/queryset_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/db/read_replica.py` & `edx-django-utils-5.6.0/edx_django_utils/db/read_replica.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/db/tests/test_queryset_utils.py` & `edx-django-utils-5.6.0/edx_django_utils/db/tests/test_queryset_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/db/tests/test_read_replica.py` & `edx-django-utils-5.6.0/edx_django_utils/db/tests/test_read_replica.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/ip/__init__.py` & `edx-django-utils-5.6.0/edx_django_utils/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/ip/internal/ip.py` & `edx-django-utils-5.6.0/edx_django_utils/ip/internal/ip.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/ip/internal/tests/test_ip.py` & `edx-django-utils-5.6.0/edx_django_utils/ip/internal/tests/test_ip.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/logging/internal/filters.py` & `edx-django-utils-5.6.0/edx_django_utils/logging/internal/filters.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/logging/internal/log_sensitive.py` & `edx-django-utils-5.6.0/edx_django_utils/logging/internal/log_sensitive.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/logging/tests/test_log_sensitive.py` & `edx-django-utils-5.6.0/edx_django_utils/logging/tests/test_log_sensitive.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/logging/tests/test_logging.py` & `edx-django-utils-5.6.0/edx_django_utils/logging/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/__init__.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/middleware.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/code_owner/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/utils.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/code_owner/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/middleware.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/transactions.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/transactions.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/utils.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/middleware.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/scripts/new_relic_nrql_search.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/scripts/new_relic_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
-This script takes a regex to search through the NRQL of New Relic alert policies
+This script takes a regex to search through the New Relic alert policies
 and New dashboards.
 
 This script makes use of New Relic's GraphQL API. See https://api.newrelic.com/graphiql.
 
 For help::
 
-    python edx_django_utils/monitoring/scripts/new_relic_nrql_search.py --help
+    python edx_django_utils/monitoring/scripts/new_relic_search.py --help
 
 """
 import json
 import os
 import re
 from string import Template
 
@@ -18,82 +18,117 @@
 import requests
 
 
 @click.command()
 @click.option(
     '--regex',
     required=True,
-    help="The regex to use to search NRQL in alert policies and dashboards.",
+    help="The regex to use to search in alert policies and dashboards.",
 )
 @click.option(
     '--policy_id',
     multiple=True,
     help="Optionally provide a specific policy id to check. Multiple can be supplied.",
 )
 @click.option(
     '--dashboard_guid',
     multiple=True,
     help="Optionally provide a specific dashboard guid to check. Multiple can be supplied.",
 )
-def main(regex, policy_id, dashboard_guid):
+@click.option(
+    '--skip_text_widgets',
+    is_flag=True,
+    default=False,
+    help="Optionally skip text widgets and only search NRQL in dashboards",
+)
+@click.option(
+    '--retries',
+    required=False,
+    default=1,
+    help="Optionally specify the number of times to retry a graphql request before exiting. Default is 1.",
+)
+def main(regex, policy_id, dashboard_guid, skip_text_widgets, retries):
     """
-    Search NRQL in New Relic alert policies and dashboards using regex.
+    Search NRQL and markdown in New Relic alert policies and dashboards using regex.
 
     Example usage:
 
-        new_relic_nrql_search.py --regex tnl
+        new_relic_search.py --regex tnl
 
     Note: The search ignores case since NRQL is case insensitive.
 
     Pre-requisite, set the following environment variable (in a safe way):
 
         NEW_RELIC_API_KEY=XXXXXXX
 
     See https://docs.newrelic.com/docs/apis/intro-apis/new-relic-api-keys/#user-api-key for details
     on setting an API key.
 
-    To skip alert policies or dashboards, just use a non-existent id, like --policy_id 0 or --dashboard_guid 0.
+    To skip alert policies or dashboards, just use a non-existent id, like --policy_id 0 or --dashboard_guid 0. To only
+    search NRQL and not markdown text, use --skip_text_widgets.
 
     """
     # Set environment variables
     api_key = os.environ['NEW_RELIC_API_KEY']
     headers = {
         "Content-Type": "application/json",
         "X-Api-Key": api_key,
     }
 
     compiled_regex = re.compile(regex)
 
-    account_ids = get_account_ids(headers)
+    account_ids = get_account_ids(headers, retries)
     for account_id in account_ids:
-        search_alert_policies(compiled_regex, account_id, headers, policy_id)
+        search_alert_policies(compiled_regex, account_id, headers, policy_id, retries)
     print()
-    search_dashboards(compiled_regex, headers, dashboard_guid)
+    search_dashboards(compiled_regex, headers, dashboard_guid, skip_text_widgets, retries)
     print(flush=True)
 
 
-def get_account_ids(headers):
+def get_with_retries(url, headers, params, retries):
+    response = requests.get(url, headers=headers, params=params)
+    # this is a bit silly but it allows us to retry on HTTP errors iff we have retries left
+    try:
+        response.raise_for_status()  # could be an HTTP error response
+    except requests.exceptions.HTTPError as http_error:
+        if retries == 0:
+            raise Exception from http_error
+        print(f"HTTPError when fetching request: {http_error}. Retrying")
+        return get_with_retries(url, headers, params, retries=retries-1)
+
+    response_data = response.json()
+
+    # sometimes errors come back as 'errors' in the data block instead of HTTP errors
+    errors = response_data['data'].get('errors', None)
+    if errors is not None and retries > 0:
+        print(f"Errors when fetching request: {errors}. Retrying")
+        return get_with_retries(url, headers, params, retries=retries-1)
+    else:
+        # if the response succeeded or we're at 0 retries, return whatever we got
+        return response_data
+
+
+def get_account_ids(headers, retries):
     """
     Returns a list of the New Relic account ids to be searched.
     """
-    response = requests.get(
+    response_data = get_with_retries(
         'https://api.newrelic.com/graphql',
-        headers=headers,
-        params={'query': """
+        headers,
+        {'query': """
             {
               actor {
                 accounts {
                   id
                 }
               }
             }
         """},
+        retries,
     )
-    response.raise_for_status()  # could be an error response
-    response_data = response.json()
     account_ids = [account['id'] for account in response_data['data']['actor']['accounts']]
     return account_ids
 
 
 # Template with variables:
 # - account_id
 # - cursor; can be null or cursor string
@@ -134,76 +169,74 @@
           }
         }
       }
     }
 """)
 
 
-def search_alert_policies(regex, account_id, headers, policy_id):
+def search_alert_policies(regex, account_id, headers, policy_id, retries):
     """
     Searches New Relic alert policy NRQL using the regex argument.
 
     Arguments:
         regex (re.Pattern): compiled regex used to compare against NRQL
         account_id (int): the id of the New Relic account in which to search.
         headers (dict): headers required to make http requests to New Relic.
         policy_id (tuple): optional tuple of policy ids supplied from the command-line.
+        retries (int): optional number of times to retry a failed request supplied from the command line. Default is 1.
     """
     policies = []
     cursor = 'null'
     while True:
-        response = requests.get(
+        response_data = get_with_retries(
             'https://api.newrelic.com/graphql',
-            headers=headers,
-            params={'query': ALERT_POLICY_LIST_TEMPLATE.substitute(
+            headers,
+            {'query': ALERT_POLICY_LIST_TEMPLATE.substitute(
                 account_id=account_id,
                 cursor=cursor
             )},
+            retries,
         )
-        response.raise_for_status()  # could be an error response
-        response_data = response.json()
         query_results = response_data['data']['actor']['account']['alerts']['policiesSearch']
         policies += query_results['policies']
         if not query_results['nextCursor']:
             break
         cursor = f"\"{query_results['nextCursor']}\""
     # Note: policy_id is an optional tuple of policy ids supplied from the command-line.
     if policy_id:
         policies = [policy for policy in policies if policy['id'] in policy_id]
     print(f"Searching for regex {regex.pattern} in {len(policies)} alert policies in account {account_id}...")
     policy_ids_printed = {}
     for policy in policies:
         print('.', end='', flush=True)
 
         # get the NRQL alert conditions from the alert policy
-        response = requests.get(
+        response_data = get_with_retries(
             'https://api.newrelic.com/graphql',
-            headers=headers,
-            params={'query': NRQL_ALERT_CONDITIONS_TEMPLATE.substitute(
+            headers,
+            {'query': NRQL_ALERT_CONDITIONS_TEMPLATE.substitute(
                 account_id=account_id,
                 policy_id=policy['id'],
             )},
+            retries,
         )
-        response.raise_for_status()  # could be an error response
-        response_data = response.json()
 
         nrql_conditions = response_data['data']['actor']['account']['alerts']['nrqlConditionsSearch']['nrqlConditions']
         for nrql_condition in nrql_conditions:
             nrql_query = nrql_condition['nrql']['query']
             if regex.search(nrql_query, re.IGNORECASE):
-
                 # Print the alert policy header for the first alert condition matched
                 if policy['id'] not in policy_ids_printed:
                     policy_ids_printed[policy['id']] = True
                     print('\n')
                     print(
                         f"Found in \"{policy['name']}\" "
                         # NOTE: The API doesn't provide a link to the policy, so this is a static link to
                         #   the alert policies home page.
-                        f"(policy_id={policy['id']}, search_link=https://one.nr/0X8woZOZvQx):"
+                        f"(policy_id={policy['id']}, search_link=https://onenr.io/0X8woZOZvQx):"
                     )
                     print('')
 
                 # Print the alert condition that matched
                 print(f"- {nrql_condition['name']}: {nrql_query}")
 
     if policy_ids_printed:
@@ -256,34 +289,35 @@
           }
         }
       }
     }
 """
 
 
-def search_dashboards(regex, headers, dashboard_guid):
+def search_dashboards(regex, headers, dashboard_guid, skip_text_widgets, retries):
     """
     Searches New Relic alert policy NRQL using the regex argument.
 
     Arguments:
         regex (re.Pattern): compiled regex used to compare against NRQL
         headers (dict): headers required to make http requests to New Relic
         dashboard_guid (tuple): optional tuple of dashboard guids supplied from the command-line.
+        skip_text_widgets (bool): optional flag to only search NRQL widgets, supplied from command line
+        retries (int): optional number of times to retry requests, supplied from the command line. Default is 1.
     """
     # load details of all dashboards
     dashboards = []
     cursor = 'null'
     while True:
-        response = requests.get(
+        response_data = get_with_retries(
             'https://api.newrelic.com/graphql',
-            headers=headers,
-            params={'query': DASHBOARD_LIST_QUERY_TEMPLATE.substitute(cursor=cursor)},
+            headers,
+            {'query': DASHBOARD_LIST_QUERY_TEMPLATE.substitute(cursor=cursor)},
+            retries,
         )
-        response.raise_for_status()  # could be an error response
-        response_data = response.json()
         query_results = response_data['data']['actor']['entitySearch']['results']
         dashboards += query_results['entities']
         if not query_results['nextCursor']:
             break
         cursor = f"\"{query_results['nextCursor']}\""
     # Filter out dashboard pages, which the dashboard entity query will not be able to find.
     # - Note: This could probably be handled in the original query, but not sure how.
@@ -291,49 +325,54 @@
     # Note: dashboard_guid is an optional tuple of dashboard guids supplied from the command-line.
     if dashboard_guid:
         dashboards = [dashboard for dashboard in dashboards if dashboard['guid'] in dashboard_guid]
     print(f"Searching for regex {regex.pattern} in {len(dashboards)} dashboards...")
     dashboard_guids_printed = {}
     for dashboard in dashboards:
         print('.', end='', flush=True)
+        found = False
 
         # get the dashboard details
-        response = requests.get(
+        response_data = get_with_retries(
             'https://api.newrelic.com/graphql',
-            headers=headers,
-            params={
+            headers,
+            {
                 'query': DASHBOARD_ENTITY_QUERY,
                 'variables': json.dumps({'guids': dashboard['guid']}),
-            }
+            },
+            retries,
         )
-        response.raise_for_status()  # could be an error response
-        response_data = response.json()
 
         if response_data['data']['actor']['entities'][0]['pages']:
             for page in response_data['data']['actor']['entities'][0]['pages']:
                 for widget in page['widgets']:
-                    if 'nrqlQueries' not in widget['rawConfiguration']:
-                        continue
-
-                    for nrql_query in widget['rawConfiguration']['nrqlQueries']:
-                        query = nrql_query['query']
-                        if regex.search(query, re.IGNORECASE):
-
-                            # Print the dashboard header for the first widget nrql that matches
-                            if dashboard['guid'] not in dashboard_guids_printed:
-                                dashboard_guids_printed[dashboard['guid']] = True
-                                print('\n')
-                                print(
-                                    f"Found in \"{dashboard['name']}\" "
-                                    f"(guid={dashboard['guid']}, link={dashboard['permalink']}):"
-                                )
-                                print('')
-
+                    found_text = None
+                    if 'text' in widget['rawConfiguration'] and not skip_text_widgets:
+                        widget_text = widget['rawConfiguration']['text']
+                        if regex.search(widget_text, re.IGNORECASE):
+                            found = True
+                            found_text = widget_text
+                    if 'nrqlQueries' in widget['rawConfiguration']:
+                        for nrql_query in widget['rawConfiguration']['nrqlQueries']:
+                            query = nrql_query['query']
+                            if regex.search(query, re.IGNORECASE):
+                                found = True
+                                found_text = query
+                    # Print the dashboard header for the first widget/nrql that matches
+                    if found:
+                        if dashboard['guid'] not in dashboard_guids_printed:
+                            dashboard_guids_printed[dashboard['guid']] = True
+                            print('\n')
+                            print(
+                                f"Found in \"{dashboard['name']}\" "
+                                f"(guid={dashboard['guid']}, link={dashboard['permalink']}):"
+                            )
+                            print('')
                             # Print the widget NRQL that matches
-                            print(f"- {widget['title']}: {query}")
+                        print(f"- {widget['title']}: {found_text}")
 
     if dashboard_guids_printed:
         command_line = ''
         for dashboard_guid in dashboard_guids_printed.keys():
             command_line += f'--dashboard_guid {dashboard_guid} '
         print("\n\nRun again with found dashboards: {}".format(command_line))
     else:
```

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Tests for CachedCustomMonitoringMiddleware and associated utilities.
 
 Note: See test_middleware.py for the rest of the middleware tests.
 """
-from unittest.mock import call, patch
+from unittest.mock import Mock, call, patch
 
 import ddt
 from django.test import TestCase
 
 from edx_django_utils.cache import RequestCache
 from edx_django_utils.monitoring import (
     CachedCustomMonitoringMiddleware,
@@ -28,14 +28,15 @@
 @ddt.ddt
 class TestCustomMonitoringMiddleware(TestCase):
     """
     Test the monitoring_utils middleware and helpers
     """
     def setUp(self):
         super().setUp()
+        self.mock_response = Mock()
         RequestCache.clear_all_namespaces()
 
     @patch('newrelic.agent')
     @ddt.data(
         (CachedCustomMonitoringMiddleware, False, 'process_response'),
         (CachedCustomMonitoringMiddleware, False, 'process_exception'),
         (DeprecatedCachedCustomMonitoringMiddleware, True, 'process_response'),
@@ -58,15 +59,15 @@
         nr_agent_calls_expected = [
             call('hello', 10),
             call('world', 20),
             call('foo', 2),
         ]
 
         # fake a response to trigger attributes reporting
-        middleware_method = getattr(cached_monitoring_middleware_class(), middleware_method_name)
+        middleware_method = getattr(cached_monitoring_middleware_class(self.mock_response), middleware_method_name)
         middleware_method(
             'fake request',
             'fake response',
         )
 
         # Assert call counts to newrelic.agent.add_custom_parameter()
         expected_call_count = len(nr_agent_calls_expected)
@@ -97,16 +98,17 @@
 
         # based on the metric data above, we expect the following calls to newrelic:
         nr_agent_calls_expected = [
             call('hello', None),
             call('error_adding_accumulated_metric', 'name=hello, new_value=10, cached_value=None'),
         ]
 
+        self.mock_response = Mock()
         # fake a response to trigger metrics reporting
-        cached_monitoring_middleware_class().process_response(
+        cached_monitoring_middleware_class(self.mock_response).process_response(
             'fake request',
             'fake response',
         )
 
         # Assert call counts to newrelic.agent.add_custom_parameter()
         expected_call_count = len(nr_agent_calls_expected)
         if is_deprecated:
```

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_middleware.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/test_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,27 @@
 class TestMonitoringMemoryMiddleware(TestCase):
     """
     Tests for MonitoringMemoryMiddleware
     """
     @override_switch('edx_django_utils.monitoring.enable_memory_middleware', False)
     @patch('edx_django_utils.monitoring.internal.middleware.log')
     def test_memory_monitoring_when_disabled(self, mock_logger):
-        MonitoringMemoryMiddleware().process_response(
+        mock_response = Mock()
+        MonitoringMemoryMiddleware(mock_response).process_response(
             'fake request',
             'fake response',
         )
         mock_logger.info.assert_not_called()
 
     @override_switch('edx_django_utils.monitoring.enable_memory_middleware', True)
     @patch('edx_django_utils.monitoring.internal.middleware.log')
     def test_memory_monitoring_when_enabled(self, mock_logger):
         request = RequestFactory().get('/')
-        MonitoringMemoryMiddleware().process_response(
+        mock_response = Mock()
+        MonitoringMemoryMiddleware(mock_response).process_response(
             request,
             'fake response',
         )
         mock_logger.info.assert_called()
 
 
 class TestDeploymentMonitoringMiddleware(TestCase):
```

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_utils.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/monitoring/utils.py` & `edx-django-utils-5.6.0/edx_django_utils/monitoring/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/plugins/__init__.py` & `edx-django-utils-5.6.0/edx_django_utils/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/plugins/constants.py` & `edx-django-utils-5.6.0/edx_django_utils/plugins/constants.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/plugins/pluggable_override.py` & `edx-django-utils-5.6.0/edx_django_utils/plugins/pluggable_override.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_apps.py` & `edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_apps.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_contexts.py` & `edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_manager.py` & `edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_settings.py` & `edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_signals.py` & `edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_signals.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_urls.py` & `edx-django-utils-5.6.0/edx_django_utils/plugins/plugin_urls.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/plugins/utils.py` & `edx-django-utils-5.6.0/edx_django_utils/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/security/csp/middleware.py` & `edx-django-utils-5.6.0/edx_django_utils/security/csp/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/security/csp/tests/test_middleware.py` & `edx-django-utils-5.6.0/edx_django_utils/security/csp/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/tests/test_pluggable_override.py` & `edx-django-utils-5.6.0/edx_django_utils/tests/test_pluggable_override.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/user/__init__.py` & `edx-django-utils-5.6.0/edx_django_utils/user/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/user/management/commands/manage_group.py` & `edx-django-utils-5.6.0/edx_django_utils/user/management/commands/manage_group.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/user/management/commands/manage_user.py` & `edx-django-utils-5.6.0/edx_django_utils/user/management/commands/manage_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/user/management/tests/test_manage_group.py` & `edx-django-utils-5.6.0/edx_django_utils/user/management/tests/test_manage_group.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/user/management/tests/test_manage_user.py` & `edx-django-utils-5.6.0/edx_django_utils/user/management/tests/test_manage_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils/user/tests/test_user.py` & `edx-django-utils-5.6.0/edx_django_utils/user/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/edx_django_utils.egg-info/PKG-INFO` & `edx-django-utils-5.6.0/edx_django_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: edx-django-utils
-Version: 5.5.0
+Version: 5.6.0
 Summary: EdX utilities for Django Application development.
 Home-page: https://github.com/openedx/edx-django-utils
 Author: edX
 Author-email: oscm@edx.org
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -230,14 +231,25 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+Added
+
+* Support added for Django 4.2
+
+[5.6.0] - 2023-07-24
+--------------------
+
+Changed
+~~~~~~~
+* Updated and renamed new_relic_nrql_search to search in text widgets as well as NRQL queries
+
 [5.5.0] - 2023-06-01
 --------------------
 
 Changed
 ~~~~~~~
 * Switched to ``sphinx-book-theme`` as the new standard theme across all Open
   edX repos.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
```

### Comparing `edx-django-utils-5.5.0/edx_django_utils.egg-info/SOURCES.txt` & `edx-django-utils-5.6.0/edx_django_utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 edx_django_utils/monitoring/internal/__init__.py
 edx_django_utils/monitoring/internal/middleware.py
 edx_django_utils/monitoring/internal/transactions.py
 edx_django_utils/monitoring/internal/utils.py
 edx_django_utils/monitoring/internal/code_owner/__init__.py
 edx_django_utils/monitoring/internal/code_owner/middleware.py
 edx_django_utils/monitoring/internal/code_owner/utils.py
-edx_django_utils/monitoring/scripts/new_relic_nrql_search.py
+edx_django_utils/monitoring/scripts/new_relic_search.py
 edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py
 edx_django_utils/monitoring/tests/__init__.py
 edx_django_utils/monitoring/tests/test_custom_monitoring.py
 edx_django_utils/monitoring/tests/test_middleware.py
 edx_django_utils/monitoring/tests/test_utils.py
 edx_django_utils/monitoring/tests/code_owner/__init__.py
 edx_django_utils/monitoring/tests/code_owner/mock_views.py
```

### Comparing `edx-django-utils-5.5.0/requirements/base.in` & `edx-django-utils-5.6.0/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/requirements/constraints.txt` & `edx-django-utils-5.6.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.5.0/setup.py` & `edx-django-utils-5.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     },
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
 )
```

