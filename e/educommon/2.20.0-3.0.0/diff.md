# Comparing `tmp/educommon-2.20.0.tar.gz` & `tmp/educommon-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "educommon-2.20.0.tar", last modified: Tue Jul 18 06:09:32 2023, max compression
+gzip compressed data, was "educommon-3.0.0.tar", last modified: Mon Jul 24 05:37:24 2023, max compression
```

## Comparing `educommon-2.20.0.tar` & `educommon-3.0.0.tar`

### file list

```diff
@@ -1,427 +1,435 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.708430 educommon-2.20.0/
--rw-r--r--   0 root         (0) root         (0)   110498 2023-07-18 06:09:18.000000 educommon-2.20.0/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)      102 2022-07-05 14:23:59.000000 educommon-2.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-18 06:09:32.707430 educommon-2.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2022-07-05 14:23:59.000000 educommon-2.20.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     1981 2022-07-05 14:23:59.000000 educommon-2.20.0/UPGRADE.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 06:09:32.708430 educommon-2.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2466 2022-07-05 14:23:59.000000 educommon-2.20.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.345430 educommon-2.20.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.361430 educommon-2.20.0/src/educommon/
--rw-r--r--   0 root         (0) root         (0)      475 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.366430 educommon-2.20.0/src/educommon/about/
--rw-r--r--   0 root         (0) root         (0)     2685 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/README.rst
--rw-r--r--   0 root         (0) root         (0)      149 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/__init__.py
--rw-r--r--   0 root         (0) root         (0)      346 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.345430 educommon-2.20.0/src/educommon/about/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.367430 educommon-2.20.0/src/educommon/about/static/edu_about/
--rw-r--r--   0 root         (0) root         (0)     8382 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/static/edu_about/barsgroup.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.375430 educommon-2.20.0/src/educommon/about/ui/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      535 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/about-window.js
--rw-r--r--   0 root         (0) root         (0)     6090 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/actions.py
--rw-r--r--   0 root         (0) root         (0)      700 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/common-tab.html
--rw-r--r--   0 root         (0) root         (0)    11192 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/packages-tab.js
--rw-r--r--   0 root         (0) root         (0)      129 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/postgresql-extensions-tab.js
--rw-r--r--   0 root         (0) root         (0)     5381 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/ui.py
--rw-r--r--   0 root         (0) root         (0)      718 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.380430 educommon-2.20.0/src/educommon/async_tasks/
--rw-r--r--   0 root         (0) root         (0)      166 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)      146 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/apps.py
--rw-r--r--   0 root         (0) root         (0)      267 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.382430 educommon-2.20.0/src/educommon/async_tasks/fixtures/
--rw-r--r--   0 root         (0) root         (0)      303 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/fixtures/initial_data.json
--rw-r--r--   0 root         (0) root         (0)     3468 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/locks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.385430 educommon-2.20.0/src/educommon/async_tasks/migrations/
--rw-r--r--   0 root         (0) root         (0)     4309 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      603 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/migrations/0002_load_initial_data.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3618 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/models.py
--rw-r--r--   0 root         (0) root         (0)     1487 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/statuses.py
--rw-r--r--   0 root         (0) root         (0)    11236 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.394430 educommon-2.20.0/src/educommon/audit_log/
--rw-r--r--   0 root         (0) root         (0)     2829 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5924 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/actions.py
--rw-r--r--   0 root         (0) root         (0)      302 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     4994 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/apps.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.395430 educommon-2.20.0/src/educommon/audit_log/error_log/
--rw-r--r--   0 root         (0) root         (0)      153 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/error_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2310 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/error_log/actions.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.396430 educommon-2.20.0/src/educommon/audit_log/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.396430 educommon-2.20.0/src/educommon/audit_log/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/management/commands/reinstall_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1187 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.405430 educommon-2.20.0/src/educommon/audit_log/migrations/
--rw-r--r--   0 root         (0) root         (0)     4547 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     2907 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0002_install_audit_log.py
--rw-r--r--   0 root         (0) root         (0)      492 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0003_logproxy.py
--rw-r--r--   0 root         (0) root         (0)      342 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0004_reinstall_audit_log.py
--rw-r--r--   0 root         (0) root         (0)      769 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0005_postgresql_error.py
--rw-r--r--   0 root         (0) root         (0)      669 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py
--rw-r--r--   0 root         (0) root         (0)     1472 2022-07-08 03:53:12.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8272 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/models.py
--rw-r--r--   0 root         (0) root         (0)     1307 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/permissions.py
--rw-r--r--   0 root         (0) root         (0)     8820 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/proxies.py
--rw-r--r--   0 root         (0) root         (0)      251 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/routers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.409430 educommon-2.20.0/src/educommon/audit_log/sql/
--rw-r--r--   0 root         (0) root         (0)     1395 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/sql/configure_audit_log.sql
--rw-r--r--   0 root         (0) root         (0)      431 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/sql/configure_selective_audit_log.sql
--rw-r--r--   0 root         (0) root         (0)     1841 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/sql/create_selective_tables_function.sql
--rw-r--r--   0 root         (0) root         (0)    14310 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/sql/install_audit_log.sql
--rw-r--r--   0 root         (0) root         (0)     2137 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.410430 educommon-2.20.0/src/educommon/audit_log/utils/
--rw-r--r--   0 root         (0) root         (0)    12583 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/utils/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.411430 educommon-2.20.0/src/educommon/auth/
--rw-r--r--   0 root         (0) root         (0)      135 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.425430 educommon-2.20.0/src/educommon/auth/rbac/
--rw-r--r--   0 root         (0) root         (0)      378 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27149 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/actions.py
--rw-r--r--   0 root         (0) root         (0)      473 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/app_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.429430 educommon-2.20.0/src/educommon/auth/rbac/backends/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3082 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/backends/base.py
--rw-r--r--   0 root         (0) root         (0)    10328 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/backends/caching.py
--rw-r--r--   0 root         (0) root         (0)     5066 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/backends/simple.py
--rw-r--r--   0 root         (0) root         (0)     3016 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/checker.py
--rw-r--r--   0 root         (0) root         (0)     1154 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/config.py
--rw-r--r--   0 root         (0) root         (0)      562 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.432430 educommon-2.20.0/src/educommon/auth/rbac/management/
--rw-r--r--   0 root         (0) root         (0)      127 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.433430 educommon-2.20.0/src/educommon/auth/rbac/management/commands/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5551 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/management/commands/rbac.py
--rw-r--r--   0 root         (0) root         (0)    16332 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.435430 educommon-2.20.0/src/educommon/auth/rbac/migrations/
--rw-r--r--   0 root         (0) root         (0)     5578 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      681 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py
--rw-r--r--   0 root         (0) root         (0)      574 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/migrations/0003_permission_hidden.py
--rw-r--r--   0 root         (0) root         (0)     2181 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15466 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/models.py
--rw-r--r--   0 root         (0) root         (0)      927 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.348430 educommon-2.20.0/src/educommon/auth/rbac/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.439430 educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/
--rw-r--r--   0 root         (0) root         (0)      335 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/role-add-window.js
--rw-r--r--   0 root         (0) root         (0)     7914 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/role-edit-window.js
--rw-r--r--   0 root         (0) root         (0)     3768 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/roles-list-window.js
--rw-r--r--   0 root         (0) root         (0)      536 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js
--rw-r--r--   0 root         (0) root         (0)    15794 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/ui.py
--rw-r--r--   0 root         (0) root         (0)     7929 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/utils.py
--rw-r--r--   0 root         (0) root         (0)      513 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.446430 educommon-2.20.0/src/educommon/auth/simple_auth/
--rw-r--r--   0 root         (0) root         (0)      289 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11903 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/actions.py
--rw-r--r--   0 root         (0) root         (0)     1112 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     2587 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/checkers.py
--rw-r--r--   0 root         (0) root         (0)      453 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.447430 educommon-2.20.0/src/educommon/auth/simple_auth/migrations/
--rw-r--r--   0 root         (0) root         (0)     1491 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      745 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.348430 educommon-2.20.0/src/educommon/auth/simple_auth/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.448430 educommon-2.20.0/src/educommon/auth/simple_auth/static/simple_auth/
--rw-r--r--   0 root         (0) root         (0)      123 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/static/simple_auth/simple_auth.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.349430 educommon-2.20.0/src/educommon/auth/simple_auth/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.450430 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/
--rw-r--r--   0 root         (0) root         (0)     1577 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.451430 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/email/
--rw-r--r--   0 root         (0) root         (0)      635 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html
--rw-r--r--   0 root         (0) root         (0)     1444 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html
--rw-r--r--   0 root         (0) root         (0)     1340 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html
--rw-r--r--   0 root         (0) root         (0)     4676 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/ui.py
--rw-r--r--   0 root         (0) root         (0)      270 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.456430 educommon-2.20.0/src/educommon/contingent/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3074 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/actions.py
--rw-r--r--   0 root         (0) root         (0)      309 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     6968 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/base.py
--rw-r--r--   0 root         (0) root         (0)    60706 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/catalogs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.465430 educommon-2.20.0/src/educommon/contingent/contingent_plugin/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      721 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/actions.py
--rw-r--r--   0 root         (0) root         (0)      711 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.467430 educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/
--rw-r--r--   0 root         (0) root         (0)     1680 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     1241 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      893 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/model_views.py
--rw-r--r--   0 root         (0) root         (0)     2495 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/models.py
--rw-r--r--   0 root         (0) root         (0)     5296 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/observer.py
--rw-r--r--   0 root         (0) root         (0)      205 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/plugin_meta.py
--rw-r--r--   0 root         (0) root         (0)     3311 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/storage.py
--rw-r--r--   0 root         (0) root         (0)     7094 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.471430 educommon-2.20.0/src/educommon/contingent/json_data/
--rw-r--r--   0 root         (0) root         (0)    53540 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/json_data/okogu.json
--rw-r--r--   0 root         (0) root         (0)    30723 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/json_data/oksm.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.472430 educommon-2.20.0/src/educommon/django/
--rw-r--r--   0 root         (0) root         (0)      125 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.479430 educommon-2.20.0/src/educommon/django/db/
--rw-r--r--   0 root         (0) root         (0)      129 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7092 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.481430 educommon-2.20.0/src/educommon/django/db/migration/
--rw-r--r--   0 root         (0) root         (0)     1882 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9734 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/migration/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.484430 educommon-2.20.0/src/educommon/django/db/mixins/
--rw-r--r--   0 root         (0) root         (0)    14747 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/django/db/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24890 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/mixins/date_interval.py
--rw-r--r--   0 root         (0) root         (0)    12510 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/mixins/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.487430 educommon-2.20.0/src/educommon/django/db/model_view/
--rw-r--r--   0 root         (0) root         (0)    12516 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/model_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/model_view/table-view.html
--rw-r--r--   0 root         (0) root         (0)     2107 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/django/db/models.py
--rw-r--r--   0 root         (0) root         (0)    11197 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/observer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.491430 educommon-2.20.0/src/educommon/django/db/partitioning/
--rw-r--r--   0 root         (0) root         (0)     4455 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/README.md
--rw-r--r--   0 root         (0) root         (0)    22512 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.491430 educommon-2.20.0/src/educommon/django/db/partitioning/management/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.497430 educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py
--rw-r--r--   0 root         (0) root         (0)     2280 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/clear_table.py
--rw-r--r--   0 root         (0) root         (0)     2127 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/split_table.py
--rw-r--r--   0 root         (0) root         (0)    20345 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/partitioning.sql
--rw-r--r--   0 root         (0) root         (0)     3401 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/triggers.sql
--rw-r--r--   0 root         (0) root         (0)     3274 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/routers.py
--rw-r--r--   0 root         (0) root         (0)     9489 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.499430 educommon-2.20.0/src/educommon/django/db/validators/
--rw-r--r--   0 root         (0) root         (0)     2084 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/validators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38870 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/validators/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.502430 educommon-2.20.0/src/educommon/django/storages/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.513430 educommon-2.20.0/src/educommon/django/storages/atcfs/
--rw-r--r--   0 root         (0) root         (0)     2656 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/README.rst
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6079 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/api.py
--rw-r--r--   0 root         (0) root         (0)      435 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/app_meta.py
--rw-r--r--   0 root         (0) root         (0)      172 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.515430 educommon-2.20.0/src/educommon/django/storages/atcfs/management/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.517430 educommon-2.20.0/src/educommon/django/storages/atcfs/management/commands/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7567 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py
--rw-r--r--   0 root         (0) root         (0)      207 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/models.py
--rw-r--r--   0 root         (0) root         (0)     3108 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/monkey_patching.py
--rw-r--r--   0 root         (0) root         (0)      847 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/settings.py
--rw-r--r--   0 root         (0) root         (0)     4135 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.518430 educommon-2.20.0/src/educommon/django/storages/atcfs/templates/
--rw-r--r--   0 root         (0) root         (0)      196 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/templates/atcfs_unavailable.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.519430 educommon-2.20.0/src/educommon/extjs/
--rw-r--r--   0 root         (0) root         (0)      143 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/extjs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.520430 educommon-2.20.0/src/educommon/extjs/fields/
--rw-r--r--   0 root         (0) root         (0)      166 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/extjs/fields/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/extjs/fields/input_params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.538430 educommon-2.20.0/src/educommon/importer/
--rw-r--r--   0 root         (0) root         (0)    37974 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/XLSReader.py
--rw-r--r--   0 root         (0) root         (0)      140 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13456 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/api.py
--rw-r--r--   0 root         (0) root         (0)      798 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/constants.py
--rw-r--r--   0 root         (0) root         (0)    10392 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/loggers.py
--rw-r--r--   0 root         (0) root         (0)    37557 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/proxy.py
--rw-r--r--   0 root         (0) root         (0)     6315 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/proxy_import.py
--rw-r--r--   0 root         (0) root         (0)     2087 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/refactoring-notes.txt
--rw-r--r--   0 root         (0) root         (0)     1585 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/report.py
--rw-r--r--   0 root         (0) root         (0)     8704 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/test_file.xls
--rw-r--r--   0 root         (0) root         (0)     3983 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/ui.py
--rw-r--r--   0 root         (0) root         (0)     1306 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.541430 educommon-2.20.0/src/educommon/integration_entities/
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/README.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      448 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/consts.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/entities.py
--rw-r--r--   0 root         (0) root         (0)      335 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/enums.py
--rw-r--r--   0 root         (0) root         (0)     8675 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/helpers.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.541430 educommon-2.20.0/src/educommon/ioc/
--rw-r--r--   0 root         (0) root         (0)     4098 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ioc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.544430 educommon-2.20.0/src/educommon/m3/
--rw-r--r--   0 root         (0) root         (0)    17732 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.546430 educommon-2.20.0/src/educommon/m3/extensions/
--rw-r--r--   0 root         (0) root         (0)      269 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.547430 educommon-2.20.0/src/educommon/m3/extensions/listeners/
--rw-r--r--   0 root         (0) root         (0)     9021 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.553430 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/__init__.py
--rw-r--r--   0 root         (0) root         (0)      916 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js
--rw-r--r--   0 root         (0) root         (0)     6145 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/listeners.py
--rw-r--r--   0 root         (0) root         (0)     7648 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/mixins.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/related-objects-window.html
--rw-r--r--   0 root         (0) root         (0)      474 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/signals.py
--rw-r--r--   0 root         (0) root         (0)     3529 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/ui.py
--rw-r--r--   0 root         (0) root         (0)     3026 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/utils.py
--rw-r--r--   0 root         (0) root         (0)     6971 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/ui.py
--rw-r--r--   0 root         (0) root         (0)     5187 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/transaction_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.556430 educommon-2.20.0/src/educommon/objectpack/
--rw-r--r--   0 root         (0) root         (0)      126 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14370 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/actions.py
--rw-r--r--   0 root         (0) root         (0)      268 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.562430 educommon-2.20.0/src/educommon/objectpack/templates/
--rw-r--r--   0 root         (0) root         (0)      437 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/base-grid-window.js
--rw-r--r--   0 root         (0) root         (0)     1408 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/filter-panel.js
--rw-r--r--   0 root         (0) root         (0)     1544 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/grid-panel.js
--rw-r--r--   0 root         (0) root         (0)     1842 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/multiSelectWindow.js
--rw-r--r--   0 root         (0) root         (0)     6741 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/multiselect-page-fix.js
--rw-r--r--   0 root         (0) root         (0)     1838 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/relations-check-mixin-template.html
--rw-r--r--   0 root         (0) root         (0)    15059 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.566430 educommon-2.20.0/src/educommon/report/
--rw-r--r--   0 root         (0) root         (0)    18050 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8846 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.580430 educommon-2.20.0/src/educommon/report/constructor/
--rw-r--r--   0 root         (0) root         (0)     1138 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/README.rst
--rw-r--r--   0 root         (0) root         (0)     1300 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      211 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/app_meta.py
--rw-r--r--   0 root         (0) root         (0)      424 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/apps.py
--rw-r--r--   0 root         (0) root         (0)    26060 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.581430 educommon-2.20.0/src/educommon/report/constructor/builders/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.587430 educommon-2.20.0/src/educommon/report/constructor/builders/excel/
--rw-r--r--   0 root         (0) root         (0)      160 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56385 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/_base.py
--rw-r--r--   0 root         (0) root         (0)     4843 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/_header.py
--rw-r--r--   0 root         (0) root         (0)       85 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/constants.py
--rw-r--r--   0 root         (0) root         (0)     6273 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/product.py
--rw-r--r--   0 root         (0) root         (0)     5182 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/with_merged_cells.py
--rw-r--r--   0 root         (0) root         (0)     1095 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/config.py
--rw-r--r--   0 root         (0) root         (0)     3540 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.594430 educommon-2.20.0/src/educommon/report/constructor/editor/
--rw-r--r--   0 root         (0) root         (0)       97 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/editor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39015 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/editor/actions.py
--rw-r--r--   0 root         (0) root         (0)    39225 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/editor/edit-window.js
--rw-r--r--   0 root         (0) root         (0)     3247 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/editor/list-window.js
--rw-r--r--   0 root         (0) root         (0)    24876 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/editor/ui.py
--rw-r--r--   0 root         (0) root         (0)     1353 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.611430 educommon-2.20.0/src/educommon/report/constructor/migrations/
--rw-r--r--   0 root         (0) root         (0)     3497 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     5113 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0002_report_filters.py
--rw-r--r--   0 root         (0) root         (0)      576 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0003_reportfilter_exclude.py
--rw-r--r--   0 root         (0) root         (0)     1473 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py
--rw-r--r--   0 root         (0) root         (0)      535 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0005_reportcolumn_visible.py
--rw-r--r--   0 root         (0) root         (0)     1388 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0006_reportsorting.py
--rw-r--r--   0 root         (0) root         (0)     1645 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0007_include_available_units.py
--rw-r--r--   0 root         (0) root         (0)      647 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py
--rw-r--r--   0 root         (0) root         (0)      623 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py
--rw-r--r--   0 root         (0) root         (0)      973 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2421 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/mixins.py
--rw-r--r--   0 root         (0) root         (0)    18818 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/models.py
--rw-r--r--   0 root         (0) root         (0)      171 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/plugin_meta.py
--rw-r--r--   0 root         (0) root         (0)     1948 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/registries.py
--rw-r--r--   0 root         (0) root         (0)     6918 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/utils.py
--rw-r--r--   0 root         (0) root         (0)      536 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/validators.py
--rw-r--r--   0 root         (0) root         (0)    10100 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/reporter.py
--rw-r--r--   0 root         (0) root         (0)    10124 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.618430 educommon-2.20.0/src/educommon/rest/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1264 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/actions.py
--rw-r--r--   0 root         (0) root         (0)     3887 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/context.py
--rw-r--r--   0 root         (0) root         (0)     2525 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/controllers.py
--rw-r--r--   0 root         (0) root         (0)      493 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/misc.py
--rw-r--r--   0 root         (0) root         (0)     4888 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.622430 educommon-2.20.0/src/educommon/secure_media/
--rw-r--r--   0 root         (0) root         (0)     4001 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/secure_media/README.rst
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/secure_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1318 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/secure_media/app_meta.py
--rw-r--r--   0 root         (0) root         (0)      108 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/thread_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.632430 educommon-2.20.0/src/educommon/utils/
--rw-r--r--   0 root         (0) root         (0)     2508 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4066 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/caching.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/conversion.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/crypto.py
--rw-r--r--   0 root         (0) root         (0)     9133 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/date.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.634430 educommon-2.20.0/src/educommon/utils/db/
--rw-r--r--   0 root         (0) root         (0)     7729 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2886 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/db/postgresql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.657430 educommon-2.20.0/src/educommon/utils/fonts/
--rw-r--r--   0 root         (0) root         (0)   275572 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/fonts/Arial.ttf
--rw-r--r--   0 root         (0) root         (0)   811820 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/fonts/Calibri.ttf
--rw-r--r--   0 root         (0) root         (0)   265528 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/fonts/Tahoma.ttf
--rw-r--r--   0 root         (0) root         (0)     4875 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.659430 educommon-2.20.0/src/educommon/utils/licence/
--rw-r--r--   0 root         (0) root         (0)     5217 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/licence/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1230 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/licence/converters.py
--rw-r--r--   0 root         (0) root         (0)     3445 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)     1238 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/patches.py
--rw-r--r--   0 root         (0) root         (0)     9547 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/plugins.py
--rw-r--r--   0 root         (0) root         (0)     2021 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/registry.py
--rw-r--r--   0 root         (0) root         (0)      520 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/seqtools.py
--rw-r--r--   0 root         (0) root         (0)     8848 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/serializer.py
--rw-r--r--   0 root         (0) root         (0)     2907 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/storage.py
--rw-r--r--   0 root         (0) root         (0)     2863 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.660430 educommon-2.20.0/src/educommon/utils/system_app/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.662430 educommon-2.20.0/src/educommon/utils/system_app/management/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.663430 educommon-2.20.0/src/educommon/utils/system_app/management/commands/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9513 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/management/commands/delete_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.664430 educommon-2.20.0/src/educommon/utils/system_app/templatetags/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      312 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/templatetags/educommon.py
--rw-r--r--   0 root         (0) root         (0)    14374 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.670430 educommon-2.20.0/src/educommon/utils/xml/
--rw-r--r--   0 root         (0) root         (0)     2243 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/catalog.json
--rw-r--r--   0 root         (0) root         (0)     1760 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/resolver.py
--rw-r--r--   0 root         (0) root         (0)    13160 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd
--rw-r--r--   0 root         (0) root         (0)    13465 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd
--rw-r--r--   0 root         (0) root         (0)     5234 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/xenc-schema.xsd
--rw-r--r--   0 root         (0) root         (0)    10293 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/xmldsig-core-schema.xsd
--rw-r--r--   0 root         (0) root         (0)      450 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon/version.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.676430 educommon-2.20.0/src/educommon/ws_log/
--rw-r--r--   0 root         (0) root         (0)     5467 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/README.rst
--rw-r--r--   0 root         (0) root         (0)     1013 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9269 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/actions.py
--rw-r--r--   0 root         (0) root         (0)      150 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     7369 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.681430 educommon-2.20.0/src/educommon/ws_log/migrations/
--rw-r--r--   0 root         (0) root         (0)     2810 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     1014 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py
--rw-r--r--   0 root         (0) root         (0)     1786 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py
--rw-r--r--   0 root         (0) root         (0)     1036 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py
--rw-r--r--   0 root         (0) root         (0)     1690 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py
--rw-r--r--   0 root         (0) root         (0)      583 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0006_auto_20170327_1027.py
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py
--rw-r--r--   0 root         (0) root         (0)     1376 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py
--rw-r--r--   0 root         (0) root         (0)      581 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5781 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/models.py
--rw-r--r--   0 root         (0) root         (0)      925 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/provider.py
--rw-r--r--   0 root         (0) root         (0)     3483 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.684430 educommon-2.20.0/src/educommon/ws_log/smev/
--rw-r--r--   0 root         (0) root         (0)      140 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/smev/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5871 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/smev/applications.py
--rw-r--r--   0 root         (0) root         (0)      673 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/smev/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.356430 educommon-2.20.0/src/educommon/ws_log/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.685430 educommon-2.20.0/src/educommon/ws_log/templates/report/
--rw-r--r--   0 root         (0) root         (0)    10439 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/templates/report/smev_logs.xlsx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.687430 educommon-2.20.0/src/educommon/ws_log/templates/ui-js/
--rw-r--r--   0 root         (0) root         (0)      513 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js
--rw-r--r--   0 root         (0) root         (0)     1103 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js
--rw-r--r--   0 root         (0) root         (0)     4147 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/ui.py
--rw-r--r--   0 root         (0) root         (0)     1800 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.362430 educommon-2.20.0/src/educommon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15274 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.707430 educommon-2.20.0/tests/
--rw-r--r--   0 root         (0) root         (0)     6381 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_contingent_plugin_utils.py
--rw-r--r--   0 root         (0) root         (0)     2611 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_delete_check.py
--rw-r--r--   0 root         (0) root         (0)     5074 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_delete_objects.py
--rw-r--r--   0 root         (0) root         (0)     3226 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_django_db_utils.py
--rw-r--r--   0 root         (0) root         (0)    21913 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_interval_mixins.py
--rw-r--r--   0 root         (0) root         (0)     1916 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_patches.py
--rw-r--r--   0 root         (0) root         (0)     7105 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_personal_data_fields.py
--rw-r--r--   0 root         (0) root         (0)    14782 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_report.py
--rw-r--r--   0 root         (0) root         (0)     1727 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_service_db_router.py
--rw-r--r--   0 root         (0) root         (0)     2363 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2198 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_utils_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8531 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_validators.py
--rw-r--r--   0 root         (0) root         (0)     6443 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/tests_rbac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.812141 educommon-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      102 2022-07-05 14:23:59.000000 educommon-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-24 05:37:24.811141 educommon-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2022-07-05 14:23:59.000000 educommon-3.0.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1981 2022-07-05 14:23:59.000000 educommon-3.0.0/UPGRADE.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 05:37:24.812141 educommon-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-07-24 05:37:11.000000 educommon-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.622141 educommon-3.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.639141 educommon-3.0.0/src/educommon/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.642141 educommon-3.0.0/src/educommon/about/
+-rw-r--r--   0 root         (0) root         (0)     2685 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/README.rst
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      259 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.622141 educommon-3.0.0/src/educommon/about/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.643141 educommon-3.0.0/src/educommon/about/static/edu_about/
+-rw-r--r--   0 root         (0) root         (0)     8382 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/static/edu_about/barsgroup.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.649141 educommon-3.0.0/src/educommon/about/ui/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      535 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/ui/about-window.js
+-rw-r--r--   0 root         (0) root         (0)     5975 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/ui/actions.py
+-rw-r--r--   0 root         (0) root         (0)      700 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/ui/common-tab.html
+-rw-r--r--   0 root         (0) root         (0)    11192 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/ui/packages-tab.js
+-rw-r--r--   0 root         (0) root         (0)      129 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/ui/postgresql-extensions-tab.js
+-rw-r--r--   0 root         (0) root         (0)     5272 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/ui/ui.py
+-rw-r--r--   0 root         (0) root         (0)      625 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.652141 educommon-3.0.0/src/educommon/async_tasks/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/apps.py
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.652141 educommon-3.0.0/src/educommon/async_tasks/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      303 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/async_tasks/fixtures/initial_data.json
+-rw-r--r--   0 root         (0) root         (0)     3489 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/locks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.654141 educommon-3.0.0/src/educommon/async_tasks/migrations/
+-rw-r--r--   0 root         (0) root         (0)     4205 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/migrations/0002_load_initial_data.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3539 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/models.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/statuses.py
+-rw-r--r--   0 root         (0) root         (0)    11237 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.659141 educommon-3.0.0/src/educommon/audit_log/
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/actions.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     5033 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/apps.py
+-rw-r--r--   0 root         (0) root         (0)      880 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.660141 educommon-3.0.0/src/educommon/audit_log/error_log/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/error_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/error_log/actions.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.660141 educommon-3.0.0/src/educommon/audit_log/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.661141 educommon-3.0.0/src/educommon/audit_log/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/management/commands/reinstall_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.665141 educommon-3.0.0/src/educommon/audit_log/migrations/
+-rw-r--r--   0 root         (0) root         (0)     4461 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0002_install_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0003_logproxy.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0004_reinstall_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0005_postgresql_error.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8173 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/models.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     8562 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/proxies.py
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/routers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.668141 educommon-3.0.0/src/educommon/audit_log/sql/
+-rw-r--r--   0 root         (0) root         (0)     1395 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/audit_log/sql/configure_audit_log.sql
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/sql/configure_selective_audit_log.sql
+-rw-r--r--   0 root         (0) root         (0)     1841 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/audit_log/sql/create_selective_tables_function.sql
+-rw-r--r--   0 root         (0) root         (0)    14310 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/audit_log/sql/install_audit_log.sql
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.669141 educommon-3.0.0/src/educommon/audit_log/utils/
+-rw-r--r--   0 root         (0) root         (0)    12533 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/utils/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.669141 educommon-3.0.0/src/educommon/auth/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.672141 educommon-3.0.0/src/educommon/auth/rbac/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26872 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/actions.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/app_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.673141 educommon-3.0.0/src/educommon/auth/rbac/backends/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/backends/base.py
+-rw-r--r--   0 root         (0) root         (0)    10290 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/backends/caching.py
+-rw-r--r--   0 root         (0) root         (0)     5038 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/backends/simple.py
+-rw-r--r--   0 root         (0) root         (0)     2957 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/checker.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/config.py
+-rw-r--r--   0 root         (0) root         (0)      502 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.674141 educommon-3.0.0/src/educommon/auth/rbac/management/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.674141 educommon-3.0.0/src/educommon/auth/rbac/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5520 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/management/commands/rbac.py
+-rw-r--r--   0 root         (0) root         (0)    16250 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.675141 educommon-3.0.0/src/educommon/auth/rbac/migrations/
+-rw-r--r--   0 root         (0) root         (0)     5474 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py
+-rw-r--r--   0 root         (0) root         (0)      470 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/migrations/0003_permission_hidden.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15185 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/models.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.625141 educommon-3.0.0/src/educommon/auth/rbac/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.678141 educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/
+-rw-r--r--   0 root         (0) root         (0)      335 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/role-add-window.js
+-rw-r--r--   0 root         (0) root         (0)     7914 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/role-edit-window.js
+-rw-r--r--   0 root         (0) root         (0)     3768 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/roles-list-window.js
+-rw-r--r--   0 root         (0) root         (0)      536 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js
+-rw-r--r--   0 root         (0) root         (0)    15735 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/ui.py
+-rw-r--r--   0 root         (0) root         (0)     7819 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/utils.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.682141 educommon-3.0.0/src/educommon/auth/simple_auth/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11943 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/actions.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/checkers.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.683141 educommon-3.0.0/src/educommon/auth/simple_auth/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.626141 educommon-3.0.0/src/educommon/auth/simple_auth/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.684141 educommon-3.0.0/src/educommon/auth/simple_auth/static/simple_auth/
+-rw-r--r--   0 root         (0) root         (0)      123 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/simple_auth/static/simple_auth/simple_auth.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.626141 educommon-3.0.0/src/educommon/auth/simple_auth/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.686141 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/
+-rw-r--r--   0 root         (0) root         (0)     1577 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.687141 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/email/
+-rw-r--r--   0 root         (0) root         (0)      635 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html
+-rw-r--r--   0 root         (0) root         (0)     1444 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/ui.py
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.690141 educommon-3.0.0/src/educommon/contingent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/actions.py
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     6854 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/base.py
+-rw-r--r--   0 root         (0) root         (0)    60031 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/catalogs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.695141 educommon-3.0.0/src/educommon/contingent/contingent_plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      717 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/actions.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.696141 educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1594 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      769 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/model_views.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/models.py
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/observer.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/plugin_meta.py
+-rw-r--r--   0 root         (0) root         (0)     3314 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/storage.py
+-rw-r--r--   0 root         (0) root         (0)     7161 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.698141 educommon-3.0.0/src/educommon/contingent/json_data/
+-rw-r--r--   0 root         (0) root         (0)    53540 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/contingent/json_data/okogu.json
+-rw-r--r--   0 root         (0) root         (0)    30723 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/contingent/json_data/oksm.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.700141 educommon-3.0.0/src/educommon/django/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.702141 educommon-3.0.0/src/educommon/django/db/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7049 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.703141 educommon-3.0.0/src/educommon/django/db/migration/
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9527 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/migration/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.704141 educommon-3.0.0/src/educommon/django/db/mixins/
+-rw-r--r--   0 root         (0) root         (0)    14740 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24715 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/mixins/date_interval.py
+-rw-r--r--   0 root         (0) root         (0)    12225 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/mixins/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.705141 educommon-3.0.0/src/educommon/django/db/model_view/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/model_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/db/model_view/table-view.html
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/models.py
+-rw-r--r--   0 root         (0) root         (0)    10990 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/observer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.710141 educommon-3.0.0/src/educommon/django/db/partitioning/
+-rw-r--r--   0 root         (0) root         (0)     4455 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/db/partitioning/README.md
+-rw-r--r--   0 root         (0) root         (0)    22378 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.712141 educommon-3.0.0/src/educommon/django/db/partitioning/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.714141 educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/clear_table.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/split_table.py
+-rw-r--r--   0 root         (0) root         (0)    20345 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/db/partitioning/partitioning.sql
+-rw-r--r--   0 root         (0) root         (0)     3401 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/db/partitioning/triggers.sql
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/routers.py
+-rw-r--r--   0 root         (0) root         (0)     9366 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.714141 educommon-3.0.0/src/educommon/django/db/validators/
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/validators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38608 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/validators/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.715141 educommon-3.0.0/src/educommon/django/storages/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.719141 educommon-3.0.0/src/educommon/django/storages/atcfs/
+-rw-r--r--   0 root         (0) root         (0)     2656 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/README.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6004 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/api.py
+-rw-r--r--   0 root         (0) root         (0)      349 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.720141 educommon-3.0.0/src/educommon/django/storages/atcfs/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.721141 educommon-3.0.0/src/educommon/django/storages/atcfs/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7416 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/models.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/monkey_patching.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/settings.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.721141 educommon-3.0.0/src/educommon/django/storages/atcfs/templates/
+-rw-r--r--   0 root         (0) root         (0)      196 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/templates/atcfs_unavailable.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.725141 educommon-3.0.0/src/educommon/extjs/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/extjs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.725141 educommon-3.0.0/src/educommon/extjs/fields/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/extjs/fields/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/extjs/fields/input_params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.731141 educommon-3.0.0/src/educommon/importer/
+-rw-r--r--   0 root         (0) root         (0)    37531 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/XLSReader.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13402 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/api.py
+-rw-r--r--   0 root         (0) root         (0)      733 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/constants.py
+-rw-r--r--   0 root         (0) root         (0)    10270 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/loggers.py
+-rw-r--r--   0 root         (0) root         (0)    37353 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     6244 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/proxy_import.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/importer/refactoring-notes.txt
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/report.py
+-rw-r--r--   0 root         (0) root         (0)     8704 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/importer/test_file.xls
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/ui.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.733141 educommon-3.0.0/src/educommon/integration_entities/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/README.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      448 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/consts.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/entities.py
+-rw-r--r--   0 root         (0) root         (0)      335 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/enums.py
+-rw-r--r--   0 root         (0) root         (0)     8675 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.733141 educommon-3.0.0/src/educommon/ioc/
+-rw-r--r--   0 root         (0) root         (0)     4028 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ioc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.735141 educommon-3.0.0/src/educommon/logger/
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/apps.py
+-rw-r--r--   0 root         (0) root         (0)      230 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/consts.py
+-rw-r--r--   0 root         (0) root         (0)      400 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/records.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.736141 educommon-3.0.0/src/educommon/m3/
+-rw-r--r--   0 root         (0) root         (0)    17570 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.736141 educommon-3.0.0/src/educommon/m3/extensions/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.737141 educommon-3.0.0/src/educommon/m3/extensions/listeners/
+-rw-r--r--   0 root         (0) root         (0)     8897 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.740141 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      916 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js
+-rw-r--r--   0 root         (0) root         (0)     6200 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/listeners.py
+-rw-r--r--   0 root         (0) root         (0)     7660 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/mixins.py
+-rw-r--r--   0 root         (0) root         (0)       94 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/related-objects-window.html
+-rw-r--r--   0 root         (0) root         (0)      467 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/signals.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/ui.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6912 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/ui.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/transaction_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.741141 educommon-3.0.0/src/educommon/objectpack/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/objectpack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14320 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/objectpack/actions.py
+-rw-r--r--   0 root         (0) root         (0)      220 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/objectpack/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.747141 educommon-3.0.0/src/educommon/objectpack/templates/
+-rw-r--r--   0 root         (0) root         (0)      437 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/base-grid-window.js
+-rw-r--r--   0 root         (0) root         (0)     1408 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/filter-panel.js
+-rw-r--r--   0 root         (0) root         (0)     1544 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/grid-panel.js
+-rw-r--r--   0 root         (0) root         (0)     1842 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/multiSelectWindow.js
+-rw-r--r--   0 root         (0) root         (0)     6741 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/multiselect-page-fix.js
+-rw-r--r--   0 root         (0) root         (0)     1838 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/relations-check-mixin-template.html
+-rw-r--r--   0 root         (0) root         (0)    14752 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/objectpack/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.748141 educommon-3.0.0/src/educommon/report/
+-rw-r--r--   0 root         (0) root         (0)    17854 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8705 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.753141 educommon-3.0.0/src/educommon/report/constructor/
+-rw-r--r--   0 root         (0) root         (0)     1138 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/report/constructor/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/apps.py
+-rw-r--r--   0 root         (0) root         (0)    25938 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.754141 educommon-3.0.0/src/educommon/report/constructor/builders/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.755141 educommon-3.0.0/src/educommon/report/constructor/builders/excel/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55790 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/_header.py
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6229 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/product.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/with_merged_cells.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/config.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.759141 educommon-3.0.0/src/educommon/report/constructor/editor/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/editor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38811 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/editor/actions.py
+-rw-r--r--   0 root         (0) root         (0)    39225 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/report/constructor/editor/edit-window.js
+-rw-r--r--   0 root         (0) root         (0)     3247 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/report/constructor/editor/list-window.js
+-rw-r--r--   0 root         (0) root         (0)    24628 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/editor/ui.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.762141 educommon-3.0.0/src/educommon/report/constructor/migrations/
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     5009 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0002_report_filters.py
+-rw-r--r--   0 root         (0) root         (0)      472 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0003_reportfilter_exclude.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0005_reportcolumn_visible.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0006_reportsorting.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0007_include_available_units.py
+-rw-r--r--   0 root         (0) root         (0)      557 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/mixins.py
+-rw-r--r--   0 root         (0) root         (0)    18764 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/models.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/plugin_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/registries.py
+-rw-r--r--   0 root         (0) root         (0)     6557 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/utils.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/validators.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/reporter.py
+-rw-r--r--   0 root         (0) root         (0)     9974 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.763141 educommon-3.0.0/src/educommon/rest/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/actions.py
+-rw-r--r--   0 root         (0) root         (0)     3908 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/context.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/controllers.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/misc.py
+-rw-r--r--   0 root         (0) root         (0)     4840 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.765141 educommon-3.0.0/src/educommon/secure_media/
+-rw-r--r--   0 root         (0) root         (0)     4001 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/secure_media/README.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/secure_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/secure_media/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/thread_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.768141 educommon-3.0.0/src/educommon/utils/
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4066 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/caching.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/conversion.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/crypto.py
+-rw-r--r--   0 root         (0) root         (0)     9122 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/date.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.769141 educommon-3.0.0/src/educommon/utils/db/
+-rw-r--r--   0 root         (0) root         (0)     7734 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/db/postgresql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.783141 educommon-3.0.0/src/educommon/utils/fonts/
+-rw-r--r--   0 root         (0) root         (0)   275572 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/fonts/Arial.ttf
+-rw-r--r--   0 root         (0) root         (0)   811820 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/fonts/Calibri.ttf
+-rw-r--r--   0 root         (0) root         (0)   265528 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/fonts/Tahoma.ttf
+-rw-r--r--   0 root         (0) root         (0)     4815 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.783141 educommon-3.0.0/src/educommon/utils/licence/
+-rw-r--r--   0 root         (0) root         (0)     5095 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/licence/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/licence/converters.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/patches.py
+-rw-r--r--   0 root         (0) root         (0)     9469 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/registry.py
+-rw-r--r--   0 root         (0) root         (0)      520 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/seqtools.py
+-rw-r--r--   0 root         (0) root         (0)     8787 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/storage.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.784141 educommon-3.0.0/src/educommon/utils/system_app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.784141 educommon-3.0.0/src/educommon/utils/system_app/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.784141 educommon-3.0.0/src/educommon/utils/system_app/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9297 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/management/commands/delete_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.785141 educommon-3.0.0/src/educommon/utils/system_app/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/templatetags/educommon.py
+-rw-r--r--   0 root         (0) root         (0)    14251 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.795141 educommon-3.0.0/src/educommon/utils/xml/
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/xml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/xml/catalog.json
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/xml/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    13160 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd
+-rw-r--r--   0 root         (0) root         (0)    13465 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd
+-rw-r--r--   0 root         (0) root         (0)     5234 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/xml/xenc-schema.xsd
+-rw-r--r--   0 root         (0) root         (0)    10293 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/xml/xmldsig-core-schema.xsd
+-rw-r--r--   0 root         (0) root         (0)      448 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon/version.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.800141 educommon-3.0.0/src/educommon/ws_log/
+-rw-r--r--   0 root         (0) root         (0)     5467 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/ws_log/README.rst
+-rw-r--r--   0 root         (0) root         (0)      932 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9153 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/actions.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.803141 educommon-3.0.0/src/educommon/ws_log/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2706 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      910 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0006_auto_20170327_1027.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5634 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/models.py
+-rw-r--r--   0 root         (0) root         (0)      885 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/provider.py
+-rw-r--r--   0 root         (0) root         (0)     3487 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.804141 educommon-3.0.0/src/educommon/ws_log/smev/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/smev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/smev/applications.py
+-rw-r--r--   0 root         (0) root         (0)      601 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/smev/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.635141 educommon-3.0.0/src/educommon/ws_log/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.804141 educommon-3.0.0/src/educommon/ws_log/templates/report/
+-rw-r--r--   0 root         (0) root         (0)    10439 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/ws_log/templates/report/smev_logs.xlsx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.807141 educommon-3.0.0/src/educommon/ws_log/templates/ui-js/
+-rw-r--r--   0 root         (0) root         (0)      513 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js
+-rw-r--r--   0 root         (0) root         (0)     1103 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js
+-rw-r--r--   0 root         (0) root         (0)     4038 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/ui.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.640141 educommon-3.0.0/src/educommon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.811141 educommon-3.0.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_contingent_plugin_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_delete_check.py
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_delete_objects.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_django_db_utils.py
+-rw-r--r--   0 root         (0) root         (0)    21544 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_interval_mixins.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_patches.py
+-rw-r--r--   0 root         (0) root         (0)     7024 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_personal_data_fields.py
+-rw-r--r--   0 root         (0) root         (0)    14369 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_report.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_service_db_router.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_utils_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8031 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_validators.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/tests_rbac.py
```

### Comparing `educommon-2.20.0/PKG-INFO` & `educommon-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: educommon
-Version: 2.20.0
+Version: 3.0.0
 Summary: Общая кодовая база для проектов БЦ Образование
 Home-page: https://stash.bars-open.ru/projects/EDUBASE/repos/educommon
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Django :: 1.7
 Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
```

### Comparing `educommon-2.20.0/README.rst` & `educommon-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/UPGRADE.rst` & `educommon-3.0.0/UPGRADE.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/setup.py` & `educommon-3.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# coding: utf-8
-from os.path import dirname
-from os.path import join
 import platform
-
-from setuptools import find_packages
-from setuptools import setup
+from os.path import (
+    dirname,
+    join,
+)
+
+from setuptools import (
+    find_packages,
+    setup,
+)
 
 
 linux_dependencies = tuple()
 if platform.system() == 'Linux':
     linux_dependencies = ('distro>=1.3.0,<2',)
 
 
@@ -23,17 +26,18 @@
             'Intended Audience :: Developers',
             'Environment :: Web Environment',
             'Natural Language :: Russian',
             'Natural Language :: English',
             'Operating System :: OS Independent',
             'Development Status :: 5 - Production/Stable',
             'Programming Language :: Python',
-            'Programming Language :: Python :: 2.7',
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
+            'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
             'Framework :: Django :: 1.7',
             'Framework :: Django :: 1.8',
             'Framework :: Django :: 1.9',
             'Framework :: Django :: 1.10',
             'Framework :: Django :: 1.11',
             'Framework :: Django :: 2.0',
             'Framework :: Django :: 2.1',
@@ -45,26 +49,26 @@
         dependency_links=(
             'http://pypi.bars-open.ru/simple/m3-builder',
         ),
         setup_requires=(
             'm3-builder>=1.2,<2',
         ),
         install_requires=(
-            'six>=1.11,<2',
             'Django>=1.11,<2.3',
             'django-mptt',
             'python-dateutil',
             'termcolor',
             'django-sendfile',
             'requests',
             'celery',
             'spyne',
             'xlsxwriter>=0.9.3,<1',
 
             'm3-builder>=1.2,<2',
+            'm3-db-utils>=0.3.4',
             'm3-django-compat>=1.9.1,<2',
             'm3-core>=2.2.16,<3',
             'm3-ui>=2.2.40,<3',
             'm3-objectpack>=2.2.36,<3',
             'm3-simple-report>=1.4.1,<2',
             'm3-spyne-smev>=0.2.4,<1',
             'python-magic==0.4.15'
```

### Comparing `educommon-2.20.0/src/educommon/about/README.rst` & `educommon-3.0.0/src/educommon/about/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/about/static/edu_about/barsgroup.png` & `educommon-3.0.0/src/educommon/about/static/edu_about/barsgroup.png`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/about/ui/about-window.js` & `educommon-3.0.0/src/educommon/about/ui/about-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/about/ui/actions.py` & `educommon-3.0.0/src/educommon/about/ui/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,48 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from abc import ABCMeta
-from abc import abstractmethod
-from platform import python_version
-
-from django.db import connection
-from django.db import connections
-from m3_builder.build import get_build_info
-from objectpack.actions import BasePack
-from objectpack.actions import BaseWindowAction
-from objectpack.actions import ObjectPack
-from objectpack.models import VirtualModel
-import six
-
-from educommon.utils.system import get_os_version
-from educommon.utils.system import get_postgresql_version
-
-from ..utils import get_installed_distributions
-from .ui import AboutWindow
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
+from platform import (
+    python_version,
+)
+
+from django.db import (
+    connection,
+    connections,
+)
+from m3_builder.build import (
+    get_build_info,
+)
+
+from objectpack.actions import (
+    BasePack,
+    BaseWindowAction,
+    ObjectPack,
+)
+from objectpack.models import (
+    VirtualModel,
+)
+
+from educommon.about.ui.ui import (
+    AboutWindow,
+)
+from educommon.about.utils import (
+    get_installed_distributions,
+)
+from educommon.utils.system import (
+    get_os_version,
+    get_postgresql_version,
+)
 
 
 # -----------------------------------------------------------------------------
 
 
 class Package(VirtualModel):
-
     """Виртуальная модель 'Пакеты, установленные в системе'."""
 
     def __init__(self, data):
         self.id = data['id']
         self.name = data['name']
         self.version = data['version']
 
@@ -128,15 +140,15 @@
             header='Версия',
             width=1,
         ),
     )
 # -----------------------------------------------------------------------------
 
 
-class AboutPack(six.with_metaclass(ABCMeta, BasePack)):
+class AboutPack(BasePack, metaclass=ABCMeta):
 
     """Пак окна 'Информация о системе'."""
 
     title = 'О системе'
 
     @property
     @abstractmethod
```

### Comparing `educommon-2.20.0/src/educommon/about/ui/common-tab.html` & `educommon-3.0.0/src/educommon/about/ui/common-tab.html`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/about/ui/packages-tab.js` & `educommon-3.0.0/src/educommon/about/ui/packages-tab.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/about/ui/ui.py` & `educommon-3.0.0/src/educommon/about/ui/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,30 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.template.loader import render_to_string
-from m3_ext.ui.containers.grids import ExtGrid
-from m3_ext.ui.misc.store import ExtDataStore
-from objectpack.ui import ObjectGridTab
-from objectpack.ui import TabbedWindow
-from objectpack.ui import WindowTab
-
-from educommon.m3 import get_pack
-from educommon.utils.ui import local_template
-from educommon.utils.ui import make_button
+from django.template.loader import (
+    render_to_string,
+)
+from m3_ext.ui.containers.grids import (
+    ExtGrid,
+)
+from m3_ext.ui.misc.store import (
+    ExtDataStore,
+)
+
+from objectpack.ui import (
+    ObjectGridTab,
+    TabbedWindow,
+    WindowTab,
+)
+
+from educommon.m3 import (
+    get_pack,
+)
+from educommon.utils.ui import (
+    local_template,
+    make_button,
+)
 
 
 class CommonTab(WindowTab):
 
     """Вкладка с общей информацией о системе."""
 
     title = 'Общие сведения'
```

### Comparing `educommon-2.20.0/src/educommon/async_tasks/locks.py` & `educommon-3.0.0/src/educommon/async_tasks/locks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-# coding: utf-8
 import logging
 
-from celery.result import AsyncResult
-from django.core.cache import cache
-from django.utils.functional import cached_property
+from celery.result import (
+    AsyncResult,
+)
+from django.core.cache import (
+    cache,
+)
+from django.utils.functional import (
+    cached_property,
+)
+
+from educommon.async_tasks.exceptions import (
+    TaskUniqueException,
+)
 
-from educommon.async_tasks.exceptions import TaskUniqueException
 
 # по-умолчанию задача считается уникальной в течении
 DEFAULT_LOCK_EXPIRE = 30 * 60
 
 
 class TaskLocker:
     """Класс, отвечающий за блокировку задач"""
```

### Comparing `educommon-2.20.0/src/educommon/async_tasks/migrations/0001_initial.py` & `educommon-3.0.0/src/educommon/async_tasks/migrations/0001_initial.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('contenttypes', '0001_initial'),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/async_tasks/statuses.py` & `educommon-3.0.0/src/educommon/async_tasks/statuses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from celery.result import states
-import six
+from celery.result import (
+    states,
+)
 
 
 STATUS_PENDING = 1
 STATUS_RECEIVED = 2
 STATUS_STARTED = 3
 STATUS_SUCCESS = 4
 STATUS_REVOKED = 5
@@ -26,28 +24,28 @@
     STATUS_FAILURE: states.FAILURE,
     STATUS_RETRY: states.RETRY,
     STATUS_IGNORED: states.IGNORED,
     STATUS_REJECTED: states.REJECTED,
 }
 
 # состояния задач celery по статусам
-TASK_STATUSES = dict((v, k) for k, v in six.iteritems(TASK_STATES))
+TASK_STATUSES = dict((v, k) for k, v in TASK_STATES.items())
 
 
 # отображение статусов
 STATUS_CHOICES = (
-    (STATUS_PENDING, u'Неизвестно'),
-    (STATUS_RECEIVED, u'В очереди'),
-    (STATUS_STARTED, u'Выполняется'),
-    (STATUS_SUCCESS, u'Успешно выполнена'),
-    (STATUS_REVOKED, u'Остановлена'),
-    (STATUS_FAILURE, u'Ошибка'),
-    (STATUS_RETRY, u'Перезапуск'),
-    (STATUS_IGNORED, u'Игнорирована'),
-    (STATUS_REJECTED, u'Отменена'),
+    (STATUS_PENDING, 'Неизвестно'),
+    (STATUS_RECEIVED, 'В очереди'),
+    (STATUS_STARTED, 'Выполняется'),
+    (STATUS_SUCCESS, 'Успешно выполнена'),
+    (STATUS_REVOKED, 'Остановлена'),
+    (STATUS_FAILURE, 'Ошибка'),
+    (STATUS_RETRY, 'Перезапуск'),
+    (STATUS_IGNORED, 'Игнорирована'),
+    (STATUS_REJECTED, 'Отменена'),
 )
 
 
 def get_state_str(status_idx):
     return TASK_STATES[status_idx]
```

### Comparing `educommon-2.20.0/src/educommon/async_tasks/tasks.py` & `educommon-3.0.0/src/educommon/async_tasks/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-# coding: utf-8
-u"""Базовые классы для асинхронных задач."""
-from __future__ import absolute_import
-
-from collections import OrderedDict
-from datetime import datetime
+"""Базовые классы для асинхронных задач."""
 import logging
-
-from celery import Task
-from celery import states
-from kombu import uuid
-
-from . import models
-from . import statuses
-from .locks import TaskLocker
+from collections import (
+    OrderedDict,
+)
+from datetime import (
+    datetime,
+)
+
+from celery import (
+    Task,
+    states,
+)
+from kombu import (
+    uuid,
+)
+
+from educommon.async_tasks import (
+    models,
+    statuses,
+)
+from educommon.async_tasks.locks import (
+    TaskLocker,
+)
 
 
 class AsyncTask(Task):
-
-    u"""Базовый класс асинхронных задач."""
+    """Базовый класс асинхронных задач."""
 
     abstract = True
 
     # описание (имя) асинх.задачи (отображается в реестре)
     description = None
 
     def debug(self, *args, **kwargs):
-        u"""логирование в debug-лог."""
+        """Логирование в debug-лог."""
         logger = logging.getLogger('educommon.async')
         logger.debug(*args, **kwargs)
 
     def apply_async(self, args=None, kwargs=None, task_id=None, producer=None,
                     link=None, link_error=None, **options):
-        u"""Постановка задачи в очередь.
+        """Постановка задачи в очередь.
 
         автор задачи задаётся снаружи через 2 поля в словаре kwargs:
             object_id и content_type
         """
         if kwargs is None:
             kwargs = {}
 
@@ -68,44 +76,44 @@
         )
 
         self.debug("Task %s added" % self.__name__)
 
         return async_result
 
     def run(self, *args, **kwargs):
-        u"""Выполнение задачи (отложенное)."""
+        """Выполнение задачи (отложенное)."""
         # начальное состояние задачи
         self.state = {
             # результаты задачи
             'values': OrderedDict(),
             # описание результата
             'description': self.description,
             # прогресс выполнения задачи
-            'progress': u'Неизвестно'
+            'progress': 'Неизвестно'
         }
         self.update_state(
             state=statuses.get_state_str(statuses.STATUS_STARTED),
             meta=self.state
         )
         self.debug("Task %s run (task_id = %s )" % (
             self.__name__, self.request.id))
         return {}
 
     def after_return(self, status, retval, task_id, args, kwargs, einfo):
-        u"""Завершение задачи."""
+        """Завершение задачи."""
         self.debug("Task %s completed" % self.__name__)
 
         if isinstance(retval, dict):
             self.update_state(
                 state=retval.get('task_state', status), meta=retval)
         else:
             self.update_state(state=status, meta=retval)
 
     def update_state(self, task_id=None, state=None, meta=None):
-        u"""Обновленение модели при изменении состояния асинх. результата.
+        """Обновленение модели при изменении состояния асинх. результата.
 
         :param str task_id: id задачи celery
         :param str task_state: состояние задачи celery (celery.states)
         :param meta: состояние метаданых (см. базовый класс в Celery).
         """
         if task_id is None:
             task_id = self.request.id
@@ -114,34 +122,34 @@
             task_id=task_id
         ).order_by('queued_on').first()
 
         if not running_task:
             return
 
         if state == states.SUCCESS:
-            self.state['values'][u'Время выполения'] = (
+            self.state['values']['Время выполения'] = (
                 datetime.now() - running_task.queued_on)
 
         super(AsyncTask, self).update_state(
             task_id=task_id, state=state, meta=meta)
 
         running_task.status = statuses.get_status_idx(state)
 
         if state == states.STARTED:
             # если обновление статуса связано с переходом в состояние 'RUNNING'
             running_task.queued_on = datetime.now()
         running_task.clean_and_save()
 
     def set_progress(self, task_id=None, task_state=states.STARTED,
                      progress=None, values=None):
-        u"""Обновление состояния выполнения задачи.
+        """Обновление состояния выполнения задачи.
 
         :param str task_id: id задачи celery
         :param str task_state: состояние задачи celery (celery.states)
-        :param unicode progress: строковое описание состояния выполнения задачи
+        :param str progress: строковое описание состояния выполнения задачи
         :param dict values: значения задаваемые процедурой выполнения задачи
         """
         if task_id is None:
             task_id = self.request.id
 
         if progress:
             self.state['progress'] = progress
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/__init__.py` & `educommon-3.0.0/src/educommon/audit_log/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# coding: utf-8
-u"""Подсистема логирования изменений в БД.
+"""Подсистема логирования изменений в БД.
 
 В PostgreSQL должна быть поддержка hstore. В Ubuntu требуется
 установленный пакет postgresql-contrib.
 
 До подключения логирования от суперпользователя необходимо
 выполнить SQL команды.
 
@@ -44,14 +43,12 @@
 Текст для отображения колонки "Объект" в окне просмотра журнала изменений
 берется как результат вызова одного из трех методов модели в следующем порядке:
     - log_display()
     - display()
     - __str__()
 Для каждой модели проекта желательно добавить/изменить один из данных методов.
 """
-from __future__ import absolute_import
-
 import django
 
 
 assert django.VERSION >= (1, 9), 'django version must be >= 1.9'
 default_app_config = __name__ + '.apps.AppConfig'
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/actions.py` & `educommon-3.0.0/src/educommon/audit_log/actions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,72 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from datetime import date
-from datetime import timedelta
-from functools import partial
-
-from django.contrib.postgres.fields.hstore import HStoreField
-from django.db.models import GenericIPAddressField
-from m3.actions.results import PreJsonResult
-from m3_ext.ui.all_components import ExtStringField
-from objectpack.actions import BaseAction
-from objectpack.actions import ObjectPack
-from objectpack.filters import ColumnFilterEngine
-from objectpack.ui import make_combo_box
-
-from educommon import ioc
-from educommon.m3 import PackValidationMixin
-from educommon.objectpack.actions import ViewWindowPackMixin
-from educommon.utils.ui import DatetimeFilterCreator
-from educommon.utils.ui import FilterByField
-
-from .permissions import PERM_GROUP__AUDIT_LOG
-from .proxies import LogProxy
-from .ui import ViewChangeWindow
-from .utils import get_model_choices
-from .utils import make_hstore_filter
-from .utils import make_name_filter
+from datetime import (
+    date,
+    timedelta,
+)
+from functools import (
+    partial,
+)
+
+from django.contrib.postgres.fields.hstore import (
+    HStoreField,
+)
+from django.db.models import (
+    GenericIPAddressField,
+)
+from m3.actions.results import (
+    PreJsonResult,
+)
+from m3_ext.ui.all_components import (
+    ExtStringField,
+)
+
+from objectpack.actions import (
+    BaseAction,
+    ObjectPack,
+)
+from objectpack.filters import (
+    ColumnFilterEngine,
+)
+from objectpack.ui import (
+    make_combo_box,
+)
+
+from educommon import (
+    ioc,
+)
+from educommon.audit_log.permissions import (
+    PERM_GROUP__AUDIT_LOG,
+)
+from educommon.audit_log.proxies import (
+    LogProxy,
+)
+from educommon.audit_log.ui import (
+    ViewChangeWindow,
+)
+from educommon.audit_log.utils import (
+    get_model_choices,
+    make_hstore_filter,
+    make_name_filter,
+)
+from educommon.m3 import (
+    PackValidationMixin,
+)
+from educommon.objectpack.actions import (
+    ViewWindowPackMixin,
+)
+from educommon.utils.ui import (
+    DatetimeFilterCreator,
+    FilterByField,
+)
 
 
 class AuditLogPack(ViewWindowPackMixin, PackValidationMixin, ObjectPack):
+    """Журнал изменений."""
 
-    u"""Журнал изменений."""
-
-    title = u'Журнал изменений'
+    title = 'Журнал изменений'
     model = LogProxy
     width = 1000
     height = 600
     allow_paging = True
 
     list_sort_order = ('-time',)
 
@@ -54,77 +84,77 @@
         get_to=date.today
     )
 
     columns = [
         {
             'data_index': 'time',
             'width': 140,
-            'header': u'Дата и время',
+            'header': 'Дата и время',
             'sortable': True,
             'filter': date_filter.filter
         },
         {
             'data_index': 'user_name',
             'width': 130,
-            'header': u'Пользователь',
+            'header': 'Пользователь',
             'filter': ff(
                 'table__name',
                 lookup=lambda x: make_name_filter('surname', x)
             ) & ff(
                 'table__name',
                 lookup=lambda x: make_name_filter('firstname', x)
             ) & ff(
                 'table__name',
                 lookup=lambda x: make_name_filter('patronymic', x)
             )
         },
         {
             'data_index': 'operation',
             'width': 60,
-            'header': u'Операция',
+            'header': 'Операция',
             'filter': ff(
                 'operation',
                 ask_before_deleting=False
             ),
         },
         {
             'data_index': 'model_name',
             'width': 220,
-            'header': u'Модель объекта',
+            'header': 'Модель объекта',
             'filter': ff(
                 'table',
                 control_creator=lambda: make_combo_box(
                     data=get_model_choices(),
                     ask_before_deleting=False,
                 ),
             ),
         },
         {
             'data_index': 'object_id',
             'width': 50,
-            'header': u'Код объекта',
+            'header': 'Код объекта',
             'filter': ff('object_id'),
         },
         {
             'data_index': 'ip',
             'width': 60,
-            'header': u'IP',
+            'header': 'IP',
             'filter': ff(
                 'ip',
-                parser_map=(GenericIPAddressField, 'unicode', '%s__contains'),
+                parser_map=(GenericIPAddressField, 'str', '%s__contains'),
                 control_creator=ExtStringField,
             ),
         },
         {
             'data_index': 'object_string',
             'width': 180,
-            'header': u'Объект',
+            'header': 'Объект',
             'filter': ff(
                 'data',
-                parser_map=(HStoreField, 'unicode', '%s__values__icontains'),
+                parser_map=(HStoreField, 'str', '%s__values__icontains'),
                 lookup=lambda x: make_hstore_filter('data', x),
                 control_creator=ExtStringField,
             ),
         },
     ]
 
     def __init__(self):
@@ -135,15 +165,15 @@
         self.need_check_permission = True
         self.perm_code = PERM_GROUP__AUDIT_LOG
 
         for action in self.actions:
             action.perm_code = 'view'
 
     def configure_grid(self, grid):
-        u"""Настройка грида.
+        """Настройка грида.
 
         Устанавливает интервал дат фильтрации по умолчанию
         в параметрах запроса.
         """
         super(AuditLogPack, self).configure_grid(grid)
         grid.store.base_params = self.date_filter.base_params
 
@@ -169,16 +199,15 @@
     def extend_menu(self, menu):
         return menu.administry(
             menu.Item(self.title, self.list_window_action),
         )
 
 
 class ViewChangeAction(BaseAction):
-
-    u"""Action для просмотра изменений."""
+    """Action для просмотра изменений."""
 
     def context_declaration(self):
         result = super(ViewChangeAction, self).context_declaration()
         result[self.parent.id_param_name] = dict(type='int')
         return result
 
     def run(self, request, context):
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/apps.py` & `educommon-3.0.0/src/educommon/audit_log/apps.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,36 @@
-# coding: utf-8
 # pylint: disable=function-redefined, unused-argument
-from __future__ import absolute_import
-
-from contextlib import closing
-
-from django.apps import AppConfig
-from django.conf import settings
-from django.core.checks import Critical
-from django.core.checks import register
-from django.core.exceptions import ImproperlyConfigured
-from django.db import connections
-from django.db.models.signals import post_migrate
-
-from educommon.utils.db.postgresql import create_extension
-from educommon.utils.db.postgresql import is_extension_exists
+from contextlib import (
+    closing,
+)
+
+from django.apps import (
+    AppConfig,
+)
+from django.conf import (
+    settings,
+)
+from django.core.checks import (
+    Critical,
+    register,
+)
+from django.core.exceptions import (
+    ImproperlyConfigured,
+)
+from django.db import (
+    connections,
+)
+from django.db.models.signals import (
+    post_migrate,
+)
+
+from educommon.utils.db.postgresql import (
+    create_extension,
+    is_extension_exists,
+)
 
 
 class AppConfig(AppConfig):
 
     name = __name__.rpartition('.')[0]
 
     @property
@@ -25,15 +38,15 @@
         return '.'.join((
             self.name,
             self.__class__.__name__,
             self._configure_audit_log.__name__,
         ))
 
     def _create_postgresql_extensions(self):
-        u"""Создает в БД необходимые расширения PostgreSQL.
+        """Создает в БД необходимые расширения PostgreSQL.
 
         Расширения создаются только при наличии прав. Если прав нет, ничего не
         происходит. При запуске системы будет критическая ошибка Django и
         сообщение о необходимости создания недостающих расширений.
         """
         alias = settings.DEFAULT_DB_ALIAS
         if not is_extension_exists(alias, 'postgres_fdw'):
@@ -46,46 +59,51 @@
 
         for alias in (settings.DEFAULT_DB_ALIAS,
                       settings.SERVICE_DB_ALIAS):
             if not is_extension_exists(alias, 'hstore'):
                 create_extension(alias, 'hstore', quite=True)
 
     def _configure_audit_log(self, connection):
-        u"""Настраивает AuditLog при первом подключении к БД."""
+        """Настраивает AuditLog при первом подключении к БД."""
         # Настройка параметров подключения к сервисной БД, обновление триггеров
-        from educommon.audit_log.utils import configure
+        from educommon.audit_log.utils import (
+            configure,
+        )
         configure()
 
         # Проверка подключения подключения к сервисной БД через FDW.
-        from educommon.audit_log.utils import check_connection_fdw
+        from educommon.audit_log.utils import (
+            check_connection_fdw,
+        )
         success, error_message = check_connection_fdw()
         if not success:
             raise ImproperlyConfigured(
-                u"{0} - Ошибка подключения к сервисной базе через "
-                u"postgres_fdw. Необходимо убедится что 'Журнал изменений' "
-                u"настроен корректно.".format(error_message)
+                "{0} - Ошибка подключения к сервисной базе через "
+                "postgres_fdw. Необходимо убедится что 'Журнал изменений' "
+                "настроен корректно.".format(error_message)
             )
 
     def _configure_db(self, **kwargs):
-        from .utils import is_initialized
+        from educommon.audit_log.utils import (
+            is_initialized,
+        )
 
         self._create_postgresql_extensions()
         if is_initialized(settings.DEFAULT_DB_ALIAS):
             self._configure_audit_log(
                 connections[settings.DEFAULT_DB_ALIAS]
             )
 
     def ready(self):
         post_migrate.connect(self._configure_db, sender=self)
 
 
-
 @register
 def check_postgres_fdw(app_configs, **kwargs):
-    u"""Проверяет наличие в основной БД расширения postgres_fdw."""
+    """Проверяет наличие в основной БД расширения postgres_fdw."""
     errors = []
 
     if not is_extension_exists(settings.DEFAULT_DB_ALIAS, 'postgres_fdw'):
         dbname = settings.DATABASES[settings.DEFAULT_DB_ALIAS]['NAME']
         msg = (
             "'postgres_fdw' PostgreSQL extension not installed in '{}' "
             "database."
@@ -99,15 +117,15 @@
         errors.append(Critical(msg, hint, id='audit_log.C001'))
 
     return errors
 
 
 @register
 def check_hstore(app_configs, **kwargs):
-    u"""Проверяет наличие в основной и в сервисной БД расширения hstore."""
+    """Проверяет наличие в основной и в сервисной БД расширения hstore."""
     errors = []
 
     msg = "'hstore' PostgreSQL extension not installed in '{}' database."
     hint = (
         "Execute this SQL in '{dbname}' database:\n"
         '{indent}CREATE EXTENSION hstore;'
     )
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/constants.py` & `educommon-3.0.0/src/educommon/audit_log/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import os
 
 
 # ID блокировок postgresql. Должны быть уникальны в пределах проекта
 PG_LOCK_ID = 2710589049657585281
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/error_log/actions.py` & `educommon-3.0.0/src/educommon/audit_log/error_log/actions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,57 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from objectpack.actions import ObjectPack
-
-from educommon.m3 import PackValidationMixin
-from educommon.objectpack.ui import BaseListWindow
-
-from ..models import PostgreSQLError
-from ..permissions import PERM_GROUP__AUDIT_LOG_ERRORS
+from objectpack.actions import (
+    ObjectPack,
+)
+
+from educommon.audit_log.models import (
+    PostgreSQLError,
+)
+from educommon.audit_log.permissions import (
+    PERM_GROUP__AUDIT_LOG_ERRORS,
+)
+from educommon.m3 import (
+    PackValidationMixin,
+)
+from educommon.objectpack.ui import (
+    BaseListWindow,
+)
 
 
 class PostgreSQLErrorPack(PackValidationMixin, ObjectPack):
+    """Журнал кастомных ошибок PostgreSQL."""
 
-    u"""Журнал кастомных ошибок PostgreSQL."""
-
-    title = u'Журнал ошибок PostgreSQL'
+    title = 'Журнал ошибок PostgreSQL'
 
     model = PostgreSQLError
     allow_paging = True
     can_delete = True
 
     list_sort_order = ('-time',)
     columns = (
         dict(
             data_index='time',
             width=140,
             fixed=True,
-            header=u'Дата и время',
+            header='Дата и время',
         ),
         dict(
             data_index='ip',
             width=80,
             fixed=True,
-            header=u'IP',
+            header='IP',
         ),
         dict(
             data_index='level',
             width=100,
             fixed=True,
-            header=u'Уровень ошибки',
+            header='Уровень ошибки',
         ),
         dict(
             data_index='text',
-            header=u'Сообщение об ошибке',
+            header='Сообщение об ошибке',
         ),
     )
 
     list_window = BaseListWindow
 
     def __init__(self):
         super(PostgreSQLErrorPack, self).__init__()
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/helpers.py` & `educommon-3.0.0/src/educommon/audit_log/helpers.py`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/audit_log/management/commands/reinstall_audit_log.py` & `educommon-3.0.0/src/educommon/audit_log/management/commands/reinstall_audit_log.py`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/audit_log/middleware.py` & `educommon-3.0.0/src/educommon/audit_log/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-import six
-
-from .utils import get_audit_log_context
-from .utils import set_db_param
+from educommon.audit_log.utils import (
+    get_audit_log_context,
+    set_db_param,
+)
 
 
 try:
-    from django.utils.deprecation import MiddlewareMixin
+    from django.utils.deprecation import (
+        MiddlewareMixin,
+    )
 except ImportError:
     MiddlewareMixin = object
 
 
-
 class AuditLogMiddleware(MiddlewareMixin):
-
-    u"""Устанавливает параметры из запроса в текущей сессии БД.
+    """Устанавливает параметры из запроса в текущей сессии БД.
 
     Устанавливает в custom settings postgresql:
       - audit_log.user_id - id пользователя;
       - audit_log.user_type_id - id ContentType модели пользователя;
       - audit_log.ip - IP адрес, с которого пришел запрос.
 
     В дальнейшем эта информация используется в логирующем триггере.
     """
 
     def process_request(self, request):
-        for name, value in six.iteritems(get_audit_log_context(request)):
+        for name, value in get_audit_log_context(request).items():
             set_db_param('audit_log.' + name, value)
 
     def process_response(self, request, response):
         for name in ('user_id', 'user_type_id', 'ip'):
             set_db_param('audit_log.' + name, None)
         return response
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/migrations/0001_initial.py` & `educommon-3.0.0/src/educommon/audit_log/migrations/0001_initial.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.contrib.postgres.fields.hstore import HStoreField
-from django.db import migrations
-from django.db import models
-
-from educommon.django.db.migration.operations import CreateSchema
+from django.contrib.postgres.fields.hstore import (
+    HStoreField,
+)
+from django.db import (
+    migrations,
+    models,
+)
+
+from educommon.django.db.migration.operations import (
+    CreateSchema,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
     ]
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/migrations/0002_install_audit_log.py` & `educommon-3.0.0/src/educommon/audit_log/migrations/0002_install_audit_log.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
 import codecs
 import os.path
 
-from django.conf import settings
-from django.db import connections
-from django.db import migrations
-from django.db.migrations.operations.base import Operation
-
-from ..constants import EXCLUDED_TABLES
-from ..constants import PG_LOCK_ID
-from ..constants import SQL_FILES_DIR
-from ..utils import get_db_connection_params
+from django.conf import (
+    settings,
+)
+from django.db import (
+    connections,
+    migrations,
+)
+from django.db.migrations.operations.base import (
+    Operation,
+)
+
+from educommon.audit_log.constants import (
+    EXCLUDED_TABLES,
+    PG_LOCK_ID,
+    SQL_FILES_DIR,
+)
+from educommon.audit_log.utils import (
+    get_db_connection_params,
+)
 
 
 class InitDefaultDatabase(Operation):
-
-    u"""Настраивает основную БД."""
+    """Настраивает основную БД."""
 
     reversible = True
 
     def state_forwards(self, app_label, state):
         pass
 
     def database_forwards(self, app_label, schema_editor, from_state,
@@ -48,16 +53,15 @@
         with codecs.open(sql_file_path, 'r', 'utf-8') as sql_file:
             sql = sql_file.read().replace('%', '%%')
 
         schema_editor.execute(sql)
 
 
 class LoadTableData(Operation):
-
-    u"""Заполняет данными модель Table."""
+    """Заполняет данными модель Table."""
 
     reversible = True
 
     def state_forwards(self, app_label, state):
         pass
 
     def database_forwards(self, app_label, schema_editor, from_state,
@@ -78,16 +82,15 @@
 
     def database_backwards(self, app_label, schema_editor, from_state,
                            to_state):
         pass
 
 
 class Migration(migrations.Migration):
-
-    u"""Инициализация подсистемы журналирования изменений в БД."""
+    """Инициализация подсистемы журналирования изменений в БД."""
 
     dependencies = [
         ('audit_log', '0001_initial'),
     ]
 
     operations = [
         InitDefaultDatabase(),
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/migrations/0005_postgresql_error.py` & `educommon-3.0.0/src/educommon/audit_log/migrations/0005_postgresql_error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
+from django.db import (
+    migrations,
+)
 
-from django.db import migrations
-
-from ..utils.operations import ReinstallAuditLog
+from educommon.audit_log.utils.operations import (
+    ReinstallAuditLog,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('audit_log', '0004_reinstall_audit_log'),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py` & `educommon-3.0.0/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Generated by Django 2.2.15 on 2020-08-06 17:07
-
 import datetime
 
-from django.db import migrations
-from django.db import models
 import django.core.validators
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('audit_log', '0005_postgresql_error'),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py` & `educommon-3.0.0/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-# Generated by Django 2.2.15 on 2020-08-06 17:07
 import os
 
-from django.conf import settings
-from django.db import connections
-from django.db import migrations
+from django.conf import (
+    settings,
+)
+from django.db import (
+    connections,
+    migrations,
+)
 
-from educommon.audit_log.constants import PG_LOCK_ID
-from educommon.audit_log.constants import SQL_FILES_DIR
-from educommon.audit_log.utils import execute_sql_file
-from educommon.audit_log.utils import get_db_connection_params
+from educommon.audit_log.constants import (
+    PG_LOCK_ID,
+    SQL_FILES_DIR,
+)
+from educommon.audit_log.utils import (
+    execute_sql_file,
+    get_db_connection_params,
+)
 
 
 def create_select_table_function(apps, schema_editor):
     """Создается функция в БД."""
     if schema_editor.connection.alias != settings.DEFAULT_DB_ALIAS:
         return
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/models.py` & `educommon-3.0.0/src/educommon/audit_log/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,132 +1,149 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from datetime import datetime
-
-from celery.signals import before_task_publish
-from celery.signals import task_postrun
-from celery.signals import task_prerun
-from django.contrib.contenttypes.models import ContentType
-from django.contrib.postgres.fields import HStoreField
-from django.core.validators import MinValueValidator
-from django.db import models
-from django.db.backends.signals import connection_created
-from django.dispatch.dispatcher import receiver
-import six
-
-from educommon.django.db.models import BaseModel
-from educommon.django.db.models import ReadOnlyMixin
-from educommon.thread_data import thread_data
-
-from .utils import get_audit_log_context
-from .utils import get_model_by_table
-from .utils import set_db_param
+from datetime import (
+    datetime,
+)
+
+from celery.signals import (
+    before_task_publish,
+    task_postrun,
+    task_prerun,
+)
+from django.contrib.contenttypes.models import (
+    ContentType,
+)
+from django.contrib.postgres.fields import (
+    HStoreField,
+)
+from django.core.validators import (
+    MinValueValidator,
+)
+from django.db import (
+    models,
+)
+from django.db.backends.signals import (
+    connection_created,
+)
+from django.dispatch.dispatcher import (
+    receiver,
+)
+
+from educommon.audit_log.utils import (
+    get_audit_log_context,
+    get_model_by_table,
+    set_db_param,
+)
+from educommon.django.db.models import (
+    BaseModel,
+    ReadOnlyMixin,
+)
+from educommon.thread_data import (
+    thread_data,
+)
 
 
 class Table(ReadOnlyMixin, BaseModel):
 
     name = models.CharField(
         max_length=250,
-        verbose_name=u'Имя таблицы'
+        verbose_name='Имя таблицы'
     )
     schema = models.CharField(
         max_length=250,
-        verbose_name=u'Схема таблицы'
+        verbose_name='Схема таблицы'
     )
 
     class Meta:
         unique_together = ('name', 'schema')
-        verbose_name = u'Логируемая таблица'
-        verbose_name_plural = u'Логируемые таблицы'
+        verbose_name = 'Логируемая таблица'
+        verbose_name_plural = 'Логируемые таблицы'
 
 
 class AuditLog(ReadOnlyMixin, BaseModel):
 
     OPERATION_CREATE = 1
     OPERATION_UPDATE = 2
     OPERATION_DELETE = 3
     OPERATION_CHOICES = (
-        (OPERATION_CREATE, u'Создание'),
-        (OPERATION_UPDATE, u'Изменение'),
-        (OPERATION_DELETE, u'Удаление')
+        (OPERATION_CREATE, 'Создание'),
+        (OPERATION_UPDATE, 'Изменение'),
+        (OPERATION_DELETE, 'Удаление')
     )
 
     user_id = models.IntegerField(
         null=True,
         db_index=True,
-        verbose_name=u'Пользователь',
+        verbose_name='Пользователь',
     )
     user_type_id = models.IntegerField(
         null=True,
         db_index=True,
-        verbose_name=u'Тип пользователя',
+        verbose_name='Тип пользователя',
     )
     ip = models.GenericIPAddressField(
         null=True,
-        verbose_name=u'IP адрес'
+        verbose_name='IP адрес'
     )
     time = models.DateTimeField(
         auto_now_add=True,
         db_index=True,
-        verbose_name=u'Дата, время'
+        verbose_name='Дата, время'
     )
     table = models.ForeignKey(
         Table,
-        verbose_name=u'Таблица',
+        verbose_name='Таблица',
         on_delete=models.CASCADE,
     )
     object_id = models.IntegerField(
         db_index=True,
-        verbose_name=u'Объект модели'
+        verbose_name='Объект модели'
     )
     data = HStoreField(
         null=True,
-        verbose_name=u'Объект'
+        verbose_name='Объект'
     )
     changes = HStoreField(
         null=True,
-        verbose_name=u'Изменения'
+        verbose_name='Изменения'
     )
     operation = models.SmallIntegerField(
         choices=OPERATION_CHOICES,
-        verbose_name=u'Действие'
+        verbose_name='Действие'
     )
 
     def is_read_only(self):
-        u"""Запрещает запись в лог приложению."""
+        """Запрещает запись в лог приложению."""
         return True
 
     def get_read_only_error_message(self, delete):
-        action_text = u'удалить' if delete else u'изменить'
-        result = u'Нельзя {} запись лога.'.format(action_text)
+        action_text = 'удалить' if delete else 'изменить'
+        result = 'Нельзя {} запись лога.'.format(action_text)
         return result
 
     @property
     def model(self):
-        u"""Класс измененной модели."""
+        """Класс измененной модели."""
         return get_model_by_table(self.table)
 
     @property
     def fields(self):
-        u"""Все поля измененной модели.
+        """Все поля измененной модели.
 
         :returns dict: {имя колонки в БД: поле, ...}
         """
         model = self.model
         if model:
             result = {
                 field.get_attname_column()[1]: field
                 for field in model._meta.fields
             }
             return result
 
     @property
     def user(self):
-        u"""Пользователь, внесший изменения."""
+        """Пользователь, внесший изменения."""
         result = None
         try:
             content_type = ContentType.objects.get(id=self.user_type_id)
         except ContentType.DoesNotExist:
             pass
         else:
             model_class = content_type.model_class()
@@ -135,46 +152,45 @@
                     return model_class.objects.get(pk=self.user_id)
                 except model_class.DoesNotExist:
                     pass
 
         return result
 
     class Meta:
-        verbose_name = u'Запись журнала изменений'
-        verbose_name_plural = u'Записи журнала изменений'
+        verbose_name = 'Запись журнала изменений'
+        verbose_name_plural = 'Записи журнала изменений'
 
 
 class PostgreSQLError(BaseModel):
-
-    u"""Журнал ошибок, возникающих при работе триггеров журнала изменений."""
+    """Журнал ошибок, возникающих при работе триггеров журнала изменений."""
 
     user_id = models.IntegerField(
-        u'Пользователь',
+        'Пользователь',
         null=True,
     )
     ip = models.GenericIPAddressField(
-        u'IP адрес',
+        'IP адрес',
         null=True,
     )
     time = models.DateTimeField(
-        u'Дата, время',
+        'Дата, время',
         auto_now_add=True,
         validators=[MinValueValidator(datetime(1900, 1, 1))],
     )
     level = models.CharField(
-        u'Уровень ошибки',
+        'Уровень ошибки',
         max_length=50,
     )
     text = models.TextField(
-        u'Текст ошибки',
+        'Текст ошибки',
     )
 
     class Meta:
-        verbose_name = u'Ошибка PostgreSQL'
-        verbose_name_plural = u'Ошибки PostgreSQL'
+        verbose_name = 'Ошибка PostgreSQL'
+        verbose_name_plural = 'Ошибки PostgreSQL'
         db_table = 'audit"."postgresql_errors'
 
 
 class LoggableModelMixin(models.Model):
     """Делает модель логируемой."""
     need_to_log = True
 
@@ -191,15 +207,15 @@
 
 
 _package_name = __name__.rpartition('.')[0]
 
 
 @before_task_publish.connect(dispatch_uid=_package_name + 'save')
 def _save_audit_log_context_for_task(body, **_):
-    u"""Дополняет параметры задания данными для журнала изменений.
+    """Дополняет параметры задания данными для журнала изменений.
 
     В словарь ``kwargs``, передаваемый в метод ``apply_async`` задания,
     добавляет параметр ``audit_log_params``, содержащий результат вызова
     функции :func:`~extedu.audit_log.utils.get_audit_log_context`.
 
     Работает только если запуск задания осуществляется в рамках обработки
     HTTP-запроса, т.е. если в :obj:`extedu.thread_data.http_request` сохранен
@@ -211,15 +227,15 @@
     body['kwargs'] = body.get('kwargs', {})
     request = thread_data.http_request
     body['kwargs']['audit_log_params'] = get_audit_log_context(request)
 
 
 @task_prerun.connect(dispatch_uid=_package_name + 'set')
 def _set_audit_log_context_for_task(kwargs, **_):
-    u"""До выполнения задания сохраняет параметры контекста журнала изменений.
+    """До выполнения задания сохраняет параметры контекста журнала изменений.
 
     Сохраненные в :obj:`extedu.thread_data.audit_log_params` параметры
     будут переданы в БД при подключении (см.
     ``_send_audit_log_context_to_db``).
     """
     if 'audit_log_params' in kwargs:
         thread_data.audit_log_params = kwargs['audit_log_params']
@@ -230,10 +246,10 @@
     if hasattr(thread_data, 'audit_log_params'):
         del thread_data.audit_log_params
 
 
 @receiver(connection_created, dispatch_uid=_package_name + 'send')
 def _send_audit_log_context_to_db(**kwargs):
     if hasattr(thread_data, 'audit_log_params'):
-        for name, value in six.iteritems(thread_data.audit_log_params):
+        for name, value in thread_data.audit_log_params.items():
             set_db_param('audit_log.' + name, value)
 # -----------------------------------------------------------------------------
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/permissions.py` & `educommon-3.0.0/src/educommon/audit_log/permissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-
 PERM_GROUP__AUDIT_LOG = 'audit_log'
 PERM_GROUP__AUDIT_LOG_ERRORS = 'audit_log_errors'
 
 
 PERM__AUDIT_LOG__VIEW = PERM_GROUP__AUDIT_LOG + '/view'
 PERM__AUDIT_LOG__ERRORS__VIEW = PERM_GROUP__AUDIT_LOG_ERRORS + '/view'
 PERM__AUDIT_LOG__ERRORS__DELETE = PERM_GROUP__AUDIT_LOG_ERRORS + '/delete'
 
 
 permissions = (
     (PERM__AUDIT_LOG__VIEW,
-     u'Просмотр',
-     u'Разрешает просмотр журнала изменений.'),
+     'Просмотр',
+     'Разрешает просмотр журнала изменений.'),
     (PERM__AUDIT_LOG__ERRORS__VIEW,
-     u'Просмотр журнала ошибок PostgreSQL',
-     u'Разрешает просмотр журнала ошибок PostgreSQL.'),
+     'Просмотр журнала ошибок PostgreSQL',
+     'Разрешает просмотр журнала ошибок PostgreSQL.'),
     (PERM__AUDIT_LOG__ERRORS__DELETE,
-     u'Удаление записей журнала ошибок PostgreSQL',
-     u'Разрешает удаление записей из журнала ошибок PostgreSQL.'),
+     'Удаление записей журнала ошибок PostgreSQL',
+     'Разрешает удаление записей из журнала ошибок PostgreSQL.'),
 )
 
 
 dependencies = {
     PERM__AUDIT_LOG__ERRORS__DELETE: {
         PERM__AUDIT_LOG__ERRORS__VIEW,
     },
 }
 
 
 groups = {
-    PERM_GROUP__AUDIT_LOG: u'Журнал изменений',
-    PERM_GROUP__AUDIT_LOG_ERRORS: u'Журнал изменений',
+    PERM_GROUP__AUDIT_LOG: 'Журнал изменений',
+    PERM_GROUP__AUDIT_LOG_ERRORS: 'Журнал изменений',
 }
 
 
 partitions = {
-    u'Администрирование': (
+    'Администрирование': (
         PERM_GROUP__AUDIT_LOG,
         PERM_GROUP__AUDIT_LOG_ERRORS,
     ),
 }
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/proxies.py` & `educommon-3.0.0/src/educommon/audit_log/proxies.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,192 +1,203 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import os
 
-from django.conf import settings
-from django.contrib.contenttypes.models import ContentType
-from django.db.models import BooleanField
-from django.db.models import DateField
-from django.db.models import DateTimeField
-from django.db.models import FileField
-from django.db.models import FloatField
-from django.db.models import IntegerField
-from django.db.models import TimeField
-from django.db.models.fields.related import RelatedField
-from django.utils.dateparse import parse_date
-from django.utils.dateparse import parse_datetime
-from django.utils.dateparse import parse_time
-from django.utils.encoding import force_text
-from m3_django_compat import get_related
-import six
-
-from .models import AuditLog
+from django.conf import (
+    settings,
+)
+from django.contrib.contenttypes.models import (
+    ContentType,
+)
+from django.db.models import (
+    BooleanField,
+    DateField,
+    DateTimeField,
+    FileField,
+    FloatField,
+    IntegerField,
+    TimeField,
+)
+from django.db.models.fields.related import (
+    RelatedField,
+)
+from django.utils.dateparse import (
+    parse_date,
+    parse_datetime,
+    parse_time,
+)
+from django.utils.encoding import (
+    force_text,
+)
+from m3_django_compat import (
+    get_related,
+)
+
+from educommon.audit_log.models import (
+    AuditLog,
+)
 
 
 class LogProxy(AuditLog):
-
-    u"""Прокси-модель для отображения."""
+    """Прокси-модель для отображения."""
 
     class Meta:
         proxy = True
 
     @property
     def user_name(self):
-        u"""Отображаемое имя пользователя."""
+        """Отображаемое имя пользователя."""
         user_type_id = self.user_type_id
         user_id = self.user_id
         if user_type_id is not None and user_id is not None:
             try:
                 model = ContentType.objects.get(id=user_type_id).model_class()
             except ContentType.DoesNotExist:
-                result = u'Model:{}, id:{}'.format(user_type_id, user_id)
+                result = 'Model:{}, id:{}'.format(user_type_id, user_id)
             else:
                 try:
                     result = model.objects.get(id=user_id).person.fullname
                 except model.DoesNotExist:
-                    result = u'{}({})'.format(
+                    result = '{}({})'.format(
                         model._meta.verbose_name, user_id
                     )
         else:
-            result = u''
+            result = ''
         return result
 
     @property
     def model_fullname(self):
-        u"""Отображаемое и системное имя модели."""
+        """Отображаемое и системное имя модели."""
         model = self.model
         if model:
-            return u'{} - {}'.format(model._meta.verbose_name, model.__name__)
+            return '{} - {}'.format(model._meta.verbose_name, model.__name__)
         return self.table.name
 
     @property
     def model_name(self):
-        u"""Отображаемое имя модели."""
+        """Отображаемое имя модели."""
         model = self.model
 
         if model:
             verbose = model._meta.verbose_name
             if verbose:
-                return u' - '.join((force_text(verbose), model.__name__))
+                return ' - '.join((force_text(verbose), model.__name__))
             return model.__name__
         return self.table.name
 
     @property
     def diff(self):
-        u"""Возвращает diff для объекта.
+        """Возвращает diff для объекта.
 
         :return: list[dict]: Словари, с ключами "name", "old", "new", где:
             "name" - verbose_name поля модели, если удалось определить,
                      иначе его имя,
             "old" и "new" - старое и новое значение поля соответственно.
         """
         empty = {}
 
         if self.operation == self.OPERATION_CREATE:
-            keys = six.iterkeys(self.data)
+            keys = self.data.keys()
             data = empty
             new_data = self.data or empty
         elif self.operation == self.OPERATION_UPDATE:
-            keys = six.iterkeys(self.changes)
+            keys = self.changes.keys()
             data = self.data or empty
             new_data = self.changes or empty
         elif self.operation == self.OPERATION_DELETE:
-            keys = six.iterkeys(self.data)
+            keys = self.data.keys()
             data = self.data or empty
             new_data = empty
         else:
             keys = data = new_data = empty
 
         result = [
             {
                 'name': self.get_field_string(key),
-                'old': self.convert_field_value(key, data.get(key, u'')),
-                'new': self.convert_field_value(key, new_data.get(key, u''))
+                'old': self.convert_field_value(key, data.get(key, '')),
+                'new': self.convert_field_value(key, new_data.get(key, ''))
             }
             for key in keys
         ]
         result.sort(key=lambda x: x['name'])
 
         return result
 
     def get_field_string(self, column_name):
-        u"""Возвращает отображаемое имя поля модели.
+        """Возвращает отображаемое имя поля модели.
 
         :param str column_name: имя столбца в БД.
-        :return unicode: verbose_name столбца, если есть, иначе column_name.
+        :return str: verbose_name столбца, если есть, иначе column_name.
         """
         name = column_name
         if self.fields:
             field = self.fields.get(column_name)
             if field and field.verbose_name:
                 name = force_text(field.verbose_name)
         return name
 
     def convert_field_value(self, column_name, value):
-        u"""Возвращает значение поля."""
+        """Возвращает значение поля."""
         def get_choice(choices, choice_id):
             if choice_id:
                 choice_id = int(choice_id)
             return dict(choices).get(choice_id, choice_id)
 
         if value is None:
-            return u''
+            return ''
 
         if self.fields:
             field = self.fields.get(column_name)
             if field:
                 try:
                     if isinstance(field, RelatedField):
                         if value:
                             related = get_related(field)
                             model = related.parent_model
                             field_name = related.relation.field_name
                             qs = model._default_manager.filter(
                                 **{field_name: value}
                             )[:1]
                             if qs:
-                                value = u'{{{}}} {}'.format(
+                                value = '{{{}}} {}'.format(
                                     qs[0].id,
                                     self._get_object_verbose_name(qs[0]),
                                 )
                     elif isinstance(field, BooleanField):
                         value_map = {
-                            't': u'Да', 'f': u'Нет'
+                            't': 'Да', 'f': 'Нет'
                         }
                         value = value_map.get(value, value)
                     elif isinstance(field, IntegerField) and field.choices:
                         value = get_choice(field.choices, value)
                 except (ValueError, TypeError):
                     pass
         return force_text(value)
 
     @property
     def object_string(self):
-        u"""Отображаемое имя экземпляра модели.
+        """Отображаемое имя экземпляра модели.
 
-        :rtype unicode
+        :rtype str
         """
         instance = self.instance
         if instance:
             return self._get_object_verbose_name(instance)
         return self._get_removed_object_verbose_name()
 
     @property
     def instance(self):
-        u"""Восстановленный экземпляр модели."""
+        """Восстановленный экземпляр модели."""
         result = None
 
         if self.model:
             result = self.model()
             fields_dict = {
                 field.name: field for field in
                 self.model._meta.fields
             }
-            for key, value in six.iteritems(self.data):
+            for key, value in self.data.items():
                 field = fields_dict.get(key)
                 converted_value = value
                 if field:
                     try:
                         if isinstance(field, DateTimeField):
                             converted_value = parse_datetime(value)
                         elif isinstance(field, DateField):
@@ -207,29 +218,29 @@
                     except (ValueError, TypeError):
                         pass
                 setattr(result, key, converted_value)
         return result
 
     @staticmethod
     def _get_object_verbose_name(instance):
-        u"""Возвращает отображаемое значение в unicode для инстанса модели."""
+        """Возвращает отображаемое значение в str для инстанса модели."""
         # pylint: disable=broad-except
 
         if hasattr(instance, 'log_display'):
             try:
                 return instance.log_display()
             except Exception:
                 pass
         elif hasattr(instance, 'display'):
             try:
                 return instance.display()
             except Exception:
                 pass
-        return six.text_type(instance)
+        return str(instance)
 
     def _get_removed_object_verbose_name(self):
-        u"""Возвращает отображаемое значение в unicode для инстанса модели."""
+        """Возвращает отображаемое значение в str для инстанса модели."""
         attrs = ('name', 'fullname', 'full_name', 'code', 'id')
         for attr in attrs:
             if attr in self.data:
                 return self.data[attr]
-        return u''
+        return ''
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/sql/configure_audit_log.sql` & `educommon-3.0.0/src/educommon/audit_log/sql/configure_audit_log.sql`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/audit_log/sql/create_selective_tables_function.sql` & `educommon-3.0.0/src/educommon/audit_log/sql/create_selective_tables_function.sql`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/audit_log/sql/install_audit_log.sql` & `educommon-3.0.0/src/educommon/audit_log/sql/install_audit_log.sql`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/audit_log/utils/__init__.py` & `educommon-3.0.0/src/educommon/audit_log/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,62 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from contextlib import closing
-from functools import reduce
-from operator import and_
-from os import path
 import os
-
-from django.apps import apps
-from django.conf import settings
-from django.db import connection
-from django.db import connections
-from django.db.models import Q
-from django.db.models.fields import related
-from django.db.transaction import atomic
-from django.http import HttpRequest
-from m3_django_compat import get_related
-import six
-
-from educommon import ioc
-from educommon.audit_log.constants import EXCLUDED_TABLES
-from educommon.audit_log.constants import PG_LOCK_ID
-from educommon.audit_log.constants import SQL_FILES_DIR
-from educommon.utils.misc import cached_property
+from contextlib import (
+    closing,
+)
+from functools import (
+    reduce,
+)
+from operator import (
+    and_,
+)
+from os import (
+    path,
+)
+
+from django.apps import (
+    apps,
+)
+from django.conf import (
+    settings,
+)
+from django.db import (
+    connection,
+    connections,
+)
+from django.db.models import (
+    Q,
+)
+from django.db.models.fields import (
+    related,
+)
+from django.db.transaction import (
+    atomic,
+)
+from django.http import (
+    HttpRequest,
+)
+from m3_django_compat import (
+    get_related,
+)
+
+from educommon import (
+    ioc,
+)
+from educommon.audit_log.constants import (
+    EXCLUDED_TABLES,
+    PG_LOCK_ID,
+    SQL_FILES_DIR,
+)
+from educommon.utils.misc import (
+    cached_property,
+)
 
 
 def configure():
-    u"""Изменяет параметры подключения к сервисной БД, обновляет триггеры."""
+    """Изменяет параметры подключения к сервисной БД, обновляет триггеры."""
     params = get_db_connection_params()
     params['lock_id'] = PG_LOCK_ID
     execute_sql_file(
         'default',
         os.path.join(SQL_FILES_DIR, 'configure_audit_log.sql'),
         params
     )
@@ -41,15 +67,17 @@
             os.path.join(SQL_FILES_DIR, 'configure_selective_audit_log.sql'),
             params
         )
 
 
 def _set_audit_log_tables():
     """Собирает логируемые таблицы."""
-    from django.apps import apps
+    from django.apps import (
+        apps,
+    )
 
     table_names = set(
         model._meta.db_table
         for model in apps.get_models()
         if getattr(model, 'need_to_log', False)
     )
 
@@ -80,15 +108,15 @@
     # т.к. логов, ссылающихся на удаляемые таблицы, больше не существует:
     Table.objects.filter(
         name__in=table_names_for_deleting,
     ).delete()
 
 
 def is_initialized(database_alias):
-    u"""Проверяет, проинициализированы ли средства журналирования.
+    """Проверяет, проинициализированы ли средства журналирования.
 
     :param str database_alias: Алиас БД, в которой будет проверяться наличие
         средств журналирования.
 
     :rtype: bool
     """
     # Проверка наличия схемы audit.
@@ -132,15 +160,15 @@
             if cursor.fetchone() is None:
                 return False
 
     return True
 
 
 def check_connection_fdw():
-    u"""Проверяет подключение к сервисной БД через PostgreSQL FDW.
+    """Проверяет подключение к сервисной БД через PostgreSQL FDW.
 
     :returns: Кортеж из двух элементов: первый указывает на работоспособность
         подключения (``True`` - есть, ``False`` - нет подключения), второй --
         содержит текст ошибки, если подключения нет.
     :rtype: tuple
     """
     with closing(connection.cursor()) as cursor:
@@ -150,54 +178,54 @@
             return False, str(error)
         else:
             return True, None
 
 
 @atomic
 def execute_sql_file(database_alias, file_name, params=None):
-    u"""Исполняет SQL-скрипт, из файла по указанному пути."""
+    """Исполняет SQL-скрипт, из файла по указанному пути."""
     cursor = connections[database_alias].cursor()
 
     file_path = path.join(path.dirname(__file__), file_name)
     with open(file_path, 'r') as f:
         file_contents = f.read()
 
     if params:
         file_contents = file_contents.format(**params)
 
     cursor.execute(file_contents)
 
 
 def get_db_connection_params():
-    u"""Возвращает параметры подключения к сервисной БД."""
+    """Возвращает параметры подключения к сервисной БД."""
     target_db_conf = settings.DATABASES[settings.SERVICE_DB_ALIAS]
     return dict(
         host=target_db_conf['HOST'],
         dbname=target_db_conf['NAME'],
         port=target_db_conf['PORT'],
         user=target_db_conf['USER'],
         password=target_db_conf['PASSWORD']
     )
 
 
 @atomic()
 def set_db_param(key, value):
-    u"""Устанавливает параметры в custom settings postgresql."""
+    """Устанавливает параметры в custom settings postgresql."""
     cursor = connection.cursor()
     if value:
-        value = six.text_type(value)
+        value = str(value)
     else:
-        value = u''
+        value = ''
 
-    sql = u"SELECT set_config(%s, %s, False);"
+    sql = 'SELECT set_config(%s, %s, False);'
     cursor.execute(sql, (key, value))
 
 
 def get_ip(request):
-    u"""Возвращает ip источника запроса.
+    """Возвращает ip источника запроса.
 
     :param request: запрос
     :type django.http.HttpRequest
 
     :return IP адрес
     :rtype str or None
     """
@@ -216,32 +244,32 @@
         x_forward_ip, _, _ = x_forward_for.partition(',')
         return x_forward_ip.strip()
 
     return request.META.get('REMOTE_ADDR', None)
 
 
 def make_hstore_filter(field, value):
-    u"""Создает lookup фильтр из строки.
+    """Создает lookup фильтр из строки.
 
     :param str field: название поля (type hstore).
-    :param unicode value: значение, по которому фильтруется queryset.
+    :param str value: значение, по которому фильтруется queryset.
     Если строка, то разбивается на отдельные слова.
     """
     result = reduce(
         and_,
         (Q(**{'%s__values__icontains' % field: x}) for x in value.split(' '))
     )
     return result
 
 
 def make_name_filter(field, value):
-    u"""Создает lookup фильтра по фамилии/имени/отчеству пользователя.
+    """Создает lookup фильтра по фамилии/имени/отчеству пользователя.
 
     :param str field: название поля ('firstname', 'surname', 'patronymic').
-    :param unicode value: значение, по которому фильтруется queryset.
+    :param str value: значение, по которому фильтруется queryset.
     """
     ContentType = apps.get_model('contenttypes', 'ContentType')
     Employee = apps.get_model('employee', 'Employee')
     SysAdmin = apps.get_model('sysadmin', 'SysAdmin')
 
     result = None
     for model in (Employee, SysAdmin):
@@ -255,15 +283,15 @@
         if result:
             result |= qobj
         else:
             result = qobj
     return result
 
 
-class ModelRegistry(object):
+class ModelRegistry:
 
     @cached_property
     def table_model(self):
         return {
             model._meta.db_table: model
             for model in apps.get_models(include_auto_created=True)
             if not (model._meta.proxy)
@@ -273,15 +301,15 @@
         return self.table_model.get(table_name)
 
 
 model_registry = ModelRegistry()
 
 
 def get_model_choices(excluded=None):
-    u"""Список выбора для комбобокса.
+    """Список выбора для комбобокса.
 
     Ключ - id таблицы, отображаемое значение - name
     и verbose_name модели.
     """
     total_exclude = EXCLUDED_TABLES
     table_class = apps.get_model('audit_log', 'Table')
     if excluded:
@@ -297,15 +325,15 @@
         key=lambda x: x[1]
     )
 
     return tuple(result)
 
 
 def _get_m2m_model_fields(model):
-    u"""Возвращает поля автоматически созданной m2m таблицы.
+    """Возвращает поля автоматически созданной m2m таблицы.
 
     :return Два поля типа ForeignKey или None, если таблица не
             соответствует автоматически созданной.
     """
     result = [
         field
         for field
@@ -313,44 +341,44 @@
         if isinstance(field, related.ForeignKey)
     ]
     if len(result) == 2:
         return result
 
 
 def get_table_name(table):
-    u"""Возвращает имя таблицы в понятном пользователю виде."""
+    """Возвращает имя таблицы в понятном пользователю виде."""
     model = get_model_by_table(table)
     if model:
         class_name = model.__name__
         verbose_name = model._meta.verbose_name.capitalize()
         if model._meta.auto_created:
             fields = _get_m2m_model_fields(model)
             if fields:
                 names = [
                     get_related(f).parent_model._meta.verbose_name
                     for f in fields
                 ]
-                verbose_name = u'Связь {}, {}'.format(names[0], names[1])
+                verbose_name = 'Связь {}, {}'.format(names[0], names[1])
 
-        return u'{} - {}'.format(
+        return '{} - {}'.format(
             verbose_name,
             class_name
         )
     else:
         return table.name
 
 
 def get_model_by_table(table):
-    u"""Возвращает класс модели по имени таблицы."""
+    """Возвращает класс модели по имени таблицы."""
     assert isinstance(table, apps.get_model('audit_log', 'Table'))
     return model_registry.get_model(table.name)
 
 
 def get_audit_log_context(request):
-    u"""Возвращает параметры контекста журналирования изменений."""
+    """Возвращает параметры контекста журналирования изменений."""
     result = {}
 
     current_user = ioc.get('get_current_user')(request)
     if current_user:
         ContentType = apps.get_model('contenttypes', 'ContentType')
 
         result['user_id'] = current_user.id
```

### Comparing `educommon-2.20.0/src/educommon/audit_log/utils/operations.py` & `educommon-3.0.0/src/educommon/audit_log/utils/operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-# coding: utf-8
 # pylint: disable=abstract-method
-from __future__ import absolute_import
-
 import codecs
 import os
 
-from django.conf import settings
-from django.db.migrations.operations.base import Operation
-
-from ..constants import PG_LOCK_ID
-from ..constants import SQL_FILES_DIR
-from ..utils import get_db_connection_params
+from django.conf import (
+    settings,
+)
+from django.db.migrations.operations.base import (
+    Operation,
+)
+
+from educommon.audit_log.constants import (
+    PG_LOCK_ID,
+    SQL_FILES_DIR,
+)
+from educommon.audit_log.utils import (
+    get_db_connection_params,
+)
 
 
 class ReinstallAuditLog(Operation):
-
-    u"""Пересоздаёт функции журнала изменений в БД.
+    """Пересоздаёт функции журнала изменений в БД.
 
     Используется для миграции после модификации sql файла.
 
     Удаляет схему audit. В этой схеме не должно храниться никаких таблиц
     с данными.
     После удаления устанавливает audit_log заново.
     """
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/actions.py` & `educommon-3.0.0/src/educommon/auth/rbac/actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,107 +1,152 @@
-# coding: utf-8
-u"""Паки и экшены для окна реестра "Роли"."""
-from __future__ import absolute_import
-
-from collections import defaultdict
-from functools import reduce
-from itertools import chain
-from operator import or_
+"""Паки и экшены для окна реестра "Роли"."""
 import json
-
-from django.contrib.contenttypes.models import ContentType
-from django.db.models import Case
-from django.db.models import F
-from django.db.models import Q
-from django.db.models import Value
-from django.db.models import When
-from django.db.models.fields import CharField
-from django.db.models.functions import Concat
-from django.utils.functional import cached_property
-from m3.actions import ApplicationLogicException
-from m3.actions import PreJsonResult
-from m3.actions.results import OperationResult
-from m3_django_compat import atomic
-from m3_django_compat import get_request_params
-from objectpack.actions import BaseAction
-from objectpack.actions import BasePack
-from objectpack.actions import ObjectPack
-from objectpack.actions import ObjectRowsAction
-from objectpack.actions import ObjectSelectWindowAction
-from objectpack.exceptions import ValidationError
-from objectpack.models import VirtualModel
-from objectpack.tools import extract_int_list
-from objectpack.tree_object_pack.actions import TreeObjectPack
-import six
-
-from educommon.auth.rbac.config import rbac_config
-from educommon.auth.rbac.utils import get_permission_full_title
-from educommon.m3 import convert_validation_error_to
-from educommon.m3 import get_id_value
-from educommon.m3 import get_pack
-from educommon.m3 import get_pack_id
-
-from . import ui
-from .constants import PERM_SOURCE__DEPENDENCIES
-from .constants import PERM_SOURCE__NESTED_ROLE
-from .constants import PERM_SOURCE__ROLE
-from .manager import rbac
-from .models import Permission
-from .models import Role
-from .models import RoleParent
-from .models import RolePermission
-from .models import RoleUserType
-from .models import UserRole
-from .permissions import PERM_GROUP__ROLE
+from collections import (
+    defaultdict,
+)
+from functools import (
+    reduce,
+)
+from itertools import (
+    chain,
+)
+from operator import (
+    or_,
+)
+
+from django.contrib.contenttypes.models import (
+    ContentType,
+)
+from django.db.models import (
+    Case,
+    F,
+    Q,
+    Value,
+    When,
+)
+from django.db.models.fields import (
+    CharField,
+)
+from django.db.models.functions import (
+    Concat,
+)
+from django.utils.functional import (
+    cached_property,
+)
+from m3.actions import (
+    ApplicationLogicException,
+    PreJsonResult,
+)
+from m3.actions.results import (
+    OperationResult,
+)
+from m3_django_compat import (
+    atomic,
+    get_request_params,
+)
+
+from objectpack.actions import (
+    BaseAction,
+    BasePack,
+    ObjectPack,
+    ObjectRowsAction,
+    ObjectSelectWindowAction,
+)
+from objectpack.exceptions import (
+    ValidationError,
+)
+from objectpack.models import (
+    VirtualModel,
+)
+from objectpack.tools import (
+    extract_int_list,
+)
+from objectpack.tree_object_pack.actions import (
+    TreeObjectPack,
+)
+
+from educommon.auth.rbac import (
+    ui,
+)
+from educommon.auth.rbac.config import (
+    rbac_config,
+)
+from educommon.auth.rbac.constants import (
+    PERM_SOURCE__DEPENDENCIES,
+    PERM_SOURCE__NESTED_ROLE,
+    PERM_SOURCE__ROLE,
+)
+from educommon.auth.rbac.manager import (
+    rbac,
+)
+from educommon.auth.rbac.models import (
+    Permission,
+    Role,
+    RoleParent,
+    RolePermission,
+    RoleUserType,
+    UserRole,
+)
+from educommon.auth.rbac.permissions import (
+    PERM_GROUP__ROLE,
+)
+from educommon.auth.rbac.utils import (
+    get_permission_full_title,
+)
+from educommon.m3 import (
+    convert_validation_error_to,
+    get_id_value,
+    get_pack,
+    get_pack_id,
+)
 
 
 def _get_role(role_id):
     try:
         return Role.objects.get(pk=role_id)
     except Role.DoesNotExist:
         raise ApplicationLogicException(
-            u'Роль ID:{} не существует'.format(role_id)
+            'Роль ID:{} не существует'.format(role_id)
         )
 
 
 class RolesTreeRowsAction(ObjectRowsAction):
-
-    u"""Экшн, отдающий данные иерархии ролей.
+    """Экшн, отдающий данные иерархии ролей.
 
     Т.к. одна и та же роль может быть включена в несколько ролей, то она также
     может отображаться вложенной в несколько ролей.
     """
 
     @cached_property
     def _parent_ids(self):
-        u"""Id ролей, содержащих в себе другие роли.
+        """Id ролей, содержащих в себе другие роли.
 
         :rtype: set
         """
         result = RoleParent.objects.values_list('parent', flat=True).distinct()
 
         return set(result)
 
     def is_leaf(self, role):
-        u"""Возвращает True, если данная роль не включает другие роли.
+        """Возвращает True, если данная роль не включает другие роли.
 
         :param role: Роль.
         :type role: Role
 
         :rtype: bool
         """
         if get_request_params(self.request).get('filter', False):
             result = True
         else:
             result = role.id not in self._parent_ids
 
         return result
 
     def prepare_object(self, obj):
-        u"""Сохранение данных роли в словарь перед сериализацией в JSON."""
+        """Сохранение данных роли в словарь перед сериализацией в JSON."""
         data = super(RolesTreeRowsAction, self).prepare_object(obj)
 
         data['leaf'] = self.is_leaf(obj)
 
         return data
 
     def run(self, *args, **kwargs):
@@ -109,16 +154,15 @@
 
         data = result.data.get('rows', [])
 
         return PreJsonResult(data)
 
 
 class AddRoleToRoleWindowAction(ObjectSelectWindowAction):
-
-    u"""Отображение окна добавления одной роли в другую."""
+    """Отображение окна добавления одной роли в другую."""
 
     def create_window(self):
         self.win = ui.RoleSelectWindow()
 
     def set_window_params(self):
         super(AddRoleToRoleWindowAction, self).set_window_params()
 
@@ -126,60 +170,57 @@
 
         role_id = getattr(self.context, self.parent.id_param_name)
         role = _get_role(role_id)
         self.win_params['role'] = role
 
 
 class AddRoleToRoleAction(BaseAction):
-
-    u"""Добавление одной роли к другой."""
+    """Добавление одной роли к другой."""
 
     @convert_validation_error_to(ApplicationLogicException)
     def run(self, request, context):
         role_parent = RoleParent(
             role=_get_role(getattr(context, self.parent.id_param_name)),
             parent=_get_role(context.parent_id),
         )
         role_parent.full_clean()
         role_parent.save()
 
         return OperationResult()
 
 
 class DeleteRoleFromRoleAction(BaseAction):
-
-    u"""Удаление одной роли из другой."""
+    """Удаление одной роли из другой."""
 
     def run(self, request, context):
         try:
             role_parent = RoleParent.objects.get(
                 role=_get_role(getattr(context, self.parent.id_param_name)),
                 parent_id=context.parent_id
             )
         except RoleParent.DoesNotExist:
             raise ApplicationLogicException(
-                u'Выбранная роль должна являться вложенной ролью.'
+                'Выбранная роль должна являться вложенной ролью.'
             )
 
         role_parent.delete()
 
         return OperationResult()
 
 
 class Pack(TreeObjectPack):
-
-    u"""Пак окна реестра "Роли"."""
+    """Пак окна реестра "Роли"."""
 
     model = Role
-    title = u'Роли'
+    title = 'Роли'
 
     columns = [
         dict(
             data_index='name',
-            header=u'Название',
+            header='Название',
             searchable=True,
         ),
     ]
 
     list_window = ui.RolesListWindow
     add_window = ui.RoleAddWindow
     edit_window = ui.RoleEditWindow
@@ -219,15 +260,15 @@
                        self.add_role_to_role_window_action,
                        self.add_role_to_role_action,
                        self.delete_role_from_role_action):
             action.perm_code = 'edit'
         # ---------------------------------------------------------------------
 
     def extend_menu(self, menu):
-        u"""Размещает в меню Пуск ссылку Администрирование --> Роли."""
+        """Размещает в меню Пуск ссылку Администрирование --> Роли."""
         return menu.administry(
             menu.Item(self.title, self.list_window_action),
         )
 
     def declare_context(self, action):
         result = super(Pack, self).declare_context(action)
 
@@ -241,16 +282,16 @@
             result['role_id'] = dict(type='int_or_none', default=None)
 
         if action is self.add_role_to_role_action:
             result['parent_id'] = dict(type='int')
 
         if action is self.save_action:
             result.update(
-                name=dict(type='unicode'),
-                description=dict(type='unicode', default=u''),
+                name=dict(type='str'),
+                description=dict(type='str', default=''),
                 permissions=dict(type='int_list', default=[]),
                 user_type_ids=dict(type='json_or_none', default=None),
             )
         if action is self.delete_role_from_role_action:
             result['parent_id'] = dict(type=int)
 
         return result
@@ -284,15 +325,15 @@
             # В этом режиме надо исключить возможность создания циклов в
             # иерархии ролей, поэтому из результатов запроса надо исключить
             # все подчиненные роли.
             try:
                 role = Role.objects.get(pk=context.role_id)
             except Role.DoesNotExist:
                 raise ApplicationLogicException(
-                    u'Роль ID:{} не найдена'.format(context.role_id)
+                    'Роль ID:{} не найдена'.format(context.role_id)
                 )
 
             result = result.exclude(
                 pk__in=set([role.id]) | set(r.id for r in role.subroles)
             )
 
         return result
@@ -323,39 +364,39 @@
         result_action = result_pack.result_permissions_action
         params['result_action_url'] = result_action.get_absolute_url()
 
         if rbac_config.user_types:
             params['show_user_types'] = True
             params['user_types'] = tuple(
                 (u_type.id, u_type.name)
-                for u_type in six.itervalues(
+                for u_type in (
                     ContentType.objects.get_for_models(
                         *rbac_config.user_types
-                    )
+                    ).values()
                 )
             )
             if not params['create_new']:
                 params['user_type_ids'] = tuple(
                     params['object'].user_types.values_list('pk', flat=True)
                 )
 
         if not params['create_new']:
             params['permission_ids'] = list(
                 params['object'].permissions.values_list('pk', flat=True)
             )
 
         params['can_edit'] = rbac.has_access(self.save_action, request)
         if not params['can_edit']:
-            params['title'] = self.format_window_title(u'Просмотр')
+            params['title'] = self.format_window_title('Просмотр')
 
         return params
 
     @staticmethod
     def _bind_user_types_to_role(role, types):
-        u"""Привязывает типы пользователей к роли.
+        """Привязывает типы пользователей к роли.
 
         При необходимости удаления типов пользователей, происходит
         проверка на наличие уже существующих пользователей с
         удаляемыми типами.
 
         :param role: роль в системе
         :type role: educommon.auth.rbac.models.Role
@@ -372,22 +413,22 @@
         )
         # Проверка, есть ли пользователи с удаляемыми типами
         if types_to_delete and user_roles_to_delete.exists():
             related_content_types = ContentType.objects.filter(
                 pk__in=types_to_delete
             )
             raise ApplicationLogicException(
-                u'Невозможно отменить назначение роли для пользователей '
-                u'типа {}, т.к. данная роль уже назначена {} '
-                u'пользователей.'.format(
-                    u', '.join(
-                        u'"{}"'.format(ct.name) for ct in related_content_types
+                'Невозможно отменить назначение роли для пользователей '
+                'типа {}, т.к. данная роль уже назначена {} '
+                'пользователей.'.format(
+                    ', '.join(
+                        '"{}"'.format(ct.name) for ct in related_content_types
                     ),
-                    u'этому типу'
-                    if len(types_to_delete) == 1 else u'этим типам',
+                    'этому типу'
+                    if len(types_to_delete) == 1 else 'этим типам',
                 )
             )
         # Удаление лишних типов пользователей
         RoleUserType.objects.filter(
             role=role, user_type__in=types_to_delete
         ).delete()
         # Добавление новых типов пользователей
@@ -410,15 +451,15 @@
             self._bind_user_types_to_role(obj, context.user_type_ids or ())
         # Сохранение связи с родительской ролью
         if create_new and context.parent_id is not None:
             try:
                 parent = Role.objects.get(pk=context.parent_id)
             except Role.DoesNotExist:
                 raise ApplicationLogicException(
-                    u'Роль ID:{} не существует.'.format(context.parent_id)
+                    'Роль ID:{} не существует.'.format(context.parent_id)
                 )
 
             RoleParent.objects.create(role=obj, parent=parent)
         else:
             new_permissions = set(extract_int_list(request, 'permissions'))
             old_permissions = set(obj.permissions.values_list('pk', flat=True))
 
@@ -432,18 +473,16 @@
             # Добавление новых прав в роль
             for permission_id in new_permissions - old_permissions:
                 RolePermission.objects.get_or_create(
                     role=obj, permission_id=permission_id
                 )
 
 
-@six.python_2_unicode_compatible
 class Partition(VirtualModel):
-
-    u"""Виртуальная модель "Раздел системы".
+    """Виртуальная модель "Раздел системы".
 
     Используется в связи с тем, что сведения о разделах не сохраняются в БД.
     """
 
     def __init__(self, data):
         self.__dict__.update(data)
 
@@ -457,23 +496,22 @@
         return cls.data
 
     def __str__(self):
         return self.title
 
 
 class PartitionsPack(ObjectPack):
-
-    u"""Пак для грида "Разделы системы" окна редактирования роли."""
+    """Пак для грида "Разделы системы" окна редактирования роли."""
 
     model = Partition
 
     columns = [
         dict(
             data_index='__str__',
-            header=u'Модуль',
+            header='Модуль',
         ),
     ]
 
     allow_paging = False
 
     def __init__(self):
         super(PartitionsPack, self).__init__()
@@ -484,33 +522,32 @@
 
         for action in self.actions:
             action.perm_code = 'view'
         # ---------------------------------------------------------------------
 
 
 class PermissionsPack(ObjectPack):
-
-    u"""Пак для грида "Права доступа" окна редактирования роли."""
+    """Пак для грида "Права доступа" окна редактирования роли."""
 
     model = Permission
 
     columns = (
         dict(
             data_index='title_with_group',
-            header=u'Разрешение',
+            header='Разрешение',
             column_renderer='columnRenderer',
             width=4,
         ),
         dict(
             data_index='description',
             hidden=True,
         ),
         dict(
             data_index='dependencies',
-            header=u'Включает разрешения',
+            header='Включает разрешения',
             width=5,
         ),
     )
     list_sort_order = ('title_with_group',)
 
     allow_paging = False
 
@@ -552,15 +589,15 @@
         # Определение название раздела по его id.
         try:
             partition = PartitionsPack.model.objects.get(
                 id=context.partition_id
             ).title
         except PartitionsPack.model.DoesNotExists:
             raise ApplicationLogicException(
-                u'Раздел {} не существует'.format(context.partition_id)
+                'Раздел {} не существует'.format(context.partition_id)
             )
 
         query = super(PermissionsPack, self).get_rows_query(
             request, context
         ).filter(
             # Условия для выборки разрешений только из раздела partition.
             reduce(or_, (
@@ -571,49 +608,48 @@
         ).annotate(title_with_group=Case(
             # Добавление названия группы к названию разрешения.
             output_field=CharField(),
             *(
                 When(
                     name__startswith=group + '/',
                     then=Concat(
-                        Value(title + u' - ' if title else u''),
+                        Value(title + ' - ' if title else ''),
                         F('title'),
                     )
                 )
-                for group, title in six.iteritems(rbac.groups)
+                for group, title in rbac.groups.items()
             )
         ))
 
         return query
 # -----------------------------------------------------------------------------
 
 def _get_group_name(perm_name):
     """Возвращает имя группы разрешения."""
     return perm_name.split('/')[0]
 
 def _get_group_title(perm_name):
-    u"""Возвращает название группы разрешений."""
+    """Возвращает название группы разрешений."""
     group_name = _get_group_name(perm_name)
     group_title = rbac.groups[group_name]
     return group_title
 
 
 def _get_partition_title(perm_name):
     group_name = perm_name.split('/')[0]
 
-    for title, names in six.iteritems(rbac.partitions):
+    for title, names in rbac.partitions.items():
         if group_name in names:
             return title
 
-    return u''
+    return ''
 
 
 class ResultPermissionsAction(BaseAction):
-
-    u"""Возвращает данные для грида "Итоговые разрешения"."""
+    """Возвращает данные для грида "Итоговые разрешения"."""
 
     def _get_nested_roles(self, role_id):
         role_children = defaultdict(set)
         query = RoleParent.objects.values_list('parent', 'role')
 
         for parent_id, child_id in query:
             role_children[parent_id].add(child_id)
@@ -655,15 +691,15 @@
                 hidden=False,
             ).values_list(
                 'pk', 'name', 'title', 'description'
             )
         }
         permissions_by_name = {
             name: (pk, title, description)
-            for pk, (name, title, description) in six.iteritems(permissions_by_id)
+            for pk, (name, title, description) in permissions_by_id.items()
         }
 
         for perm_id in permission_ids:
             # Может случиться так, что к роли будут привязаны скрытые
             # разрешения, но в permissions_by_id скрытых разрешений нет.
             if perm_id not in permissions_by_id:
                 # Пропускаем скрытые разрешения.
@@ -721,16 +757,15 @@
                     source=perm_data['source'],
                 ))
 
         return PreJsonResult(data)
 
 
 class ResultPermissionsPack(BasePack):
-
-    u"""Набор действий для грида "Итоговые разрешения" окна редактирования."""
+    """Набор действий для грида "Итоговые разрешения" окна редактирования."""
 
     def __init__(self):
         super(ResultPermissionsPack, self).__init__()
         # ---------------------------------------------------------------------
 
         self.result_permissions_action = ResultPermissionsAction()
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/backends/base.py` & `educommon-3.0.0/src/educommon/auth/rbac/backends/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-# coding: utf-8
-from __future__ import absolute_import
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
+
+from educommon import (
+    ioc,
+)
 
-from abc import ABCMeta
-from abc import abstractmethod
 
-import six
-
-from educommon import ioc
-
-
-class BackendBase(six.with_metaclass(ABCMeta, object)):
-
-    u"""Базовый класс для бэкендов RBAC."""
+class BackendBase(metaclass=ABCMeta):
+    """Базовый класс для бэкендов RBAC."""
 
     def __init__(self, manager):
         self._manager = manager
 
     def _need_check_access(self, action):
-        u"""Возвращает True, если ``action`` предполагает проверку доступа.
+        """Возвращает True, если ``action`` предполагает проверку доступа.
 
         :rtype: bool
         """
         return (
             action.parent.need_check_permission or
             action.need_check_permission
         )
 
     def _get_current_user(self, request):
-        u"""Возвращает текущего пользователя.
+        """Возвращает текущего пользователя.
 
         :rtype: bool
         """
         return ioc.get('get_current_user')(request)
 
     def _get_action_permissions(self, action):
-        u"""Возвращает имена разрешений экшена.
+        """Возвращает имена разрешений экшена.
 
         :rtype: tuple
         """
         if action.sub_permissions:
             result = tuple(
                 action.get_perm_code(sub_perm)
                 for sub_perm in action.sub_permissions
             )
         else:
             result = (action.get_perm_code(),)
 
         return result
 
     def _check_permission(self, permission_name, action, request, user):
-        u"""Проверяет возможность предоставления доступа.
+        """Проверяет возможность предоставления доступа.
 
         Если для указанного разрешения определены правила, то выполняет их
         проверку.
 
         :rtype: bool
         """
         if permission_name in self._manager.permission_rules:
@@ -68,26 +66,26 @@
             # только наличия у пользователя разрешения как такового.
             result = True
 
         return result
 
     @abstractmethod
     def has_perm(self, user, perm_name):
-        u"""Проверяет наличие у пользователя разрешения.
+        """Проверяет наличие у пользователя разрешения.
 
         :param user: Пользователь, возвращаемый функцией
             ioc.get('get_current_user').
         :param basestring perm_name: Имя разрешения.
 
         :rtype: bool
         """
 
     @abstractmethod
     def has_access(self, action, request):
-        u"""Проверяет наличие у текущего пользователя разрешения.
+        """Проверяет наличие у текущего пользователя разрешения.
 
         :param action: Экшн, к которому проверяется наличие доступа.
         :type action: m3.actions.Action
 
         :param request: HTTP-запрос.
         :type request: django.http.HttpRequest
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/backends/caching.py` & `educommon-3.0.0/src/educommon/auth/rbac/backends/caching.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,65 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from collections import defaultdict
-from datetime import date
-from itertools import chain
-from logging import getLogger
-from time import time
-
-from django.contrib.contenttypes.models import ContentType
-from django.core.cache import cache
-from django.db.models.query_utils import Q
-from django.db.models.signals import post_delete
-from django.db.models.signals import post_save
-import six
-
-from educommon.utils.misc import cached_property
-
-from ..models import Permission
-from ..models import Role
-from ..models import RoleParent
-from ..models import RolePermission
-from ..models import UserRole
-from .base import BackendBase
+from collections import (
+    defaultdict,
+)
+from datetime import (
+    date,
+)
+from itertools import (
+    chain,
+)
+from logging import (
+    getLogger,
+)
+from time import (
+    time,
+)
+
+from django.contrib.contenttypes.models import (
+    ContentType,
+)
+from django.core.cache import (
+    cache,
+)
+from django.db.models.query_utils import (
+    Q,
+)
+from django.db.models.signals import (
+    post_delete,
+    post_save,
+)
+
+from educommon.auth.rbac.backends.base import (
+    BackendBase,
+)
+from educommon.auth.rbac.models import (
+    Permission,
+    Role,
+    RoleParent,
+    RolePermission,
+    UserRole,
+)
+from educommon.utils.misc import (
+    cached_property,
+)
 
 
 class CachingBackend(BackendBase):
-
-    u"""Бэкенд, кеширующий объекты подсистемы RBAC.
+    """Бэкенд, кеширующий объекты подсистемы RBAC.
 
     Перезагружает данные из БД в следующих случаях:
 
         - при инициализации подсистемы RBAC;
         - при изменении или удалении ролей;
         - при изменении прав в ролях;
         - при назначении или отзыве ролей у пользователей.
     """
 
     CACHE_KEY = 'RBAC_DATA_CHANGE_TIME'
-    u"""Ключ кеша, в котором сохраняется время изменения объектов в БД."""
+    """Ключ кеша, в котором сохраняется время изменения объектов в БД."""
 
     # Модели, данные которых кэшируются.
     _cached_models = {
         Permission,
         Role,
         RoleParent,
         UserRole,
@@ -82,117 +100,117 @@
         )
         post_delete.connect(
             self._signal_handler,
             dispatch_uid=get_dispatch_uid('post_delete'),
         )
 
     def _signal_handler(self, sender, **kwargs):
-        u"""Обработчик сигналов об изменениях в моделях."""
+        """Обработчик сигналов об изменениях в моделях."""
         if (
             # changed приходит только от post_init
             kwargs.get('changed', False) or
             # а port_save и post_delete нужно обрабатывать только для
             # кэшируемых моделей
             sender in self._cached_models
         ):
             self._set_data_change_time()
 
     def _get_data_change_time(self):
-        u"""Возвращает время последнего изменения объектов RBAC в БД."""
+        """Возвращает время последнего изменения объектов RBAC в БД."""
         t = cache.get(self.CACHE_KEY)
         return float(t) if t else None
 
     def _set_data_change_time(self):
-        u"""Сохраняет время последнего изменения объектов RBAC в БД."""
+        """Сохраняет время последнего изменения объектов RBAC в БД."""
         t = time()
-        cache.set(self.CACHE_KEY, six.text_type(t), self.CACHE_TIMEOUT)
+        cache.set(self.CACHE_KEY, str(t), self.CACHE_TIMEOUT)
         return t
 
     def _is_out_of_date(self):
-        u"""Возвращает True, если кешированные данные устарели."""
+        """Возвращает True, если кешированные данные устарели."""
         data_change_time = self._get_data_change_time()
         if data_change_time is None:
             # Либо, объекты еще не кэшировались, либо истекло время хранения
             # ключа, поэтому пора перезагрузить объекты RBAC.
             data_change_time = self._set_data_change_time()
 
         return self._loaded_at < data_change_time
 
     def _clear(self):
-        u"""Очистка кеша объектов RBAC."""
+        """Очистка кеша объектов RBAC."""
         self._permissions_by_id.clear()
         self._permissions_by_name.clear()
         self._role_permissions.clear()
         self._role_children.clear()
         self._user_roles.clear()
 
     def _load_permissions(self):
-        u"""Загрузка данных о разрешениях RBAC."""
+        """Загрузка данных о разрешениях RBAC."""
         for pk, name in Permission.objects.values_list('pk', 'name'):
             self._permissions_by_id[pk] = name
             self._permissions_by_name[name] = pk
 
     def _load_role_hierarchy(self):
-        u"""Загрузка данных о подчиненности ролей RBAC."""
+        """Загрузка данных о подчиненности ролей RBAC."""
         query = RoleParent.objects.values_list('parent', 'role')
 
         for parent_id, role_id in query:
             self._role_children[parent_id].add(role_id)
 
     def _load_role_permissions(self):
-        u"""Загрузка данных о разрешениях ролей RBAC."""
+        """Загрузка данных о разрешениях ролей RBAC."""
         for role_id, permission_id in RolePermission.objects.values_list(
             'role', 'permission'
         ):
             self._role_permissions[role_id].add(permission_id)
 
     def _load_user_roles(self):
-        u"""Загрузка данных о ролях пользователей."""
+        """Загрузка данных о ролях пользователей."""
         query = UserRole.objects.filter(
             Q(date_to__isnull=True) | Q(date_to__gte=date.today()),
         ).values_list(
             'content_type', 'object_id', 'date_from', 'date_to', 'role'
         )
 
         for ct_id, obj_id, date_from, date_to, role_id in query:
             self._user_roles[ct_id, obj_id].add(
                 (date_from, date_to, role_id)
             )
 
     def _get_role_descendants(self, role_id, include_self=False):
-        u"""Возвращает вложенные роли."""
+        """Возвращает вложенные роли."""
         result = set()
 
         if include_self:
             result.add(role_id)
 
         for child_role_id in self._role_children[role_id]:
             result.update(
                 self._get_role_descendants(child_role_id, include_self=True)
             )
 
         return result
 
     def _get_user_roles(self, user):
-        u"""Возвращает все роли пользователя, в т.ч. и вложенные.
+        """Возвращает все роли пользователя, в т.ч. и вложенные.
 
         :rtype: set
         """
         content_type_id = ContentType.objects.get_for_model(user).id
         roles_data = self._user_roles[content_type_id, user.id]
         today = date.today()
 
         return set(chain(*(
             self._get_role_descendants(role_id, include_self=True)
             for date_from, date_to, role_id in roles_data
             if (date_from or today) <= today <= (date_to or today)
         )))
 
     def _get_user_permissions(self, user):
-        u"""Возврвщает все доступные пользователю разрешения.
+        """Возврвщает все доступные пользователю разрешения.
 
         :rtype: itertools.chain
         """
         def get_role_permissions(role_id):
             # pylint: disable=protected-access
             for permission_id in self._role_permissions[role_id]:
                 yield permission_id
@@ -203,15 +221,15 @@
 
         return chain(*(
             get_role_permissions(role_id)
             for role_id in self._get_user_roles(user)
         ))
 
     def _reload(self, force=False):
-        u"""Перезагрузка кешируемых объектов при необходимости.
+        """Перезагрузка кешируемых объектов при необходимости.
 
         :param bool force: Указывает на необходимость принудительной
             перезагрузки.
         """
         if force or self._is_out_of_date():
             self._clear()
 
@@ -219,15 +237,15 @@
             self._load_role_permissions()
             self._load_role_hierarchy()
             self._load_user_roles()
 
             self._loaded_at = time()
 
     def has_perm(self, user, perm_name):
-        u"""Проверяет наличие у пользователя разрешения.
+        """Проверяет наличие у пользователя разрешения.
 
         :param user: Пользователь, возвращаемый функцией
             ioc.get('get_current_user').
         :param basestring perm_name: Имя разрешения.
 
         :rtype: bool
         """
@@ -235,15 +253,15 @@
 
         assert perm_name in self._permissions_by_name, perm_name
 
         permission_id = self._permissions_by_name[perm_name]
         return permission_id in self._get_user_permissions(user)
 
     def has_access(self, action, request):
-        u"""Проверяет наличие у текущего пользователя разрешения.
+        """Проверяет наличие у текущего пользователя разрешения.
 
         :param action: Экшн, к которому проверяется наличие доступа.
         :type action: m3.actions.Action
 
         :param request: HTTP-запрос.
         :type request: django.http.HttpRequest
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/backends/simple.py` & `educommon-3.0.0/src/educommon/auth/rbac/backends/simple.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from datetime import date
-
-from django.contrib.contenttypes.models import ContentType
-
-from ..models import Permission
-from ..models import Role
-from ..models import RolePermission
-from ..models import UserRole
-from .base import BackendBase
+from datetime import (
+    date,
+)
+
+from django.contrib.contenttypes.models import (
+    ContentType,
+)
+
+from educommon.auth.rbac.backends.base import (
+    BackendBase,
+)
+from educommon.auth.rbac.models import (
+    Permission,
+    Role,
+    RolePermission,
+    UserRole,
+)
 
 
 def _get_user_roles(user):
-    u"""Возвращает все роли пользователя, в т.ч. и вложенные.
+    """Возвращает все роли пользователя, в т.ч. и вложенные.
 
     :param user: Пользователь, возвращаемый функцией
         ioc.get('get_current_user').
 
     :rtype: set
     """
     # Роли, назначенные непосредственно пользователю
@@ -35,15 +40,15 @@
         user_roles.add(role)
         user_roles.update(role.subroles)
 
     return user_roles
 
 
 def _get_user_permissions_query(user, permissions=None):
-    u"""Возвращает все доступные пользователю разрешения.
+    """Возвращает все доступные пользователю разрешения.
 
     :param user: Пользователь, возвращаемый функцией
         ioc.get('get_current_user').
     :param permissions: Имена разрешений, среди которых нужно искать
         разрешения, доступные пользователю.
 
     :rtype: QuerySet
@@ -64,23 +69,23 @@
     )
 
     return result
 
 
 class SimpleBackend(BackendBase):
 
-    u"""Предоставляет прямой доступ к объектам RBAC.
+    """Предоставляет прямой доступ к объектам RBAC.
 
     Доступ к объектам RBAC (разрешениям, ролям и их связям между собой)
     осуществляется через ORM. Кеширование не осуществляется, поэтому
     использование данного бэкенда может приводить к излишней нагрузке на СУБД.
     """
 
     def _get_user_permissions(self, user, permissions=None):
-        u"""Возвращает имена всех доступных пользователю разрешений.
+        """Возвращает имена всех доступных пользователю разрешений.
 
         :param user: Пользователь, возвращаемый функцией
             ioc.get('get_current_user').
         :param permissions: Имена разрешений, среди которых нужно искать
             разрешения, доступные пользователю.
 
         :rtype: generator
@@ -90,27 +95,27 @@
             'name', flat=True
         ):
             yield name
             for name in self._manager.get_dependent_permissions(name):
                 yield name
 
     def has_perm(self, user, perm_name):
-        u"""Проверяет наличие у пользователя разрешения.
+        """Проверяет наличие у пользователя разрешения.
 
         :param user: Пользователь, возвращаемый функцией
             ioc.get('get_current_user').
         :param basestring perm_name: Имя разрешения.
 
         :rtype: bool
         """
         result = perm_name in self._get_user_permissions(user)
         return result
 
     def has_access(self, action, request):
-        u"""Проверяет наличие у текущего пользователя разрешения.
+        """Проверяет наличие у текущего пользователя разрешения.
 
         :param action: Экшн, к которому проверяется наличие доступа.
         :type action: m3.actions.Action
 
         :param request: HTTP-запрос.
         :type request: django.http.HttpRequest
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/checker.py` & `educommon-3.0.0/src/educommon/auth/rbac/checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from m3.actions import AbstractPermissionChecker
-from m3.actions import Action
-from m3.actions import ActionPack
-
-from .manager import rbac
+from m3.actions import (
+    AbstractPermissionChecker,
+    Action,
+    ActionPack,
+)
+
+from educommon.auth.rbac.manager import (
+    rbac,
+)
 
 
 class PermissionChecker(AbstractPermissionChecker):
-
-    u"""Класс, проверяющий наличие необходимых у пользователя прав.
+    """Класс, проверяющий наличие необходимых у пользователя прав.
 
     Наличие прав у пользователя определяется в зависимости от ролей,
     назначенных пользователю.
 
     Использование данного permission checker'а предполагает, что у каждого пака
     и у каждого экшена системы определены атрибуты perm_code. При этом,
     perm_code пака определяет раздел перечня разрешений, например: employee,
     pupil, unit и т.д. Атрибут perm_code у экшена определяет вид действия:
     view, add, edit, delete, report и т.д. Также в экшенах возможно определение
     подвидов действий, например: all, own и т.д.
     """
 
     def has_action_permission(self, request, action, subpermission=None):
-        u"""Проверяет права доступа пользователя к экшену.
+        """Проверяет права доступа пользователя к экшену.
 
         :param request: Http-запрос.
         :type request: django.http.Request
 
         :param action: Экшн, наличие прав на выполнение которого проверяется.
         :type action: m3_core.actions.Action
 
@@ -39,15 +39,15 @@
 
     def has_pack_permission(self, request, pack, permission):
         # Не используется
         raise NotImplementedError()
 
     @staticmethod
     def get_perm_code(action_or_pack, subpermission=None):
-        u"""Возвращает код разрешения для пака или экшена."""
+        """Возвращает код разрешения для пака или экшена."""
         if isinstance(action_or_pack, ActionPack):
             pack, action = action_or_pack, None
         elif isinstance(action_or_pack, Action):
             pack, action = action_or_pack.parent, action_or_pack
         else:
             raise TypeError(type(action_or_pack))
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/config.py` & `educommon-3.0.0/src/educommon/auth/rbac/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-# coding: utf-8
-from __future__ import absolute_import
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
 
-from abc import ABCMeta
-from abc import abstractproperty
 
-import six
-
-
-class IConfig(six.with_metaclass(ABCMeta, object)):
-    u"""Конфигурация управлением доступом на основе ролей.
+class IConfig(metaclass=ABCMeta):
+    """Конфигурация управлением доступом на основе ролей.
 
     Позволяет ограничивать выбор классов, на которые может ссылаться
     :class:`~educommon.auth.rbac.models.UserRole` в атрибуте ``user``.
     """
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def user_types(self):
         """Типы классов пользователей, которым назначаются роли.
 
         Отсутствие указывает на то, что ограничение по назначаемым ролям будет
         отключено.
 
         :rtype: set of django.db.models.Model or bool
         """
 
 
 class DefaultConfig(IConfig):
-    u"""Конфигурация без ограничения ролей пользователей."""
+    """Конфигурация без ограничения ролей пользователей."""
 
     user_types = False
 
 
 # : Конфигурация управлением доступом.
 rbac_config = DefaultConfig()
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/management/commands/rbac.py` & `educommon-3.0.0/src/educommon/auth/rbac/management/commands/rbac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-# coding: utf-8
-u"""Management-команда для обслуживания системы авторизации."""
-from __future__ import absolute_import
-
+"""Management-команда для обслуживания системы авторизации."""
 import os
 
-from django.core.management import CommandError
-from m3_django_compat import BaseCommand
-from termcolor import colored
-import six
-
-from educommon.auth.rbac.manager import rbac
-
-from ...manager import _get_actions
-from ...models import Permission
+from django.core.management import (
+    CommandError,
+)
+from m3_django_compat import (
+    BaseCommand,
+)
+from termcolor import (
+    colored,
+)
+
+from educommon.auth.rbac.manager import (
+    _get_actions,
+    rbac,
+)
+from educommon.auth.rbac.models import (
+    Permission,
+)
 
 
 class Command(BaseCommand):
 
-    u"""Обслуживание системы авторизации."""
+    """Обслуживание системы авторизации."""
 
     use_argparse = False
 
     def _show_actions(self, *permissions, **options):
-        u"""Вывод списка экшенов системы.
+        """Вывод списка экшенов системы.
 
         :param permissions: Имена разрешений, для которых нужно вывести список
             экшенов.
         """
         if not permissions:
             permissions = sorted(rbac.permissions_by_name.keys())
 
@@ -53,15 +58,15 @@
                 )
                 for action in actions_by_permission[name]
             )
             for action in actions:
                 self.stdout.write('   ' + action + '\n')
 
     def _show_permissions(self, status='all'):
-        u"""Вывод разрешений.
+        """Вывод разрешений.
 
         :param registered_only: определяет, какие разрешения нужно выводить:
             None - все, True - только зарегистрированные в системе, False - все
             разрешения, имеющиеся в БД.
         """
         db_perms = set(Permission.objects.values_list('name', flat=True))
         sys_perms = set(rbac.permissions_by_name.keys())
@@ -92,24 +97,24 @@
                 status, color = '[  REGISTERED  ]', 'green'
 
             self.stdout.write(
                 colored(template.format(status, permission), color)
             )
 
     def _show(self, objects='permissions', *args, **options):
-        u"""Отображение данных системы авторизации."""
+        """Отображение данных системы авторизации."""
         if objects == 'permissions':
             self._show_permissions(*args)
         elif objects == 'actions':
             self._show_actions(*args, **options)
         else:
             raise CommandError('Unknown objects type: {}'.format(objects))
 
     def _clean_permissions(self):
-        u"""Удаление из БД незарегистрированных в системе разрешений."""
+        """Удаление из БД незарегистрированных в системе разрешений."""
         permissions = Permission.objects.exclude(
             name__in=rbac.permissions_by_name,
         )
 
         if not permissions:
             return
 
@@ -119,15 +124,15 @@
         for permission in permissions:
             permission.delete()
             self.stdout.write(
                 colored(template.format(permission.name), 'red')
             )
 
     def _clean(self, objects='all', **options):
-        u"""Удаление незарегистрированных правил и разрешений."""
+        """Удаление незарегистрированных правил и разрешений."""
         if objects == 'all':
             self._clean_permissions()
         elif objects == 'permissions':
             self._clean_permissions()
         else:
             raise CommandError('Unknown objects type: {}'.format(objects))
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/manager.py` & `educommon-3.0.0/src/educommon/auth/rbac/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,64 +1,82 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from collections import Iterable
-from collections import defaultdict
-from importlib import import_module
-
-from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
-from django.dispatch.dispatcher import Signal
-from django.utils.functional import cached_property
-from m3.actions import ControllerCache
-from m3_django_compat import atomic
-from m3_django_compat import get_installed_apps
-import six
-
-from educommon.utils.db.postgresql import Lock
-
-from .models import Permission
+from collections import (
+    Iterable,
+    defaultdict,
+)
+from importlib import (
+    import_module,
+)
+from typing import (
+    Optional,
+)
+
+from django.conf import (
+    settings,
+)
+from django.core.exceptions import (
+    ImproperlyConfigured,
+)
+from django.dispatch.dispatcher import (
+    Signal,
+)
+from django.utils.functional import (
+    cached_property,
+)
+from m3.actions import (
+    ControllerCache,
+)
+from m3_django_compat import (
+    atomic,
+    get_installed_apps,
+)
+
+from educommon.auth.rbac.models import (
+    Permission,
+)
+from educommon.utils.db.postgresql import (
+    Lock,
+)
 
 
 def _get_handler(handler):
-    u"""Возвращает функцию-обработчик правила."""
+    """Возвращает функцию-обработчик правила."""
     module, handler = handler.rsplit('.', 1)
     module = __import__(module, fromlist=[handler])
     handler = getattr(module, handler)
     return handler
 
 
 def _get_app_permissions_modules():
-    u"""Возвращает модули permissions из приложений системы.
+    """Возвращает модули permissions из приложений системы.
 
     :rtype: generator
     """
     for app_name in get_installed_apps():
         try:
             yield import_module('.permissions', app_name)
         except ImportError as error:
             if 'No module named' not in error.args[0]:
                 raise
             continue
 
 
 def _get_actions():
-    u"""Возвращает экшены системы, доступ к которым нужно проверять.
+    """Возвращает экшены системы, доступ к которым нужно проверять.
 
     :rtype: generator
     """
     for controller in ControllerCache.get_controllers():
         for pack in controller.get_packs():
             for action in pack.actions:
                 if pack.need_check_permission or action.need_check_permission:
                     yield action
 
 
 def _set_permission(permission, name, title, description, hidden):
-    u"""Сохраняет разрешение в БД.
+    """Сохраняет разрешение в БД.
 
     Если разрешение отсутствует в БД, то создает его. Иначе обновляет его
     обработчик, название и дескриптор.
     """
     changed = False
 
     if permission is None:
@@ -82,106 +100,102 @@
         permission.full_clean()
         permission.save()
         changed = True
 
     return changed
 
 
-class RBACManager(object):
-
-    u"""Менеджер системы авторизации RBAC."""
+class RBACManager:
+    """Менеджер системы авторизации RBAC."""
 
     post_init = Signal(providing_args=('changed',))
-    u"""Сигнал, отправляемый после обновления разрешений в БД.
+    """Сигнал, отправляемый после обновления разрешений в БД.
 
     :param bool changed: Указывает, были ли в процессе инициализации подсистемы
         сделаны какие-либо изменения в БД (созданы, либо изменены, разрешения).
     """
 
     def __init__(self):
         self.partitions = defaultdict(set)  # Разделы системы
         self.groups = {}  # Группы разрешений
         self.permissions_by_name = {}
         self.permission_dependencies = defaultdict(set)
         self.permission_rules = defaultdict(list)
         self.hidden_permissions = set()
 
     def get_group_params(self, permission_name):
-        u"""Возвращает имя и наименование группы по имени разрешения.
+        """Возвращает имя и наименование группы по имени разрешения.
 
         :rtype: tuple
-        :returns: ``(u'employee', u'Сотрудники')``
+        :returns: ``('employee', 'Сотрудники')``
         """
         group_name = permission_name.split('/')[0]
         return group_name, self.groups[group_name]
 
-    def get_partition_title(self, group_name):
-        u"""Возвращает наименование раздела по имени группы разрешений.
-
-        :rtype: unicode
-        """
-        for title, group_names in six.iteritems(self.partitions):
+    def get_partition_title(self, group_name) -> Optional[str]:
+        """Возвращает наименование раздела по имени группы разрешений."""
+        for title, group_names in self.partitions.items():
             if group_name in group_names:
                 return title
 
     def _collect_partitions(self, permission_modules):
-        u"""Сбор информации о разделах системы.
+        """Сбор информации о разделах системы.
 
         Разделами системы являются объединения групп разрешений.
         """
         self.partitions.clear()
 
         processed_codes = set()
 
         for module in permission_modules:
             partitions = getattr(module, 'partitions', None)
             if partitions is None:
                 continue
 
-            for title, group_codes in six.iteritems(partitions):
+            for title, group_codes in partitions.items():
                 for code in group_codes:
                     assert code not in processed_codes, (
-                        u'Группа разрешений "{}" уже закреплена за другим '
-                        u'разделом системы.'.format(code)
+                        'Группа разрешений "{}" уже закреплена за другим '
+                        'разделом системы.'.format(code)
                     )
                     self.partitions[title].add(code)
                     processed_codes.add(code)
 
     def _collect_groups(self, permission_modules):
-        u"""Сбор информации о группах разрешений."""
+        """Сбор информации о группах разрешений."""
         self.groups.clear()
 
         for module in permission_modules:
             groups = getattr(module, 'groups', None)
             if groups is None:
                 continue
 
-            for code, title in six.iteritems(groups):
+            for code, title in groups.items():
                 assert code not in self.groups, (
-                    u'Группа разрешений "{}" ({}) уже описана в другом '
-                    u'приложении.'.format(code, title)
+                    'Группа разрешений "{}" ({}) уже описана в другом '
+                    'приложении.'.format(code, title)
                 )
 
                 self.groups[code] = title
 
     def _collect_permissions(self, permissions_modules):
-        u"""Сбор разрешений системы."""
+        """Сбор разрешений системы."""
         self.permissions_by_name.clear()
         self.hidden_permissions.clear()
 
         # Сбор названий разрешений всей системы
         for action in _get_actions():
             if action.sub_permissions:
-                for sub_perm, title in six.iteritems(action.sub_permissions):
+                for sub_perm, title in action.sub_permissions.items():
                     perm_name = action.get_perm_code(sub_perm)
-                    self.permissions_by_name[perm_name] = (title, u'')
+                    self.permissions_by_name[perm_name] = (title, '')
             else:
                 title = action.parent.sub_permissions.get(action.perm_code)
                 perm_name = action.get_perm_code()
-                self.permissions_by_name[perm_name] = (title, u'')
+                self.permissions_by_name[perm_name] = (title, '')
 
         # Заполнение параметров разрешений
         for module in permissions_modules:
             for params in getattr(module, 'permissions', []):
                 if len(params) == 3:
                     name, title, description = params
                 elif len(params) == 4:
@@ -196,36 +210,36 @@
                 assert name in self.permissions_by_name, (
                     'Permission {} not found'.format(name)
                 )
 
                 _title, _description = self.permissions_by_name[name]
                 self.permissions_by_name[name] = (
                     title or _title,
-                    description or _description or u'',
+                    description or _description or '',
                 )
 
     def _collect_dependencies(self, permissions_modules):
-        u"""Сбор зависимостей между разрешениями."""
+        """Сбор зависимостей между разрешениями."""
         self.permission_dependencies.clear()
 
         for module in permissions_modules:
             module_dependencies = getattr(module, 'dependencies', {})
             if callable(module_dependencies):
                 module_dependencies = module_dependencies()
 
-            for name, dependencies in six.iteritems(module_dependencies):
+            for name, dependencies in module_dependencies.items():
                 assert name in self.permissions_by_name, (
                     'Permission {} not found'.format(name)
                 )
                 assert name not in self.hidden_permissions or all(
                     dependency in self.hidden_permissions
                     for dependency in dependencies
                 ), (
-                    u'Скрытые разрешения могут зависеть только от скрытых '
-                    u'разрешений: ' + name
+                    'Скрытые разрешения могут зависеть только от скрытых '
+                    'разрешений: ' + name
                 )
                 if __debug__:
                     for dependency in dependencies:
                         if name == dependency:
                             raise AssertionError(
                                 'Permission {} can''t depend on itself'
                                 .format(dependency)
@@ -234,39 +248,39 @@
                             raise AssertionError(
                                 'Permission {} not found'.format(dependency)
                             )
 
                 self.permission_dependencies[name].update(dependencies)
 
     def _collect_rules(self, permissions_modules):
-        u"""Сбор обработчиков правил для разрешений системы."""
+        """Сбор обработчиков правил для разрешений системы."""
         self.permission_rules.clear()
 
         for module in permissions_modules:
-            for perm, handlers in six.iteritems(getattr(module, 'rules', {})):
+            for perm, handlers in getattr(module, 'rules', {}).items():
                 if not isinstance(handlers, Iterable):
                     handlers = [handlers]
 
                 for handler in handlers:
-                    if isinstance(handler, six.string_types):
+                    if isinstance(handler, str):
                         handler = _get_handler(handler)
                     assert callable(handler), handler
                     self.permission_rules[perm].append(handler)
 
     def _update_db(self):
-        u"""Обновление списка разрешений в БД на основе разрешений системы."""
+        """Обновление списка разрешений в БД на основе разрешений системы."""
         with Lock(settings.DEFAULT_DB_ALIAS, 'rbac_lock'):
             permissions_changed = False
 
             permissions = {
                 permission.name: permission
                 for permission in Permission.objects.iterator()
             }
 
-            for params in six.iteritems(self.permissions_by_name):
+            for params in self.permissions_by_name.items():
                 name, (title, description) = params
                 changed = _set_permission(
                     permissions.get(name),
                     name,
                     title,
                     description,
                     name in self.hidden_permissions,
@@ -274,15 +288,15 @@
                 if changed:
                     permissions_changed = True
                 self.permissions_by_name[name] = (name, title)
 
             self.post_init.send(sender=self, changed=permissions_changed)
 
     def get_dependent_permissions(self, name, _result=None):
-        u"""Возвращает разрешения, от которых зависит указанное разрешение.
+        """Возвращает разрешения, от которых зависит указанное разрешение.
 
         :param str name: Имя разрешения.
 
         :rtype: set of str
         """
         if _result is None:
             primary_name = name
@@ -300,15 +314,15 @@
         if primary_name:
             _result.remove(primary_name)
 
         return _result
 
     @atomic
     def init(self, update_db=True):
-        u"""Инициализация системы авторизации.
+        """Инициализация системы авторизации.
 
         1. Загружает из приложений системы списки правил и разрешений. Их поиск
            осуществляется в модуле ``permissions``.
         2. Для каждого правила и разрешения создает/обновляет запись в БД.
         3. Объекты модели ``Permission`` сохраняет в словаре
            ``self.permissions_by_name``.
 
@@ -359,15 +373,15 @@
             )
         else:
             backend = backend_class(self)
 
         return backend
 
     def has_access(self, action, request):
-        u"""Проверяет наличие у текущего пользователя разрешения.
+        """Проверяет наличие у текущего пользователя разрешения.
 
         Если у пака need_check_permission равен True, то проверка прав доступа
         будет выполняться для всех экшенов этого пака вне зависимости от
         значения параметра need_check_permission у экшенов. Также проверка
         наличия разрешений будет выполняться, если у пака значение параметра
         need_check_permission равно False, но у экшена оно равно True. В
         остальных случаях метод сразу возвращает True.
@@ -384,15 +398,15 @@
         :type request: django.http.HttpRequest
 
         :rtype: bool
         """
         return self._backend.has_access(action, request)
 
     def has_perm(self, user, perm_name):
-        u"""Проверяет наличие у пользователя разрешения.
+        """Проверяет наличие у пользователя разрешения.
 
         .. important::
 
            Проверка доступа в данном методе происходит **без** учета правил,
            назначенных соответствующим разрешениям.
 
         :param user: Пользователь, возвращаемый функцией
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/migrations/0001_initial.py` & `educommon-3.0.0/src/educommon/auth/rbac/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('contenttypes', '0001_initial'),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py` & `educommon-3.0.0/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [('rbac', '0001_initial'), ]
 
     operations = [
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py` & `educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,44 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
 import django.db.models.deletion
-import django.db.models.manager
-import m3_django_compat
+from django import (
+    VERSION,
+)
+from django.conf import (
+    settings,
+)
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
+    initial = True
+
     dependencies = [
         ('contenttypes', '0002_remove_content_type_name'),
-        ('rbac', '0003_permission_hidden'),
     ]
+    # из-за отсутвия функционала для исправления плана миграций в Django
+    # версий младше чем 1.10,здесь решается вопрос загрузки contingent_plugin
+    # первым в списке выполняемых миграций. Начиная с версии 1.10 данный
+    # способ не подходит ввиду ввода проверки на корректность плана миграций
+    if VERSION < (1, 10):
+        run_before = [
+            (app_name.split('.')[-1], '__first__')
+            for app_name in settings.PROJECT_APPS
+        ]
 
     operations = [
         migrations.CreateModel(
-            name='RoleUserType',
+            name='ContingentModelChanged',
             fields=[
-                ('id', models.AutoField(
-                    auto_created=True,
-                    primary_key=True,
-                    serialize=False,
-                    verbose_name='ID')),
-                ('role', models.ForeignKey(
-                    on_delete=django.db.models.deletion.CASCADE,
-                    related_name='+',
-                    to='rbac.Role',
-                    verbose_name='Роль')),
-                ('user_type', models.ForeignKey(
-                    on_delete=django.db.models.deletion.CASCADE,
-                    related_name='+',
-                    to='contenttypes.ContentType',
-                    verbose_name='Тип пользователя')),
-            ],
-            options={
-                'verbose_name': 'Тип пользователя роли',
-                'verbose_name_plural': 'Типы пользователей ролей',
-            }, ),
-        migrations.AlterModelManagers(
-            name='userrole',
-            managers=[
-                ('objects', m3_django_compat.Manager()),
-                ('actual_objects', django.db.models.manager.Manager()),
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('object_id', models.PositiveIntegerField()),
+                ('content_type', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='contenttypes.ContentType')),
             ],
         ),
-        migrations.AddField(
-            model_name='role',
-            name='user_types',
-            field=models.ManyToManyField(
-                related_name='_role_user_types_+',
-                through='rbac.RoleUserType',
-                to='contenttypes.ContentType',
-                verbose_name='Может быть назначена'), ),
         migrations.AlterUniqueTogether(
-            name='roleusertype',
-            unique_together=set([('role', 'user_type')]), ),
+            name='contingentmodelchanged',
+            unique_together=set([('content_type', 'object_id')]),
+        ),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/models.py` & `educommon-3.0.0/src/educommon/auth/rbac/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,128 +1,154 @@
-# coding: utf-8
 # pylint: disable=no-init
-u"""Модели для хранения данных системы авторизации RBAC."""
-from __future__ import absolute_import
-
-from django.contrib.contenttypes.models import ContentType
-from django.core.exceptions import NON_FIELD_ERRORS
-from django.core.exceptions import ValidationError
-from django.db import models
-from django.db.models.fields import FieldDoesNotExist
-from django.db.models.signals import post_delete
-from django.db.models.signals import pre_delete
-from django.dispatch import receiver
-from m3 import ApplicationLogicException
-from m3.db import safe_delete
-from m3_django_compat import ModelOptions
-from m3_django_compat import atomic
-from m3_django_compat.models import GenericForeignKey
-import six
-
-from educommon.auth.rbac.utils import get_permission_full_title
-from educommon.django.db.mixins.date_interval import ActualObjectsManager
-from educommon.django.db.mixins.date_interval import DateIntervalMeta
-from educommon.django.db.mixins.date_interval import DateIntervalMixin
-from educommon.django.db.mixins.validation import post_clean
-from educommon.django.db.models import BaseModel
-from educommon.django.db.utils import model_modifier_metaclass
-from educommon.m3.extensions.listeners.delete_check.mixins import \
-    CascadeDeleteMixin
+"""Модели для хранения данных системы авторизации RBAC."""
+from django.contrib.contenttypes.models import (
+    ContentType,
+)
+from django.core.exceptions import (
+    NON_FIELD_ERRORS,
+    ValidationError,
+)
+from django.db import (
+    models,
+)
+from django.db.models.fields import (
+    FieldDoesNotExist,
+)
+from django.db.models.signals import (
+    post_delete,
+    pre_delete,
+)
+from django.dispatch import (
+    receiver,
+)
+from m3 import (
+    ApplicationLogicException,
+)
+from m3.db import (
+    safe_delete,
+)
+from m3_django_compat import (
+    ModelOptions,
+    atomic,
+)
+from m3_django_compat.models import (
+    GenericForeignKey,
+)
 
-from . import config
-from .permissions import PERM__ROLE__EDIT
+from educommon.auth.rbac import (
+    config,
+)
+from educommon.auth.rbac.permissions import (
+    PERM__ROLE__EDIT,
+)
+from educommon.auth.rbac.utils import (
+    get_permission_full_title,
+)
+from educommon.django.db.mixins.date_interval import (
+    ActualObjectsManager,
+    DateIntervalMeta,
+    DateIntervalMixin,
+)
+from educommon.django.db.mixins.validation import (
+    post_clean,
+)
+from educommon.django.db.models import (
+    BaseModel,
+)
+from educommon.django.db.utils import (
+    model_modifier_metaclass,
+)
+from educommon.m3.extensions.listeners.delete_check.mixins import (
+    CascadeDeleteMixin,
+)
 
 
-@six.python_2_unicode_compatible
 class Permission(BaseModel):
-
-    u"""Разрешение."""
+    """Разрешение."""
 
     name = models.CharField(
-        u'Имя',
+        'Имя',
         max_length=100,
         db_index=True,
         unique=True,
     )
     title = models.CharField(
-        u'Название',
+        'Название',
         max_length=200,
         blank=True, null=True,
     )
     description = models.TextField(
-        u'Описание',
+        'Описание',
         blank=True,
     )
     hidden = models.BooleanField(
-        u'Видимость пользователям',
+        'Видимость пользователям',
         default=False,
     )
 
     class Meta:
-        verbose_name = u'Разрешение'
-        verbose_name_plural = u'Разрешения'
+        verbose_name = 'Разрешение'
+        verbose_name_plural = 'Разрешения'
 
     def __str__(self):
-        return u'Permission<{}: {}>'.format(self.id, self.name)
+        return 'Permission<{}: {}>'.format(self.id, self.name)
 
 
-@six.python_2_unicode_compatible
 class Role(CascadeDeleteMixin, BaseModel):
-
-    u"""Роль."""
+    """Роль."""
 
     name = models.CharField(
-        u'Название',
+        'Название',
         max_length=300,
         db_index=True,
         unique=True,
     )
     description = models.TextField(
-        u'Описание',
+        'Описание',
         blank=True,
     )
     can_be_assigned = models.BooleanField(
-        u'Может быть назначена пользователю',
+        'Может быть назначена пользователю',
         default=True,
     )
     permissions = models.ManyToManyField(
         Permission,
         related_name='roles',
         through='RolePermission',
     )
     user_types = models.ManyToManyField(
         ContentType,
-        verbose_name=u'Может быть назначена',
+        verbose_name='Может быть назначена',
         through='RoleUserType',
         related_name='+',
     )
 
     class Meta:
-        verbose_name = u'Роль'
-        verbose_name_plural = u'Роли'
+        verbose_name = 'Роль'
+        verbose_name_plural = 'Роли'
 
     def __str__(self):
-        return u'Role<{}: {}>'.format(self.id, self.name)
+        return 'Role<{}: {}>'.format(self.id, self.name)
 
     @property
     def subroles(self):
-        u"""Возвращает все вложенные роли данной роли.
+        """Возвращает все вложенные роли данной роли.
 
         :rtype: set
         """
         result = set()
 
         for role_parent in RoleParent.objects.filter(parent_id=self.id):
             result.add(role_parent.role)
             result.update(role_parent.role.subroles)
 
         return result
 
     def get_permissions(self):
-        u"""Возвращает все разрешения роли, в т.ч. вложенных ролей.
+        """Возвращает все разрешения роли, в т.ч. вложенных ролей.
 
         :rtype: QuerySet
         """
         roles = set([self]) | self.subroles
         result = Permission.objects.filter(
             pk__in=RolePermission.objects.filter(
                 role__in=roles,
@@ -133,15 +159,15 @@
 
     def simple_clean(self, errors):
         super(Role, self).simple_clean(errors)
 
         if (self.pk and not self.can_be_assigned and
                 self.userrole_set.exists()):
             errors['can_be_assigned'].append(
-                u'Есть пользователи, которым назначана роль "{}" '.format(
+                'Есть пользователи, которым назначана роль "{}" '.format(
                     self.name
                 )
             )
 
     def safe_delete(self):
         # safe_delete неправильно работает внутри транзакций, из-за этого
         # при вызове commit() валится IntegrityError, который надо обрабатывать
@@ -164,64 +190,65 @@
             else:
                 raise
 
         return result
 
 
 class RoleUserType(BaseModel):
-
-    u"""M2M-модель "Тип пользователя роли"."""
+    """M2M-модель "Тип пользователя роли"."""
 
     role = models.ForeignKey(
         Role,
-        verbose_name=u'Роль',
+        verbose_name='Роль',
         related_name='+',
         on_delete=models.CASCADE,
     )
     user_type = models.ForeignKey(
         ContentType,
-        verbose_name=u'Тип пользователя',
+        verbose_name='Тип пользователя',
         related_name='+',
         on_delete=models.CASCADE,
     )
 
     cascade_delete_for = (role,)
     display_related_error = False
 
     class Meta:
         unique_together = ('role', 'user_type')
-        verbose_name = u'Тип пользователя роли'
-        verbose_name_plural = u'Типы пользователей ролей'
+        verbose_name = 'Тип пользователя роли'
+        verbose_name_plural = 'Типы пользователей ролей'
 
     def simple_clean(self, errors):
         super(RoleUserType, self).simple_clean(errors)
 
-        from educommon.auth.rbac.config import rbac_config
+        from educommon.auth.rbac.config import (
+            rbac_config,
+        )
 
         if not self.role.can_be_assigned:
             errors['role'].append(
-                u'Роль "{}" не может назначаться пользователям'.format(
+                'Роль "{}" не может назначаться пользователям'.format(
                     self.role.name
                 )
             )
 
         if (
             rbac_config.user_types and
             self.user_type.model_class() not in rbac_config.user_types
         ):
             errors['role'].append(
-                u'Роль "{}" не может быть назначена типу "{}".'.format(
+                'Роль "{}" не может быть назначена типу "{}".'.format(
                     self.role.name,
                     self.user_type.name,
                 )
             )
 
     @staticmethod
     def clean_role(instance, errors, **kwargs):
-        u"""Проверяет типы пользователей роли при её изменении.
+        """Проверяет типы пользователей роли при её изменении.
 
         Не допускает ситуаций, когда при отключении возможности назначения
         роли пользователям остаются ссылки на типы пользователей.
 
         Вызывается через сигнал ``post_clean`` модели
         :class:`~educommon.auth.rbac.models.Role`.
 
@@ -232,88 +259,85 @@
         :type errors: :class:`defaultdict`
         """
         if instance.can_be_assigned:
             return
 
         if instance.user_types.exists():
             errors[NON_FIELD_ERRORS].append(
-                u'Для снятия флага "Может быть назначена пользователя", '
-                u'необходимо отвязать все типы пользователей.'
+                'Для снятия флага "Может быть назначена пользователя", '
+                'необходимо отвязать все типы пользователей.'
             )
 
 
 post_clean.connect(
     receiver=RoleUserType.clean_role,
     sender=Role,
     dispatch_uid='RoleUserType.clean_role'
 )
 
 
 class RolePermission(BaseModel):
-
-    u"""M2M-модель "Разрешение роли"."""
+    """M2M-модель "Разрешение роли"."""
 
     role = models.ForeignKey(
         Role,
-        verbose_name=u'Роль',
+        verbose_name='Роль',
         on_delete=models.CASCADE,
     )
     permission = models.ForeignKey(
         Permission,
-        verbose_name=u'Разрешение',
+        verbose_name='Разрешение',
         on_delete=models.CASCADE,
     )
 
     cascade_delete_for = (role,)
     display_related_error = False
 
     class Meta:
-        verbose_name = u'Разрешение роли'
-        verbose_name_plural = u'Разрешения ролей'
+        verbose_name = 'Разрешение роли'
+        verbose_name_plural = 'Разрешения ролей'
         unique_together = ('role', 'permission')
         db_table = 'rbac_role_permissions'
 
     def __str__(self):
         return 'Роль: {}; Разрешение: {}'.format(
             self.role.name, self.permission.title)
 
 
 @receiver(pre_delete, sender=RolePermission)
 def protect_role_edit_permission(instance, **kwargs):
-    u"""Предотвращает удаление из всех ролей разрешение на редактирование роли.
+    """Предотвращает удаление из всех ролей разрешение на редактирование роли.
 
     Если это разрешение удалить из всех ролей, то никто из пользователей больше
     не сможет внести изменения в реестр ролей.
     """
     if (
         not RolePermission.objects.filter(
             permission__name=PERM__ROLE__EDIT,
         ).exclude(
             id=instance.pk,
         ).exists() and
         instance.permission.name == PERM__ROLE__EDIT
     ):
         raise ApplicationLogicException(
-            u'Роль "{role}" является единственной ролью в Cистеме, в которой '
-            u'есть разрешение "{permission}". В системе должна оставаться '
-            u'возможность настройки ролей, поэтому удаление из неё этого '
-            u'разрешения невозможно. Для удаления разрешения "{permission}" '
-            u'из роли "{role}" сначала назначьте данное разрешение любой '
-            u'другой роли в системе.'
+            'Роль "{role}" является единственной ролью в Cистеме, в которой '
+            'есть разрешение "{permission}". В системе должна оставаться '
+            'возможность настройки ролей, поэтому удаление из неё этого '
+            'разрешения невозможно. Для удаления разрешения "{permission}" '
+            'из роли "{role}" сначала назначьте данное разрешение любой '
+            'другой роли в системе.'
             .format(
                 role=instance.role.name,
                 permission=get_permission_full_title(instance.permission.name),
             )
         )
 
 
-@six.python_2_unicode_compatible
 class RoleParent(BaseModel):
-
-    u"""M2M-модель "Вложенная роль"."""
+    """M2M-модель "Вложенная роль"."""
 
     parent = models.ForeignKey(
         Role, related_name='+', on_delete=models.CASCADE
     )
     role = models.ForeignKey(
         Role, related_name='+', on_delete=models.CASCADE
     )
@@ -322,122 +346,120 @@
     display_related_error = False
 
     def simple_clean(self, errors):
         super(RoleParent, self).simple_clean(errors)
 
         if self.parent.id == self.role.id:
             errors['parent'].append(
-                u'Роль не может содержать сама себя'
+                'Роль не может содержать сама себя'
             )
 
         # ---------------------------------------------------------------------
         # Проверка отсутствия цикла
         query = RoleParent.objects.all()
         if self.pk:
             query = query.exclude(pk=self.pk)
 
         def check(target_role, role):
             for role_parent in query.filter(role=role):
                 if target_role.id == role_parent.parent_id:
-                    raise ValidationError(u'В иерархии ролей обнаружен цикл')
+                    raise ValidationError('В иерархии ролей обнаружен цикл')
                 check(target_role, role_parent.parent)
 
         try:
             # Проверка, нет ли self.role среди предков self.parent
             check(self.role, self.parent)
         except ValidationError as error:
             errors['parent'].extend(error.messages)
         # ---------------------------------------------------------------------
 
     def __str__(self):
-        return u'RoleParent({} --> {})'.format(
-            six.text_type(self.role), six.text_type(self.parent)
+        return 'RoleParent({} --> {})'.format(
+            str(self.role), str(self.parent)
         )
 
     class Meta:
         unique_together = ('parent', 'role')
-        verbose_name = u'Вложенная роль'
-        verbose_name_plural = u'Вложенные роли'
+        verbose_name = 'Вложенная роль'
+        verbose_name_plural = 'Вложенные роли'
 
 
 UserRoleMeta = model_modifier_metaclass(
     DateIntervalMeta,
     date_from=dict(
-        verbose_name=u'Действует с',
+        verbose_name='Действует с',
     ),
     date_to=dict(
-        verbose_name=u'по',
+        verbose_name='по',
     ),
 )
 
 
-@six.python_2_unicode_compatible
-class UserRole(six.with_metaclass(UserRoleMeta, DateIntervalMixin, BaseModel)):
-
-    u"""M2M-модель "Роль пользователя"."""
+class UserRole(DateIntervalMixin, BaseModel, metaclass=UserRoleMeta):
+    """M2M-модель "Роль пользователя"."""
 
     no_intersections_for = ('content_type', 'object_id', 'role')
 
     content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
     object_id = models.PositiveIntegerField()
     user = GenericForeignKey()
     role = models.ForeignKey(
         Role,
-        verbose_name=u'Роль',
+        verbose_name='Роль',
         on_delete=models.CASCADE,
     )
 
     actual_objects = ActualObjectsManager()
 
     class Meta:
-        verbose_name = u'Роль пользователя'
-        verbose_name_plural = u'Роли пользователя'
+        verbose_name = 'Роль пользователя'
+        verbose_name_plural = 'Роли пользователя'
 
     def __str__(self):
-        return u'UserRole({} --> {})'.format(
-            six.text_type(self.user), six.text_type(self.role),
+        return 'UserRole({} --> {})'.format(
+            str(self.user), str(self.role),
         )
 
     def interval_intersected_error_message(self, others=None):
         return (
-            u'Роль "{}" уже назначена этому пользователю в указанном '
-            u'интервале дат.'.format(self.role.name)
+            'Роль "{}" уже назначена этому пользователю в указанном '
+            'интервале дат.'.format(self.role.name)
         )
 
     def simple_clean(self, errors):
         super(UserRole, self).simple_clean(errors)
 
         if not self.role.can_be_assigned:
             errors['role'].append(
-                u'Роль "{}" не может быть назначена пользователю'.format(
+                'Роль "{}" не может быть назначена пользователю'.format(
                     self.role.name
                 )
             )
 
         if (
             config.rbac_config.user_types and
             self.role_id and
             self.content_type_id and
             not RoleUserType.objects.filter(
                 role_id=self.role_id,
                 user_type_id=self.content_type_id,
             ).exists()
         ):
             errors['role'].append(
-                u'Роль "{}" не доступна для назначения '
-                u'пользователям типа "{}".'.format(
+                'Роль "{}" не доступна для назначения '
+                'пользователям типа "{}".'.format(
                     self.role.name,
                     self.content_type.name,
                 )
             )
 
 
 @receiver(post_delete)
 def delete_user_roles(instance, **kwargs):  # pylint: disable=unused-argument
-    u"""Удаление привязки ролей к пользователям при удалении пользователя."""
+    """Удаление привязки ролей к пользователям при удалении пользователя."""
     # Если модель была удалена из Системы, то при накатывании миграций, в
     # которых удаляются записи таких моделей случается AttributeError.
     try:
         content_type = ContentType.objects.get_for_model(instance)
     except AttributeError:
         return
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/role-edit-window.js` & `educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/role-edit-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/roles-list-window.js` & `educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/roles-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js` & `educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/ui.py` & `educommon-3.0.0/src/educommon/auth/rbac/ui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,122 @@
-# coding: utf-8
 # pylint: disable=attribute-defined-outside-init, no-member
-from __future__ import absolute_import
-
 import json
 
-from django.utils.safestring import mark_safe
-from m3.actions.context import ActionContext
-from m3_ext.ui.containers.containers import ExtContainer
-from m3_ext.ui.containers.containers import ExtToolbarMenu
-from m3_ext.ui.containers.context_menu import ExtContextMenu
-from m3_ext.ui.containers.forms import ExtPanel
-from m3_ext.ui.containers.grids import ExtGridCheckBoxSelModel
-from m3_ext.ui.containers.trees import ExtTree
-from m3_ext.ui.fields import ExtMultiSelectField
-from m3_ext.ui.icons import Icons
-from m3_ext.ui.menus import ExtContextMenuItem
-from m3_ext.ui.misc import ExtDataStore
-from m3_ext.ui.misc.label import ExtLabel
-from m3_ext.ui.panels.grids import ExtObjectGrid
-from objectpack.tree_object_pack.ui import BaseObjectTree
-from objectpack.tree_object_pack.ui import BaseTreeSelectWindow
-from objectpack.ui import BaseListWindow
-from objectpack.ui import ColumnsConstructor
-from objectpack.ui import ObjectTab
-from objectpack.ui import WindowTab
-
-from educommon import ioc
-from educommon.auth.rbac.constants import PERM_SOURCES
-from educommon.objectpack.ui import ModelEditWindow
-from educommon.objectpack.ui import TabbedEditWindow
-from educommon.utils.ui import switch_window_in_read_only_mode
-
-from .models import Role
+from django.utils.safestring import (
+    mark_safe,
+)
+from m3.actions.context import (
+    ActionContext,
+)
+from m3_ext.ui.containers.containers import (
+    ExtContainer,
+    ExtToolbarMenu,
+)
+from m3_ext.ui.containers.context_menu import (
+    ExtContextMenu,
+)
+from m3_ext.ui.containers.forms import (
+    ExtPanel,
+)
+from m3_ext.ui.containers.grids import (
+    ExtGridCheckBoxSelModel,
+)
+from m3_ext.ui.containers.trees import (
+    ExtTree,
+)
+from m3_ext.ui.fields import (
+    ExtMultiSelectField,
+)
+from m3_ext.ui.icons import (
+    Icons,
+)
+from m3_ext.ui.menus import (
+    ExtContextMenuItem,
+)
+from m3_ext.ui.misc import (
+    ExtDataStore,
+)
+from m3_ext.ui.misc.label import (
+    ExtLabel,
+)
+from m3_ext.ui.panels.grids import (
+    ExtObjectGrid,
+)
+
+from objectpack.tree_object_pack.ui import (
+    BaseObjectTree,
+    BaseTreeSelectWindow,
+)
+from objectpack.ui import (
+    BaseListWindow,
+    ColumnsConstructor,
+    ObjectTab,
+    WindowTab,
+)
+
+from educommon import (
+    ioc,
+)
+from educommon.auth.rbac.constants import (
+    PERM_SOURCES,
+)
+from educommon.auth.rbac.models import (
+    Role,
+)
+from educommon.objectpack.ui import (
+    ModelEditWindow,
+    TabbedEditWindow,
+)
+from educommon.utils.ui import (
+    switch_window_in_read_only_mode,
+)
 
 
 class RolesTree(BaseObjectTree):
-
-    u"""Грид для отображения иерархии ролей.
+    """Грид для отображения иерархии ролей.
 
     Отличается от обычного грида для отображения деревьев тем, что помимо
     кнопок "Новый в корне" и "Новый дочерний" имеет кнопку "Добавить в роль".
     """
 
     def __init__(self, *args, **kwargs):
         super(RolesTree, self).__init__(*args, **kwargs)
 
         # Меню "Добавить"
         self.top_bar.button_add_to_role = ExtContextMenuItem(
-            text=u'Добавить в роль',
+            text='Добавить в роль',
             icon_cls='add_item',
             handler='topBarAddToRole',
         )
         self.top_bar.add_menu.menu.items.append(
             self.top_bar.button_add_to_role
         )
 
         # Меню "Удалить"
         self.top_bar.items.remove(self.top_bar.button_delete)
         self.top_bar.button_delete_from_role = ExtContextMenuItem(
-            text=u'Удалить из роли',
+            text='Удалить из роли',
             icon_cls='delete_item',
             handler='topBarDeleteFromRole',
         )
         self.top_bar.button_delete = ExtContextMenuItem(
-            text=u'Удалить из системы',
+            text='Удалить из системы',
             icon_cls='delete_item',
             handler='topBarDelete',
         )
 
         menu = ExtContextMenu()
         menu.items.extend((
             self.top_bar.button_delete_from_role,
             self.top_bar.button_delete,
         ))
         self.top_bar.delete_menu = ExtToolbarMenu(
             icon_cls="delete_item",
             menu=menu,
-            text=u'Удалить'
+            text='Удалить'
         )
         self.top_bar.items.append(self.top_bar.delete_menu)
 
         # Передаем индексы, так как некорректно
         # формируется client_id для данных элементов.
         self.add_menu_index = self.top_bar.items.index(
             self.top_bar.add_menu
@@ -96,16 +132,15 @@
         )
         self.delete_from_role_index = menu.items.index(
             self.top_bar.button_delete_from_role
         )
 
 
 class RolesListWindow(BaseListWindow):
-
-    u"""Окно для отображения иерархии ролей."""
+    """Окно для отображения иерархии ролей."""
 
     def _init_components(self):
         super(RolesListWindow, self)._init_components()
 
         self.grid = RolesTree()
 
     def set_params(self, params):
@@ -120,49 +155,48 @@
             self.grid.action_new = None
 
             # Отключение контролов для изменения ролей
             for control in (
                 self.grid.top_bar.button_edit,
                 self.grid.context_menu_row.menuitem_edit
             ):
-                control.text = u'Просмотр'
+                control.text = 'Просмотр'
                 control.icon_cls = Icons.APPLICATION_VIEW_DETAIL
 
             # Изменение контролов для удаления ролей
             self.grid.action_delete = None
             self.grid.url_delete = None
             self.grid.top_bar.items.remove(self.grid.top_bar.delete_menu)
         # ---------------------------------------------------------------------
         self.template_globals = template
 
 
 class RoleSelectWindow(BaseTreeSelectWindow):
-
-    u"""Окно выбора роли, в которую будет добавлена указанная роль."""
+    """Окно выбора роли, в которую будет добавлена указанная роль."""
 
     def _init_components(self):
         super(RoleSelectWindow, self)._init_components()
 
         self.label_message = ExtLabel(
-            text=u'Выберите роль, в которую будет добавлена роль "{}":',
+            text='Выберите роль, в которую будет добавлена роль "{}":',
             style={'padding': '5px'},
             region='north',
         )
 
     def _do_layout(self):
         super(RoleSelectWindow, self)._do_layout()
 
         self.layout = 'border'
 
         self.items.insert(0, self.label_message)
 
     def set_params(self, params):
         super(RoleSelectWindow, self).set_params(params)
 
-        self.title = u'Добавление одной роли в другую'
+        self.title = 'Добавление одной роли в другую'
 
         self.grid.region = 'center'
         self.grid.action_new = None
         self.grid.action_edit = None
         self.grid.action_delete = None
 
         if self.grid.action_context is None:
@@ -173,35 +207,34 @@
             mark_safe(self.label_message.text.format(params['role'].name))
         )
 # -----------------------------------------------------------------------------
 
 
 def _make_user_type_field(name='user_type_ids', **kwargs):
     field = ExtMultiSelectField(
-        label=u'Может быть назначена',
+        label='Может быть назначена',
         anchor='100%',
         hide_edit_trigger=False,
         hide_trigger=False,
         hide_dict_select_trigger=False,
         **kwargs
     )
     field.name = name
 
     return field
 
 
 class PermissionsChangeTab(ObjectTab):
-
-    u"""Вкладка "Разрешения роли" окна редактирования роли.
+    """Вкладка "Разрешения роли" окна редактирования роли.
 
     Содержит элементы интерфейса для изменения параметров роли: названия,
     текстового описания, перечня разрешений и т.д.
     """
 
-    title = u'Разрешения роли'
+    title = 'Разрешения роли'
 
     model = Role
 
     field_fabric_params = dict(
         field_list=('name', 'description', 'can_be_assigned'),
     )
 
@@ -220,15 +253,15 @@
         self.grid__permissions = ExtObjectGrid()
         self.grid__permissions.top_bar.hidden = True
         self.grid__permissions.store.auto_load = False
 
         self.panel__description = ExtPanel(
             header=True,
             padding=5,
-            title=u'Описание разрешения',
+            title='Описание разрешения',
         )
 
     def do_layout(self, win, tab):
         super(PermissionsChangeTab, self).do_layout(win, tab)
 
         tab.border = False
         # ---------------------------------------------------------------------
@@ -300,65 +333,63 @@
             )
 
         params['partitions_pack'].configure_grid(self.grid__partitions)
         params['permissions_pack'].configure_grid(self.grid__permissions)
 
 
 class ResultPermissionsTree(ExtTree):
-
-    u"""Панель для отображения итоговых разрешений в виде дерева.
+    """Панель для отображения итоговых разрешений в виде дерева.
 
     В дереве отображается три уровня: разделы, группы и сами разрешения.
     """
 
     def __init__(self, *args, **kwargs):
         super(ResultPermissionsTree, self).__init__()
 
         ColumnsConstructor.from_config((
             dict(
                 data_index='title',
-                header=u'Наименование',
+                header='Наименование',
             ),
             dict(
                 data_index='description',
                 hidden=True,
             ),
             dict(
-                data_index=u'source',
-                header=u'Источник',
+                data_index='source',
+                header='Источник',
             ),
         )).configure_grid(self)
 
 
 class ResultPermissionsTab(WindowTab):
-
-    u"""Вкладка "Итоговые разрешения" окна редактирования роли.
+    """Вкладка "Итоговые разрешения" окна редактирования роли.
 
     Предназначена для отображения результирующего набора разрешений, которые
     предоставляет роль. В этот набор входят:
 
         - разрешения, добавленные в роль;
         - разрешения, зависящие тех, которые добавлены в роль;
         - разрешения вложенных ролей.
 
     Для каждого разрешения указывается источник: сама роль, зависимое
     разрешение или вложенная роль.
     """
 
-    title = u'Итоговые разрешения'
+    title = 'Итоговые разрешения'
 
     def init_components(self, win):
         super(ResultPermissionsTab, self).init_components(win)
 
         self.tree__result_permissions = ResultPermissionsTree()
 
         self.panel__description = ExtPanel(
             header=True,
             padding=5,
-            title=u'Описание разрешения',
+            title='Описание разрешения',
         )
 
     def do_layout(self, win, tab):
         super(ResultPermissionsTab, self).do_layout(win, tab)
         # ---------------------------------------------------------------------
 
         win.tab__result_permissions = tab
@@ -378,16 +409,15 @@
         self.tree__result_permissions.flex = 1
         self.panel__description.flex = 0
         self.panel__description.height = 100
         # ---------------------------------------------------------------------
 
 
 class RoleAddWindow(ModelEditWindow):
-
-    u"""Окно добавления роли."""
+    """Окно добавления роли."""
 
     model = Role
 
     field_fabric_params = dict(
         field_list=('name', 'description', 'can_be_assigned'),
         model_register=ioc.get('observer'),
     )
@@ -408,16 +438,15 @@
         if params.get('show_user_types', False):
             self.field__user_types.set_store(
                 ExtDataStore(data=params['user_types'])
             )
 
 
 class RoleEditWindow(TabbedEditWindow):
-
-    u"""Окно редактирования роли."""
+    """Окно редактирования роли."""
 
     model = Role
 
     tabs = (
         PermissionsChangeTab,
         ResultPermissionsTab,
     )
```

### Comparing `educommon-2.20.0/src/educommon/auth/rbac/utils.py` & `educommon-3.0.0/src/educommon/auth/rbac/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-# coding: utf-8
-u"""Вспомогательные средства для работы с подсистемой RBAC."""
-from __future__ import absolute_import
-
+"""Вспомогательные средства для работы с подсистемой RBAC."""
 import operator
-
-import six
-from m3.actions import Action
-from m3.actions import ActionPack
-
-from educommon.m3 import get_pack
-
-
-if six.PY2:
-    from inspect import getargspec as getfullargspec
-else:
-    from inspect import getfullargspec
+from inspect import (
+    getfullargspec,
+)
+
+from m3.actions import (
+    Action,
+    ActionPack,
+)
+
+from educommon.m3 import (
+    get_pack,
+)
 
 
 def _resolve_packs_or_actions(packs_or_actions):
-    u"""Возвращает список из паков и экшенов, заданных классами и строками."""
+    """Возвращает список из паков и экшенов, заданных классами и строками."""
     def resolve(pack_or_action):
         if isinstance(pack_or_action, tuple):
             pack, action = pack_or_action
             pack = get_pack(pack)
             result = getattr(pack, action)
         else:
             result = get_pack(pack_or_action)
@@ -33,15 +30,15 @@
         for pack_or_action in packs_or_actions
     ]
 
     return result
 
 
 def _rule_filter(rule_handler, packs_or_actions, operator_):
-    u"""Возвращает обработчик правила, "обернутый" в фильтрующую функцию."""
+    """Возвращает обработчик правила, "обернутый" в фильтрующую функцию."""
     def action_in_list(action):
         for pack_or_action in _resolve_packs_or_actions(packs_or_actions):
             if (
                 isinstance(pack_or_action, Action) and
                 action.__class__ is pack_or_action.__class__
             ) or (
                 isinstance(pack_or_action, ActionPack) and
@@ -57,43 +54,43 @@
         else:
             return True
 
     return wrapper
 
 
 def only_for(rule_handler, *packs_or_actions):
-    u"""Выполняет правило только для указанных паков и экшенов.
+    """Выполняет правило только для указанных паков и экшенов.
 
     Экшены задаются в виде кортежа из двух элементов: первый элемент определяет
     пак (см. educommon.m3.get_pack()), а второй - имя атрибута этого пака, в
     котором содержится экшен. Иначе аргумент будет определять пак целиком.
 
     :param rule_handler: Обработчик правила.
 
     :rtype: callable
     """
     return _rule_filter(rule_handler, packs_or_actions, operator.truth)
 
 
 def except_for(rule_handler, *packs_or_actions):
-    u"""Выполняет правило для всех паков и экшенов, кроме указанных.
+    """Выполняет правило для всех паков и экшенов, кроме указанных.
 
     Экшены задаются в виде кортежа из двух элементов: первый элемент определяет
     пак (см. educommon.m3.get_pack()), а второй - имя атрибута этого пака, в
     котором содержится экшен. Иначе аргумент будет определять пак целиком.
 
     :param rule_handler: Обработчик правила.
 
     :rtype: callable
     """
     return _rule_filter(rule_handler, packs_or_actions, operator.not_)
 
 
 def invert_rule(rule_handler):
-    u"""Применяет к обработчику правил RBAC операцию "логическое НЕ".
+    """Применяет к обработчику правил RBAC операцию "логическое НЕ".
 
     .. code-block:: python
        :caption: ``permissions.py``
 
        rules = {
            PERM_SOME_ACTION: invert_rule(user_is_employee),
        }
@@ -103,15 +100,15 @@
     def wrapper(action, request, user, *args, **kwargs):
         return not rule_handler(action, request, user, *args, **kwargs)
 
     return wrapper
 
 
 def any_rules(*rule_handlers):
-    u"""Объединяет обработчики правил RBAC операцией "логическое ИЛИ".
+    """Объединяет обработчики правил RBAC операцией "логическое ИЛИ".
 
     В результате объединения доступ будет разрешен если хотя бы один из
     обработчиков разрешит доступ.
 
     .. code-block:: python
        :caption: ``permissions.py``
 
@@ -127,15 +124,15 @@
                 return True
         return False
 
     return wrapper
 
 
 def all_rules(*rule_handlers):
-    u"""Объединяет обработчики правил RBAC операцией "логическое И".
+    """Объединяет обработчики правил RBAC операцией "логическое И".
 
     В результате объединения доступ будет разрешен только если каждый из
     обработчиков разрешит доступ.
 
     Например, разрешить доступ к какому-либо действию над объектом только для
     сотрудников текущего учреждения можно объединив два правила:
 
@@ -154,15 +151,15 @@
                 return False
         return True
 
     return wrapper
 
 
 def get_rbac_rule_data(request, action):
-    u"""Возвращает данные для обработчика правила RBAC.
+    """Возвращает данные для обработчика правила RBAC.
 
     Если у :arg:`action` есть метод ``get_rbac_rule_data()``, то вызывает его.
     Иначе вызывает такой метод у набора действий (ActionPack), в который входит
     действие :arg:`action`.
 
     У метода ``get_rbac_rule_data()`` может быть один аргумент ``request``,
     либо два аргумента: ``request`` и ``action``.
@@ -196,19 +193,21 @@
 
         setattr(request, '_rbac_rule_data', data)
 
     return getattr(request, '_rbac_rule_data')
 
 
 def get_permission_full_title(permission_name):
-    u"""Возвращает полное наименование разрешения по его имени.
+    """Возвращает полное наименование разрешения по его имени.
 
     Полное наименование состоит их наименований раздела, группы и
     разрешения.
     """
-    from .manager import rbac
+    from educommon.auth.rbac.manager import (
+        rbac,
+    )
 
     _, permission_title = rbac.permissions_by_name[permission_name]
     group_name, group_title = rbac.get_group_params(permission_name)
     partition_title = rbac.get_partition_title(group_name)
 
-    return u' - '.join((partition_title, group_title, permission_title))
+    return ' - '.join((partition_title, group_title, permission_title))
```

### Comparing `educommon-2.20.0/src/educommon/auth/simple_auth/actions.py` & `educommon-3.0.0/src/educommon/auth/simple_auth/actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,76 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from uuid import uuid4
 import datetime
-
-from django import http
-from django.conf import settings
-from django.contrib import auth
-from django.core.exceptions import ValidationError
-from django.core.mail.message import EmailMessage
-from django.http import HttpResponseRedirect
-from django.shortcuts import render
-from django.template.loader import render_to_string
-from m3.actions.exceptions import ApplicationLogicException
-from m3.actions.results import OperationResult
-from m3.actions.results import PreJsonResult
-from m3_django_compat import get_user_model
-from m3_ext.ui.shortcuts import MessageBox
-from objectpack.actions import BaseAction
-from objectpack.actions import BasePack
-from six.moves.urllib.parse import urljoin
-
-from educommon import ioc
-from educommon.m3 import convert_validation_error_to
-
-from . import checkers
-from . import const
-from . import validators
-from .models import ResetPasswords
+from urllib.parse import (
+    urljoin,
+)
+from uuid import (
+    uuid4,
+)
+
+from django import (
+    http,
+)
+from django.conf import (
+    settings,
+)
+from django.contrib import (
+    auth,
+)
+from django.core.exceptions import (
+    ValidationError,
+)
+from django.core.mail.message import (
+    EmailMessage,
+)
+from django.http import (
+    HttpResponseRedirect,
+)
+from django.shortcuts import (
+    render,
+)
+from django.template.loader import (
+    render_to_string,
+)
+from m3.actions.exceptions import (
+    ApplicationLogicException,
+)
+from m3.actions.results import (
+    OperationResult,
+    PreJsonResult,
+)
+from m3_django_compat import (
+    get_user_model,
+)
+from m3_ext.ui.shortcuts import (
+    MessageBox,
+)
+
+from objectpack.actions import (
+    BaseAction,
+    BasePack,
+)
+
+from educommon import (
+    ioc,
+)
+from educommon.auth.simple_auth import (
+    checkers,
+    const,
+    validators,
+)
+from educommon.auth.simple_auth.models import (
+    ResetPasswords,
+)
+from educommon.m3 import (
+    convert_validation_error_to,
+)
 
 
 class AuthPack(BasePack):
-
-    u"""Пак аутентификации."""
+    """Пак аутентификации."""
 
     url = const.AUTH_PACK_URL
 
     login_checker = checkers.DefaultLoginChecker()
 
     def __init__(self):
         super(AuthPack, self).__init__()
@@ -62,16 +96,16 @@
             self.change_password_page_action,
             self.change_password_action
         ))
 
     def declare_context(self, action):
         ctx = super(AuthPack, self).declare_context(action)
         if action is self.login_action:
-            ctx['login'] = dict(type='unicode', default=u'')
-            ctx['password'] = dict(type='unicode', default=u'')
+            ctx['login'] = dict(type='str', default='')
+            ctx['password'] = dict(type='str', default='')
         return ctx
 
     def get_login_url(self):
         return self.login_action.get_absolute_url()
 
     def get_logout_url(self):
         return self.logout_action.get_absolute_url()
@@ -89,16 +123,15 @@
         return self.change_password_page_action.get_absolute_url()
 
     def get_change_password_url(self):
         return self.change_password_action.get_absolute_url()
 
 
 class LoginPageAction(BaseAction):
-
-    u"""Экшн отображает страницу входа."""
+    """Экшн отображает страницу входа."""
 
     url = const.LOGIN_PAGE_URL
     template_file_name = 'simple_auth/login_page.html'
 
     def _get_login_panel(self, request, context):
         get_login_panel = ioc.get('simple_auth__get_login_panel')
 
@@ -119,16 +152,15 @@
             request,
             self.template_file_name,
             self.get_template_context(request, context)
         )
 
 
 class LoginAction(BaseAction):
-
-    u"""Проверяет данные и выполняет вход."""
+    """Проверяет данные и выполняет вход."""
 
     url = '/login'
 
     def run(self, request, context):
         username = context.login
         password = context.password
 
@@ -151,16 +183,15 @@
                 redirect='/',
             ))
 
         return result
 
 
 class ResetPasswordPageAction(BaseAction):
-
-    u"""Экшен страницы восстановления пароля."""
+    """Экшен страницы восстановления пароля."""
 
     url = const.RESET_PASSWORD_PAGE_URL
     template_file_name = 'simple_auth/reset_password_page.html'
 
     def get_template_context(self, request, context):
         return dict(
             login_page_url=self.parent.get_login_page_url(),
@@ -171,16 +202,15 @@
         return render(
             request, self.template_file_name,
             self.get_template_context(request, context)
         )
 
 
 class ResetPasswordAction(BaseAction):
-
-    u"""Экшен восстановления пароля."""
+    """Экшен восстановления пароля."""
 
     url = const.RESET_PASSWORD_URL
     email_template_file_name = 'simple_auth/email/reset_password.html'
 
     def context_declaration(self):
         return {'email': {'type': 'str'}}
 
@@ -205,16 +235,16 @@
 
         return get_user_by_email(email)
 
     def run(self, request, context):
         user = ResetPasswordAction._get_user_by_email(context.email)
         if user is None:
             return OperationResult(False, message=(
-                u'Этот адрес электронной почты не связан ни с одной учетной '
-                u'записью. Вы уверены, что зарегистрированы?'
+                'Этот адрес электронной почты не связан ни с одной учетной '
+                'записью. Вы уверены, что зарегистрированы?'
             ))
 
         now = datetime.datetime.now()
         life = getattr(settings, 'RESET_CODES_LIFE', None)
         life = datetime.timedelta(minutes=life or const.RESET_CODES_LIFE)
 
         # Удаляем устаревшие записи
@@ -232,29 +262,28 @@
         template = render_to_string(
             self.email_template_file_name,
             template_context
         )
 
         # Отправка письма
         msg = EmailMessage(
-            u'Восстановление пароля', template,
+            'Восстановление пароля', template,
             settings.DEFAULT_FROM_EMAIL, [context.email]
         )
         msg.content_subtype = 'html'
         msg.send()
 
         return OperationResult(
-            message=u'На указанный адрес отправлено письмо с дальнейшими'
-                    u' инструкциями.'
+            message='На указанный адрес отправлено письмо с дальнейшими'
+                    ' инструкциями.'
         )
 
 
 class ChangeResetPasswordPageAction(BaseAction):
-
-    u"""Экшен страницы изменения сброшенного пароля."""
+    """Экшен страницы изменения сброшенного пароля."""
 
     url = const.CHANGE_RESET_PASSWORD_PAGE_URL
     template_file_name = 'simple_auth/change_reset_password_page.html'
 
     def context_declaration(self):
         return {'code': {'type': 'str'}}
 
@@ -280,25 +309,24 @@
         return render(
             request, self.template_file_name,
             self.get_template_context(request, context)
         )
 
 
 class ChangeResetPasswordAction(BaseAction):
-
-    u"""Экшен изменения сброшенного пароля."""
+    """Экшен изменения сброшенного пароля."""
 
     url = const.CHANGE_RESET_PASSWORD_URL
     validator = validators.DefaultPasswordValidator()
 
     def context_declaration(self):
         return {
             'code': {'type': 'str'},
-            'password': {'type': 'unicode'},
-            'password_confirm': {'type': 'unicode'}
+            'password': {'type': 'str'},
+            'password_confirm': {'type': 'str'}
         }
 
     @convert_validation_error_to(
         ApplicationLogicException, model=ResetPasswords
     )
     def run(self, request, context):
         password = context.password
@@ -314,54 +342,52 @@
             ).get(code=context.code).user
         except ResetPasswords.DoesNotExist:
             return HttpResponseRedirect(
                 self.parent.get_reset_password_page_url()
             )
 
         if password != confirm:
-            raise ValidationError(u'Пароль и подтверждение не совпадают!')
+            raise ValidationError('Пароль и подтверждение не совпадают!')
 
         errors = self.validator.validate(password)
         if errors:
             raise ValidationError(errors)
 
         user.set_password(password)
         user.save()
 
         ResetPasswords.objects.filter(user=user).delete()
-        return OperationResult(message=u'Новый пароль установлен!')
+        return OperationResult(message='Новый пароль установлен!')
 
 
 class LogoutConfirmAction(BaseAction):
-
-    u"""Экшн для отображения подтверждения выхода."""
+    """Экшн для отображения подтверждения выхода."""
 
     url = '/logout-confirm'
 
     def run(self, request, context):
         msg_box = MessageBox(
-            u'', u'Вы действительно хотите выйти из системы?',
+            '', 'Вы действительно хотите выйти из системы?',
             MessageBox.ICON_QUESTION, MessageBox.BTN_YESNO)
 
-        msg_box.handler_yes = u"""
+        msg_box.handler_yes = """
         Ext.Ajax.request({
             url: '%(url)s',
             params: {'confirm': true},
             success: function(response){
                 var json = Ext.util.JSON.decode(response.responseText);
                 window.location = json.redirect ? json.redirect : '/';
             }
         });
         """ % {'url': self.parent.logout_action.get_absolute_url()}
         return http.HttpResponse(msg_box.get_script())
 
 
 class LogoutAction(BaseAction):
-
-    u"""Экшн выполняет выход."""
+    """Экшн выполняет выход."""
 
     url = '/logout'
 
     def run(self, request, context):
 
         auth.logout(request)
```

### Comparing `educommon-2.20.0/src/educommon/auth/simple_auth/app_meta.py` & `educommon-3.0.0/src/educommon/auth/simple_auth/app_meta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,55 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from django.conf.urls import url
-from m3.actions import ControllerCache
-from m3_ext.ui.app_ui import GENERIC_USER
-from m3_ext.ui.app_ui import DesktopLoader
-from m3_ext.ui.app_ui import DesktopShortcut
-from objectpack.desktop import uificate_the_controller
-
-from educommon import ioc
-
-from .actions import AuthPack
+from django.conf.urls import (
+    url,
+)
+from m3.actions import (
+    ControllerCache,
+)
+from m3_ext.ui.app_ui import (
+    GENERIC_USER,
+    DesktopLoader,
+    DesktopShortcut,
+)
+
+from objectpack.desktop import (
+    uificate_the_controller,
+)
+
+from educommon import (
+    ioc,
+)
+from educommon.auth.simple_auth.actions import (
+    AuthPack,
+)
 
 
 auth_controller = ioc.get('auth_controller')
 
 
 def register_actions():
     auth_controller.extend_packs((
         AuthPack(),
     ))
 
 
 def register_desktop_menu():
-    u"""Добавляет в меню Пуск пункт "Выход"."""
+    """Добавляет в меню Пуск пункт "Выход"."""
     auth_pack = ControllerCache.find_pack(AuthPack)
     DesktopLoader.add(
         GENERIC_USER,
         DesktopLoader.TOOLBOX,
         DesktopShortcut(
             pack=auth_pack.logout_confirm_action,
-            name=u'Выход',
+            name='Выход',
             index=256,
             icon='logout'
         )
     )
 
     uificate_the_controller(auth_controller)
 
 
 def register_urlpatterns():
-    u"""Регистрация URL контроллера."""
+    """Регистрация URL контроллера."""
     return [
         url(*auth_controller.urlpattern),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/auth/simple_auth/checkers.py` & `educommon-3.0.0/src/educommon/auth/simple_auth/checkers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-# coding: utf-8
-u"""Классы, осуществляющие проверку пользовательских данных."""
-from __future__ import absolute_import
+"""Классы, осуществляющие проверку пользовательских данных."""
+from m3_django_compat import (
+    get_user_model,
+)
 
-from m3_django_compat import get_user_model
 
-
-MESSAGE_USER_NOT_EXISTS = u'Пользователь не найден.'
-MESSAGE_PASSWORD_INCORRECT = u'Неверный логин или пароль.'
-MESSAGE_USER_INACTIVE = u'Пользователь заблокирован'
+MESSAGE_USER_NOT_EXISTS = 'Пользователь не найден.'
+MESSAGE_PASSWORD_INCORRECT = 'Неверный логин или пароль.'
+MESSAGE_USER_INACTIVE = 'Пользователь заблокирован'
 
 
 User = get_user_model()
 
 
-class DefaultLoginChecker(object):
-
-    u"""Проверяет данные при входе."""
+class DefaultLoginChecker:
+    """Проверяет данные при входе."""
 
     def _check_lic(self, *args, **kwargs):
         # TODO: проверка лицензии
         request = kwargs['request']
         return None
 
     def _check_user_exists(self, *args, **kwargs):
-        u"""Проверка существования пользователя с таким username."""
+        """Проверка существования пользователя с таким username."""
         username = kwargs['username']
         if not User.objects.filter(username=username).exists():
             return MESSAGE_USER_NOT_EXISTS
 
     def _check_user_active(self, *args, **kwargs):
-        u"""Проверка что пользователь активен."""
+        """Проверка что пользователь активен."""
         username = kwargs['username']
         try:
             user = User.objects.get(username=username)
         except User.DoesNotExist:
             return MESSAGE_USER_NOT_EXISTS
         else:
             if not user.is_active:
                 return MESSAGE_USER_INACTIVE
 
     def _check_user_password(self, *args, **kwargs):
-        u"""Проверка существования пользователя с таким username/password."""
+        """Проверка существования пользователя с таким username/password."""
         username = kwargs['username']
         password = kwargs['password']
         try:
             user = User.objects.get(username=username)
         except User.DoesNotExist:
             return MESSAGE_USER_NOT_EXISTS
         else:
@@ -55,15 +53,15 @@
         _check_lic,
         _check_user_exists,
         _check_user_active,
         _check_user_password,
     ]
 
     def check(self, request, username, password):
-        u"""Выполняет проверки по цепочке до первой ошибки.
+        """Выполняет проверки по цепочке до первой ошибки.
 
         Если ошибки не возникло, LoginAction производит аутентификацию
         средствами django.
         """
         for checker in self._checkers:
             error = checker(
                 self, request=request, username=username, password=password)
```

### Comparing `educommon-2.20.0/src/educommon/auth/simple_auth/migrations/0001_initial.py` & `educommon-3.0.0/src/educommon/auth/simple_auth/migrations/0001_initial.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.conf import settings
-from django.db import migrations
-from django.db import models
+from django.conf import (
+    settings,
+)
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html` & `educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html` & `educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html` & `educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html` & `educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/auth/simple_auth/ui.py` & `educommon-3.0.0/src/educommon/auth/simple_auth/ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,95 @@
-# coding: utf-8
-from __future__ import absolute_import
+from inspect import (
+    isclass,
+)
+
+from django.template.context import (
+    RequestContext,
+)
+from m3_django_compat import (
+    get_template,
+)
 
-from inspect import isclass
 
-from django.template.context import RequestContext
-from m3_django_compat import get_template
-
-
-class HtmlPageComponent(object):
-
-    u"""Компонент HTML-страницы.
+class HtmlPageComponent:
+    """Компонент HTML-страницы.
 
     Компонент имеет свой шаблон Django, умеет компилировать себя в HTML-код.
     Использование компонент для формирования элементов HTML-страниц позволяет
     работать с элементами страниц как с объектами.
     """
 
     id = None
-    u"""Идентификатор элемента."""
+    """Идентификатор элемента."""
 
     template_path = None
-    u"""Путь к шаблону Django, содержащему HTML-код элемента панели.
+    """Путь к шаблону Django, содержащему HTML-код элемента панели.
 
     В данном шаблоне будет доступен экземпляр (объект) данного компонента в
     переменной ``element``.
 
     .. note:
        При необходимости добавления других переменных в конекст шаблона
        переопределяйте метод :py:meth:`_get_template_context`
     """
 
     def __init__(self, request, context, **params):
-        u"""Инициализация элемента панели.
+        """Инициализация элемента панели.
 
         :param request: HTTP-запрос.
         :type request: django.http.HttpRequest
 
         :param context: Контекст операции.
         :type context: m3.action.context.ActionContext
         """
         self.request = request
         self.context = context
         self.params = params
 
     def _get_template(self):
-        u"""Возвращает шаблон элемента панели.
+        """Возвращает шаблон элемента панели.
 
         :rtype: django.template.base.Template
         """
-        assert self.template_path is not None, u'Не указан путь к шаблону.'
+        assert self.template_path is not None, 'Не указан путь к шаблону.'
 
         return get_template(self.template_path)
 
     def _get_template_context(self):
-        u"""Возвращает контекст шаблона.
+        """Возвращает контекст шаблона.
 
         В параметре ``element`` будет доступен сам элемент.
 
         :rtype: django.template.context.RequestContext
         """
         result = RequestContext(self.request)
 
         result['element'] = self
 
         return result
 
     def render(self):
-        u"""Компиляция шаблона элемента панели.
+        """Компиляция шаблона элемента панели.
 
-        :rtype: unicode
+        :rtype: str
         """
         template = self._get_template()
         template_context = self._get_template_context()
 
         return template.render(template_context)
 
 
 class Container(HtmlPageComponent):
-
-    u"""Контейнер компонент HTML-страницы.
+    """Контейнер компонент HTML-страницы.
 
     Логически состоит из вложенных элементов и других контейнеров.
     """
 
     items = []
-    u"""Элементы контейнера.
+    """Элементы контейнера.
 
     Может содержать как экземпляры компонент, так и классы. Если при компиляции
     контейнера в списке элементов окажется класс, то перед компиляцией этого
     элемента будет создан его экземпляр.
     """
 
     def __init__(self, request, context, **params):
@@ -99,29 +100,29 @@
             if isclass(item):
                 items.append(item(self.request, self.context, **self.params))
             else:
                 items.append(item)
         self.items = items
 
     def _get_template_context(self):
-        u"""Возвращает контекст шаблона.
+        """Возвращает контекст шаблона.
 
         Дополняет конекст шаблона переменной ``items``, содержащей
         упорядоченный список вложенных элементов контейнера.
 
         :rtype: django.template.context.RequestContext
         """
         result = super(Container, self)._get_template_context()
 
         result['items'] = self.items
 
         return result
 
     def get_item_by_id(self, item_id):
-        u"""Возвращает первый элемент с идентификатором ``item_id``."""
+        """Возвращает первый элемент с идентификатором ``item_id``."""
         for item in self.items:
             if item.id == item_id:
                 return item
 
     def remove_item_by_id(self, item_id):
-        u"""Удаляет из списка элементов контейнера элемент с указанным id."""
+        """Удаляет из списка элементов контейнера элемент с указанным id."""
         self.items[:] = [item for item in self.items if item.id == item_id]
```

### Comparing `educommon-2.20.0/src/educommon/contingent/actions.py` & `educommon-3.0.0/src/educommon/contingent/actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,103 +1,107 @@
-# coding: utf-8
-u"""Паки справочников контингента."""
-from __future__ import absolute_import
-
-from django.db.models import Q
-from objectpack.actions import ObjectPack
-
-from .catalogs import OkoguVirtualModel
-from .catalogs import OksmVirtialModel
+"""Паки справочников контингента."""
+from django.db.models import (
+    Q,
+)
+
+from objectpack.actions import (
+    ObjectPack,
+)
+
+from educommon.contingent.catalogs import (
+    OkoguVirtualModel,
+    OksmVirtialModel,
+)
 
 
 class OkoguPack(ObjectPack):
-    u"""Пак, предоставляющий средства для просмотра справочника ОКОГУ."""
+    """Пак, предоставляющий средства для просмотра справочника ОКОГУ."""
 
-    title = u'ОКОГУ'
+    title = 'ОКОГУ'
 
     model = OkoguVirtualModel
 
     columns = [
         dict(
             data_index='id',
-            header=u'Код',
+            header='Код',
             width=1,
             searchable=True,
         ),
         dict(
             data_index='full_name',
-            header=u'Полное наименование',
+            header='Полное наименование',
             width=3,
             searchable=True,
         ),
         dict(
             data_index='short_name',
-            header=u'Сокращенное наименование',
+            header='Сокращенное наименование',
             width=2,
             searchable=True,
         ),
     ]
     list_sort_order = ('id',)
     column_name_on_select = 'full_name'
 
     def configure_grid(self, grid):
-        u"""Конфигурирование грида.
+        """Конфигурирование грида.
 
         Добавляется css класс для переноса строк в ячейках грида
         """
         super(OkoguPack, self).configure_grid(grid)
 
         grid.cls = 'word-wrap-grid'  # перенос строк в ячейках грида
 
 
 class OKSMPack(ObjectPack):
-    u"""Справочник ОКСМ."""
+    """Справочник ОКСМ."""
 
-    title = u'Справочник ОКСМ'
+    title = 'Справочник ОКСМ'
     model = OksmVirtialModel
     read_only = True
     list_sort_order = ['shortname']
     column_name_on_select = 'shortname'
 
     columns = [
         {
             'data_index': 'shortname',
-            'header': u'Краткое наименование страны',
+            'header': 'Краткое наименование страны',
             'sortable': True,
             'searchable': True,
             'width': 2
         },
         {
             'data_index': 'code',
-            'header': u'Код',
+            'header': 'Код',
             'sortable': True,
             'searchable': True,
             'width': 1
         },
         {
             'data_index': 'full_name',
-            'header': u'Полное наименование',
+            'header': 'Полное наименование',
             'sortable': True,
             'searchable': True,
             'width': 3
         }
     ]
 
     def get_rows_query(self, request, context):
-        u"""
+        """
         Метод выполняет фильтрацию QuerySet.
 
         Исключается отображение РФ.
         """
         records = super(OKSMPack, self).get_rows_query(request, context)
 
         return records.exclude(code=OksmVirtialModel.rf_code)
 
     def apply_search(self, query, request, context):
-        u"""Поиск по краткому наименованию или коду."""
+        """Поиск по краткому наименованию или коду."""
         query = super(
             OKSMPack, self).apply_search(query, request, context)
 
         if hasattr(context, 'filter'):
             query = query.filter(Q(shortname__icontains=context.filter) |
                                  Q(code=context.filter))
         return query
```

### Comparing `educommon-2.20.0/src/educommon/contingent/base.py` & `educommon-3.0.0/src/educommon/contingent/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# coding: utf-8
-u"""Набор классов для реализации справочников контингента.
+"""Набор классов для реализации справочников контингента.
 
 BaseCatalogVirtualModel - виртуальная модель на основе JSON файла.
 BaseEnumerateProductSpecific - перечисление с продуктовыми зависимостями.
 BaseModelView - перечисление на основе виртуальной модели.
 """
-from __future__ import absolute_import
-
 import json
 import os
 
-from m3.db import BaseEnumerate
-from objectpack.models import VirtualModel
-import six
+from m3.db import (
+    BaseEnumerate,
+)
+
+from objectpack.models import (
+    VirtualModel,
+)
 
 
 def load_values(filename):
-    u"""Загружает данные справочника из файла в формате JSON.
+    """Загружает данные справочника из файла в формате JSON.
 
     Файл должен располагаться в папке json_data и содержать словарь значений.
 
     :param str filename: Имя файла (без пути!) с данными справочника.
 
     :rtype: dict
     """
@@ -30,18 +31,16 @@
         result = json.load(infile)
 
     assert isinstance(result, list), type(result)
 
     return result
 
 
-@six.python_2_unicode_compatible
 class BaseCatalogVirtualModel(VirtualModel):
-
-    u"""Виртуальная модель для справочников на основе JSON файла.
+    """Виртуальная модель для справочников на основе JSON файла.
 
     Виртуальная модель на основе BaseCatalogVirtualModel выгружает данные
     из JSON файла. Каждая запись может содержать множество полей.
     JSON файл при этом должен иметь определенную структуру
     [
         // Запись в моделе
         {
@@ -50,15 +49,15 @@
             ...
         },
         ...
     ]
     """
 
     id_field = None
-    u"""Имя поля, значение которого будет являться идентификатором записи.
+    """Имя поля, значение которого будет являться идентификатором записи.
 
     Копируется в поле ``id``.
     """
 
     # В потомках данные заполняются вызовом
     # _load_enum_values("my-catalog.json")
     data = None
@@ -77,30 +76,29 @@
     def _get_ids(cls):
         for record in cls.data:
             if cls.id_field is not None:
                 record['id'] = record[cls.id_field]
             yield record
 
     def __init__(self, params):
-        u"""Инициализация объекта модели.
+        """Инициализация объекта модели.
 
         :param dict params: Данные объекта модели.
         """
         super(BaseCatalogVirtualModel, self).__init__()
         for param in params:
             setattr(self, param, params[param])
 
     def __str__(self):
-        u"""Строковое представление записи в виртуальной модели."""
+        """Строковое представление записи в виртуальной модели."""
         raise NotImplementedError
 
 
-class ProductSpecific(object):
-
-    u"""Интерфейс для продукто-зависимых перечислений.
+class ProductSpecific:
+    """Интерфейс для продукто-зависимых перечислений.
 
     Предоставляет возможность выбора специально заданных
     значений из справочника для конкретного продукта.
     Для этого, при инциализации проекта, необходимо выполнить:
         EduProgramKind.set_category(EduProgramKind.WEBEDU_CODES),
     в этом случае пользователи увидят не весь справочник обр.программ по УФТТ,
     а только программы, необходимые в школах.
@@ -115,45 +113,43 @@
     SSUZ_CODES = ()
     EXTEDU_CODES = ()
 
     current_kind = None
 
     @classmethod
     def set_category(cls, list_codes):
-        u"""Активация одной из категорий."""
+        """Активация одной из категорий."""
         cls.current_kind = tuple(list_codes)
 
 
 class BaseEnumerateProductSpecific(BaseEnumerate, ProductSpecific):
-
-    u"""BaseEnumerate c ProductSpecific возможностями."""
+    """BaseEnumerate c ProductSpecific возможностями."""
 
     @classmethod
     def set_category(cls, list_codes):
-        u"""Активация одной из категорий."""
+        """Активация одной из категорий."""
         assert all(code in cls.values for code in list_codes), (
-            u'Все значения list_codes должны содержаться в values класса'
+            'Все значения list_codes должны содержаться в values класса'
         )
         super(BaseEnumerateProductSpecific, cls).set_category(list_codes)
 
     @classmethod
     def get_choices(cls):
-        u"""Возвращает заданные для конкретных продуктов значения."""
+        """Возвращает заданные для конкретных продуктов значения."""
         codes = cls.current_kind or cls.values
 
         return [
             (k, v)
-            for k, v in six.iteritems(cls.values)
+            for k, v in cls.values.items()
             if k in codes
         ]
 
 
 class BaseModelView(ProductSpecific):
-
-    u"""Базовый класс для перечисления на основе виртуальной модели.
+    """Базовый класс для перечисления на основе виртуальной модели.
 
     Перечисления необходимы для создании полей модели ссылающихся
     на справочник, а также для сторов UI компонент.
     При переопределении необходимо указать
     model - модель, наследник BaseCatalogVirtualModel
     value_field - поле, выступающее в качестве значения
     display_field - поле для отображения
@@ -166,15 +162,15 @@
     value_field = None
 
     # Поле для отображения
     display_field = None
 
     @classmethod
     def get_choices(cls):
-        u"""Отображаем данные для выбора.
+        """Отображаем данные для выбора.
 
         :return: [(value_field, display_field), ...]
         """
         codes = cls.current_kind or [
             rec[cls.value_field]
             for rec in cls.model.data]
```

### Comparing `educommon-2.20.0/src/educommon/contingent/catalogs.py` & `educommon-3.0.0/src/educommon/contingent/catalogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,85 +1,87 @@
-# coding: utf-8
 # pylint: disable=no-init
-u"""Реализации справочников и моделей контингента."""
-from __future__ import absolute_import
-
-from collections import namedtuple
-
-from m3.db import BaseEnumerate
-from six import python_2_unicode_compatible
-
-from .base import BaseCatalogVirtualModel
-from .base import BaseEnumerateProductSpecific
-from .base import BaseModelView
-from .base import load_values
+"""Реализации справочников и моделей контингента."""
+from collections import (
+    namedtuple,
+)
+
+from m3.db import (
+    BaseEnumerate,
+)
+
+from educommon.contingent.base import (
+    BaseCatalogVirtualModel,
+    BaseEnumerateProductSpecific,
+    BaseModelView,
+    load_values,
+)
 
 
 class Okfs(BaseEnumerate):
-    u"""Справочник ОКФС."""
+    """Справочник ОКФС."""
 
     values = {
-        11: u"Государственная собственность",
-        49: u"Иная смешанная российская собственность",
-        20: u"Иностранная собственность",
-        14: u"Муниципальная собственность",
-        10: u"Российская собственность",
-        27: u"Смешанная иностранная собственность",
-        17: u"Смешанная российская собственность",
-        40: u"Смешанная российская собственность с долей "
-            u"государственной собственности",
-        42: u"Смешанная российская собственность с долей собственности "
-            u"субъектов Российской Федерации",
-        41: u"Смешанная российская собственность с долей федеральной "
-            u"собственности",
-        43: u"Смешанная российская собственность с долями федеральной "
-            u"собственности и собственности субъектов Российской Федерации",
-        50: u"Собственность благотворительных организаций",
-        61: u"Собственность государственных корпораций",
-        22: u"Собственность иностранных государств",
-        24: u"Собственность иностранных граждан и лиц без гражданства",
-        23: u"Собственность иностранных юридических лиц",
-        21: u"Собственность международных организаций",
-        15: u"Собственность общественных и религиозных "
-            u"организаций (объединений)",
-        53: u"Собственность общественных объединений",
-        51: u"Собственность политических общественных объединений",
-        19: u"Собственность потребительской кооперации",
-        52: u"Собственность профессиональных союзов",
-        54: u"Собственность религиозных объединений",
-        18: u"Собственность российских граждан, постоянно "
-            u"проживающих за границей",
-        13: u"Собственность субъектов Российской Федерации",
-        33: u"Совместная муниципальная и иностранная собственность",
-        30: u"Совместная российская и иностранная собственность",
-        35: u"Совместная собственность общественных и религиозных "
-            u"организаций (объединений) и  иностранная собственность",
-        32: u"Совместная собственность субъектов Российской Федерации "
-            u"и иностранная собственность",
-        31: u"Совместная федеральная и иностранная собственность",
-        34: u"Совместная частная и иностранная собственность",
-        12: u"Федеральная собственность",
-        16: u"Частная собственность"
+        11: "Государственная собственность",
+        49: "Иная смешанная российская собственность",
+        20: "Иностранная собственность",
+        14: "Муниципальная собственность",
+        10: "Российская собственность",
+        27: "Смешанная иностранная собственность",
+        17: "Смешанная российская собственность",
+        40: "Смешанная российская собственность с долей "
+            "государственной собственности",
+        42: "Смешанная российская собственность с долей собственности "
+            "субъектов Российской Федерации",
+        41: "Смешанная российская собственность с долей федеральной "
+            "собственности",
+        43: "Смешанная российская собственность с долями федеральной "
+            "собственности и собственности субъектов Российской Федерации",
+        50: "Собственность благотворительных организаций",
+        61: "Собственность государственных корпораций",
+        22: "Собственность иностранных государств",
+        24: "Собственность иностранных граждан и лиц без гражданства",
+        23: "Собственность иностранных юридических лиц",
+        21: "Собственность международных организаций",
+        15: "Собственность общественных и религиозных "
+            "организаций (объединений)",
+        53: "Собственность общественных объединений",
+        51: "Собственность политических общественных объединений",
+        19: "Собственность потребительской кооперации",
+        52: "Собственность профессиональных союзов",
+        54: "Собственность религиозных объединений",
+        18: "Собственность российских граждан, постоянно "
+            "проживающих за границей",
+        13: "Собственность субъектов Российской Федерации",
+        33: "Совместная муниципальная и иностранная собственность",
+        30: "Совместная российская и иностранная собственность",
+        35: "Совместная собственность общественных и религиозных "
+            "организаций (объединений) и  иностранная собственность",
+        32: "Совместная собственность субъектов Российской Федерации "
+            "и иностранная собственность",
+        31: "Совместная федеральная и иностранная собственность",
+        34: "Совместная частная и иностранная собственность",
+        12: "Федеральная собственность",
+        16: "Частная собственность"
     }
 
 
 class Citizenship(BaseEnumerate):
-    u"""Гражданство."""
+    """Гражданство."""
 
     RF_CITIZEN = 1
     DOUBLE_CITIZEN = 2
     EXTERNAL_CITIZEN = 3
     WITHOUT_CITIZEN = 4
 
     values = {
-        RF_CITIZEN: u"Гражданин Российской Федерации",
-        DOUBLE_CITIZEN: u"Гражданин Российской Федерации и "
-                        u"иностранного государства (двойное гражданство)",
-        EXTERNAL_CITIZEN: u"Иностранный гражданин",
-        WITHOUT_CITIZEN: u"Лицо без гражданства"
+        RF_CITIZEN: "Гражданин Российской Федерации",
+        DOUBLE_CITIZEN: "Гражданин Российской Федерации и "
+                        "иностранного государства (двойное гражданство)",
+        EXTERNAL_CITIZEN: "Иностранный гражданин",
+        WITHOUT_CITIZEN: "Лицо без гражданства"
     }
 
     # соотнесение значений из КО с тем, как представлено гражданство в РИС
     # основной справочник, в `values`, не соответствует тому, что
     #   указано в confluence по этому полю:
     # https://conf.bars.group/pages/viewpage.action?pageId=15292952 п. 2.1.6
     values_received_from_contingent = {
@@ -87,32 +89,32 @@
         1: EXTERNAL_CITIZEN,
         2: WITHOUT_CITIZEN,
         3: DOUBLE_CITIZEN
     }
 
 
 class PhysicalCultureGroups(BaseEnumerate):
-    u"""Физкультурные группы."""
+    """Физкультурные группы."""
 
     MAIN = 21
     PREPARATORY = 22
     SPECIAL_A = 23
     SPECIAL_B = 24
 
     values = {
-        MAIN: u"Основная",
-        PREPARATORY: u"Подготовительная",
-        SPECIAL_A: u"Специальная А",
-        SPECIAL_B: u"Специальная Б"
+        MAIN: "Основная",
+        PREPARATORY: "Подготовительная",
+        SPECIAL_A: "Специальная А",
+        SPECIAL_B: "Специальная Б"
 
     }
 
 
 class HealthGroups(BaseEnumerate):
-    u"""Справочник "Группы здоровья"."""
+    """Справочник "Группы здоровья"."""
 
     HEALTHY = 11
     SLIGHT_DEVIATIONS = 12
     CHRONIC_DISEASES_AND_WELLNESS = 13
     CHRONIC_DISEASES_AND_POOR_HEALTH = 14
     CHRONIC_DISEASE_AND_OBSERVED = 15
 
@@ -131,168 +133,168 @@
     AFTER_18_YEAR_CODES = [
         FIRST_GROUP_18_YEARS_OLD,
         SECOND_GROUP_18_YEARS_OLD,
         THIRD_GROUP_18_YEARS_OLD
     ]
 
     values = {
-        HEALTHY: u"Группа 1 - здоровые",
-        SLIGHT_DEVIATIONS: u"Группа 2 - с незначительными отклонениями",
-        CHRONIC_DISEASES_AND_WELLNESS: u"Группа 3 - с хроническими "
-                                       u"заболеваниями и хорошим "
-                                       u"самочувствием, либо с временными "
-                                       u"отклонениями в состоянии здоровья",
-        CHRONIC_DISEASES_AND_POOR_HEALTH: u"Группа 4 - с хроническими "
-                                          u"заболеваниями и плохим "
-                                          u"самочувствием",
-        CHRONIC_DISEASE_AND_OBSERVED: u"Группа 5 - с хроническими "
-                                      u"заболеваниями и "
-                                      u"наблюдаются в специальных лечебницах",
-        FIRST_GROUP_18_YEARS_OLD: u'Группа 1 (18 лет и старше)',
-        SECOND_GROUP_18_YEARS_OLD: u'Группа 2 (18 лет и старше)',
-        THIRD_GROUP_18_YEARS_OLD: u'Группа 3 (18 лет и старше)',
+        HEALTHY: "Группа 1 - здоровые",
+        SLIGHT_DEVIATIONS: "Группа 2 - с незначительными отклонениями",
+        CHRONIC_DISEASES_AND_WELLNESS: "Группа 3 - с хроническими "
+                                       "заболеваниями и хорошим "
+                                       "самочувствием, либо с временными "
+                                       "отклонениями в состоянии здоровья",
+        CHRONIC_DISEASES_AND_POOR_HEALTH: "Группа 4 - с хроническими "
+                                          "заболеваниями и плохим "
+                                          "самочувствием",
+        CHRONIC_DISEASE_AND_OBSERVED: "Группа 5 - с хроническими "
+                                      "заболеваниями и "
+                                      "наблюдаются в специальных лечебницах",
+        FIRST_GROUP_18_YEARS_OLD: 'Группа 1 (18 лет и старше)',
+        SECOND_GROUP_18_YEARS_OLD: 'Группа 2 (18 лет и старше)',
+        THIRD_GROUP_18_YEARS_OLD: 'Группа 3 (18 лет и старше)',
     }
 
 
 class DisabilityGroups(BaseEnumerate):
-    u"""Группы инвалидности."""
+    """Группы инвалидности."""
 
     FIRST_GROUP = 11
     SECOND_GROUP = 12
     THIRD_GROUP = 13
     DISABLED_CHILD = 14
 
     values = {
-        FIRST_GROUP: u"Первая группа",
-        SECOND_GROUP: u"Вторая группа",
-        THIRD_GROUP: u"Третья группа",
-        DISABLED_CHILD: u"Ребенок-инвалид (для лиц до 18 лет)"
+        FIRST_GROUP: "Первая группа",
+        SECOND_GROUP: "Вторая группа",
+        THIRD_GROUP: "Третья группа",
+        DISABLED_CHILD: "Ребенок-инвалид (для лиц до 18 лет)"
     }
 
 
 class CertainCategoriesOfDisability(BaseEnumerate):
-    u"""Отдельные категории инвалидности."""
+    """Отдельные категории инвалидности."""
 
     DISABLED_SINCE_CHILDHOOD = 21
     ARMY_INVALID = 22
 
     values = {
-        DISABLED_SINCE_CHILDHOOD: u"Инвалид с детства",
-        ARMY_INVALID: u"Инвалид вследствие военной травмы или заболевания, "
-                      u"полученного в период прохождения военной службы"
+        DISABLED_SINCE_CHILDHOOD: "Инвалид с детства",
+        ARMY_INVALID: "Инвалид вследствие военной травмы или заболевания, "
+                      "полученного в период прохождения военной службы"
     }
 
 
 class OrganizationKindByFounder(BaseEnumerate):
-    u"""Вид организации по учредителю."""
+    """Вид организации по учредителю."""
 
     RF = 1
     RF_SUBJECT = 2
     MO = 3
     RF_COMMERCIAL_ORGANIZATION = 4
     EXTERNAL_COMMERCIAL_ORGANIZATION = 5
     RF_NON_COMMERCIAL_ORGANIZATION = 6
     EXTERNAL_NON_COMMERCIAL_ORGANIZATION = 7
     RF_RELIGION_ORGANIZATION = 8
     EXTERNAL_RELIGION_ORGANIZATION = 9
     RF_CITIZENSHIP = 10
     EXTERNAL_CITIZENSHIP = 11
 
     values = {
-        RF: u"Российская Федерация",
-        RF_SUBJECT: u"Субъект Российской Федерации",
-        MO: u"Муниципальное образование",
-        RF_COMMERCIAL_ORGANIZATION: u"Российские коммерческие организации",
-        EXTERNAL_COMMERCIAL_ORGANIZATION: u"Иностранные коммерческие "
-                                          u"организации",
-        RF_NON_COMMERCIAL_ORGANIZATION: u"Российские некоммерческие "
-                                        u"организации",
-        EXTERNAL_NON_COMMERCIAL_ORGANIZATION: u"Иностранные некоммерческие "
-                                              u"организации",
-        RF_RELIGION_ORGANIZATION: u"Российские религиозные организации",
-        EXTERNAL_RELIGION_ORGANIZATION: u"Иностранные религиозные "
-                                        u"организации",
-        RF_CITIZENSHIP: u"Граждане Российской Федерации",
-        EXTERNAL_CITIZENSHIP: u"Иностранные граждане"
+        RF: "Российская Федерация",
+        RF_SUBJECT: "Субъект Российской Федерации",
+        MO: "Муниципальное образование",
+        RF_COMMERCIAL_ORGANIZATION: "Российские коммерческие организации",
+        EXTERNAL_COMMERCIAL_ORGANIZATION: "Иностранные коммерческие "
+                                          "организации",
+        RF_NON_COMMERCIAL_ORGANIZATION: "Российские некоммерческие "
+                                        "организации",
+        EXTERNAL_NON_COMMERCIAL_ORGANIZATION: "Иностранные некоммерческие "
+                                              "организации",
+        RF_RELIGION_ORGANIZATION: "Российские религиозные организации",
+        EXTERNAL_RELIGION_ORGANIZATION: "Иностранные религиозные "
+                                        "организации",
+        RF_CITIZENSHIP: "Граждане Российской Федерации",
+        EXTERNAL_CITIZENSHIP: "Иностранные граждане"
     }
 
 
 class OrganizationStatus(BaseEnumerate):
-    u"""Статусы организаций."""
+    """Статусы организаций."""
 
     FUNCTIONS = 1
     CAPITAL_REPAIRS = 2
     RECONSTRUCTION = 3
     ACTIVITY_STOPPED = 4
     CONTINGENT_MISSING = 5
     PENDING_THE_OPENING = 6
     LIQUIDATED = 7
     CLOSED = 8
     JOINED_OTHER_ORGANIZATIONS = 9
 
     values = {
-        FUNCTIONS: u"Функционирует",
-        CAPITAL_REPAIRS: u"Капитальный ремонт",
-        RECONSTRUCTION: u"Реконструкция",
-        ACTIVITY_STOPPED: u"Деятельность приостановлена",
-        CONTINGENT_MISSING: u"Контингент отсутствует",
-        PENDING_THE_OPENING: u"Ожидает открытия",
-        LIQUIDATED: u"Ликвидирована",
-        CLOSED: u"Закрыта",
-        JOINED_OTHER_ORGANIZATIONS: u"Присоединена к другой организации"
+        FUNCTIONS: "Функционирует",
+        CAPITAL_REPAIRS: "Капитальный ремонт",
+        RECONSTRUCTION: "Реконструкция",
+        ACTIVITY_STOPPED: "Деятельность приостановлена",
+        CONTINGENT_MISSING: "Контингент отсутствует",
+        PENDING_THE_OPENING: "Ожидает открытия",
+        LIQUIDATED: "Ликвидирована",
+        CLOSED: "Закрыта",
+        JOINED_OTHER_ORGANIZATIONS: "Присоединена к другой организации"
     }
 
 
 class EduProgramKind(BaseEnumerateProductSpecific):
-    u"""
+    """
     Справочник образовательных программ.
 
     Содержит все виды обр.программ по УФТТ
     """
 
     JUNIOR_COMMON = 12
     DEFAULT_COMMON = 13
     MIDDLE_COMMON = 14
 
     values = {
-        1: u"Основная общеобразовательная программа",
-        11: u"Образовательная программа дошкольного образования",
+        1: "Основная общеобразовательная программа",
+        11: "Образовательная программа дошкольного образования",
         JUNIOR_COMMON: (
-            u"Образовательная программа начального общего образования"
+            "Образовательная программа начального общего образования"
         ),
         DEFAULT_COMMON: (
-            u"Образовательная программа основного общего образования"
+            "Образовательная программа основного общего образования"
         ),
         MIDDLE_COMMON: (
-            u"Образовательная программа среднего общего образования"
+            "Образовательная программа среднего общего образования"
         ),
-        15: u"Адаптированная основная общеобразовательная программа",
-        2: u"Основная профессиональная образовательная программа",
-        21: u"Образовательная программа среднего профессионального"
-            u" образования",
-        211: u"Программа подготовки квалифицированных рабочих, служащих",
-        212: u"Программа подготовки специалистов среднего звена",
-        23: u"Образовательная программа, адаптированная для обучения лиц"
-            u" с ограниченными возможностями здоровья",
-        3: u"Основная программа профессионального обучения",
-        31: u"Программа профессиональной подготовки по профессиям рабочих,"
-            u" должностям служащих",
-        32: u"Программа переподготовки рабочих, служащих,",
-        33: u"Программа повышения квалификации рабочих, служащих.",
-        4: u"Дополнительная образовательная программа",
-        41: u"Дополнительная общеобразовательная программа",
-        411: u"Дополнительная общеразвивающая программа",
-        412: u"Дополнительная предпрофессиональная программа",
-        42: u"Дополнительная профессиональная программа",
-        421: u"Программа повышения квалификации",
-        422: u"Программа профессиональной переподготовки",
-        5: u"Адаптированная образовательная программа",
-        51: u"Адаптированная основная общеобразовательная программа",
-        52: u"Образовательная программа, адаптированная для обучения лиц с"
-            u" ограниченными возможностями здоровья",
+        15: "Адаптированная основная общеобразовательная программа",
+        2: "Основная профессиональная образовательная программа",
+        21: "Образовательная программа среднего профессионального"
+            " образования",
+        211: "Программа подготовки квалифицированных рабочих, служащих",
+        212: "Программа подготовки специалистов среднего звена",
+        23: "Образовательная программа, адаптированная для обучения лиц"
+            " с ограниченными возможностями здоровья",
+        3: "Основная программа профессионального обучения",
+        31: "Программа профессиональной подготовки по профессиям рабочих,"
+            " должностям служащих",
+        32: "Программа переподготовки рабочих, служащих,",
+        33: "Программа повышения квалификации рабочих, служащих.",
+        4: "Дополнительная образовательная программа",
+        41: "Дополнительная общеобразовательная программа",
+        411: "Дополнительная общеразвивающая программа",
+        412: "Дополнительная предпрофессиональная программа",
+        42: "Дополнительная профессиональная программа",
+        421: "Программа повышения квалификации",
+        422: "Программа профессиональной переподготовки",
+        5: "Адаптированная образовательная программа",
+        51: "Адаптированная основная общеобразовательная программа",
+        52: "Образовательная программа, адаптированная для обучения лиц с"
+            " ограниченными возможностями здоровья",
     }
 
     # коды, соответствующие видам обр.программ в Электронной Школе
     WEBEDU_CODES = (
         1, 11, 12, 13, 14, 15, 211, 212, 4, 41, 411, 412
     )
 
@@ -303,29 +305,29 @@
     SSUZ_CODES = (211, 212)
 
     # коды, соответствующие видам обр.программ в Электронном Доп.образовании
     EXTEDU_CODES = ()
 
 
 class EduDocumentOnEducationTypes(BaseEnumerate):
-    u"""Справочник 'Типы документов об образовании'."""
+    """Справочник 'Типы документов об образовании'."""
 
     values = {
-        11: u'Аттестат о среднем общем образовании',
-        12: u'Аттестат об основном общем образовании',
-        4: u'Справка об обучении',
-        41: u'Свидетельство об обучении для лиц с ограниченными возможностями '
-            u'здоровья (с различными формами умственной отсталости)',
-        6: u'Другой документ об образовании',
-        7: u'Другой документ об обучении'
+        11: 'Аттестат о среднем общем образовании',
+        12: 'Аттестат об основном общем образовании',
+        4: 'Справка об обучении',
+        41: 'Свидетельство об обучении для лиц с ограниченными возможностями '
+            'здоровья (с различными формами умственной отсталости)',
+        6: 'Другой документ об образовании',
+        7: 'Другой документ об обучении'
     }
 
 
 class DifficultSituations(BaseEnumerateProductSpecific):
-    u"""Трудные жизненные ситуации."""
+    """Трудные жизненные ситуации."""
 
     DISABILITY = 2
     LIMITED_ABILITIES = 3
     DEAF = 301
     BLINDLY = 302
     MUTE = 303
     IMMOBILIZE = 304
@@ -334,53 +336,53 @@
     AUTISTIC = 307
     IMPAIRED_MENTAL = 308
     MENTAL_ILLNESS = 309
     NERVOUS_SYSTEM_DISEASE = 310
     COMPLEX_DEFECTS = 311
 
     values = {
-        101: u"Дети, оставшиеся без попечения родителей "
-             u"по причине смерти родителей",
-        102: u"Дети, оставшиеся без попечения родителей "
-             u"по причине лишения родителей родительских прав",
-        103: u"Дети, оставшиеся без попечения родителей по "
-             u"причине ограничения родителей в родительских правах",
-        104: u"Дети, оставшиеся без попечения родителей по "
-             u"причине признания родителей недееспособными",
-        105: u"Дети, оставшиеся без попечения родителей по "
-             u"причине болезни родителей",
-        106: u"Дети, оставшиеся без попечения родителей по "
-             u"причине длительного отсутствия родителей",
-        DISABILITY: u"Дети-инвалиды",
-        LIMITED_ABILITIES: u"Дети с ограниченными возможностями здоровья",
-        DEAF: u"Дети с нарушениями слуха",
-        BLINDLY: u"Дети с нарушениями зрения",
-        MUTE: u"Дети с тяжелыми нарушениями речи",
-        IMMOBILIZE: u"Дети с нарушением опорно-двигательного аппарата",
-        PARALYSIS: u"Дети с детским церебральным параличом",
-        INTELLIGENT_VIOLATION: u"Дети с интеллектуальными нарушениями",
-        AUTISTIC: u"Дети с расстройством аутистического спектра",
-        IMPAIRED_MENTAL: u"Дети с задержкой психического развития",
-        MENTAL_ILLNESS: u"Дети с психическими заболеваниями",
-        NERVOUS_SYSTEM_DISEASE: u"Дети с заболеваниями нервной системы",
-        COMPLEX_DEFECTS: u"Дети со сложной структурой дефекта",
-        4: u"Дети - жертвы вооруженных и межнациональных конфликтов, "
-           u"экологических и техногенных катастроф, стихийных бедствий",
-        5: u"Дети - жертвы экологических и техногенных катастроф, "
-           u"стихийных бедствий",
-        6: u"Дети из семей беженцев и вынужденных переселенцев",
-        7: u"Дети, оказавшиеся в экстремальных условиях",
-        8: u"Дети - жертвы насилия",
-        9: u"Дети, отбывающие наказание в виде лишения "
-           u"свободы в воспитательных колониях",
-        10: u"Дети, с девиантным (общественно опасным) поведением",
-        11: u"Дети, проживающие в малоимущих семьях",
-        12: u"Дети с отклонениями в поведении",
-        13: u"Дети, жизнедеятельность которых объективно "
-            u"нарушена в результате сложившихся обстоятельств"
+        101: "Дети, оставшиеся без попечения родителей "
+             "по причине смерти родителей",
+        102: "Дети, оставшиеся без попечения родителей "
+             "по причине лишения родителей родительских прав",
+        103: "Дети, оставшиеся без попечения родителей по "
+             "причине ограничения родителей в родительских правах",
+        104: "Дети, оставшиеся без попечения родителей по "
+             "причине признания родителей недееспособными",
+        105: "Дети, оставшиеся без попечения родителей по "
+             "причине болезни родителей",
+        106: "Дети, оставшиеся без попечения родителей по "
+             "причине длительного отсутствия родителей",
+        DISABILITY: "Дети-инвалиды",
+        LIMITED_ABILITIES: "Дети с ограниченными возможностями здоровья",
+        DEAF: "Дети с нарушениями слуха",
+        BLINDLY: "Дети с нарушениями зрения",
+        MUTE: "Дети с тяжелыми нарушениями речи",
+        IMMOBILIZE: "Дети с нарушением опорно-двигательного аппарата",
+        PARALYSIS: "Дети с детским церебральным параличом",
+        INTELLIGENT_VIOLATION: "Дети с интеллектуальными нарушениями",
+        AUTISTIC: "Дети с расстройством аутистического спектра",
+        IMPAIRED_MENTAL: "Дети с задержкой психического развития",
+        MENTAL_ILLNESS: "Дети с психическими заболеваниями",
+        NERVOUS_SYSTEM_DISEASE: "Дети с заболеваниями нервной системы",
+        COMPLEX_DEFECTS: "Дети со сложной структурой дефекта",
+        4: "Дети - жертвы вооруженных и межнациональных конфликтов, "
+           "экологических и техногенных катастроф, стихийных бедствий",
+        5: "Дети - жертвы экологических и техногенных катастроф, "
+           "стихийных бедствий",
+        6: "Дети из семей беженцев и вынужденных переселенцев",
+        7: "Дети, оказавшиеся в экстремальных условиях",
+        8: "Дети - жертвы насилия",
+        9: "Дети, отбывающие наказание в виде лишения "
+           "свободы в воспитательных колониях",
+        10: "Дети, с девиантным (общественно опасным) поведением",
+        11: "Дети, проживающие в малоимущих семьях",
+        12: "Дети с отклонениями в поведении",
+        13: "Дети, жизнедеятельность которых объективно "
+            "нарушена в результате сложившихся обстоятельств"
     }
     # коды, соответствующие типам законного представителя в
     # Электронном Детском Саду
     KINDER_CODES = tuple(
         code
         for code in values
         if code != 9
@@ -399,35 +401,35 @@
         MENTAL_ILLNESS,
         NERVOUS_SYSTEM_DISEASE,
         COMPLEX_DEFECTS,
     )
 
 
 class LegalDelegateTypes(BaseEnumerateProductSpecific):
-    u"""Тип законного представителя."""
+    """Тип законного представителя."""
 
     PARENT = 1
     CURATOR = 2
     TRUSTEE = 3
     AGENCY_OF_TRUSTEE = 4
     ADOPTIVE_PARENT = 5
     EDUCATION_AGENCY_LEADER = 6
     LEGAL_REPRESENTATIVE = 7
 
     values = {
-        PARENT: u"Родитель",
-        CURATOR: u"Опекун",
-        TRUSTEE: u"Попечитель",
-        AGENCY_OF_TRUSTEE: u"Орган опеки и попечительства",
-        ADOPTIVE_PARENT: u"Приемный родитель",
-        EDUCATION_AGENCY_LEADER: u"Руководитель воспитательного, лечебного и "
-                                 u"иного учреждения, в котором ребенок "
-                                 u"находится на полном "
-                                 u"государственном обеспечении",
-        LEGAL_REPRESENTATIVE: u"Законный представитель"
+        PARENT: "Родитель",
+        CURATOR: "Опекун",
+        TRUSTEE: "Попечитель",
+        AGENCY_OF_TRUSTEE: "Орган опеки и попечительства",
+        ADOPTIVE_PARENT: "Приемный родитель",
+        EDUCATION_AGENCY_LEADER: "Руководитель воспитательного, лечебного и "
+                                 "иного учреждения, в котором ребенок "
+                                 "находится на полном "
+                                 "государственном обеспечении",
+        LEGAL_REPRESENTATIVE: "Законный представитель"
     }
 
     # коды, соответствующие типам законного представителя в Электронной Школе
     WEBEDU_CODES = ()
 
     # коды, соответствующие типам законного представителя в
     # Электронном Детском Саду
@@ -438,32 +440,31 @@
     SSUZ_CODES = (1, 2, 3, 4, 5, 6)
 
     # коды, соответствующие типам законного представителя в
     # Электронном Доп.образовании
     EXTEDU_CODES = ()
 
 
-@python_2_unicode_compatible
 class OkoguVirtualModel(BaseCatalogVirtualModel):
-    u"""Виртуальная модель справочника ОКОГУ."""
+    """Виртуальная модель справочника ОКОГУ."""
 
     id_field = 'code'
 
     data = load_values("okogu.json")
 
     def __str__(self):
-        u"""Строковое представление записи в виртуальной модели."""
+        """Строковое представление записи в виртуальной модели."""
         return self.full_name
 
     class Meta:
-        verbose_name = u'ОКОГУ'
+        verbose_name = 'ОКОГУ'
 
 
 class Okogu(BaseModelView):
-    u"""
+    """
     Справочник ОКОГУ.
 
     ОКОГУ - Общероссийский классификатор органов государственной власти и
     управления.
     """
 
     model = OkoguVirtualModel
@@ -476,210 +477,209 @@
                     '3300500', '3500000', '3500100',
                     '3500200', '3500300', '3500400',
                     '3500500', '4210007', '4210008',
                     '4210009', '4210014', '4210015')
 
 
 class Okopf(BaseEnumerateProductSpecific):
-    u"""Справочник ОКОПФ."""
+    """Справочник ОКОПФ."""
 
     values = {
-        "1 00 00": u"ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ЮРИДИЧЕСКИХ ЛИЦ, "
-                   u"ЯВЛЯЮЩИХСЯ КОММЕРЧЕСКИМИ КОРПОРАТИВНЫМИ ОРГАНИЗАЦИЯМИ",
-        "1 10 00": u"Хозяйственные товарищества",
-        "1 10 51": u"Полные товарищества",
-        "1 10 64": u"Товарищества на вере (коммандитные товарищества)",
-        "1 20 00": u"Хозяйственные общества",
-        "1 22 00": u"Акционерные общества",
-        "1 22 47": u"Публичные акционерные общества",
-        "1 22 67": u"Непубличные акционерные общества",
-        "1 23 00": u"Общества с ограниченной ответственностью",
-        "1 30 00": u"Хозяйственные партнерства",
-        "1 40 00": u"Производственные кооперативы (артели)",
-        "1 41 00": u"Сельскохозяйственные производственные кооперативы",
-        "1 41 53": u"Сельскохозяйственные артели (колхозы)",
-        "1 41 54": u"Рыболовецкие артели (колхозы)",
-        "1 41 55": u"Кооперативные хозяйства (коопхозы)",
-        "1 42 00": u"Производственные кооперативы "
-                   u"(кроме сельскохозяйственных "
-                   u"производственных кооперативов)",
-        "1 53 00": u"Крестьянские (фермерские) хозяйства",
-        "1 90 00": u"Прочие юридические лица, являющиеся "
-                   u"коммерческими организациями",
-        "2 00 00": u"ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ЮРИДИЧЕСКИХ ЛИЦ, "
-                   u"ЯВЛЯЮЩИХСЯ НЕКОММЕРЧЕСКИМИ КОРПОРАТИВНЫМИ ОРГАНИЗАЦИЯМИ",
-        "2 01 00": u"Потребительские кооперативы",
-        "2 01 01": u"Гаражные и гаражно-строительные кооперативы",
-        "2 01 02": u"Жилищные или жилищно-строительные кооперативы",
-        "2 01 03": u"Жилищные накопительные кооперативы",
-        "2 01 04": u"Кредитные потребительские кооперативы",
-        "2 01 05": u"Кредитные потребительские кооперативы граждан",
-        "2 01 06": u"Кредитные кооперативы второго уровня",
-        "2 01 07": u"Потребительские общества",
-        "2 01 08": u"Общества взаимного страхования",
-        "2 01 09": u"Сельскохозяйственные потребительские "
-                   u"перерабатывающие кооперативы",
-        "2 01 10": u"Сельскохозяйственные потребительские "
-                   u"сбытовые (торговые) кооперативы",
-        "2 01 11": u"Сельскохозяйственные потребительские "
-                   u"обслуживающие кооперативы",
-        "2 01 12": u"Сельскохозяйственные потребительские "
-                   u"снабженческие кооперативы",
-        "2 01 13": u"Сельскохозяйственные потребительские "
-                   u"садоводческие кооперативы",
-        "2 01 14": u"Сельскохозяйственные потребительские "
-                   u"огороднические кооперативы",
-        "2 01 15": u"Сельскохозяйственные потребительские "
-                   u"животноводческие кооперативы",
-        "2 01 20": u"Садоводческие, огороднические или дачные "
-                   u"потребительские кооперативы",
-        "2 01 21": u"Фонды проката",
-        "2 02 00": u"Общественные организации",
-        "2 02 01": u"Политические партии",
-        "2 02 02": u"Профсоюзные организации",
-        "2 02 10": u"Общественные движения",
-        "2 02 11": u"Органы общественной самодеятельности",
-        "2 02 17": u"Территориальные общественные самоуправления",
-        "2 06 00": u"Ассоциации (союзы)",
-        "2 06 01": u"Ассоциации (союзы) экономического взаимодействия "
-                   u"субъектов Российской Федерации",
-        "2 06 03": u"Советы муниципальных образований "
-                   u"субъектов Российской Федерации",
-        "2 06 04": u"Союзы (ассоциации) кредитных кооперативов",
-        "2 06 05": u"Союзы (ассоциации) кооперативов",
-        "2 06 06": u"Союзы (ассоциации) общественных объединений",
-        "2 06 07": u"Союзы (ассоциации) общин малочисленных народов",
-        "2 06 08": u"Союзы потребительских обществ",
-        "2 06 09": u"Адвокатские палаты",
-        "2 06 10": u"Нотариальные палаты",
-        "2 06 11": u"Торгово-промышленные палаты",
-        "2 06 12": u"Объединения работодателей",
-        "2 06 13": u"Объединения фермерских хозяйств",
-        "2 06 14": u"Некоммерческие партнерства",
-        "2 06 15": u"Адвокатские бюро",
-        "2 06 16": u"Коллегии адвокатов",
-        "2 06 17": u"Садоводческие, огороднические или "
-                   u"дачные некоммерческие партнерства",
-        "2 06 18": u"Ассоциации (союзы) садоводческих, огороднических и "
-                   u"дачных некоммерческих объединений",
-        "2 06 19": u"Саморегулируемые организации",
-        "2 06 20": u"Объединения (ассоциации и союзы) "
-                   u"благотворительных организаций",
-        "2 07 00": u"Товарищества собственников недвижимости",
-        "2 07 01": u"Садоводческие, огороднические или дачные "
-                   u"некоммерческие товарищества",
-        "2 07 16": u"Товарищества собственников жилья",
-        "2 11 00": u"Казачьи общества, внесенные в государственный "
-                   u"реестр казачьих обществ в Российской Федерации",
-        "2 12 00": u"Общины коренных малочисленных народов "
-                   u"Российской Федерации",
-        "3 00 00": u"ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ОРГАНИЗАЦИЙ, "
-                   u"СОЗДАННЫХ БЕЗ ПРАВ ЮРИДИЧЕСКОГО ЛИЦА",
-        "3 00 01": u"Представительства юридических лиц",
-        "3 00 02": u"Филиалы юридических лиц",
-        "3 00 03": u"Обособленные подразделения юридических лиц",
-        "3 00 04": u"Структурные подразделения обособленных "
-                   u"подразделений юридических лиц",
-        "3 00 05": u"Паевые инвестиционные фонды",
-        "3 00 06": u"Простые товарищества",
-        "3 00 08": u"Районные суды, городские суды, "
-                   u"межрайонные суды (районные суды)",
-        "4 00 00": u"ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ "
-                   u"МЕЖДУНАРОДНЫХ ОРГАНИЗАЦИЙ, ОСУЩЕСТВЛЯЮЩИХ ДЕЯТЕЛЬНОСТЬ "
-                   u"НА ТЕРРИТОРИИ РОССИЙСКОЙ ФЕДЕРАЦИИ",
-        "4 00 01": u"Межправительственные международные организации",
-        "4 00 02": u"Неправительственные международные организации",
-        "5 00 00": u"ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ДЛЯ ДЕЯТЕЛЬНОСТИ "
-                   u"ГРАЖДАН (ФИЗИЧЕСКИХ ЛИЦ)",
-        "5 01 00": u"Организационно-правовые формы для коммерческой "
-                   u"деятельности граждан",
-        "5 01 01": u"Главы крестьянских (фермерских) хозяйств",
-        "5 01 02": u"Индивидуальные предприниматели",
-        "5 02 00": u"Организационно-правовые формы для деятельности граждан, "
-                   u"не отнесенной к предпринимательству",
-        "5 02 01": u"Адвокаты, учредившие адвокатский кабинет",
-        "5 02 02": u"Нотариусы, занимающиеся частной практикой",
-        "6 00 00": u"ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ЮРИДИЧЕСКИХ ЛИЦ, "
-                   u"ЯВЛЯЮЩИХСЯ КОММЕРЧЕСКИМИ УНИТАРНЫМИ ОРГАНИЗАЦИЯМИ",
-        "6 50 00": u"Унитарные предприятия",
-        "6 51 00": u"Унитарные предприятия, основанные на праве оперативного "
-                   u"управления (казенные предприятия)",
-        "6 51 41": u"Федеральные казенные предприятия",
-        "6 51 42": u"Казенные предприятия субъектов Российской Федерации",
-        "6 51 43": u"Муниципальные казенные предприятия",
-        "6 52 00": u"Унитарные предприятия, основанные на "
-                   u"праве хозяйственного ведения",
-        "6 52 41": u"Федеральные государственные унитарные предприятия",
-        "6 52 42": u"Государственные унитарные предприятия субъектов "
-                   u"Российской Федерации",
-        "6 52 43": u"Муниципальные унитарные предприятия",
-        "7 00 00": u"ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ЮРИДИЧЕСКИХ ЛИЦ, "
-                   u"ЯВЛЯЮЩИХСЯ НЕКОММЕРЧЕСКИМИ УНИТАРНЫМИ ОРГАНИЗАЦИЯМИ",
-        "7 04 00": u"Фонды",
-        "7 04 01": u"Благотворительные фонды",
-        "7 04 02": u"Негосударственные пенсионные фонды",
-        "7 04 03": u"Общественные фонды",
-        "7 04 04": u"Экологические фонды",
-        "7 14 00": u"Автономные некоммерческие организации",
-        "7 15 00": u"Религиозные организации",
-        "7 16 00": u"Публично-правовые компании",
-        "7 16 01": u"Государственные корпорации",
-        "7 16 02": u"Государственные компании",
-        "7 16 10": u"Отделения иностранных некоммерческих "
-                   u"неправительственных организаций",
-        "7 50 00": u"Учреждения",
-        "7 51 00": u"Учреждения, созданные Российской Федерацией",
-        "7 51 01": u"Федеральные государственные автономные учреждения",
-        "7 51 03": u"Федеральные государственные бюджетные учреждения",
-        "7 51 04": u"Федеральные государственные казенные учреждения",
-        "7 52 00": u"Учреждения, созданные субъектами Российской Федерации",
-        "7 52 01": u"Государственные автономные учреждения "
-                   u"субъектов Российской Федерации",
-        "7 52 03": u"Государственные бюджетные учреждения субъектов "
-                   u"Российской Федерации",
-        "7 52 04": u"Государственные казенные учреждения субъектов "
-                   u"Российской Федерации",
-        "7 53 00": u"Государственные академии наук",
-        "7 54 00": u"Учреждения, созданные муниципальными образованиями",
-        "7 54 01": u"Муниципальные автономные учреждения",
-        "7 54 03": u"Муниципальные бюджетные учреждения",
-        "7 54 04": u"Муниципальные казенные учреждения",
-        "7 55 00": u"Частные учреждения",
-        "7 55 02": u"Благотворительные учреждения",
-        "7 55 05": u"Общественные учреждения"
+        "1 00 00": "ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ЮРИДИЧЕСКИХ ЛИЦ, "
+                   "ЯВЛЯЮЩИХСЯ КОММЕРЧЕСКИМИ КОРПОРАТИВНЫМИ ОРГАНИЗАЦИЯМИ",
+        "1 10 00": "Хозяйственные товарищества",
+        "1 10 51": "Полные товарищества",
+        "1 10 64": "Товарищества на вере (коммандитные товарищества)",
+        "1 20 00": "Хозяйственные общества",
+        "1 22 00": "Акционерные общества",
+        "1 22 47": "Публичные акционерные общества",
+        "1 22 67": "Непубличные акционерные общества",
+        "1 23 00": "Общества с ограниченной ответственностью",
+        "1 30 00": "Хозяйственные партнерства",
+        "1 40 00": "Производственные кооперативы (артели)",
+        "1 41 00": "Сельскохозяйственные производственные кооперативы",
+        "1 41 53": "Сельскохозяйственные артели (колхозы)",
+        "1 41 54": "Рыболовецкие артели (колхозы)",
+        "1 41 55": "Кооперативные хозяйства (коопхозы)",
+        "1 42 00": "Производственные кооперативы "
+                   "(кроме сельскохозяйственных "
+                   "производственных кооперативов)",
+        "1 53 00": "Крестьянские (фермерские) хозяйства",
+        "1 90 00": "Прочие юридические лица, являющиеся "
+                   "коммерческими организациями",
+        "2 00 00": "ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ЮРИДИЧЕСКИХ ЛИЦ, "
+                   "ЯВЛЯЮЩИХСЯ НЕКОММЕРЧЕСКИМИ КОРПОРАТИВНЫМИ ОРГАНИЗАЦИЯМИ",
+        "2 01 00": "Потребительские кооперативы",
+        "2 01 01": "Гаражные и гаражно-строительные кооперативы",
+        "2 01 02": "Жилищные или жилищно-строительные кооперативы",
+        "2 01 03": "Жилищные накопительные кооперативы",
+        "2 01 04": "Кредитные потребительские кооперативы",
+        "2 01 05": "Кредитные потребительские кооперативы граждан",
+        "2 01 06": "Кредитные кооперативы второго уровня",
+        "2 01 07": "Потребительские общества",
+        "2 01 08": "Общества взаимного страхования",
+        "2 01 09": "Сельскохозяйственные потребительские "
+                   "перерабатывающие кооперативы",
+        "2 01 10": "Сельскохозяйственные потребительские "
+                   "сбытовые (торговые) кооперативы",
+        "2 01 11": "Сельскохозяйственные потребительские "
+                   "обслуживающие кооперативы",
+        "2 01 12": "Сельскохозяйственные потребительские "
+                   "снабженческие кооперативы",
+        "2 01 13": "Сельскохозяйственные потребительские "
+                   "садоводческие кооперативы",
+        "2 01 14": "Сельскохозяйственные потребительские "
+                   "огороднические кооперативы",
+        "2 01 15": "Сельскохозяйственные потребительские "
+                   "животноводческие кооперативы",
+        "2 01 20": "Садоводческие, огороднические или дачные "
+                   "потребительские кооперативы",
+        "2 01 21": "Фонды проката",
+        "2 02 00": "Общественные организации",
+        "2 02 01": "Политические партии",
+        "2 02 02": "Профсоюзные организации",
+        "2 02 10": "Общественные движения",
+        "2 02 11": "Органы общественной самодеятельности",
+        "2 02 17": "Территориальные общественные самоуправления",
+        "2 06 00": "Ассоциации (союзы)",
+        "2 06 01": "Ассоциации (союзы) экономического взаимодействия "
+                   "субъектов Российской Федерации",
+        "2 06 03": "Советы муниципальных образований "
+                   "субъектов Российской Федерации",
+        "2 06 04": "Союзы (ассоциации) кредитных кооперативов",
+        "2 06 05": "Союзы (ассоциации) кооперативов",
+        "2 06 06": "Союзы (ассоциации) общественных объединений",
+        "2 06 07": "Союзы (ассоциации) общин малочисленных народов",
+        "2 06 08": "Союзы потребительских обществ",
+        "2 06 09": "Адвокатские палаты",
+        "2 06 10": "Нотариальные палаты",
+        "2 06 11": "Торгово-промышленные палаты",
+        "2 06 12": "Объединения работодателей",
+        "2 06 13": "Объединения фермерских хозяйств",
+        "2 06 14": "Некоммерческие партнерства",
+        "2 06 15": "Адвокатские бюро",
+        "2 06 16": "Коллегии адвокатов",
+        "2 06 17": "Садоводческие, огороднические или "
+                   "дачные некоммерческие партнерства",
+        "2 06 18": "Ассоциации (союзы) садоводческих, огороднических и "
+                   "дачных некоммерческих объединений",
+        "2 06 19": "Саморегулируемые организации",
+        "2 06 20": "Объединения (ассоциации и союзы) "
+                   "благотворительных организаций",
+        "2 07 00": "Товарищества собственников недвижимости",
+        "2 07 01": "Садоводческие, огороднические или дачные "
+                   "некоммерческие товарищества",
+        "2 07 16": "Товарищества собственников жилья",
+        "2 11 00": "Казачьи общества, внесенные в государственный "
+                   "реестр казачьих обществ в Российской Федерации",
+        "2 12 00": "Общины коренных малочисленных народов "
+                   "Российской Федерации",
+        "3 00 00": "ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ОРГАНИЗАЦИЙ, "
+                   "СОЗДАННЫХ БЕЗ ПРАВ ЮРИДИЧЕСКОГО ЛИЦА",
+        "3 00 01": "Представительства юридических лиц",
+        "3 00 02": "Филиалы юридических лиц",
+        "3 00 03": "Обособленные подразделения юридических лиц",
+        "3 00 04": "Структурные подразделения обособленных "
+                   "подразделений юридических лиц",
+        "3 00 05": "Паевые инвестиционные фонды",
+        "3 00 06": "Простые товарищества",
+        "3 00 08": "Районные суды, городские суды, "
+                   "межрайонные суды (районные суды)",
+        "4 00 00": "ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ "
+                   "МЕЖДУНАРОДНЫХ ОРГАНИЗАЦИЙ, ОСУЩЕСТВЛЯЮЩИХ ДЕЯТЕЛЬНОСТЬ "
+                   "НА ТЕРРИТОРИИ РОССИЙСКОЙ ФЕДЕРАЦИИ",
+        "4 00 01": "Межправительственные международные организации",
+        "4 00 02": "Неправительственные международные организации",
+        "5 00 00": "ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ДЛЯ ДЕЯТЕЛЬНОСТИ "
+                   "ГРАЖДАН (ФИЗИЧЕСКИХ ЛИЦ)",
+        "5 01 00": "Организационно-правовые формы для коммерческой "
+                   "деятельности граждан",
+        "5 01 01": "Главы крестьянских (фермерских) хозяйств",
+        "5 01 02": "Индивидуальные предприниматели",
+        "5 02 00": "Организационно-правовые формы для деятельности граждан, "
+                   "не отнесенной к предпринимательству",
+        "5 02 01": "Адвокаты, учредившие адвокатский кабинет",
+        "5 02 02": "Нотариусы, занимающиеся частной практикой",
+        "6 00 00": "ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ЮРИДИЧЕСКИХ ЛИЦ, "
+                   "ЯВЛЯЮЩИХСЯ КОММЕРЧЕСКИМИ УНИТАРНЫМИ ОРГАНИЗАЦИЯМИ",
+        "6 50 00": "Унитарные предприятия",
+        "6 51 00": "Унитарные предприятия, основанные на праве оперативного "
+                   "управления (казенные предприятия)",
+        "6 51 41": "Федеральные казенные предприятия",
+        "6 51 42": "Казенные предприятия субъектов Российской Федерации",
+        "6 51 43": "Муниципальные казенные предприятия",
+        "6 52 00": "Унитарные предприятия, основанные на "
+                   "праве хозяйственного ведения",
+        "6 52 41": "Федеральные государственные унитарные предприятия",
+        "6 52 42": "Государственные унитарные предприятия субъектов "
+                   "Российской Федерации",
+        "6 52 43": "Муниципальные унитарные предприятия",
+        "7 00 00": "ОРГАНИЗАЦИОННО-ПРАВОВЫЕ ФОРМЫ ЮРИДИЧЕСКИХ ЛИЦ, "
+                   "ЯВЛЯЮЩИХСЯ НЕКОММЕРЧЕСКИМИ УНИТАРНЫМИ ОРГАНИЗАЦИЯМИ",
+        "7 04 00": "Фонды",
+        "7 04 01": "Благотворительные фонды",
+        "7 04 02": "Негосударственные пенсионные фонды",
+        "7 04 03": "Общественные фонды",
+        "7 04 04": "Экологические фонды",
+        "7 14 00": "Автономные некоммерческие организации",
+        "7 15 00": "Религиозные организации",
+        "7 16 00": "Публично-правовые компании",
+        "7 16 01": "Государственные корпорации",
+        "7 16 02": "Государственные компании",
+        "7 16 10": "Отделения иностранных некоммерческих "
+                   "неправительственных организаций",
+        "7 50 00": "Учреждения",
+        "7 51 00": "Учреждения, созданные Российской Федерацией",
+        "7 51 01": "Федеральные государственные автономные учреждения",
+        "7 51 03": "Федеральные государственные бюджетные учреждения",
+        "7 51 04": "Федеральные государственные казенные учреждения",
+        "7 52 00": "Учреждения, созданные субъектами Российской Федерации",
+        "7 52 01": "Государственные автономные учреждения "
+                   "субъектов Российской Федерации",
+        "7 52 03": "Государственные бюджетные учреждения субъектов "
+                   "Российской Федерации",
+        "7 52 04": "Государственные казенные учреждения субъектов "
+                   "Российской Федерации",
+        "7 53 00": "Государственные академии наук",
+        "7 54 00": "Учреждения, созданные муниципальными образованиями",
+        "7 54 01": "Муниципальные автономные учреждения",
+        "7 54 03": "Муниципальные бюджетные учреждения",
+        "7 54 04": "Муниципальные казенные учреждения",
+        "7 55 00": "Частные учреждения",
+        "7 55 02": "Благотворительные учреждения",
+        "7 55 05": "Общественные учреждения"
     }
     # коды, соответствующие типам законного представителя в
     # Электронном Детском Саду
     KINDER_CODES = ('3 00 02', '5 01 02', '7 50 00',
                     '7 51 00', '7 51 01', '7 51 03',
                     '7 51 04', '7 52 00', '7 52 01',
                     '7 52 03', '7 52 04', '7 54 00',
                     '7 54 01', '7 54 03', '7 54 04',
                     '7 55 00', '7 55 05')
 
 
 class DocumentConfirmingTypes(BaseEnumerate):
-    u"""Справочник "Тип документа, подтверждающего права" """
+    """Справочник "Тип документа, подтверждающего права" """
 
     ADOPTION = 401
     BIRTH_CERT = 402
     TRUSTEE = 403
     OTHER_DOC = 499
 
     values = {
-        ADOPTION: u'Решение суда об установлении усыновления',
-        BIRTH_CERT: u'Свидетельство о рождении',
-        TRUSTEE: u'Назначение органом опеки опекуна',
-        OTHER_DOC: u'Другой документ, подтверждающий представительство',
+        ADOPTION: 'Решение суда об установлении усыновления',
+        BIRTH_CERT: 'Свидетельство о рождении',
+        TRUSTEE: 'Назначение органом опеки опекуна',
+        OTHER_DOC: 'Другой документ, подтверждающий представительство',
     }
 
 
 class IdentityDocumentsTypes(BaseEnumerate):
-
-    u"""Справочник "Типы документов удостоверяющих личность".
+    """Справочник "Типы документов удостоверяющих личность".
 
     Ключи, это id из таблицы certificate,
     из которой перенесены данные в этот справочник.
 
     Значения это кортежи в которых, первое значение это значение по ключу,
     а второе (не обязательное), код УФТТ.
     """
@@ -715,154 +715,154 @@
     # типы документов, которые могут не иметь серии
     SERIESLESS_DOCS = (3, 4, 6, 15, 18, 19, 20, 21, 24, 25, 26, 27, 28)
 
     Value = namedtuple('Value', ['value', 'uftt_code'])
 
     values = {
         BIRTH_CERT: Value(
-            u'Свидетельство о рождении', 11
+            'Свидетельство о рождении', 11
         ),
         PASSPORT: Value(
-            u'Паспорт гражданина РФ', 12
+            'Паспорт гражданина РФ', 12
         ),
         DOC: Value(
-            u'Другой документ, удостоверяющий личность', 4
+            'Другой документ, удостоверяющий личность', 4
         ),
         TEMP_CARD_IDENT_RF: Value(
-            u'Временное удостоверение личности гражданина РФ', 17
+            'Временное удостоверение личности гражданина РФ', 17
         ),
         PASSPORT_ALIEN: Value(
-            u'Паспорт иностранного гражданина', 21
+            'Паспорт иностранного гражданина', 21
         ),
         FOREIGN_PASSPORT: Value(
-            u'Загранпаспорт гражданина РФ', 13
+            'Загранпаспорт гражданина РФ', 13
         ),
         ARMY_TICK: Value(
-            u'Военный билет', 15
+            'Военный билет', 15
         ),
         DIP_PASS_RF: Value(
-            u'Дипломатический паспорт гражданина Российской Федерации', None
+            'Дипломатический паспорт гражданина Российской Федерации', None
         ),
         PASSPORT_USSR: Value(
-            u'Паспорт гражданина СССР', 4
+            'Паспорт гражданина СССР', 4
         ),
         PASSPORT_MINMOR: Value(
-            u'Паспорт Минморфлота', 4
+            'Паспорт Минморфлота', 4
         ),
         PASSPORT_NAUTA: Value(
-            u'Паспорт моряка', 4
+            'Паспорт моряка', 4
         ),
         TEMP_RF: Value(
-            u'Разрешение на временное проживание в Российской Федерации', 28
+            'Разрешение на временное проживание в Российской Федерации', 28
         ),
         REFUGEE_RF: Value(
-            u'Свидетельство о рассмотрении ходатайства о признании  беженцем '
-            u'на территории Российской Федерации', 29
+            'Свидетельство о рассмотрении ходатайства о признании  беженцем '
+            'на территории Российской Федерации', 29
         ),
         BIRTH_CERT_INTR: Value(
-            u'Свидетельство о рождении, выданное уполномоченным органом '
-            u'иностранного государства', 31
+            'Свидетельство о рождении, выданное уполномоченным органом '
+            'иностранного государства', 31
         ),
         FROM_PRISON: Value(
-            u'Справка об освобождении из места лишения свободы', 4
+            'Справка об освобождении из места лишения свободы', 4
         ),
         REFUGEE: Value(
-            u'Удостоверение личности лица, признанного беженцем', 24
+            'Удостоверение личности лица, признанного беженцем', 24
         ),
         OFFICER: Value(
-            u'Удостоверение личности офицера', 4
+            'Удостоверение личности офицера', 4
         ),
         MILLITARY_RF: Value(
-            u'Удостоверение личности военнослужащего РФ', 14
+            'Удостоверение личности военнослужащего РФ', 14
         ),
         TEMP_MILLITARY: Value(
-            u'Временное удостоверение, выданное взамен военного билета', 16
+            'Временное удостоверение, выданное взамен военного билета', 16
         ),
         WITHOUT_CITIZEN_RF: Value(
-            u'Удостоверение личности лица без гражданства в РФ', 22
+            'Удостоверение личности лица без гражданства в РФ', 22
         ),
         DOC_CITIZEN_RF: Value(
-            u'Удостоверение личности отдельных категорий лиц, находящихся на '
-            u'территории РФ, подавших заявление о признании гражданами РФ или '
-            u'о приеме в гражданство РФ', 23
+            'Удостоверение личности отдельных категорий лиц, находящихся на '
+            'территории РФ, подавших заявление о признании гражданами РФ или '
+            'о приеме в гражданство РФ', 23
         ),
         DOC_REFUGEE_RF: Value(
-            u'Удостоверение личности лица, ходатайствующего о признании '
-            u'беженцем на территории РФ', 25
+            'Удостоверение личности лица, ходатайствующего о признании '
+            'беженцем на территории РФ', 25
         ),
         DOC_TEMP_RF: Value(
-            u'Удостоверение личности лица, получившего временное '
-            u'убежище на территории РФ', 26),
+            'Удостоверение личности лица, получившего временное '
+            'убежище на территории РФ', 26),
         DOC_PERM_RF: Value(
-            u'Вид на жительство в Российской Федерации', 27
+            'Вид на жительство в Российской Федерации', 27
         ),
         CERTIFICATE_PERM_RF: Value(
-            u'Свидетельство о предоставлении временного убежища на территории '
-            u'Российской Федерации', 30
+            'Свидетельство о предоставлении временного убежища на территории '
+            'Российской Федерации', 30
         ),
     }
 
     @classmethod
     def get_full_items(cls):
-        u"""Возвращает все значения справочника."""
+        """Возвращает все значения справочника."""
         result = []
 
         for item in cls.get_items():
             cls.__append_to_result(item, result)
 
         return result
 
     @classmethod
     def get_uftt_items(cls):
-        u"""Возвращает значения справочника, у которых есть код УФТТ."""
+        """Возвращает значения справочника, у которых есть код УФТТ."""
         result = []
 
         for item in cls.get_items():
             if item[1].uftt_code is None:
                 continue
             cls.__append_to_result(item, result)
 
         return result
 
     @classmethod
     def get_items_without_uftt(cls):
-        u"""Возвращает значения справочника, у которых нет кода УФТТ."""
+        """Возвращает значения справочника, у которых нет кода УФТТ."""
         result = []
 
         for item in cls.get_items():
             if not item[1].uftt_code is None:
                 continue
             cls.__append_to_result(item, result)
 
         return result
 
     @classmethod
     def get_value_by_id(cls, key):
-        u"""Возвращает значение по ключу, если ключа нет возвращает None."""
+        """Возвращает значение по ключу, если ключа нет возвращает None."""
         try:
             return cls.values[key].value
         except KeyError:
             return
 
     @classmethod
     def __append_to_result(cls, item, result):
-        u"""
+        """
         Добавляет значения к результирующему списку.
 
-        :param item: tuple, например (ключ1, (u"значение", УФТТ код))
+        :param item: tuple, например (ключ1, ("значение", УФТТ код))
         :param result: [(key1, value1), (key2, value2), .. (keyN, valueN)]
         :rtype : list
         """
         key = item[0]
         value = item[1].value
         result.append((key, value))
 
 
 class AdaptationType(BaseEnumerate):
-    u"""Вид адаптированности."""
+    """Вид адаптированности."""
 
     HALF_BLIND = 201
     BLIND = 202
     HALF_DEAF = 203
     DEAF = 204
     HALF_DEAF_HARD = 205
     WEAK = 206
@@ -870,53 +870,53 @@
     DELAYED = 208
     RETARDED = 209
     RETARDED_HARD = 210
     OTHER = 211
     AUTISTIC_DISORDER = 212
 
     values = {
-        HALF_BLIND: u"для слабовидящих обучающихся",
-        BLIND: u"для слепых обучающихся",
-        HALF_DEAF: u"для слабослышащих",
-        DEAF: u"для глухих",
+        HALF_BLIND: "для слабовидящих обучающихся",
+        BLIND: "для слепых обучающихся",
+        HALF_DEAF: "для слабослышащих",
+        DEAF: "для глухих",
         HALF_DEAF_HARD:
-            u"для слабослышащих обучающихся, имеющих сложную структуру "
-            u"дефекта (нарушение слуха и задержка психического развития)",
+            "для слабослышащих обучающихся, имеющих сложную структуру "
+            "дефекта (нарушение слуха и задержка психического развития)",
         WEAK:
-            u"для обучающихся, имеющих нарушения опорно-двигательного "
-            u"аппарата",
-        SPEECH_PATHOLOGY: u"для обучающихся, имеющих тяжелые нарушения речи",
-        DELAYED: u"для обучающихся с задержкой психического развития",
-        RETARDED: u"для обучающихся с умственной отсталостью",
+            "для обучающихся, имеющих нарушения опорно-двигательного "
+            "аппарата",
+        SPEECH_PATHOLOGY: "для обучающихся, имеющих тяжелые нарушения речи",
+        DELAYED: "для обучающихся с задержкой психического развития",
+        RETARDED: "для обучающихся с умственной отсталостью",
         RETARDED_HARD:
-            u"для обучающихся с умственной отсталостью, имеющих сложную "
-            u"структуру дефекта",
-        OTHER: u"для обучающихся с иными ограничениями здоровья",
+            "для обучающихся с умственной отсталостью, имеющих сложную "
+            "структуру дефекта",
+        OTHER: "для обучающихся с иными ограничениями здоровья",
         AUTISTIC_DISORDER:
-            u"для обучающихся с расстройствами аутистического спектра",
+            "для обучающихся с расстройствами аутистического спектра",
     }
 
 
 class TypeTrainingLongTermTreatment(BaseEnumerate):
-    u"""Справочник "Виды обучения при длительном лечении"."""
+    """Справочник "Виды обучения при длительном лечении"."""
 
     IS_HOME_STUDY = 1
     IS_MED_ORG_STUDY = 2
     IS_HEALING_ORG_STUDY = 3
 
     values = {
-        IS_HOME_STUDY: u'Обучение на дому',
-        IS_MED_ORG_STUDY: u'Обучение в медицинской организации',
-        IS_HEALING_ORG_STUDY: u'Обучение в организации, осуществляющей '
-                              u'лечение, оздоровление и (или) отдых',
+        IS_HOME_STUDY: 'Обучение на дому',
+        IS_MED_ORG_STUDY: 'Обучение в медицинской организации',
+        IS_HEALING_ORG_STUDY: 'Обучение в организации, осуществляющей '
+                              'лечение, оздоровление и (или) отдых',
     }
 
 
 class EducationOrganization(BaseEnumerateProductSpecific):
-    u"""Образовательная организация."""
+    """Образовательная организация."""
 
     PROFESSIONAL_ORGANIZATION_CODE = 14
     EDUCATION_ORGANIZATION_CODE = 1
     INDIVIDUAL_BUSINESS = 3
     FOR_THE_DEAF = 1301
     FOR_THE_HEARING_IMPAIRED = 1302
     FOR_LATE_DEAFENED = 1303
@@ -926,199 +926,196 @@
     WITH_DISORDERS_OF_MS = 1307
     WITH_MENTAL_RETARDATION = 1308
     WITH_AUTISM_DISORDERS = 1310
     WITH_SEVERE_DEFECTS = 1311
     FOR_OTHERS_WITH_DISORDERS = 1312
 
     values = {
-        EDUCATION_ORGANIZATION_CODE: u"Образовательная организация",
-        11: u"Дошкольная образовательная организация",
-        12: u"Общеобразовательная организация",
-        13: u"ОО, с деятельностью по адаптированным программам",
+        EDUCATION_ORGANIZATION_CODE: "Образовательная организация",
+        11: "Дошкольная образовательная организация",
+        12: "Общеобразовательная организация",
+        13: "ОО, с деятельностью по адаптированным программам",
         FOR_THE_DEAF: (
-            u"ОО, с деятельностью по адаптированным программам (для глухих)"),
+            "ОО, с деятельностью по адаптированным программам (для глухих)"),
         FOR_THE_HEARING_IMPAIRED: (
-            u"ОО, с деятельностью по адаптированным программам "
-            u"(для слабослышащих)"),
+            "ОО, с деятельностью по адаптированным программам "
+            "(для слабослышащих)"),
         FOR_LATE_DEAFENED: (
-            u"ОО, с деятельностью по адаптированным программам "
-            u"(для позднооглохших)"),
+            "ОО, с деятельностью по адаптированным программам "
+            "(для позднооглохших)"),
         FOR_THE_BLIND: (
-            u"ОО, с деятельностью по адаптированным программам (для слепых)"),
+            "ОО, с деятельностью по адаптированным программам (для слепых)"),
         FOR_THE_VISUALLY_IMPAIRED: (
-            u"ОО, с деятельностью по адаптированным программам "
-            u"(для слабовидящих)"),
+            "ОО, с деятельностью по адаптированным программам "
+            "(для слабовидящих)"),
         WITH_SEVERE_SPEECH_DISORDERS: (
-            u"ОО, с деятельностью по адаптированным "
-            u"программам (с тяжелыми нарушениями речи)"),
+            "ОО, с деятельностью по адаптированным "
+            "программам (с тяжелыми нарушениями речи)"),
         WITH_DISORDERS_OF_MS: (
-            u"ОО, с деятельностью по адаптированным программам "
-            u"(с нарушениями опорно-двигательного аппарата)"),
+            "ОО, с деятельностью по адаптированным программам "
+            "(с нарушениями опорно-двигательного аппарата)"),
         WITH_MENTAL_RETARDATION: (
-            u"ОО, с деятельностью по адаптированным"
-            u" программам (с задержкой психического развития)"),
-        1309: u"ОО, с деятельностью по адаптированным"
-              u" программам (с умственной отсталостью)",
+            "ОО, с деятельностью по адаптированным"
+            " программам (с задержкой психического развития)"),
+        1309: "ОО, с деятельностью по адаптированным"
+              " программам (с умственной отсталостью)",
         WITH_AUTISM_DISORDERS: (
-            u"ОО, с деятельностью по адаптированным"
-            u" программам (с расстройствами аутистического спектра)"),
-        WITH_SEVERE_DEFECTS: u"ОО, с деятельностью по адаптированным"
-                             u" программам (со сложными дефектами)",
+            "ОО, с деятельностью по адаптированным"
+            " программам (с расстройствами аутистического спектра)"),
+        WITH_SEVERE_DEFECTS: "ОО, с деятельностью по адаптированным"
+                             " программам (со сложными дефектами)",
         FOR_OTHERS_WITH_DISORDERS: (
-            u"ОО, с деятельностью по адаптированным программам "
-            u"(для других обучающихся с ОВЗ)"),
-        PROFESSIONAL_ORGANIZATION_CODE: u"Профессиональная образовательная"
-                                        u" организация",
-        15: u"Образовательная организация высшего образования",
-        16: u"Организация дополнительного образования",
-        17: u"Организация дополнительного профессионального образования",
-        2: u"Организация, осуществляющая обучение",
-        21: u"Научная организация",
-        22: u"Центр психолого-педагогической, "
-            u"медицинской и социальной помощи",
-        23: u"Организация для детей-сирот и детей, "
-            u"оставшихся без попечения родителей",
-        24: u"Организация, осуществляющая лечение, "
-            u"оздоровление и (или) отдых",
-        25: u"Организация, осуществляющая социальное обслуживание",
-        26: u"Дипломатическое представительство РФ",
-        27: u"Консульское учреждение РФ",
-        28: u"Представительство РФ при международных"
-            u" (межгосударственных, межправительственных) организациях",
-        29: u"Иные юридические лица",
-        INDIVIDUAL_BUSINESS: u"Индивидуальный предприниматель, "
-                             u"осуществляющий образовательную деятельность"
+            "ОО, с деятельностью по адаптированным программам "
+            "(для других обучающихся с ОВЗ)"),
+        PROFESSIONAL_ORGANIZATION_CODE: "Профессиональная образовательная"
+                                        " организация",
+        15: "Образовательная организация высшего образования",
+        16: "Организация дополнительного образования",
+        17: "Организация дополнительного профессионального образования",
+        2: "Организация, осуществляющая обучение",
+        21: "Научная организация",
+        22: "Центр психолого-педагогической, "
+            "медицинской и социальной помощи",
+        23: "Организация для детей-сирот и детей, "
+            "оставшихся без попечения родителей",
+        24: "Организация, осуществляющая лечение, "
+            "оздоровление и (или) отдых",
+        25: "Организация, осуществляющая социальное обслуживание",
+        26: "Дипломатическое представительство РФ",
+        27: "Консульское учреждение РФ",
+        28: "Представительство РФ при международных"
+            " (межгосударственных, межправительственных) организациях",
+        29: "Иные юридические лица",
+        INDIVIDUAL_BUSINESS: "Индивидуальный предприниматель, "
+                             "осуществляющий образовательную деятельность"
     }
     # коды, соответствующие типам законного представителя в Электронной Школе
     WEBEDU_CODES = (
         1, 2, 3, 12, 13,
         23, 24, 25, 26, 27, 28, 29,
         1301, 1302, 1303, 1304, 1305, 1306,
         1307, 1308, 1309, 1310, 1311, 1312
     )
 
     SSUZ_CODES = (14, 3)
 
 
-@python_2_unicode_compatible
 class OksmVirtialModel(BaseCatalogVirtualModel):
-
-    u"""Виртуальная модель справочника ОКСМ."""
+    """Виртуальная модель справочника ОКСМ."""
 
     rf_code = "643"
 
     id_field = 'code'
     data = load_values("oksm.json")
 
     fields_to_serialize = ['id', 'shortname']
 
     def __str__(self):
-        u"""Строковое представление записи в виртуальной модели."""
+        """Строковое представление записи в виртуальной модели."""
         return self.shortname
 
     class Meta:
-        verbose_name = u'ОКСМ'
+        verbose_name = 'ОКСМ'
 
 
 class Oksm(BaseModelView):
-    u"""
+    """
     Справочник ОКСМ.
 
     ОКСМ - Общероссийский классификатор стран мира.
     """
 
     model = OksmVirtialModel
     value_field = "code"
     display_field = "shortname"
 
 
 class CrippleGroups(BaseEnumerate):
-    u"""Справочник "Группы инвалидности"."""
+    """Справочник "Группы инвалидности"."""
 
     FIRST_GROUP = 11
     SECOND_GROUP = 12
     THIRD_GROUP = 13
     DISABLED_CHILD_GROUP = 14
 
     values = {
-        FIRST_GROUP: u'1 группа',
-        SECOND_GROUP: u'2 группа',
-        THIRD_GROUP: u'3 группа',
-        DISABLED_CHILD_GROUP: u'Ребенок-инвалид',
+        FIRST_GROUP: '1 группа',
+        SECOND_GROUP: '2 группа',
+        THIRD_GROUP: '3 группа',
+        DISABLED_CHILD_GROUP: 'Ребенок-инвалид',
     }
 
 
 class CrippleCategories(BaseEnumerate):
-    u"""Справочник "Категории инвалидности"."""
+    """Справочник "Категории инвалидности"."""
 
     values = {
-        21: u'Инвалид с детства',
-        22: u'Инвалид вследствие военной травмы или заболевания, '
-            u'полученного в период прохождения военной службы',
+        21: 'Инвалид с детства',
+        22: 'Инвалид вследствие военной травмы или заболевания, '
+            'полученного в период прохождения военной службы',
     }
 
 
 class EducationMethods(BaseEnumerate):
-    u"""Справочник "Формы образования"."""
+    """Справочник "Формы образования"."""
 
     FULL_TIME_STUDY = 11
     CORRESPONDENCE_STUDY = 12
     FULL_TIME_AND_CORRESPONDENCE_STUDY = 13
     FAMILY_STUDY = 21
     SELF_EDUCATION_STUDY = 22
 
     values = {
-        FULL_TIME_STUDY: u'Очная',
-        CORRESPONDENCE_STUDY: u'Заочная',
-        FULL_TIME_AND_CORRESPONDENCE_STUDY: u'Очно-заочная',
-        FAMILY_STUDY: u'вне организации (семейное образование)',
-        SELF_EDUCATION_STUDY: u'вне организации (самообразование)',
+        FULL_TIME_STUDY: 'Очная',
+        CORRESPONDENCE_STUDY: 'Заочная',
+        FULL_TIME_AND_CORRESPONDENCE_STUDY: 'Очно-заочная',
+        FAMILY_STUDY: 'вне организации (семейное образование)',
+        SELF_EDUCATION_STUDY: 'вне организации (самообразование)',
     }
 
 
 class EducationTypeOVZ(BaseEnumerate):
-    u"""Справочник "Вид обучения для детей с ОВЗ"."""
+    """Справочник "Вид обучения для детей с ОВЗ"."""
 
     COMMON = 1
     SEPARATE_CLASS = 2
     SEPARATE_UNIT = 3
 
     values = {
-        COMMON: u"Совместно с другими обучающимися",
-        SEPARATE_CLASS: u"В отдельных классах, группах",
+        COMMON: "Совместно с другими обучающимися",
+        SEPARATE_CLASS: "В отдельных классах, группах",
         SEPARATE_UNIT: (
-            u"В отдельных организациях, осуществляющих "
-            u"образовательную деятельность")
+            "В отдельных организациях, осуществляющих "
+            "образовательную деятельность")
     }
 
 
 class RealizationForms(BaseEnumerateProductSpecific):
-
-    u"""Справочник "Формы реализации образовательной программы"."""
+    """Справочник "Формы реализации образовательной программы"."""
 
     NETWORK = 1
     ELECTRON = 2
     REMOTE = 3
     HOME = 4
     ELECTRON_ONLY = 5
     REMOTE_ONLY = 6
     FOREIGN_NETWORK = 7
 
     values = {
-        NETWORK: u'Сетевая форма',
-        ELECTRON: u'С применением электронного обучения',
-        REMOTE: u'С применением дистанционных образовательных технологий',
-        HOME: u'Надомная форма получения образования',
-        ELECTRON_ONLY: u'С применением исключительно электронного обучения',
+        NETWORK: 'Сетевая форма',
+        ELECTRON: 'С применением электронного обучения',
+        REMOTE: 'С применением дистанционных образовательных технологий',
+        HOME: 'Надомная форма получения образования',
+        ELECTRON_ONLY: 'С применением исключительно электронного обучения',
         REMOTE_ONLY: (
-            u'С применением исключительно дистанционных '
-            u'образовательных технологий'),
+            'С применением исключительно дистанционных '
+            'образовательных технологий'),
         FOREIGN_NETWORK: (
-            u'Сетевая форма с использованием ресурсов '
-            u'иностранных организаций'),
+            'Сетевая форма с использованием ресурсов '
+            'иностранных организаций'),
     }
 
     current_kind = (1, 2, 3, 4)
 
     # коды, соответствующие видам форм образовательных программ
     # в Электронной Школе
     WEBEDU_CODES = (1, 2, 3, 4, 5, 6)
@@ -1133,15 +1130,15 @@
 
     # коды, соответствующие видам форм образовательных программ
     # в Электронном Доп.образовании
     EXTEDU_CODES = (1, 2, 3, 4)
 
 
 class DismissalReasons(BaseEnumerate):
-    u"""Справочник "Причины увольнения"."""
+    """Справочник "Причины увольнения"."""
 
     TRANSFER_TO_ORG = 1
     TRANSFER_TO_IND = 2
     DISMISS = 3
     PENSION = 4
     REDUCTION = 5
     AGREEMENT_END = 6
@@ -1149,20 +1146,20 @@
     RELOCATION = 8
     HEALTH = 9
     WILL = 10
     ARMY = 11
     EDUCATION = 12
 
     values = {
-        TRANSFER_TO_ORG: u'Перевод в другую образовательную организацию',
-        TRANSFER_TO_IND: u'Перевод в другую отрасль',
-        DISMISS: u'Уволен по решению суда, за прогул, за нарушение дисциплины',
-        PENSION: u'Уход на пенсию',
-        REDUCTION: u'Сокращение штатов',
-        AGREEMENT_END: u'Прекращение договора',
-        DEATH: u'Смерть',
-        RELOCATION: u'Смена места жительства',
-        HEALTH: u'По состоянию здоровья',
-        WILL: u'По собственному желанию',
-        ARMY: u'Призыв в армию',
-        EDUCATION: u'Дневное обучение',
+        TRANSFER_TO_ORG: 'Перевод в другую образовательную организацию',
+        TRANSFER_TO_IND: 'Перевод в другую отрасль',
+        DISMISS: 'Уволен по решению суда, за прогул, за нарушение дисциплины',
+        PENSION: 'Уход на пенсию',
+        REDUCTION: 'Сокращение штатов',
+        AGREEMENT_END: 'Прекращение договора',
+        DEATH: 'Смерть',
+        RELOCATION: 'Смена места жительства',
+        HEALTH: 'По состоянию здоровья',
+        WILL: 'По собственному желанию',
+        ARMY: 'Призыв в армию',
+        EDUCATION: 'Дневное обучение',
     }
```

### Comparing `educommon-2.20.0/src/educommon/contingent/contingent_plugin/actions.py` & `educommon-3.0.0/src/educommon/contingent/contingent_plugin/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from objectpack.actions import ObjectPack
-
-from .models import ContingentModelChanged
+from objectpack.actions import (
+    ObjectPack,
+)
+
+from educommon.contingent.contingent_plugin.models import (
+    ContingentModelChanged,
+)
 
 
 class ContingentModelChangedPack(ObjectPack):
 
-    title = u'Измененные объекты контингента'
+    title = 'Измененные объекты контингента'
     model = ContingentModelChanged
 
     columns = [
         {
             'data_index': 'content_type',
-            'header': u'Тип'
+            'header': 'Тип'
         },
         {
             'data_index': 'content_object',
-            'header': u'Объект'
+            'header': 'Объект'
         }
     ]
 
     def extend_menu(self, menu):
         return menu.SubMenu(
-            u'Администрирование', menu.Item(
+            'Администрирование', menu.Item(
                 self.title, self.list_window_action
             )
         )
```

### Comparing `educommon-2.20.0/src/educommon/contingent/contingent_plugin/apps.py` & `educommon-3.0.0/src/educommon/contingent/contingent_plugin/apps.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-# coding: utf-8
-from __future__ import unicode_literals
-
-from importlib import import_module
-
-from django.apps.config import AppConfig
+from importlib import (
+    import_module,
+)
+
+from django.apps.config import (
+    AppConfig,
+)
 
 
 class ContingentPluginAppConfig(AppConfig):
 
     name = __package__
 
     def _register_related_objects_views(self):
         """Добавляет представления для моделей приложения."""
-        from educommon.django.db.model_view import registries
+        from educommon.django.db.model_view import (
+            registries,
+        )
 
         model_views = import_module(self.name + '.model_views')
         registries['related_objects'].register(
             *model_views.related_model_views
         )
 
     def ready(self):
```

### Comparing `educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py` & `educommon-3.0.0/src/educommon/report/constructor/migrations/0006_reportsorting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-# coding: utf-8
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
 import django.db.models.deletion
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
-    dependencies = [
-        ('contenttypes', '0002_remove_content_type_name'),
-        ('contingent_plugin', '0001_initial'),
-    ]
+    dependencies = [('report_constructor', '0005_reportcolumn_visible'), ]
 
     operations = [
         migrations.CreateModel(
-            name='ContingentModelDeleted',
+            name='ReportSorting',
             fields=[
-                ('id',
-                 models.AutoField(auto_created=True,
-                                  primary_key=True,
-                                  serialize=False,
-                                  verbose_name='ID')),
-                ('object_id', models.PositiveIntegerField()),
-                ('data',
-                 models.TextField(verbose_name='Данные об удалённом объекте')),
-                ('content_type',
-                 models.ForeignKey(on_delete=django.db.models.deletion.CASCADE,
-                                   to='contenttypes.ContentType')),
+                ('id', models.AutoField(
+                    auto_created=True,
+                    primary_key=True,
+                    serialize=False,
+                    verbose_name='ID')),
+                ('direction', models.PositiveSmallIntegerField(
+                    choices=[(1, 'По возрастанию'), (2, 'По убыванию')],
+                    verbose_name='Направление сортировки')),
+                ('index', models.PositiveSmallIntegerField(
+                    verbose_name='Порядковый номер')),
+                ('column', models.OneToOneField(
+                    on_delete=django.db.models.deletion.CASCADE,
+                    to='report_constructor.ReportColumn',
+                    verbose_name='Колонка')),
             ],
-        ),
-        migrations.AlterUniqueTogether(
-            name='contingentmodeldeleted',
-            unique_together=set([('content_type', 'object_id')]),
-        ),
+            options={
+                'verbose_name': 'Сортировка',
+                'verbose_name_plural': 'Сортировка',
+            }, ),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/contingent/contingent_plugin/model_views.py` & `educommon-3.0.0/src/educommon/contingent/contingent_plugin/model_views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# coding: utf-8
-from __future__ import unicode_literals
-
-from educommon.django.db.model_view import AttrValue
-from educommon.django.db.model_view import HtmlTableView
-from educommon.django.db.model_view import Text
+from educommon.django.db.model_view import (
+    AttrValue,
+    HtmlTableView,
+    Text,
+)
 
 
 related_model_views = (
     HtmlTableView(
         model='contingent_plugin.ContingentModelChanged',
         description=Text('Измененная модель'),
         columns=(
```

### Comparing `educommon-2.20.0/src/educommon/contingent/contingent_plugin/models.py` & `educommon-3.0.0/src/educommon/contingent/contingent_plugin/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from django import VERSION
-from django.contrib.contenttypes.models import ContentType
-from django.db import models
-from m3_django_compat.models import GenericForeignKey
+from django import (
+    VERSION,
+)
+from django.contrib.contenttypes.models import (
+    ContentType,
+)
+from django.db import (
+    models,
+)
+from m3_django_compat.models import (
+    GenericForeignKey,
+)
 
 
 class ContingentModelChanged(models.Model):
 
-    u"""Данные об измененных моделях."""
+    """Данные об измененных моделях."""
 
     content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
     object_id = models.PositiveIntegerField()
     content_object = GenericForeignKey()
 
     class Meta:
         unique_together = ('content_type', 'object_id')
 
 
 class ContingentModelDeleted(models.Model):
-    u"""Данные об удалённых объектах моделей."""
+    """Данные об удалённых объектах моделей."""
 
     content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
     object_id = models.PositiveIntegerField()
     # В этом поле хранятся рассчитанные данные для выгрузки в КО
     # для полей удалаяемых объектов моделей в json-формате
     data = models.TextField('Данные об удалённом объекте')
 
@@ -32,20 +37,24 @@
         unique_together = ('content_type', 'object_id')
 
 
 # поскольку нам надо убедиться что миграция contingent_plugin должна
 # быть пройдена раньше чем остальные, изменяем план миграций,
 # но обязательно надо учесть зависимость самой миграции от contenttypes
 if VERSION >= (1, 10):
-    from django.db.models.signals import pre_migrate
-    from django.dispatch.dispatcher import receiver
+    from django.db.models.signals import (
+        pre_migrate,
+    )
+    from django.dispatch.dispatcher import (
+        receiver,
+    )
 
     @receiver(pre_migrate)
     def correct_migration_plan(plan, **kwargs):
-        u"""Изменяет план выполения миграций"""
+        """Изменяет план выполения миграций"""
         value = False
         index = 0
         for ind, migration_tuple in enumerate(plan):
             if (migration_tuple[0].name == '0001_initial') and (
                 migration_tuple[0].app_label == 'contingent_plugin'
             ):
                 value = migration_tuple
```

### Comparing `educommon-2.20.0/src/educommon/contingent/contingent_plugin/observer.py` & `educommon-3.0.0/src/educommon/contingent/contingent_plugin/observer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from django.core.exceptions import ObjectDoesNotExist
-from m3_django_compat import get_model
-import six
-
-from educommon.django.db.observer import ModelObserverBase
-from educommon.django.db.observer import ModelOnlyObserverMixin
-from educommon.django.db.observer import OriginalObjectMixin
-from educommon.utils.storage import AbstractInstanceStorage
+from django.core.exceptions import (
+    ObjectDoesNotExist,
+)
+from m3_django_compat import (
+    get_model,
+)
+
+from educommon.django.db.observer import (
+    ModelObserverBase,
+    ModelOnlyObserverMixin,
+    OriginalObjectMixin,
+)
+from educommon.utils.storage import (
+    AbstractInstanceStorage,
+)
 
 
 class ContingentFieldsObserver(
     OriginalObjectMixin,
     ModelObserverBase
 ):
-    u"""Фиксирует изменения в полях моделей.
+    """Фиксирует изменения в полях моделей.
 
     Ссылки на измененные объекты сохраняются в модели
     :class:`ContingentModelChanged`.
 
     .. code-block:: python
        :caption: Пример использования
 
@@ -39,16 +43,16 @@
 
         self.model_fields = model_fields
 
         # флаг проверки наличия полей в описанных моделях
         self.__checked = False
 
     def _is_model_fields_valid(self, model_fields):
-        u"""Проверяет наличие указаных полей model_fields в моделях."""
-        for (app_label, model_name), fields in six.iteritems(model_fields):
+        """Проверяет наличие указаных полей model_fields в моделях."""
+        for (app_label, model_name), fields in model_fields.items():
             model = get_model(app_label, model_name)
             for field_name in (fields(model) if callable(fields) else fields):
                 model._meta.get_field(field_name)
 
         self.__checked = True
 
         return True
@@ -57,26 +61,26 @@
         key = model._meta.app_label, model.__name__
         return key in self.model_fields
 
     def observe(self, model):
         pass
 
     def _get_field_names(self, model):
-        u"""Возвращает имена полей модели, за которыми ведется наблюдение.
+        """Возвращает имена полей модели, за которыми ведется наблюдение.
 
         :param model: Модель.
 
         :rtype: Iterable
         """
         key = model._meta.app_label, model.__name__
         fields = self.model_fields.get(key, ())
         return fields(model) if callable(fields) else fields
 
     def _has_changes(self, original, instance):
-        u"""Возвращает True, если объекты различаются.
+        """Возвращает True, если объекты различаются.
 
         :param original: Объект до изменений.
         :param instance: Объект после изменений.
 
         :rtype: bool
         """
         if original is None:
@@ -90,15 +94,15 @@
             new_value = getattr(instance, field_name, None)
             if old_value != new_value:
                 return True
 
         return False
 
     def _fix_changed_object(self, instance):
-        u"""Фиксирует наличие изменений в объекте."""
+        """Фиксирует наличие изменений в объекте."""
         ContentType = get_model('contenttypes', 'ContentType')
         content_type = ContentType.objects.get_for_model(instance)
 
         ContingentModelChanged = get_model(
             'contingent_plugin', 'ContingentModelChanged'
         )
         ContingentModelChanged.objects.get_or_create(
```

### Comparing `educommon-2.20.0/src/educommon/contingent/contingent_plugin/storage.py` & `educommon-3.0.0/src/educommon/contingent/contingent_plugin/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-# coding: utf-8
-from m3_django_compat import get_model
+from m3_django_compat import (
+    get_model,
+)
+
+from educommon.utils.storage import (
+    AbstractInstanceDataStorage,
+)
 
-from educommon.utils.storage import AbstractInstanceDataStorage
 
 ContingentModelDeleted = get_model(
     'contingent_plugin', 'ContingentModelDeleted')
 
 
 class ContingentDeletedInstancesDataStorage(
     AbstractInstanceDataStorage
```

### Comparing `educommon-2.20.0/src/educommon/contingent/contingent_plugin/utils.py` & `educommon-3.0.0/src/educommon/contingent/contingent_plugin/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,25 @@
-# coding: utf-8
 import json
-from functools import partial
-from django.contrib.contenttypes.models import ContentType
-
-from educommon.utils.caching import lru_cache
-from m3 import ApplicationLogicException
-
-from .models import ContingentModelDeleted
+from functools import (
+    partial,
+)
+
+from django.contrib.contenttypes.models import (
+    ContentType,
+)
+from m3 import (
+    ApplicationLogicException,
+)
+
+from educommon.contingent.contingent_plugin.models import (
+    ContingentModelDeleted,
+)
+from educommon.utils.caching import (
+    lru_cache,
+)
 
 
 JSON_ERROR_STRING = 'Произошла ошибка при попытке преобразования данных'
 
 
 def json_operation(json_function, obj, error_string=None):
     """Преобразует данные в соответствии с функцией json_function.
```

### Comparing `educommon-2.20.0/src/educommon/contingent/json_data/okogu.json` & `educommon-3.0.0/src/educommon/contingent/json_data/okogu.json`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/contingent/json_data/oksm.json` & `educommon-3.0.0/src/educommon/contingent/json_data/oksm.json`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/django/db/fields.py` & `educommon-3.0.0/src/educommon/django/db/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,67 @@
-# coding: utf-8
-u"""Кастомные поля моделей Django"""
-from datetime import datetime
-from datetime import timedelta
-
-from django.core import validators
-from django.db.models import fields
-from objectpack import IMaskRegexField
-
-from educommon.django.db.migration import date_difference_as_callable
-from educommon.django.db.validators import simple
-from educommon.extjs.fields import input_params
-from educommon.utils.misc import cached_property
+"""Кастомные поля моделей Django"""
+from datetime import (
+    datetime,
+    timedelta,
+)
+
+from django.core import (
+    validators,
+)
+from django.db.models import (
+    fields,
+)
+
+from objectpack import (
+    IMaskRegexField,
+)
+
+from educommon.django.db.migration import (
+    date_difference_as_callable,
+)
+from educommon.django.db.validators import (
+    simple,
+)
+from educommon.utils.misc import (
+    cached_property,
+)
 
 
 __all__ = [
-    u'SingleErrorDecimalField',
-    u'FIOField',
-    u'RangedDateField',
-    u'LastNameField',
-    u'FirstNameField',
-    u'MiddleNameField',
-    u'SNILSField',
-    u'BirthDateField',
-    u'DocumentSeriesField',
-    u'DocumentNumberField',
-    u'PassportSeriesField',
-    u'PassportNumberField',
-    u'INNField',
-    u'KPPField',
-    u'OGRNField'
+    'SingleErrorDecimalField',
+    'FIOField',
+    'RangedDateField',
+    'LastNameField',
+    'FirstNameField',
+    'MiddleNameField',
+    'SNILSField',
+    'BirthDateField',
+    'DocumentSeriesField',
+    'DocumentNumberField',
+    'PassportSeriesField',
+    'PassportNumberField',
+    'INNField',
+    'KPPField',
+    'OGRNField'
 ]
 
 
 class SingleErrorDecimalField(fields.DecimalField):
-
-    u"""
+    """
     Кастомный класс поля Decimal.
 
     Переопределяется метод validators для подключения
     SingleErrorDecimalValidator который приводит сообщение об ошибке к единому
     стилю не разделя ошибки по переполнению целой + дробной части и отдельно
     целой.
     """
 
     @cached_property
     def validators(self):
-        u"""
+        """
         Переопрелеление стандартного валидатора Decimal.
 
         :return: Список валидаторов.
         """
         validators = super(SingleErrorDecimalField, self).validators
         validators.pop()
         validators.append(
@@ -65,147 +77,152 @@
 
     default_validators = [
         simple.FIOValidator()
     ]
 
 
 class RangedDateField(fields.DateField):
-    u"""Поле, реализующее валидаторы по умолчанию для границ периода"""
+    """Поле, реализующее валидаторы по умолчанию для границ периода"""
+
     def __init__(self, minimum_date=datetime(1917, 1, 1).date(),
                  maximum_date=None, **kwargs):
         super(RangedDateField, self).__init__(**kwargs)
         self.validators.append(simple.date_range_validator(
             minimum=minimum_date, maximum=maximum_date))
 
 
 class LastNameField(FIOField):
     """Расширение поля ФИО для фамилии"""
-    def __init__(self, verbose_name=u'Фамилия', max_length=30, **kwargs):
+
+    def __init__(self, verbose_name='Фамилия', max_length=30, **kwargs):
         super(LastNameField, self).__init__(
             verbose_name=verbose_name, max_length=max_length, **kwargs)
 
 
 class FirstNameField(FIOField):
     """Расширение поля ФИО для имени"""
-    def __init__(self, verbose_name=u'Имя', max_length=30, **kwargs):
+
+    def __init__(self, verbose_name='Имя', max_length=30, **kwargs):
         super(FirstNameField, self).__init__(
             verbose_name=verbose_name, max_length=max_length, **kwargs)
 
 
 class MiddleNameField(FIOField):
     """Расширение поля ФИО для отчества"""
-    def __init__(self, verbose_name=u'Отчество',
+
+    def __init__(self, verbose_name='Отчество',
                  null=True, blank=True, max_length=30, **kwargs):
         super(MiddleNameField, self).__init__(
             verbose_name=verbose_name, null=null, blank=blank,
             max_length=max_length, **kwargs)
 
 
 class SNILSField(fields.CharField, IMaskRegexField):
+
     _mask_re = r'^[-\s\d]{0,14}$'
 
     default_validators = [
         simple.SNILSValidator()
     ]
 
     def __init__(
-        self, verbose_name=u'СНИЛС', **kwargs
+        self, verbose_name='СНИЛС', **kwargs
     ):
         kwargs.setdefault('max_length', 14)
         super(SNILSField, self).__init__(
             verbose_name=verbose_name, **kwargs)
 
 
 class BirthDateField(RangedDateField):
     def __init__(self, minimum_date=datetime(1917, 1, 1).date(),
                  maximum_date=date_difference_as_callable(timedelta(days=1)),
-                 verbose_name=u'Дата рождения', **kwargs):
+                 verbose_name='Дата рождения', **kwargs):
         super(BirthDateField, self).__init__(
             minimum_date=minimum_date, maximum_date=maximum_date,
             verbose_name=verbose_name, **kwargs)
 
 
 class DocumentSeriesField(fields.CharField, IMaskRegexField):
     _mask_re = r'^[a-zA-Zа-яА-ЯёЁ\d\s|\-|\.|\,|\\|\/]*$'
 
     default_validators = [
         simple.DocumentSeriesValidator()
     ]
 
     def __init__(
-        self, verbose_name=u'Серия документа', **kwargs
+        self, verbose_name='Серия документа', **kwargs
     ):
         super(DocumentSeriesField, self).__init__(
             verbose_name=verbose_name, **kwargs)
 
 
 class DocumentNumberField(fields.CharField, IMaskRegexField):
     _mask_re = r'^[a-zA-Zа-яА-ЯёЁ\d\s|\-|\.|\,|\\|\/]*$'
 
     default_validators = [
         simple.DocumentNumberValidator()
     ]
 
     def __init__(
-        self, verbose_name=u'Номер документа', **kwargs
+        self, verbose_name='Номер документа', **kwargs
     ):
         super(DocumentNumberField, self).__init__(
             verbose_name=verbose_name, **kwargs)
 
 
 class PassportSeriesField(DocumentSeriesField):
     _mask_re = r'^\d{0,4}$'
 
     default_validators = [
         simple.PassportSeriesValidator()
     ]
 
     def __init__(
-        self, verbose_name=u'Серия паспорта', **kwargs
+        self, verbose_name='Серия паспорта', **kwargs
     ):
         kwargs.setdefault('max_length', 4)
         super(PassportSeriesField, self).__init__(
             verbose_name=verbose_name, **kwargs)
 
 
 class PassportNumberField(DocumentNumberField):
     _mask_re = r'^\d{0,6}$'
 
     default_validators = [
         simple.PassportNumberValidator()
     ]
 
     def __init__(
-        self, verbose_name=u'Номер паспорта', **kwargs
+        self, verbose_name='Номер паспорта', **kwargs
     ):
         kwargs.setdefault('max_length', 6)
         super(PassportNumberField, self).__init__(
             verbose_name=verbose_name, **kwargs)
 
 
 class INNField(fields.CharField, IMaskRegexField):
     _mask_re = r'^\d{0,12}$'
 
     default_validators = [
         simple.inn_validator
     ]
 
-    def __init__(self, verbose_name=u'ИНН', **kwargs):
+    def __init__(self, verbose_name='ИНН', **kwargs):
         kwargs.setdefault('max_length', 12)
         super(INNField, self).__init__(verbose_name=verbose_name, **kwargs)
 
 
 class KPPField(fields.CharField, IMaskRegexField):
     _mask_re = r'^\d{0,9}$'
 
     default_validators = [
         simple.kpp_validator
     ]
 
-    def __init__(self, verbose_name=u'КПП', **kwargs):
+    def __init__(self, verbose_name='КПП', **kwargs):
         kwargs.setdefault('max_length', 9)
         super(KPPField, self).__init__(
             verbose_name=verbose_name, **kwargs)
         # из за стандартного валидатора дублируются сообщения об ошибке
         # привышения длинны поля
         try:
             self.validators.remove(
@@ -218,10 +235,10 @@
 class OGRNField(fields.CharField, IMaskRegexField):
     _mask_re = r'^\d{0,15}$'
 
     default_validators = [
         simple.ogrn_validator
     ]
 
-    def __init__(self, verbose_name=u'ОГРН', **kwargs):
+    def __init__(self, verbose_name='ОГРН', **kwargs):
         kwargs.setdefault('max_length', 15)
         super(OGRNField, self).__init__(verbose_name=verbose_name, **kwargs)
```

### Comparing `educommon-2.20.0/src/educommon/django/db/migration/__init__.py` & `educommon-3.0.0/src/educommon/django/db/migration/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-# coding: utf-8
-from functools import partial
-from operator import sub
 import datetime
+from functools import (
+    partial,
+)
+from operator import (
+    sub,
+)
 
 
 def date_difference_as_callable(
         diff, date_fn=datetime.date.today, operator_=sub):
-    u"""Функция, возвращающая callable-объект, не принимающий аргументов и
+    """Функция, возвращающая callable-объект, не принимающий аргументов и
     возвращающий дату.
     Используется для валидации дат, когда нужно проверить не точную дату, а
     изменяющееся значение (например, что дата не позднее сегодняшнего дня).
     Используется в паре с валидатором
     educommon.django.db.validators.simple.date_range_validator
     :param diff:
     :type diff: datetime.timedelta
@@ -24,15 +27,15 @@
     return partial(
         _get_time_difference_from_callable,
         operator_=operator_, date_fn=date_fn, diff=diff)
 
 
 def _get_time_difference_from_callable(
         operator_, date_fn, diff):
-    u"""Вспомогательная функция для сериализации валидатора при генерации
+    """Вспомогательная функция для сериализации валидатора при генерации
     файла-миграции. Нужен для того, чтобы при генерации миграции функция
     date_fn не разворачивалась в точное значение, а оставалась функцией.
     В `models.py` в качестве границы нужно использовать
     `date_difference_as_callable`, а не данную функцию.
     :param operator_:
     :param date_fn:
     :param diff:
```

### Comparing `educommon-2.20.0/src/educommon/django/db/migration/operations.py` & `educommon-3.0.0/src/educommon/django/db/migration/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,61 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from contextlib import closing
-from contextlib import contextmanager
-
-from django.core.serializers import deserialize
-from django.core.serializers import python as python_serializer_module
-from django.db import connection
-from django.db.migrations.operations.base import Operation
-from django.db.migrations.operations.fields import AddField
-from django.db.migrations.operations.fields import AlterField
-from django.db.migrations.operations.fields import RemoveField
-from django.db.migrations.operations.fields import RenameField
-from django.db.models import Max
+from contextlib import (
+    closing,
+    contextmanager,
+)
+
+from django.core.serializers import (
+    deserialize,
+    python as python_serializer_module,
+)
+from django.db import (
+    connection,
+)
+from django.db.migrations.operations.base import (
+    Operation,
+)
+from django.db.migrations.operations.fields import (
+    AddField,
+    AlterField,
+    RemoveField,
+    RenameField,
+)
+from django.db.models import (
+    Max,
+)
 
 
 def get_objects_from_fixture(file_path, file_type=None,
                              use_natural_foreign_keys=False):
-    u"""Возвращает генератор объектов из файла фикстуры.
+    """Возвращает генератор объектов из файла фикстуры.
 
     :param basestring file_path: Путь к файлу с данными.
     :param basestring file_type: Тип файла фикстуры (xml, json или yaml).
     :param bool use_natural_foreign_keys: Флаг, указывающий на необходимость
         использовать "естественные" (natural) ключи.
 
     :rtype: generator
     """
     if file_type is None:
         file_type = file_path[file_path.rfind('.') + 1:]
         if file_type not in ('json', 'xml', 'yaml'):
-            raise ValueError(u'Неподдерживаемый тип файла ' + file_path)
+            raise ValueError('Неподдерживаемый тип файла ' + file_path)
 
     with open(file_path, 'r') as infile:
         with closing(deserialize(
             file_type,
             infile.read(),
             use_natural_foreign_keys=use_natural_foreign_keys
         )) as objects:
             for obj in objects:
                 yield obj
 
 
 def correct_sequence_value(model, field='id', conn=connection):
-    u"""Корректирует значение последовательности для указанного поля модели.
+    """Корректирует значение последовательности для указанного поля модели.
 
     Устанавливает в качестве значения последовательности максимальное значение
     указанного поля. Актуально, когда, например, после загрузки какихм-либо
     данных из фикстур становится возможной ситуация, когда при добавлении
     очередной записи последовательность выдаёт значение, которое уже есть в БД.
 
     :param model: Класс модели.
@@ -65,16 +74,15 @@
             model._meta.get_field(field).column,
             max_id,
         )
     )
 
 
 class LoadFixture(Operation):
-
-    u"""Операция загрузки фикстур в миграции."""
+    """Операция загрузки фикстур в миграции."""
 
     reversible = False
 
     reduces_to_sql = False
 
     atomic = True
 
@@ -112,16 +120,15 @@
             for obj in get_objects_from_fixture(self.file_path):
                 model = obj.object.__class__
                 if self.allow_migrate_model(db_alias, model) or self.force:
                     obj.save()
 
 
 class CorrectSequence(Operation):
-
-    u"""Корректирует значение последовательности для указанного поля.
+    """Корректирует значение последовательности для указанного поля.
 
     .. seealso::
 
         :func:`~educommon.django.db.migration.operations.correct_sequence_value`
     """
 
     reversible = False
@@ -140,22 +147,21 @@
         db_alias = schema_editor.connection.alias
         model = to_state.apps.get_model(app_label, self.model_name)
         if self.allow_migrate_model(db_alias, model) or self.force:
             correct_sequence_value(model, conn=schema_editor.connection)
 
 
 class CreateSchema(Operation):
-
-    u"""Создает схему в БД."""
+    """Создает схему в БД."""
 
     reversible = True
 
     def __init__(self, schema_name, owner=None, aliases=None,
                  cascade_drop=False):
-        u"""Инициализация экземпляра.
+        """Инициализация экземпляра.
 
         :param schema_name: Имя схемы.
         :param owner: Имя владельца схемы.
         :param aliases: Алиасы БД, в которых нужно создать схему. Если не
             указаны, то схема создается во всех БД системы.
         :param bool cascade_drop: Истинное значение аргумента указывает на
             автоматическое удаление всех объектов, содержащихся в схеме, при
@@ -185,15 +191,15 @@
         if not self.aliases or schema_editor.connection.alias in self.aliases:
             sql = 'DROP SCHEMA IF EXISTS ' + self.schema_name
             if self.cascade_drop:
                 sql += ' CASCADE'
             schema_editor.execute(sql)
 
 
-class _AnotherAppMixin(object):
+class _AnotherAppMixin:
 
     def __init__(self, *args, **kwargs):
         self.__app_label = kwargs.pop('app_label', None)
 
         super().__init__(*args, **kwargs)
 
     def state_forwards(self, app_label, state):
```

### Comparing `educommon-2.20.0/src/educommon/django/db/mixins/__init__.py` & `educommon-3.0.0/src/educommon/django/db/mixins/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Классы-примеси для моделей Django."""
 from django.core.exceptions import (
     FieldDoesNotExist,
 )
 from django.db import (
     models,
 )
-
 from m3_django_compat import (
     atomic,
 )
 
 
 class DeferredActionsMixin(models.Model):
 
@@ -123,15 +122,15 @@
         super(DeleteOnSaveMixin, self).__init__(*args, **kwargs)
 
         # Список объектов, подлежащих удалению после сохранения self
         self.__objects_for_delete_before_save = set()
         self.__objects_for_delete_after_save = set()
 
     def delete_before_save(self, obj):
-        u"""Добавляет объект в список удаляемых **перед** сохранением.
+        """Добавляет объект в список удаляемых **перед** сохранением.
 
         Указанный в аргументе `obj` объект помещается в список объектов,
         которые будут удалены **до** сохранения.
 
         :param obj: Объект модели, подлежащий удалению **до** сохранения.
         :type obj: django.db.models.Model
         """
@@ -140,15 +139,15 @@
 
         assert isinstance(obj, models.Model), type(obj)
 
         if obj not in self.__objects_for_delete_after_save:
             self.__objects_for_delete_before_save.add(obj)
 
     def delete_after_save(self, obj):
-        u"""Добавляет объект в список удаляемых **после** сохранения.
+        """Добавляет объект в список удаляемых **после** сохранения.
 
         Указанный в аргументе `obj` объект помещается в список объектов,
         которые будут удалены **после** сохранения.
 
         :param obj: Объект модели, подлежащий удалению **после** сохранения.
         :type obj: django.db.models.Model
         """
@@ -210,19 +209,19 @@
         for field in self._meta.fields:
             if isinstance(field, (models.TextField, models.CharField)):
                 field_value = getattr(self, field.attname)
 
                 if field_value is not None:
                     field_value = str(field_value).strip()
                     # Удаление лишних пробелов
-                    while field_value.find(u'  ') != -1:
-                        field_value = field_value.replace(u'  ', u' ')
+                    while field_value.find('  ') != -1:
+                        field_value = field_value.replace('  ', ' ')
 
                 if not field_value:
-                    field_value = None if field.null else u''
+                    field_value = None if field.null else ''
 
                 setattr(self, field.attname, field_value)
 
         return super(StringFieldsCleanerMixin, self).clean_fields(exclude)
 
     class Meta:
         abstract = True
```

### Comparing `educommon-2.20.0/src/educommon/django/db/mixins/date_interval.py` & `educommon-3.0.0/src/educommon/django/db/mixins/date_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from datetime import date
-from datetime import datetime
-
-from django.core.exceptions import NON_FIELD_ERRORS
-from django.core.exceptions import ValidationError
-from django.db import models
-from django.db.models.query_utils import Q
-from m3_django_compat import Manager
-from m3_django_compat import ModelOptions
-from six.moves import zip
-import six
-
-from educommon import Undefined
-from educommon.utils import is_ranges_intersected
-from educommon.utils.date import date_range_to_str
+from datetime import (
+    date,
+    datetime,
+)
+
+from django.core.exceptions import (
+    NON_FIELD_ERRORS,
+    ValidationError,
+)
+from django.db import (
+    models,
+)
+from django.db.models.query_utils import (
+    Q,
+)
+from m3_django_compat import (
+    Manager,
+    ModelOptions,
+)
+
+from educommon import (
+    Undefined,
+)
+from educommon.utils import (
+    is_ranges_intersected,
+)
+from educommon.utils.date import (
+    date_range_to_str,
+)
 
 
 class BaseIntervalMeta(models.base.ModelBase):
 
     """Базовый метакласс для примесей *IntervalMixin.
 
     Добавляет к создаваемой модели поля, содержащие границы интервала. Имена
@@ -226,15 +236,15 @@
         cls,
         date_begin=None,
         date_end=None,
         lookup=None,
         include_lower_bound=True,
         include_upper_bound=True
     ):
-        u"""Метод возвращает фильтр для выборки записей, попадающих в интервал.
+        """Метод возвращает фильтр для выборки записей, попадающих в интервал.
 
         Для проверки пересечения двух интервалов a и b необходимо и
         достаточно выполнения двух условий:
         a.start <= b.end AND a.end >= b.start
 
         Пусть будут даны два интервала a и b, у которых соответственно задано
         начало и конец: a.start/a.end и b.start/b.end и считаем, что
@@ -292,15 +302,15 @@
         if date_end is None:
             date_end = cls.get_current_date()
 
         # Предполагается, что в интервалах дат дата окончания находится
         # справа по оси времени от даты начала или равна. Если будет наоборот,
         # то результат может оказаться не верным
         assert date_end >= date_begin, (
-            u'Дата окончания должна быть больше или равна дате начала'
+            'Дата окончания должна быть больше или равна дате начала'
         )
 
         from_name, to_name = cls.interval_field_names
         if lookup is not None:
             from_lookup = '__'.join([lookup, from_name])
             to_lookup = '__'.join([lookup, to_name])
         else:
@@ -377,15 +387,15 @@
         date_from, date_to = self.interval_range
         result = date_range_to_str(date_from, date_to)
         return result
 
     def interval_dates_error_message(self):
         """Возвращает сообщение о неправильных границах интервала.
 
-        :rtype: unicode
+        :rtype: str
         """
         opts = ModelOptions(self)
 
         date_from_name, date_to_name = self.interval_field_names
         result = 'Значение "{}" должно быть раньше, чем "{}"'.format(
             opts.get_field(date_from_name).verbose_name.capitalize(),
             opts.get_field(date_to_name).verbose_name.lower(),
@@ -394,15 +404,15 @@
 
     def interval_intersected_error_message(self, others=None):
         """Возвращает сообщение о пересечении интервалов.
 
         :param others: Записи, с интервалами которых пересекается интервал
             данной записи.
 
-        :rtype: unicode
+        :rtype: str
         """
         return 'Интервал пересекается с другими записями'
 
     @property
     def previous_interval(self):
         """Предыдущий интервал или None."""
         date_from_name, date_to_name = self.interval_field_names
@@ -493,18 +503,15 @@
         if errors:
             raise ValidationError(errors)
 
     class Meta:
         abstract = True
 
 
-class DateIntervalMixin(
-    six.with_metaclass(DateIntervalMeta, BaseIntervalMixin)
-):
-
+class DateIntervalMixin(BaseIntervalMixin, metaclass=DateIntervalMeta):
     """Примесь к моделям, добавляющяя интервал дат.
 
     Содержит два поля: date_from (дата начала интервала) и date_to (дата
     окончания интервала). Значение None этих полей указывает на то, что
     временной интервал не ограничен с соответствующей стороны.
     """
 
@@ -533,18 +540,15 @@
         """
         return date.today()
 
     class Meta:
         abstract = True
 
 
-class DateTimeIntervalMixin(
-    six.with_metaclass(DateTimeIntervalMeta, BaseIntervalMixin)
-):
-
+class DateTimeIntervalMixin(BaseIntervalMixin, metaclass=DateTimeIntervalMeta):
     """Примесь к моделям, добавляющия интервал дат со временем.
 
     Содержит два поля: date_from (дата начала интервала) и date_to (дата
     окончания интервала). Значение None этих полей указывает на то, что
     временной интервал не ограничен с соответствующей стороны.
     """
```

### Comparing `educommon-2.20.0/src/educommon/django/db/mixins/validation.py` & `educommon-3.0.0/src/educommon/django/db/mixins/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,50 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from collections import defaultdict
 import inspect
 import sys
-
-from django.core.exceptions import ObjectDoesNotExist
-from django.core.exceptions import ValidationError
-from django.db import IntegrityError
-from django.db import models
-from django.db import transaction
-from django.db.models.fields.related_descriptors import \
-    ForwardOneToOneDescriptor
-from django.db.models.fields.related_descriptors import \
-    ReverseOneToOneDescriptor
-from django.db.models.query import QuerySet as DjangoQuerySet
-from django.dispatch import Signal
-from django.forms.forms import NON_FIELD_ERRORS
-from m3_django_compat import Manager as DjangoManager
-from m3_django_compat import atomic
-import six
-
-from educommon.django.db.validators import IModelValidator
-from educommon.utils.misc import NoOperationCM
+from collections import (
+    defaultdict,
+)
+
+from django.core.exceptions import (
+    ObjectDoesNotExist,
+    ValidationError,
+)
+from django.db import (
+    IntegrityError,
+    models,
+    transaction,
+)
+from django.db.models.fields.related_descriptors import (
+    ForwardOneToOneDescriptor,
+    ReverseOneToOneDescriptor,
+)
+from django.db.models.query import (
+    QuerySet as DjangoQuerySet,
+)
+from django.dispatch import (
+    Signal,
+)
+from django.forms.forms import (
+    NON_FIELD_ERRORS,
+)
+from m3_django_compat import (
+    Manager as DjangoManager,
+    atomic,
+)
+
+from educommon.django.db.validators import (
+    IModelValidator,
+)
+from educommon.utils.misc import (
+    NoOperationCM,
+)
 
 
 class QuerySet(DjangoQuerySet):
-
-    u"""Доработанная для ModelValidationMixin версия QuerySet.
+    """Доработанная для ModelValidationMixin версия QuerySet.
 
     Переопределяет методы create() и get_or_create(), добавляя валидацию
     объекта перед его сохранением в БД.
     """
 
     def create(self, **kwargs):
         # Копипаста метода из Django 1.4 с добавлением вызова full_clean().
@@ -70,63 +83,60 @@
                 params.update(defaults)
                 obj = self.model(**params)
                 obj.full_clean()
                 sid = transaction.savepoint(using=self.db)
                 obj.save(force_insert=True, using=self.db)
                 transaction.savepoint_commit(sid, using=self.db)
                 return obj, True
-            except IntegrityError:
+            except IntegrityError as e:
                 transaction.savepoint_rollback(sid, using=self.db)
-                exc_info = sys.exc_info()
+
                 try:
                     return self.get(**lookup), False
                 except self.model.DoesNotExist:
-                    # Re-raise the IntegrityError with its original traceback.
-                    six.reraise(exc_info[1], None, exc_info[2])
+                    raise e from None
 
 
 class Manager(DjangoManager):
-
-    u"""Доработанная версия менеджера моделей системы.
+    """Доработанная версия менеджера моделей системы.
 
     Вместо QuerySet из Django использует доработанный QuerySet, выполняющий
     валидацию объекта перед его сохранением в БД в методе create().
     """
 
     def get_queryset(self):
         return QuerySet(self.model, using=self._db)
 
 
 pre_clean = Signal(providing_args=('errors',))
-u"""Сигнал, отправляемый перед валидацией модели.
+"""Сигнал, отправляемый перед валидацией модели.
 
 :param defaultdict errors: Словарь, содержащий ошибки валидации экземпляра
     модели.
 
 .. seealso::
 
    :py:class:`ModelValidationMixin`
 """
 
 
 post_clean = Signal(providing_args=('errors',))
-u"""Сигнал, отправляемый после валидации модели.
+"""Сигнал, отправляемый после валидации модели.
 
 :param defaultdict errors: Словарь, содержащий ошибки валидации экземпляра
     модели.
 
 .. seealso::
 
    :py:class:`ModelValidationMixin`
 """
 
 
 class ModelValidationMixin(models.Model):
-
-    u"""Примесь, добавляющая необходимость валидации перед сохранением.
+    """Примесь, добавляющая необходимость валидации перед сохранением.
 
     Также примесь переопределяет менеджер модели по умолчанию. В новом
     менеджере переопределяются два метода: create() и get_or_create(), которые
     перед созданием объекта модели выполняют валидацию.
 
     Пример:
 
@@ -181,15 +191,15 @@
 
         self.__set_valid_flag(False)
 
     def __set_valid_flag(self, value):
         self.__dict__['_ModelValidationMixin__object_is_valid'] = value
 
     def clean(self):
-        u"""Переносит валидацию объекта модели в метод simple_clean().
+        """Переносит валидацию объекта модели в метод simple_clean().
 
         При этом работа с исключениями ValidationError остается в данном
         методе, что позволяет не обрабатывать их в каждой модели.
         Если объект или связанные объекты не существуют, перехватывает
         ObjectDoesNotExist и выводит соответствующее сообщение.
         """
         errors = defaultdict(list)
@@ -237,26 +247,26 @@
         for validator in self.validators:
             validator.clean(instance=self, errors=errors)
 
         if errors:
             raise ValidationError(errors)
 
     def simple_clean(self, errors):
-        u"""Выполняет валидацию объекта модели вместо метода clean().
+        """Выполняет валидацию объекта модели вместо метода clean().
 
         :param errors: Словарь с сообщениями об ошибках. Каждый ключ словаря
             должен соответствовать полю модели, а значением ключа является
             список сообщений об ошибках в этом поле. Подробнее см.
             django.core.exceptions.ValidationError.
         :type errors: collections.defaultdict
         """
         pass
 
     def full_clean(self, exclude=None):
-        u"""Проставляет отметку о выполнении валидации экземпляра модели.
+        """Проставляет отметку о выполнении валидации экземпляра модели.
 
         Отправляет сигналы pre_clean и post_clean.
         """
         errors = defaultdict(list)
 
         pre_clean.send(sender=self.__class__, instance=self, errors=errors)
 
@@ -270,35 +280,35 @@
         if errors:
             raise ValidationError(errors)
 
         self.__set_valid_flag(True)
 
     @atomic
     def save(self, *args, **kwargs):
-        u"""После сохранения объекта снимает отметку о выполнении валидации."""
+        """После сохранения объекта снимает отметку о выполнении валидации."""
         if not self.ready_to_save:
             raise AssertionError(
-                u'Attempt to save data without validation '
-                u'(model {}.{})'.format(
+                'Attempt to save data without validation '
+                '(model {}.{})'.format(
                     self.__class__.__module__, self.__class__.__name__
                 )
             )
 
         super(ModelValidationMixin, self).save(*args, **kwargs)
 
         # Перед следующим сохранением нужно будет снова вызвать full_clean
         self.__set_valid_flag(False)
 
     @property
     def ready_to_save(self):
-        u"""Готовность к сохранению объекта модели в БД."""
+        """Готовность к сохранению объекта модели в БД."""
         return getattr(self, '_ModelValidationMixin__object_is_valid', False)
 
     def clean_and_save(self):
-        u"""Валидация объекта и сохранение."""
+        """Валидация объекта и сохранение."""
         if self.clean_and_save_inside_transaction:
             cm = atomic()
         else:
             cm = NoOperationCM()
 
         with cm:
             self.full_clean()
```

### Comparing `educommon-2.20.0/src/educommon/django/db/model_view/__init__.py` & `educommon-3.0.0/src/educommon/django/db/model_view/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,48 @@
-# coding: utf-8
-u"""Средства для работы с представлениями объектов моделей.
+"""Средства для работы с представлениями объектов моделей.
 
 Под представлением объекта модели подразумевается объект, задачей которого
 является формирование какого-либо представления (HTML, JSON и т.п.) на основе
 объекта модели.
 """
-from __future__ import absolute_import
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
+
+from django.apps import (
+    apps,
+)
+from django.template.loader import (
+    render_to_string,
+)
+from django.utils.encoding import (
+    force_text,
+)
+from m3_django_compat import (
+    get_model,
+)
+
+from educommon.utils.db import (
+    get_field,
+)
+from educommon.utils.misc import (
+    cached_property,
+    get_nested_attr,
+)
+from educommon.utils.ui import (
+    local_template,
+)
 
-from abc import ABCMeta
-from abc import abstractmethod
 
-from django.apps import apps
-from django.template.loader import render_to_string
-from django.utils.encoding import force_text
-from m3_django_compat import get_model
-import six
-
-from educommon.utils.db import get_field
-from educommon.utils.misc import cached_property
-from educommon.utils.misc import get_nested_attr
-from educommon.utils.ui import local_template
-
-
-class ModelView(six.with_metaclass(ABCMeta, object)):
-
-    u"""Базовый класс для представлений объектов модели."""
+class ModelView(metaclass=ABCMeta):
+    """Базовый класс для представлений объектов модели."""
 
     def __init__(self, model, description=None, priority=0):
-        u"""Инициализация класса представления модели
+        """Инициализация класса представления модели
 
         Представления с бОльшим приоритетом (priority) перезаписывают уже
         зарегистированные представления, у которых приоритет ниже.
         При попытке регистрации двух моделей с одинаковым приоритетом,
         который по умолчанию 0, будет выброшено исключение
 
         :param model: Модель, для которой регистрируется представление
@@ -40,145 +51,137 @@
         """
         self._model = model
         self._description = description
         self.priority = priority
 
     @cached_property
     def model(self):
-        if isinstance(self._model, six.string_types):
+        if isinstance(self._model, str):
             return apps.get_model(*self._model.split('.'))
         else:
             return self._model
 
     @abstractmethod
     def get_view(self, objects):
-        u"""Возвращает представление для указанных объектов."""
+        """Возвращает представление для указанных объектов."""
 # -----------------------------------------------------------------------------
 # Извлечение данных из объектов
 
 
-class DataExtractor(six.with_metaclass(ABCMeta, object)):
-
-    u"""Базовый класс для извлекателей данных."""
+class DataExtractor(metaclass=ABCMeta):
+    """Базовый класс для извлекателей данных."""
 
     @abstractmethod
     def get(self, obj):
-        u"""Возвращает данные, извлеченные из объекта."""
+        """Возвращает данные, извлеченные из объекта."""
 
 
 class Text(DataExtractor):
 
     def __init__(self, text):
         self._text = text
 
     def get(self, obj):
         return self._text
 
 
 class ModelVerboseName(DataExtractor):
-
-    u"""Текстовое описание объекта модели."""
+    """Текстовое описание объекта модели."""
 
     def get(self, obj):
         return obj._meta.verbose_name
 
 
 class ModelVerboseNamePlural(DataExtractor):
-
-    u"""Текстовое описание объектов модели."""
+    """Текстовое описание объектов модели."""
 
     def get(self, obj):
         return obj._meta.verbose_name_plural
 
 
 class FieldVerboseName(DataExtractor):
-
-    u"""Описание поля модели."""
+    """Описание поля модели."""
 
     def __init__(self, field_name):
         self._field_name = field_name
 
     def get(self, obj):
-        return get_field(obj, self._field_name).verbose_name or u''
+        return get_field(obj, self._field_name).verbose_name or ''
 
 
 class AttrValue(DataExtractor):
-
-    u"""Значение атрибута."""
+    """Значение атрибута."""
 
     def __init__(self, field_name):
         self._field_name = field_name
 
     def get(self, obj):
         try:
-            return get_nested_attr(obj, self._field_name) or u''
+            return get_nested_attr(obj, self._field_name) or ''
         except AttributeError:
-            return u''
+            return ''
 
 
 class JoinedAttrValues(DataExtractor):
+    """Значения атрибутов через разделитель."""
 
-    u"""Значения атрибутов через разделитель."""
-
-    def __init__(self, delimiter=u' / ', *field_names):
+    def __init__(self, delimiter=' / ', *field_names):
         self._field_names = field_names
         self._delimiter = delimiter
 
     def get(self, obj):
         values = []
         for field_name in self._field_names:
             try:
-                value = force_text(get_nested_attr(obj, field_name) or u'')
+                value = force_text(get_nested_attr(obj, field_name) or '')
             except AttributeError:
-                return u''
+                return ''
             else:
                 values.append(value)
 
         return self._delimiter.join(values)
 
 
 class FieldChoiceValue(DataExtractor):
-
-    u"""Значение поля с choices."""
+    """Значение поля с choices."""
 
     def __init__(self, field_name):
         self._field_name = field_name
 
     def get(self, obj):
         field = get_field(obj, self._field_name)
         try:
             value = get_nested_attr(obj, self._field_name)
         except AttributeError:
-            return u''
+            return ''
         else:
             return force_text(
                 dict(field.flatchoices).get(value, value),
                 strings_only=True
             )
 # -----------------------------------------------------------------------------
 
 
 class HtmlTableView(ModelView):
-
-    u"""Представление объектов в виде таблицы HTML.
+    """Представление объектов в виде таблицы HTML.
 
     При реализации представления необходимо описать ячейки заголовка таблицы и
     ячейки данных. Для описания содержимого ячеек следует использовать
     извлекатели данных (см. :class:`DataExtractor`).
 
     ::
 
       class SubjectOffice(models.Model):
           subject = models.ForeignKey(
               'subject.Subject',
-              verbose_name=u"Предмет",
+              verbose_name="Предмет",
           )
           office = models.ForeignKey(
               'office.Office',
-              verbose_name=u"Аудитория",
+              verbose_name="Аудитория",
           )
 
       subject_office_view = HtmlTableView(
           model='subject.SubjectOffice',
           columns=(
               dict(
                   header=FieldVerboseName('subject'),
@@ -210,51 +213,51 @@
 
     def __init__(self, model, columns, *args, **kwargs):
         super(HtmlTableView, self).__init__(model, *args, **kwargs)
 
         self._columns = columns
 
     def _get_description(self, model):
-        u"""Возвращает данные для заголовка таблицы."""
+        """Возвращает данные для заголовка таблицы."""
         return self._description.get(model) if self._description else None
 
     def _get_header_data(self, model):
-        u"""Возвращает данные для ячеек заголовка таблицы.
+        """Возвращает данные для ячеек заголовка таблицы.
 
         :rtype: tuple
         """
         if all(not column.get('header') for column in self._columns):
             return None
 
         return tuple(
             column['header'].get(model)
             for column in self._columns
         )
 
     def _get_body_data(self, objects):
-        u"""Возвращает данные для ячеек тела таблицы.
+        """Возвращает данные для ячеек тела таблицы.
 
         :rtype: tuple
         """
         return tuple(
             tuple(column['data'].get(obj) for column in self._columns)
             for obj in objects
         )
 
     def get_view(self, objects):
-        u"""Возвращает строку с HTML-таблицей, содержащей данные объектов.
+        """Возвращает строку с HTML-таблицей, содержащей данные объектов.
 
         :param objects: Объекты, для которых необходимо сформировать
             представление.
         :type objects: Iterable
 
-        :rtype: unicode
+        :rtype: str
         """
         if not objects:
-            return u''
+            return ''
 
         assert len(set(obj.__class__ for obj in objects)) == 1, objects
 
         if self.model is None:
             model = objects[0].__class__
         else:
             model = self.model
@@ -266,40 +269,39 @@
                 header=self._get_header_data(model),
                 body=self._get_body_data(objects),
             ),
         )
 # -----------------------------------------------------------------------------
 
 
-class ModelViewRegistry(object):
-
-    u"""Реестр представлений моделей.
+class ModelViewRegistry:
+    """Реестр представлений моделей.
 
     Предоставляет средства для регистрации представлений в реестре и получения
     представлений для модели.
     """
 
     def __init__(self, default_view=None):
         self._registry = {}
         self._default_view = default_view
 
     @staticmethod
     def _get_model_key(model):
-        if isinstance(model, six.string_types):
+        if isinstance(model, str):
             model = get_model(*model.split('.'))
 
         if model._meta.proxy:
             model = model._meta.proxy_for_model
 
         key = '.'.join((model._meta.app_label, model._meta.model_name))
 
         return key.lower()
 
     def register(self, *views):
-        u"""Регистрация представления модели.
+        """Регистрация представления модели.
 
         :param model: Модель. Может быть задана классом модели, либо строкой
             вида 'app_label.ModelClass'.
         :type model: django.db.models.base.ModelBase or basestring
 
         :param view: Представление модели.
         :type view: ModelView
@@ -308,43 +310,43 @@
             key = ModelViewRegistry._get_model_key(view.model)
             registered_view = self._registry.get(key)
 
             if registered_view and registered_view is not view:
                 # Сравниваем приоритеты представлений
                 if registered_view.priority == view.priority:
                     raise ValueError(
-                        u'Для модели {} уже зарегистрировано '
-                        u'представление {} с приоритетом {}.'.format(
+                        'Для модели {} уже зарегистрировано '
+                        'представление {} с приоритетом {}.'.format(
                             key, view, view.priority
                         )
                     )
                 elif registered_view.priority > view.priority:
                     # Пропускаем моедль, если у текущей зарегистированной
                     # модели приоритет больше
                     continue
 
             self._registry[key] = view
 
     def get(self, model):
-        u"""Возвращает представление для указанной модели.
+        """Возвращает представление для указанной модели.
 
         :param model: Модель. Может быть задана классом модели, либо строкой
             вида 'app_label.ModelClass'.
         :type model: django.db.models.base.ModelBase or basestring
 
         :rtype: ModelView or None
         """
         key = ModelViewRegistry._get_model_key(model)
         if key in self._registry:
             return self._registry[key]
         elif self._default_view:
             return self._default_view
         else:
             raise ValueError(
-                u'Для модели {} не зарегистрировано представление.'
+                'Для модели {} не зарегистрировано представление.'
                 .format(key)
             )
 # -----------------------------------------------------------------------------
 
 
 #: Реестры представлений моделей.
 registries = {}
```

### Comparing `educommon-2.20.0/src/educommon/django/db/model_view/table-view.html` & `educommon-3.0.0/src/educommon/django/db/model_view/table-view.html`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/django/db/models.py` & `educommon-3.0.0/src/educommon/django/db/models.py`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/django/db/observer.py` & `educommon-3.0.0/src/educommon/django/db/observer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-# coding: utf-8
-from __future__ import absolute_import
+from weakref import (
+    WeakValueDictionary,
+)
+
+from django.db.models.base import (
+    Model,
+)
+from django.db.models.signals import (
+    post_delete,
+    post_save,
+    pre_delete,
+    pre_save,
+)
+
+from educommon.utils import (
+    SingletonMeta,
+)
 
-from weakref import WeakValueDictionary
 
-from django.db.models.base import Model
-from django.db.models.signals import post_delete
-from django.db.models.signals import post_save
-from django.db.models.signals import pre_delete
-from django.db.models.signals import pre_save
-import six
-
-from educommon.utils import SingletonMeta
-
-
-class ModelObserverBase(six.with_metaclass(SingletonMeta, object)):
-
-    u"""Базовый класс для наблюдателей за моделями.
+class ModelObserverBase(metaclass=SingletonMeta):
+    """Базовый класс для наблюдателей за моделями.
 
     Предоставляет возможность реализовывать реакцию на изменение и удаление
     объектов моделей.
 
     В отличие от сигналов Django позволяет более гибко определять перечень
     наблюдаемых моделей, например указывать базовый класс модели (см. метод
     ``_is_observable()``).
@@ -56,28 +59,27 @@
                print '{}{{{}}}'.format(instance.__class__.__name__,
                                        instance.pk)
 
                for field in instance._meta.concrete_fields:
                    old_value = getattr(context.original, field.attname)
                    new_value = getattr(instance, field.attname)
                    if old_value != new_value:
-                       print u'\t{}: {} --> {}'.format(
+                       print '\t{}: {} --> {}'.format(
                            field.name, old_value, new_value
                        )
 
     .. seealso::
 
        * :class:`~educommon.django.db.observer.ModelOnlyObserverMixin`
        * :class:`~educommon.django.db.observer.ModelDescendantsObserverMixin`
        * :class:`~educommon.django.db.observer.OriginalObjectMixin`
     """
 
-    class Context(object):
-
-        u"""Класс-контейнер для контекста наблюдателя.
+    class Context:
+        """Класс-контейнер для контекста наблюдателя.
 
         Предназначен для хранения дополнительных объектов, связанных с
         наблюдаемым объектом. Например, в нем можно хранить объект модели в
         состоянии *до* изменения.
 
         .. caution:
 
@@ -85,41 +87,41 @@
            ссылки, поэтому для корректной работы нельзя допускать хранение
            наблюдаемого объекта в контексте, т.к. это заблокирует его
            уничтожение сборщиком мусора.
         """
 
     
     def _create_context(self, instance):
-        u"""Возвращает контекст для экземпляра модели.
+        """Возвращает контекст для экземпляра модели.
 
         :param instance: Объект (экземпляр) наблюдаемой модели.
 
         :rtype: ModelObserverBase.Context
         """
         context = self.Context()
         self._contexts[context] = instance
         return context
 
     def _get_context(self, instance):
-        u"""Возвращает объект контекста, соответствующий экземпляру модели.
+        """Возвращает объект контекста, соответствующий экземпляру модели.
 
         В случае, если для указанного экземпляра модели контекст еще не
         создавался, то он создается и добавляется в хранилище.
 
         :rtype: :class:`ModelObserverBase.Context` or None.
         """
-        for context, obj in six.iteritems(self._contexts):
+        for context, obj in self._contexts.items():
             if id(instance) == id(obj) and instance.__class__ is obj.__class__:
                 return context
 
         return self._create_context(instance)
 
     def _remove_context(self, instance):
-        u"""Удаляет из хранилища контекст для указанного экземпляра модели."""
-        for context, obj in six.iteritems(self._contexts):
+        """Удаляет из хранилища контекст для указанного экземпляра модели."""
+        for context, obj in self._contexts.items():
             if id(instance) == id(obj) and instance.__class__ is obj.__class__:
                 del self._contexts[context]
                 break
 
     def __init__(self):
         # модели, за которыми осуществляется наблюдение
         self._observables = set()
@@ -138,28 +140,28 @@
         pre_save.connect(wrapper(self.__pre_save_handler), weak=False)
         post_save.connect(wrapper(self.__post_save_handler), weak=False)
         pre_delete.connect(wrapper(self.__pre_delete_handler), weak=False)
         post_delete.connect(wrapper(self.__post_delete_handler), weak=False)
         # ---------------------------------------------------------------------
 
     def observe(self, model):
-        u"""Включает наблюдение за указанной моделью.
+        """Включает наблюдение за указанной моделью.
 
         В случае, если указанная модель является абстрактной, то наблюдение
         будет выполняться за всеми моделями, являющимися потомками указанной
         модели.
 
         :param model: Класс наблюдаемой модели.
         """
         assert model is Model or issubclass(model, Model), type(model)
 
         self._observables.add(model)
 
     def _is_observable(self, model):
-        u"""Возвращает ``True``, если модель находится под наблюдением.
+        """Возвращает ``True``, если модель находится под наблюдением.
 
         :rtype: bool
         """
         raise NotImplementedError()
 
     def __pre_save_handler(self, instance, **kwargs):
         # Если в наблюдателе есть методы для обработки save-сигналов, то
@@ -204,36 +206,33 @@
                 context=self._get_context(instance),
                 **kwargs
             )
 
         self._remove_context(instance)
 
 
-class ModelOnlyObserverMixin(object):
-
-    u"""Класс-примесь для наблюдения только за указанными моделями."""
+class ModelOnlyObserverMixin:
+    """Класс-примесь для наблюдения только за указанными моделями."""
 
     def _is_observable(self, model):
         return model in self._observables
 
 
-class ModelDescendantsObserverMixin(object):
-
-    u"""Класс примесь для наблюдения за моделями и их потомками."""
+class ModelDescendantsObserverMixin:
+    """Класс примесь для наблюдения за моделями и их потомками."""
 
     def _is_observable(self, model):
         return any(
             model is observable or issubclass(model, observable)
             for observable in self._observables
         )
 
 
-class OriginalObjectMixin(object):
-
-    u"""Класс-примесь, добавляющая в контекст наблюдателя исходный объект."""
+class OriginalObjectMixin:
+    """Класс-примесь, добавляющая в контекст наблюдателя исходный объект."""
 
     # Кеш исходных объектов. Используется для предотвращения повторной загрузки
     # при использовании нескольких наблюдателей.
     __cache = WeakValueDictionary()
 
     class _Empty:
         pass
```

### Comparing `educommon-2.20.0/src/educommon/django/db/partitioning/README.md` & `educommon-3.0.0/src/educommon/django/db/partitioning/README.md`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/django/db/partitioning/__init__.py` & `educommon-3.0.0/src/educommon/django/db/partitioning/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# coding: utf-8
-u"""Средства для реализации партиционирования таблиц в СУБД PostgreSQL.
+"""Средства для реализации партиционирования таблиц в СУБД PostgreSQL.
 
 В настоящее время поддерживается только помесячное разбиение таблиц БД на
 разделы.
 
 Для использования партиционирования таблиц необходимо выполнить следующие
 шаги:
 
@@ -25,44 +24,62 @@
 
 После выполнения указанных действий с партиционированной таблицей можно
 продолжать работать как с обычной таблицей.
 
 Подробнее о партиционировании можно почитать в дкоументации PostgreSQL
 (раздел 5.9).
 """
-from __future__ import absolute_import
-
-from contextlib import closing
-from os import path
-from time import sleep
-from types import MethodType
 import re
-
-from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
-from django.db import connections
-from django.db import router
-from django.db import transaction
-from django.db.models.options import Options
-from django.db.models.sql.compiler import cursor_iter
-from django.db.utils import DEFAULT_DB_ALIAS
-from django.utils.functional import cached_property
-from m3_django_compat import ModelOptions
-from m3_django_compat import commit_unless_managed
-from six.moves import map
-import six
-
-from educommon.django.db.observer import ModelObserverBase
+from contextlib import (
+    closing,
+)
+from os import (
+    path,
+)
+from time import (
+    sleep,
+)
+from types import (
+    MethodType,
+)
+
+from django.conf import (
+    settings,
+)
+from django.core.exceptions import (
+    ImproperlyConfigured,
+)
+from django.db import (
+    connections,
+    router,
+)
+from django.db.models.sql.compiler import (
+    cursor_iter,
+)
+from django.db.utils import (
+    DEFAULT_DB_ALIAS,
+)
+from django.utils.functional import (
+    cached_property,
+)
+from m3_django_compat import (
+    ModelOptions,
+    commit_unless_managed,
+)
+
+from educommon.django.db.observer import (
+    ModelObserverBase,
+)
 
 
 _MESSAGE_PREFIX = '[Partitioning] '
 
 
 def _check_system_settings(database_alias):
-    u"""Проверка конфигурации системы. Перечень проверок:
+    """Проверка конфигурации системы. Перечень проверок:
 
         1. Указанный алиас БД есть в конфигурации системы.
         2. Указанная БД управляется СУБД PostgreSQL.
     """
     if database_alias not in settings.DATABASES:
         raise ImproperlyConfigured(
             _MESSAGE_PREFIX +
@@ -77,15 +94,15 @@
         raise ImproperlyConfigured(
             _MESSAGE_PREFIX +
             'only PostgreSQL DBMS supported.'
         )
 
 
 def is_initialized(database_alias):
-    u"""Проверяет, проинициализированы ли средства партиционирования.
+    """Проверяет, проинициализированы ли средства партиционирования.
 
     :param str database_alias: Алиас БД, в которой будет проверяться наличие
         средств партиционирования.
 
     :rtype: bool
     """
     # Проверка наличия схемы partitioning.
@@ -138,15 +155,15 @@
 
     cursor.execute(file_contents)
 
     commit_unless_managed(database_alias)
 
 
 def init(database_alias=DEFAULT_DB_ALIAS, force=False):
-    u"""Осуществляет инициализацию средств партиционирования таблиц БД.
+    """Осуществляет инициализацию средств партиционирования таблиц БД.
 
     Под средствами партиционирования понимается набор функций, создаваемых
     в указанной базе данных. С помощью этих функций реализуется автоматическое
     создание разделов таблиц и управление записями в разделах.
 
     :param str database_alias: Алиас базы данных, в которой нужно
         инициализировать средства партиционирования.
@@ -171,15 +188,15 @@
     table_name = model._meta.db_table
     pk_column_name = model._meta.pk.name
 
     return database_alias, table_name, pk_column_name
 
 
 def is_model_partitioned(model):
-    u"""Возвращает True, если для модели включено партиционирование.
+    """Возвращает True, если для модели включено партиционирование.
 
     :rtype: bool
     """
     database_alias, table_name, _ = _get_model_params(model)
 
     with closing(connections[database_alias].cursor()) as cursor:
         cursor.execute(
@@ -192,15 +209,15 @@
             "select partitioning.is_table_partitioned(%s)",
             (table_name,)
         )
         return cursor.fetchone()[0]
 
 
 def set_partitioning_for_model(model, column_name, force=False):
-    u"""Включает партиционирование указанной таблицы или модели.
+    """Включает партиционирование указанной таблицы или модели.
 
     Для включения партиционирования для указанной таблицы создаются триггеры,
     вызывающие функции управления партиционированием. Перед включением
     партиционирования для таблиц БД должны быть проинициализированы средства
     партиционирования с помощью функции init().
 
     :param model: Модель, для которой включается партиционирование.
@@ -224,15 +241,15 @@
             _MESSAGE_PREFIX + 'not initialized'
         )
 
     _execute_sql_file(database_alias, 'triggers.sql', locals())
 
 
 def split_table(model, column_name, timeout=0):
-    u"""Переносит записи из разбиваемой таблицы в ее разделы.
+    """Переносит записи из разбиваемой таблицы в ее разделы.
 
     Недостающие разделы будут созданы автоматически.
 
     :param model: Модель, записи которой нужно перенести в разделы. Алиас
         используемой БД определяется с помощью метода db_for_write роутера
         Django.
     :param str column_name: Имя поля модели, содержащее значение даты. Это
@@ -292,15 +309,15 @@
         commit_unless_managed(database_alias)
 
         if timeout:
             sleep(timeout)
 
 
 def clear_table(model, column_name, column_value, timeout=0):
-    u"""Удаление записей по условию.
+    """Удаление записей по условию.
 
     С помощью данной команды удаляются записи из основной (не секционированной)
     таблицы, у которых значение в column_name меньше значения из column_value.
 
     :param model: Модель, записи которой нужно удалить. Алиас
         используемой БД определяется с помощью метода db_for_write роутера
         Django.
@@ -344,15 +361,15 @@
         commit_unless_managed(database_alias)
 
         if timeout:
             sleep(timeout)
 
 
 def get_model_partitions(model):
-    u"""Возвращает названия разделов таблицы.
+    """Возвращает названия разделов таблицы.
 
     :param model: Модель, записи которой перенесены в разделы. Алиас
         используемой БД определяется с помощью метода db_for_write роутера
         Django.
 
     :rtype: tuple
     """
@@ -370,15 +387,15 @@
     return tuple(
         partition_name
         for (partition_name,) in cursor
     )
 
 
 def reset_partition_constraints(model, column_name, partition_name):
-    u"""Переустанавливает ограничения для указанного раздела.
+    """Переустанавливает ограничения для указанного раздела.
 
     :param model: Модель, записи которой перенесены в разделы. Алиас
         используемой БД определяется с помощью метода db_for_write роутера
         Django.
     :param str column_name: Имя поля модели, содержащее значение даты. Это
         значение определяет раздел таблицы, в который будет помещена запись.
     :param str partition_name: Имя раздела.
@@ -396,15 +413,15 @@
         (partition_name, column_name, year, month)
     )
 
     commit_unless_managed(database_alias)
 
 
 def drop_partitions_before_date(model, date):
-    u"""Удаление старых партиций модели вплоть до месяца переданной даты.
+    """Удаление старых партиций модели вплоть до месяца переданной даты.
 
     :param Model: модель
     :type Model: django.db.models.base.ModelBase
     :param date: дата, до которой необходимо осуществить удаление партиций
     :type date: datetime.date or datetime.datetime
     """
     if is_model_partitioned(model):
@@ -421,16 +438,15 @@
             for partition in filtered_partitions:
                 cursor.execute(
                     'DROP TABLE IF EXISTS {};'.format(partition)
                 )
 
 
 class PartitioningObserver(ModelObserverBase):
-
-    u"""Оптимизирует операции вставки в партиционированные таблицы.
+    """Оптимизирует операции вставки в партиционированные таблицы.
 
     При добавлении записей в партиционированную таблицу добавление происходит
     следующим образом:
 
         1. добавляется запись в основную таблицу;
         2. такая же запись добавляется в соответствующий раздел таблицы;
         3. эта же запись удаляется из основной таблицы.
@@ -454,28 +470,28 @@
     def _partitioning_ready(self):
         return {
             database_alias: is_initialized(database_alias)
             for database_alias in connections
         }
 
     def _is_observable(self, model):
-        u"""Возвращает True только для моделей с включенным партиционированием.
+        """Возвращает True только для моделей с включенным партиционированием.
 
         :rtype: bool
         """
         if not self._partitioning_ready[router.db_for_write(model)]:
             return False
 
         if model not in self.__models:
             self.__models[model] = is_model_partitioned(model)
 
         return self.__models[model]
 
     def pre_save(self, instance, context, **kwargs):
-        u"""Оборачивает метод _save_table объекта для подмены имени таблицы.
+        """Оборачивает метод _save_table объекта для подмены имени таблицы.
 
         После замены метода ``_save_table`` ДО вызова оригинального метода
         в ``instance._meta.db_table`` записывается имя представления, через
         которое будет выполняться добавление записи, а ПОСЛЕ вызова метода
         значение ``db_table`` восстанавливается.
         """
         if instance.pk is None:
@@ -486,14 +502,14 @@
                 db_table = self._meta.db_table
                 try:
                     self._meta.db_table += suffix
                     instance_save_table(*args, **kwargs)
                 finally:
                     self._meta.db_table = db_table
 
-            instance._save_table = six.create_bound_method(wrapper, instance)
+            instance._save_table = MethodType(wrapper, instance)
 
     def post_save(self, instance, context, **kwargs):
-        u"""Восстанавливает метод _save_table объекта."""
+        """Восстанавливает метод _save_table объекта."""
 
         if '_save_table' in instance.__dict__:
             del instance.__dict__['_save_table']
```

### Comparing `educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py` & `educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from django.db import router
-from m3_django_compat import BaseCommand
-from m3_django_compat import get_model
-
-from educommon.django.db import partitioning
+from django.db import (
+    router,
+)
+from m3_django_compat import (
+    BaseCommand,
+    get_model,
+)
+
+from educommon.django.db import (
+    partitioning,
+)
 
 
 class Command(BaseCommand):
-    u"""Применяет партицирование к таблице переданной модели.
+    """Применяет партицирование к таблице переданной модели.
 
     Команда, если это необходимо, сперва инициализирует средства партицирования
     для БД, в которой хранится переданная модель, а затем создает необходимые
     триггеры. Подробнее см. в `educommon.django.db.partitioning.init` и
     `educommon.django.db.partitioning.set_partitioning_for_model`.
 
     """
     help = 'Applies partitioning to the table.'
 
     def add_arguments(self, parser):
         parser.add_argument(
             'app_label',
-            help=u'App label of an application.',
+            help='App label of an application.',
         )
         parser.add_argument(
             'model_name',
-            help=u'Model name.',
+            help='Model name.',
         )
         parser.add_argument(
             'field_name',
-            help=u'Field name. It will be the partition key.',
+            help='Field name. It will be the partition key.',
         )
 
     def handle(self, *args, **options):
         app_label = options['app_label']
         model_name = options['model_name']
         field_name = options['field_name']
         Model = get_model(app_label, model_name)
```

### Comparing `educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/clear_table.py` & `educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/clear_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from django.core.management.base import CommandError
-from django.db.models.fields import FieldDoesNotExist
-from m3_django_compat import BaseCommand
-from m3_django_compat import get_model
-
-from educommon.django.db import partitioning
+from django.core.management.base import (
+    CommandError,
+)
+from django.db.models.fields import (
+    FieldDoesNotExist,
+)
+from m3_django_compat import (
+    BaseCommand,
+    get_model,
+)
+
+from educommon.django.db import (
+    partitioning,
+)
 
 
 class Command(BaseCommand):
-    u"""Удаляет записи из таблицы БД по условию.
+    """Удаляет записи из таблицы БД по условию.
 
     С помощью данной команды удаляются записи из основной (не секционированной)
     таблицы, у которых значение в field_name меньше значения из before_value.
     Подробнее см. в `educommon.django.db.partitioning.clear_table`.
 
     """
     help = (
```

### Comparing `educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/split_table.py` & `educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/split_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from django.core.management.base import CommandError
-from django.db.models.fields import FieldDoesNotExist
-from m3_django_compat import BaseCommand
-from m3_django_compat import get_model
-
-from educommon.django.db import partitioning
+from django.core.management.base import (
+    CommandError,
+)
+from django.db.models.fields import (
+    FieldDoesNotExist,
+)
+from m3_django_compat import (
+    BaseCommand,
+    get_model,
+)
+
+from educommon.django.db import (
+    partitioning,
+)
 
 
 class Command(BaseCommand):
-    u"""Переносит все записи из таблицы БД в ее разделы.
+    """Переносит все записи из таблицы БД в ее разделы.
 
     Если до включения партиционирования таблицы БД в ней находились записи, то
     с помощью данной команды их можно перенести в соответствующие разделы.
     Подробнее см. в `educommon.django.db.partitioning.split_table`.
 
     """
     help = (
```

### Comparing `educommon-2.20.0/src/educommon/django/db/partitioning/partitioning.sql` & `educommon-3.0.0/src/educommon/django/db/partitioning/partitioning.sql`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/django/db/partitioning/triggers.sql` & `educommon-3.0.0/src/educommon/django/db/partitioning/triggers.sql`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/django/db/routers.py` & `educommon-3.0.0/src/educommon/django/db/routers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# coding: utf-8
-u"""Роутеры для приложений Django."""
-from __future__ import absolute_import
+"""Роутеры для приложений Django."""
+from abc import (
+    ABCMeta,
+)
+
+from django.core.exceptions import (
+    ImproperlyConfigured,
+)
+from m3_django_compat import (
+    DatabaseRouterBase,
+)
 
-from abc import ABCMeta
 
-from django.core.exceptions import ImproperlyConfigured
-from m3_django_compat import DatabaseRouterBase
-import six
-
-
-class ServiceDbRouterBase(six.with_metaclass(ABCMeta, DatabaseRouterBase)):
-
-    u"""Основа роутера для моделей приложений, использующих сервисную БД.
+class ServiceDbRouterBase(DatabaseRouterBase, metaclass=ABCMeta):
+    """Основа роутера для моделей приложений, использующих сервисную БД.
 
     Все модели, имена которых указаны в атрибуте ``service_db_model_names``,
     закрепляет за сервисной БД, а остальные модели приложения закрепляет за
     основной БД. Имя приложения указывается в атрибуте ``app_name``.
 
     Пример использования:
 
@@ -27,37 +28,41 @@
     # имя приложения
     app_name = None
 
     # имена моделей плагина, которые должны храниться в сервисной БД
     service_db_model_names = None
 
     def __init__(self):
-        u"""Определяет алиасы основной и сервисной баз данных."""
-        from django.conf import settings
-        from django.db.utils import DEFAULT_DB_ALIAS
+        """Определяет алиасы основной и сервисной баз данных."""
+        from django.conf import (
+            settings,
+        )
+        from django.db.utils import (
+            DEFAULT_DB_ALIAS,
+        )
 
         aliases = list(settings.DATABASES)
         if len(aliases) != 2:
             # Роутер поддерживает только конфигурации с двумя БД.
             raise ImproperlyConfigured(
-                u'Database router support only two databases'
+                'Database router support only two databases'
             )
 
         self.default_db_alias = DEFAULT_DB_ALIAS
 
         alias_index = 1 if aliases[0] == DEFAULT_DB_ALIAS else 0
         self.service_db_alias = aliases[alias_index]
 
         self.service_db_model_names = {
             model_name.lower()
             for model_name in self.service_db_model_names
         }
 
     def _db_for_model(self, model, **hints):
-        u"""Возвращает имя БД для чтения/записи данных из модели *model*."""
+        """Возвращает имя БД для чтения/записи данных из модели *model*."""
         if model._meta.app_label != self.app_name:
             # модель не имеет отношения к плагину
             return None
         elif model.__name__.lower() in self.service_db_model_names:
             return self.service_db_alias
         else:
             return self.default_db_alias
```

### Comparing `educommon-2.20.0/src/educommon/django/db/utils.py` & `educommon-3.0.0/src/educommon/django/db/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,45 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from copy import deepcopy
-from inspect import isclass
-from weakref import WeakKeyDictionary
 import warnings
+from copy import (
+    deepcopy,
+)
+from inspect import (
+    isclass,
+)
+from weakref import (
+    WeakKeyDictionary,
+)
 
-from django.core.validators import MaxLengthValidator
-from django.db.models.base import ModelBase
-from django.db.models.signals import post_delete
-from django.db.models.signals import post_save
-from django.dispatch.dispatcher import receiver
-from m3_django_compat import ModelOptions
-from m3_django_compat import atomic
-from m3_django_compat import get_model
 import django
-import six
+from django.core.validators import (
+    MaxLengthValidator,
+)
+from django.db.models.base import (
+    ModelBase,
+)
+from django.db.models.signals import (
+    post_delete,
+    post_save,
+)
+from django.dispatch.dispatcher import (
+    receiver,
+)
+from m3_django_compat import (
+    ModelOptions,
+    atomic,
+    get_model,
+)
 
 
 # Кэш оригинальных объектов
 _original_objects_cache = WeakKeyDictionary()
 
 
 def model_modifier_metaclass(meta_base=ModelBase, **params):
-    u"""Возвращает метакласс, изменяющий параметры полей модели.
+    """Возвращает метакласс, изменяющий параметры полей модели.
 
     :param dict params: Словарь с новыми значениями параметров полей. Ключ
         словаря должен содержать имя поля в модели (*field.attname*), а
         значение - словарь с новыми параметрами поля.
 
     .. note::
 
@@ -44,15 +56,15 @@
               }
           }
           class MyModel(BaseModel):
               # Модель с увеличенной до 300 символов длиной поля name.
               __metaclass__ = model_modifier_metaclass(**modified_model_params)
 
               class Meta:
-                  verbose_name = u'Образец справочника'
+                  verbose_name = 'Образец справочника'
     """
     class ModifiedModelBase(meta_base):
         def __new__(cls, name, bases, attrs):
             model = super(ModifiedModelBase, cls).__new__(
                 cls, name, bases, attrs
             )
 
@@ -60,17 +72,17 @@
             attr_overrides = {
                 'unique': '_unique',
                 'error_messages': '_error_messages',
                 'validators': '_validators',
                 'verbose_name': '_verbose_name',
             }
             opts = ModelOptions(model)
-            for field_name, field_params in six.iteritems(params):
+            for field_name, field_params in params.items():
                 field = opts.get_field(field_name)
-                for param_name, param_value in six.iteritems(field_params):
+                for param_name, param_value in field_params.items():
                     assert hasattr(field, param_name), param_name
                     setattr(field, param_name, param_value)
                     if param_name in attr_overrides:
                         setattr(field, attr_overrides[param_name], param_value)
 
                 if 'max_length' in field_params:
                     field.validators = deepcopy(field.validators)
@@ -80,27 +92,27 @@
 
             return model
 
     return ModifiedModelBase
 
 
 def nested_commit_on_success(func):
-    u"""Аналог commit_on_success, не завершающий существующую транзакцию.
+    """Аналог commit_on_success, не завершающий существующую транзакцию.
 
     .. deprecated:: 0.16
 
        Используйте :func:`m3_django_compat.atomic`.
     """
     warnings.warn('Use m3_django_compat.atomic instead', DeprecationWarning)
 
     return atomic(func, savepoint=False)
 
 
 def get_original_object(obj):
-    u"""Возвращает загруженный из БД объект модели.
+    """Возвращает загруженный из БД объект модели.
 
     Если первичный ключ не заполнен, либо в БД нет такого объекта, то
     возвращает None.
     """
     if obj.pk is None:
         result = None
     elif obj in _original_objects_cache:
@@ -116,60 +128,59 @@
 
     return result
 
 
 @receiver(post_delete)
 @receiver(post_save)
 def _clear_cache(instance, **kwargs):
-    u"""Удаляет объект из кэша функции ``get_original_object``."""
+    """Удаляет объект из кэша функции ``get_original_object``."""
     if instance in _original_objects_cache:
         del _original_objects_cache[instance]
 
 
-class LazyModel(object):
-
-    u"""Класс для отложенной загрузки моделей.
+class LazyModel:
+    """Класс для отложенной загрузки моделей.
 
     Предоставляет указывать в аргументах методов модель различными способами и
     единообразно получать доступ к модели. При этом модель может быть указана
     как строка, кортеж или класс модели.
 
     .. hint::
 
        Указание моделей в виде строк и кортежей актуально, когда есть
        потребность избежать прямого импорта моделей. Например, в коде, который
        выполняется до инициализации приложений Django ORM.
 
     .. code-block:: python
        :caption: Пример использования
 
-       class ModelProcessor(object):
+       class ModelProcessor:
            def __init__(self, model):
                self._model = LazyModel(model)
 
            @property
            def model(self):
                return self._model.get_model()
 
        mp1 = ModelProcessor('person.Person')
        mp2 = ModelProcessor(('person', 'Person'))
        mp3 = ModelProcessor(Person)
     """
 
     def __init__(self, model):
         if (
-            isinstance(model, six.string_types) and
+            isinstance(model, str) and
             '.' in model and model.index('.') == model.rindex('.')
         ):
             self.app_label, self.model_name = model.split('.')
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         elif (
             isinstance(model, tuple) and
             len(model) == 2 and
-            all(isinstance(s, six.string_types) for s in model)
+            all(isinstance(s, str) for s in model)
         ):
             self.app_label, self.model_name = model
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         elif (
             isclass(model) and
             hasattr(model, '_meta') and
             hasattr(model._meta, 'app_label') and
@@ -181,77 +192,76 @@
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         else:
             raise ValueError(
                 '"model" argument has invalid value: ' + repr(model)
             )
 
     def get_model(self):
-        u"""Возвращает класс модели, заданной при инициализации."""
+        """Возвращает класс модели, заданной при инициализации."""
         if not hasattr(self, '_model'):
             self._model = get_model(self.app_label, self.model_name)
 
         return self._model
 
 
 if django.VERSION >= (1, 8):
-    from django.db.models.expressions import Func
-    from django.db.models.lookups import Lookup
+    from django.db.models.expressions import (
+        Func,
+    )
+    from django.db.models.lookups import (
+        Lookup,
+    )
 
     class SmartExact(Func):
+        """Удаляет пробелы из строки и заменяет буквы ё на е."""
 
-        u"""Удаляет пробелы из строки и заменяет буквы ё на е."""
-
-        template = u"TRANSLATE(%(expressions)s, 'ёЁ ', 'еЕ')"
+        template = "TRANSLATE(%(expressions)s, 'ёЁ ', 'еЕ')"
 
     class SmartExactLookup(Lookup):
-
-        u"""Удаляет пробелы из строки и заменяет буквы ё на е."""
+        """Удаляет пробелы из строки и заменяет буквы ё на е."""
 
         lookup_name = 'smart_exact'
 
         def as_postgresql(self, compiler, connection):
             lhs, lhs_params = self.process_lhs(compiler, connection)
             rhs, rhs_params = self.process_rhs(compiler, connection)
 
-            sql = u"TRANSLATE(%s, 'ёЁ ', 'еЕ')"
-            sql = u'{sql} = {sql}'.format(sql=sql)
+            sql = "TRANSLATE(%s, 'ёЁ ', 'еЕ')"
+            sql = '{sql} = {sql}'.format(sql=sql)
 
             return sql % (lhs, rhs), lhs_params + rhs_params
 
     class SmartIExact(Func):
+        """Переводит в верхний регистр, удаляет пробелы, заменяет Ё на Е."""
 
-        u"""Переводит в верхний регистр, удаляет пробелы, заменяет Ё на Е."""
-
-        template = u"TRANSLATE(UPPER(%(expressions)s), 'Ё ', 'Е')"
+        template = "TRANSLATE(UPPER(%(expressions)s), 'Ё ', 'Е')"
 
     class SmartIExactLookup(Lookup):
-
-        u"""Переводит в верхний регистр, удаляет пробелы, заменяет Ё на Е."""
+        """Переводит в верхний регистр, удаляет пробелы, заменяет Ё на Е."""
 
         lookup_name = 'smart_iexact'
 
         def as_postgresql(self, compiler, connection):
             lhs, lhs_params = self.process_lhs(compiler, connection)
             rhs, rhs_params = self.process_rhs(compiler, connection)
 
-            sql = u"TRANSLATE(UPPER(%s), 'Ё ', 'Е')"
-            sql = u'{sql} = {sql}'.format(sql=sql)
+            sql = "TRANSLATE(UPPER(%s), 'Ё ', 'Е')"
+            sql = '{sql} = {sql}'.format(sql=sql)
 
             return sql % (lhs, rhs), lhs_params + rhs_params
 
     class SmartIContainsLookup(Lookup):
-
-        u"""
+        """
         Переводит в верхний регистр, удаляет пробелы, заменяет Ё на Е,
         проверяет вхождение текста.
         """
 
         lookup_name = 'smart_icontains'
 
         def as_postgresql(self, compiler, connection):
             lhs, lhs_params = self.process_lhs(compiler, connection)
             rhs, rhs_params = self.process_rhs(compiler, connection)
 
-            sql = u"TRANSLATE(UPPER(%s), 'Ё ', 'Е')"
-            sql = u"{sql} like '%%%%' || {sql} || '%%%%'".format(sql=sql)
+            sql = "TRANSLATE(UPPER(%s), 'Ё ', 'Е')"
+            sql = "{sql} like '%%%%' || {sql} || '%%%%'".format(sql=sql)
 
             return sql % (lhs, rhs), lhs_params + rhs_params
```

### Comparing `educommon-2.20.0/src/educommon/django/db/validators/__init__.py` & `educommon-3.0.0/src/educommon/django/db/validators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# coding: utf-8
-u"""Валидаторы для полей моделей Django.
+"""Валидаторы для полей моделей Django.
 
 Документация: http://djbook.ru/rel1.4/ref/validators.html
 """
-from __future__ import absolute_import
-
-from abc import ABCMeta
-from abc import abstractmethod
-
-from django.core.exceptions import ValidationError
-from six import with_metaclass
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
+
+from django.core.exceptions import (
+    ValidationError,
+)
 
 
 def validate_value(value, validator):
-    u"""Выполняет проверку значения value с помощью валидатора validator.
+    """Выполняет проверку значения value с помощью валидатора validator.
 
     Удобно использовать при проверке валидаторами значений вне модели,
     например так:
 
         from functools import partial
         is_snils_valid = partial(validate_value, validator=snils_validator)
         if is_snils_valid('064-949-063 00'):
@@ -36,20 +36,20 @@
         validator(value)
     except ValidationError:
         return False
     else:
         return True
 
 
-class IModelValidator(with_metaclass(ABCMeta, object)):
-    u"""Базовый класс валидатора модели."""
+class IModelValidator(metaclass=ABCMeta):
+    """Базовый класс валидатора модели."""
 
     @abstractmethod
     def clean(self, instance, errors):
-        u"""Валидирует объект.
+        """Валидирует объект.
 
         :param instance: экземпляр проверяемой модели.
         :type instance: django.db.models.base.Model
 
         :param errors: ошибки, выявленные в ходе проверки.
         :type errors: collections.OrderedDict
         """
```

### Comparing `educommon-2.20.0/src/educommon/django/db/validators/simple.py` & `educommon-3.0.0/src/educommon/django/db/validators/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-# coding: utf-8
 """Валидаторы для простых (текстовых, числовых и т.п.) полей модели Django."""
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from datetime import datetime
-from functools import partial
-from itertools import cycle
 import re
+from datetime import (
+    datetime,
+)
+from functools import (
+    partial,
+)
+from itertools import (
+    cycle,
+)
 
-from django.core.exceptions import NON_FIELD_ERRORS
-from django.core.exceptions import ValidationError
-from django.core.validators import DecimalValidator
-from django.core.validators import RegexValidator
-from django.utils.deconstruct import deconstructible
-from six.moves import range
-from six.moves import zip
 import magic
-import six
-
-from educommon.utils.misc import get_mime_type_for_extension
-
-from . import IModelValidator
-from . import validate_value
-from ..utils import get_original_object
+from django.core.exceptions import (
+    NON_FIELD_ERRORS,
+    ValidationError,
+)
+from django.core.validators import (
+    DecimalValidator,
+    RegexValidator,
+)
+from django.utils.deconstruct import (
+    deconstructible,
+)
+
+from educommon.django.db.utils import (
+    get_original_object,
+)
+from educommon.django.db.validators import (
+    IModelValidator,
+    validate_value,
+)
+from educommon.utils.misc import (
+    get_mime_type_for_extension,
+)
 
 
 # =============================================================================
 # СНИЛС
 # =============================================================================
 _snils_re = re.compile(r'^\d{3}-\d{3}-\d{3} \d{2}$')  # СНИЛС
 
@@ -46,15 +56,15 @@
 
     def __call__(self, value):
         super(SNILSValidator, self).__call__(value)
         snils_checksum_validator(value)
 
 
 def snils_checksum_validator(value):
-    value = six.text_type(value)
+    value = str(value)
 
     if value[:11] <= '001-001-998':
         return
 
     numbers = (int(ch) for ch in reversed(value[:11]) if ch.isdigit())
     checksum = int(value[12:14])
     summa = sum(i * n for i, n in enumerate(numbers, 1))
@@ -67,15 +77,15 @@
 
 
 regex_snils_validator = SNILSValidator()
 
 
 # для совместимости со старым валидатором-функцией
 def snils_validator(value):
-    value = six.text_type(value)
+    value = str(value)
 
     regex_snils_validator(value)
 
 
 is_snils_valid = partial(validate_value, validator=snils_validator)
 
 
@@ -95,15 +105,15 @@
 
     Проверяет корректность формата и контрольное число (последняя цифра).
 
     :raises django.core.exceptions.ValidationError: Если аргумент value
         содержит значение, несоответствующее формату ИНН, либо не пройдена
         проверка контрольного числа.
     """
-    value = six.text_type(value)
+    value = str(value)
 
     if len(value) != 10 or not value.isdigit():
         raise ValidationError('ИНН должен быть 10-ти значным числом')
 
     _check_inn_checksum((2, 4, 10, 3, 5, 9, 4, 6, 8),
                         (int(ch) for ch in value[:-1]),
                         int(value[-1]))
@@ -114,15 +124,15 @@
 
     Проверяет корректность формата и контрольное число (последние 2 цифры).
 
     :raises django.core.exceptions.ValidationError: Если аргумент value
         содержит значение, несоответствующее формату ИНН, либо не пройдена
         проверка контрольного числа.
     """
-    value = six.text_type(value)
+    value = str(value)
 
     if len(value) != 12 or not value.isdigit():
         raise ValidationError('ИНН должен быть 12-ти значным числом')
 
     _check_inn_checksum((7, 2, 4, 10, 3, 5, 9, 4, 6, 8),
                         (int(ch) for ch in value[:-2]),
                         int(value[-2]))
@@ -138,15 +148,15 @@
     Проверяет корректность формата и контрольное число (1 или 2 последние
     цифры).
 
     :raises django.core.exceptions.ValidationError: Если аргумент value
         содержит значение, несоответствующее формату ИНН, либо не пройдена
         проверка контрольного числа.
     """
-    value = six.text_type(value)
+    value = str(value)
 
     if len(value) not in (10, 12) or not value.isdigit():
         raise ValidationError('ИНН должен быть 10-ти или 12-ти значным числом')
 
     if len(value) == 10:
         inn10_validator(value)
     else:
@@ -161,15 +171,15 @@
 # =============================================================================
 # КПП, ОКАТО, ОКТМО, ОКПО, ОГРН, ОКВЭД, ОКОПФ, ОКФС
 # =============================================================================
 
 
 def kpp_validator(value):
     """Валидатор для КПП (кода причины постановки на налоговый учет)."""
-    value = six.text_type(value)
+    value = str(value)
 
     if len(value) != 9 or not value.isdigit():
         raise ValidationError('КПП должен быть 9-ти значным числом')
 
 
 is_kpp_valid = partial(validate_value, validator=kpp_validator)
 
@@ -223,15 +233,15 @@
 
     ОКАТО - общероссийский классификатор объектов административно-
     территориального деления.
 
     .. seealso::
        `Контрольное число ОКАТО <http://kontragent.info/articles/okato>`_
     """
-    value = six.text_type(value)
+    value = str(value)
 
     if not value.isdigit():
         raise ValidationError('ОКАТО должен состоять только из цифр')
 
     value_length = len(value)
     if value_length in (3, 6, 9, 12):
         # В последнем разряде указано контрольное число, проверим его
@@ -248,15 +258,15 @@
 
 
 def oktmo_validator(value):
     """Валидатор для ОКТМО.
 
     ОКТМО - Общероссийский классификатор территорий муниципальных образований.
     """
-    value = six.text_type(value)
+    value = str(value)
 
     if not value.isdigit():
         raise ValidationError('ОКТМО должен состоять только из цифр')
 
     value_length = len(value)
     if value_length not in (2, 5, 8, 11):
         raise ValidationError(
@@ -268,15 +278,15 @@
 
 
 def okpo_validator(value):
     """Валидатор кода ОКПО.
 
     ОКПО - Общероссийский классификатор предприятий и организаций.
     """
-    value = six.text_type(value)
+    value = str(value)
 
     if not value.isdigit():
         raise ValidationError('ОКПО должен состоять только из цифр')
 
     value_length = len(value)
     if value_length not in (8, 10):
         raise ValidationError('ОКПО должен состоять из 8-ми или 10-ти цифр')
@@ -298,23 +308,23 @@
     control_number = int(value[-1])  # контрольное число
 
     if number % divisor % 10 != control_number:
         raise ValidationError('Не пройдена проверка контрольного числа')
 
 
 def _ogrn_validator(value, valid_length, title):
-    value = six.text_type(value)
+    value = str(value)
 
     if not value.isdigit():
         raise ValidationError('ОГРН должен состоять только из цифр')
     if len(value) not in valid_length:
         raise ValidationError(
             '{} должен состоять из {} цифр!'.format(
                 title,
-                ' или '.join(six.text_type(l) for l in valid_length)
+                ' или '.join(str(l) for l in valid_length)
             )
         )
 
     _check_ogrn_checksum(value)
 
 
 def ogrn13_validator(value):
@@ -352,15 +362,15 @@
 
 
 def okved_validator(value):
     """Валидатор кода ОКВЭД.
 
     ОКВЭД - Общероссийский классификатор видов экономической деятельности.
     """
-    value = six.text_type(value)
+    value = str(value)
 
     if not value.isdigit():
         raise ValidationError('ОКВЭД должен состоять только из цифр')
 
     value_length = len(value)
     if value_length < 2 or 6 < value_length:
         raise ValidationError(
@@ -375,15 +385,15 @@
 
 
 def okopf_validator(value):
     """Валидатор кода ОКОПФ.
 
     ОКОПФ - Общероссийский классификатор организационно-правовых форм.
     """
-    value = six.text_type(value)
+    value = str(value)
 
     if not value.isdigit():
         raise ValidationError('ОКОПФ должен состоять только из цифр')
 
     value_length = len(value)
     if value_length != 5:
         raise ValidationError('Код ОКОПФ должен состоять из 5-ти цифр')
@@ -393,15 +403,15 @@
 
 
 def okfs_validator(value):
     """Валидатор кода ОКФС.
 
     ОКФС - Общероссийский классификатор форм собственности.
     """
-    value = six.text_type(value)
+    value = str(value)
 
     if not value.isdigit():
         raise ValidationError('ОКФС должен состоять только из цифр')
 
     value_length = len(value)
     if value_length != 2:
         raise ValidationError('Код ОКФС должен состоять из 2-ти цифр')
@@ -426,16 +436,15 @@
     if file_mime_type not in allowed_mime_types:
         raise ValidationError(
             'Mime type файла не соотвествует допустимым в системе'
         )
 
 
 @deconstructible
-class FileMimeTypeValidator(object):
-
+class FileMimeTypeValidator:
     """Валидатор для FileField модели проверяющий mimetype файла."""
 
     message = (
         'Mime type файла не допустим для загрузки в системе.'
     )
     code = 'invalid_mimetype'
 
@@ -949,15 +958,15 @@
     regex = r'^[а-яА-ЯёЁ]+([а-яА-ЯёЁ]*[\,]?[\s]{1}[а-яА-ЯёЁ]+)*$'
 
 
 regex_doc_type_validator = DocumentTypeValidator()
 
 
 def doc_type_validator(value):
-    value = six.text_type(value)
+    value = str(value)
 
     regex_doc_type_validator(value)
 
 
 is_doc_type_valid = partial(validate_value, validator=doc_type_validator)
```

### Comparing `educommon-2.20.0/src/educommon/django/storages/atcfs/README.rst` & `educommon-3.0.0/src/educommon/django/storages/atcfs/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/django/storages/atcfs/api.py` & `educommon-3.0.0/src/educommon/django/storages/atcfs/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import cgi
 import hashlib
 import re
 import uuid
+from urllib.parse import (
+    unquote,
+)
 
 import requests
-import six.moves.urllib.error
-import six.moves.urllib.parse
-import six.moves.urllib.request
 
-from . import settings
-from .exceptions import AtcfsUnavailable
+from educommon.django.storages.atcfs import (
+    settings,
+)
+from educommon.django.storages.atcfs.exceptions import (
+    AtcfsUnavailable,
+)
 
 
-class AtcfsApi(object):
+class AtcfsApi:
     """
     Класс для работы с запросами к ATCFS
     """
 
     def _build_url(self, *args):
         """
         Функция составления полного урла.
         :param args: составные части пути
         :return: фбсолютный урл
         """
         chunks = (settings.URL,) + args
-        url = u'/'.join(chunks)
+        url = '/'.join(chunks)
         return url
 
     def _get_credential_headers(self):
         """
         Метод генерации данных для аутентификации на сервере ATCFS.
         :return: словарь с необходимыми для атунетификации полями
         """
@@ -117,15 +118,15 @@
             raise Exception(response.text)
         _, params = cgi.parse_header(
             response.headers.get('Content-Disposition')
         )
         file_name = params['filename*']
         try:
             file_name = re.findall(r'UTF-8\'\'(.*)', file_name)[0]
-            file_name = six.moves.urllib.parse.unquote(file_name).decode('UTF-8')
+            file_name = unquote(file_name)
         except IndexError:
             pass
         file_content = response.content
         return file_name, file_content
 
     def delete_file(self, ident):
         """
```

### Comparing `educommon-2.20.0/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py` & `educommon-3.0.0/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import print_function
-
-from importlib import import_module
-from optparse import make_option
 import inspect
 import os
-
-from django.conf import settings
-from django.core.management.base import NoArgsCommand
-from django.db import connection
-from django.db.models.base import ModelBase
-from django.db.models.fields.files import FileDescriptor
-from m3_django_compat import commit_unless_managed
-from six.moves import zip
-import six
-
-from educommon.django.storages.atcfs.api import AtcfsApi
+from importlib import (
+    import_module,
+)
+
+from django.conf import (
+    settings,
+)
+from django.core.management import (
+    BaseCommand,
+)
+from django.db import (
+    connection,
+)
+from django.db.models.base import (
+    ModelBase,
+)
+from django.db.models.fields.files import (
+    FileDescriptor,
+)
+from m3_django_compat import (
+    commit_unless_managed,
+)
+
+from educommon.django.storages.atcfs.api import (
+    AtcfsApi,
+)
 
 
 def dictfetchall(cursor):
     """
     Вспомогательная функция.
     cursor.fetchall возвращает данные в виде списка списков:
     (('43', 'text 1'), ('44', 'text 2'), ('45', 'text 3'))
@@ -30,44 +39,43 @@
     :return: список словарей
     """
     desc = cursor.description
     columns = [col[0] for col in desc]
     return [dict(list(zip(columns, row))) for row in cursor.fetchall()]
 
 
-class Command(NoArgsCommand):
+class Command(BaseCommand):
     """
     Команда обходит все зарегистрированные модели,
     в которых есть поля FileField.
     Если для поля установлен AtcfsStorage, или он установлен глобально,
     то файл переносится на сервер ATCFS.
     """
 
-    option_list = NoArgsCommand.option_list + (
-        make_option(
+    def add_arguments(self, parser):
+        parser.add_argument(
             '--delete',
             action='store_true',
             dest='delete',
             default=False,
-            help=u'Удалять файлы вместо перемещения.'
-        ),
-    )
+            help='Удалять файлы вместо перемещения.',
+        )
 
     def __init__(self):
         super(Command, self).__init__()
         self.api = AtcfsApi()
 
     def _get_fields(self, model):
         """
         Выбираем в модели все переменные, являющиеся FileField-полями.
         :param model: класс модели
         :return: список названий полей FileField
         """
         fields = []
-        for nam, mem in six.iteritems(model.__dict__):
+        for nam, mem in model.__dict__.items():
             if callable(mem):
                 continue
             if nam.startswith('_'):
                 continue
             if isinstance(mem, FileDescriptor):
                 fields.append(nam)
         return fields
@@ -100,26 +108,26 @@
         return models
 
     def _delete_all_files(self, models):
         """
         Сервисный метод. Используется для технических нужд.
         В работе команды не учавствует.
         """
-        for model, fields in six.iteritems(models):
+        for model, fields in models.items():
             kwargs = dict(list(zip(fields, ['']*len(fields))))
             cnt = model.objects.all().update(**kwargs)
-            print(u'{0}: {1}'.format(model, cnt))
+            print('{0}: {1}'.format(model, cnt))
 
     def _send_file(self, file_name):
         """
         Непосредственная отправка файла на ATCFS.
         :param file_name: название файла
         :return: идентификатор файла в ATCFS
         """
-        ident = u''
+        ident = ''
         file_path = os.path.join(settings.MEDIA_ROOT, file_name)
         try:
             with open(file_path, 'r') as fd:
                 ident = self.api.upload_file(
                     os.path.basename(file_name), fd.read()
                 )
         except IOError:
@@ -130,19 +138,19 @@
         """
         Запрашиваем из базы напрямую объекты по модели.
         :param model: класс модели
         :param fields: список полей
         :return: список словарей в которых id и значения полей
         """
         cursor = connection.cursor()
-        select_fields = u', '.join(fields)
-        where_fields = u' OR '.join(
-            [u'COALESCE({0}, \'\') <> \'\''.format(field) for field in fields]
+        select_fields = ', '.join(fields)
+        where_fields = ' OR '.join(
+            ['COALESCE({0}, \'\') <> \'\''.format(field) for field in fields]
         )
-        sql = u'SELECT id, {0} from {1} WHERE {2};'.format(
+        sql = 'SELECT id, {0} from {1} WHERE {2};'.format(
             select_fields,
             model._meta.db_table,
             where_fields
         )
         cursor.execute(sql)
         objs = dictfetchall(cursor)
         return objs
@@ -151,55 +159,55 @@
         """
         Изменяем значения полей в базе.
         :param model: класс модели
         :param objs: словарь списков, где ключ - id объекта,
         а значение - список тюплов (название, значение)
         """
         cursor = connection.cursor()
-        sql = u''
-        for obj_id, obj_fields in six.iteritems(objs):
-            set_fields = u', '.join(
-                [u'{0[0]} = \'{0[1]}\''.format(field) for field in obj_fields]
+        sql = ''
+        for obj_id, obj_fields in objs.items():
+            set_fields = ', '.join(
+                ['{0[0]} = \'{0[1]}\''.format(field) for field in obj_fields]
             )
-            sql += u'UPDATE {0} SET {1} WHERE id = {2};'.format(
+            sql += 'UPDATE {0} SET {1} WHERE id = {2};'.format(
                 model._meta.db_table,
                 set_fields,
                 obj_id
             )
         if sql:
             cursor.execute(sql)
             commit_unless_managed()
 
     def _migrate_all_files(self, models):
         """
         Проходимся по всем моделям, всем объектам, отсылаем файлы на ATCFS.
         :param models: модели, в которых есть FileField
         """
         total = len(models)
-        for i, (model, fields) in enumerate(six.iteritems(models), start=1):
+        for i, (model, fields) in enumerate(models.items(), start=1):
             print(self.style.SQL_KEYWORD(
-                u'{0} ({1}/{2})'.format(model, i, total)
+                '{0} ({1}/{2})'.format(model, i, total)
             ))
             objs = self._get_objs(model, fields)
             updated_objs = {}
             for obj in objs:
                 updated_fields = []
                 for field_name in fields:
                     field_value = obj[field_name]
                     if field_value:
                         ident = self._send_file(field_value)
                         updated_fields.append((field_name, ident))
-                        print(u'{0},{1},{2},{3}'.format(
+                        print('{0},{1},{2},{3}'.format(
                             obj['id'],
                             field_name.decode('UTF-8'),
                             field_value.decode('UTF-8'),
                             ident.decode('UTF-8')
                         ))
                 updated_objs[obj['id']] = updated_fields
             self._update_objs(model, updated_objs)
 
-    def handle_noargs(self, **options):
+    def handle(self, *args, **options):
         models = self._get_models()
         if options['delete']:
             self._delete_all_files(models)
         else:
             self._migrate_all_files(models)
```

### Comparing `educommon-2.20.0/src/educommon/django/storages/atcfs/monkey_patching.py` & `educommon-3.0.0/src/educommon/django/storages/atcfs/monkey_patching.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# coding: utf-8
 """
 Внедряем в джанговский дефолтный FieldFile необходимый функционал
 для работы с AtcfsStorage.
 """
-from __future__ import absolute_import
-
 import re
 
-from django.core.files.storage import DefaultStorage
-from django.core.files.storage import get_storage_class
-from django.db.models.fields import files
-from django.utils.encoding import smart_str
-from django.utils.encoding import smart_unicode
+from django.core.files.storage import (
+    DefaultStorage,
+    get_storage_class,
+)
+from django.db.models.fields import (
+    files,
+)
 
-from .storage import AtcfsStorage
+from educommon.django.storages.atcfs.storage import (
+    AtcfsStorage,
+)
 
 
 DEFAULT_FILE_STORAGE = get_storage_class()
 
 
 def is_atcfs_storage(storage):
     """
@@ -49,45 +50,32 @@
 
 def new_field_file__init__(self, instance, field, name):
     old_field_file__init__(self, instance, field, name)
     if is_atcfs_storage(self.storage):
         if self.name and uuid_re.match(self.name):
             self.file_name = self.storage.name(self.name)
         else:
-            self.file_name = u''
+            self.file_name = ''
 
 files.FieldFile.__init__ = new_field_file__init__
 
 
 # Переопределяем __str__ FieldFile.
 
 old_field_file__str__ = files.FieldFile.__str__
 
 def new_field_file__str__(self):
     if is_atcfs_storage(self.storage):
-        return smart_str(self.file_name or '')
+        return self.file_name or ''
     else:
         return old_field_file__str__(self)
 
 files.FieldFile.__str__ = new_field_file__str__
 
 
-# Переопределяем __unicode__ FieldFile.
-
-old_field_file__unicode__ = files.FieldFile.__unicode__
-
-def new_field_file__unicode__(self):
-    if is_atcfs_storage(self.storage):
-        return smart_unicode(self.file_name or u'')
-    else:
-        return old_field_file__unicode__
-
-files.FieldFile.__unicode__ = new_field_file__unicode__
-
-
 # Переопределяем get_prep_value FileField.
 
 old_file_field_get_prep_value = files.FileField.get_prep_value
 
 def new_file_field_get_prep_value(self, value):
     if is_atcfs_storage(self.storage):
         if value is None:
```

### Comparing `educommon-2.20.0/src/educommon/django/storages/atcfs/settings.py` & `educommon-3.0.0/src/educommon/django/storages/atcfs/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
+from django.conf import (
+    settings,
+)
+from django.core.exceptions import (
+    ImproperlyConfigured,
+)
 
 
 try:
     URL = settings.ATCFS_CONF['URL'].rstrip('/')
     VIS_ID = settings.ATCFS_CONF['VIS_ID']
     VIS_USER = settings.ATCFS_CONF['VIS_USER']
     SECRET_KEY = settings.ATCFS_CONF['SECRET_KEY']
 except (AttributeError, KeyError):
-    msg = u'settings.ATCFS_CONF is improperly configured.'
+    msg = 'settings.ATCFS_CONF is improperly configured.'
     raise ImproperlyConfigured(msg)
 
 # Constants
 FILES_PATH = 'files'
 FILE_INFO_PATH = 'fileinfo'
 TMP_FILE_LINK_PATH = 'tmpFileLink'
 TMP_FILES_PATH = 'tmpFiles'
```

### Comparing `educommon-2.20.0/src/educommon/django/storages/atcfs/storage.py` & `educommon-3.0.0/src/educommon/django/storages/atcfs/storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,41 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import datetime
 import os
 import tempfile
 
-from django.core.files import File
-from django.core.files.storage import Storage
-from django.core.urlresolvers import reverse
-from m3 import ApplicationLogicException
-
-from .api import AtcfsApi
-from .exceptions import AtcfsUnavailable
+from django.core.files import (
+    File,
+)
+from django.core.files.storage import (
+    Storage,
+)
+from django.urls import (
+    reverse,
+)
+from m3 import (
+    ApplicationLogicException,
+)
+
+from educommon.django.storages.atcfs.api import (
+    AtcfsApi,
+)
+from educommon.django.storages.atcfs.exceptions import (
+    AtcfsUnavailable,
+)
 
 
 # Сообщение, выдаваемое в интерфейс при сохранении если сервер недоступен.
-ATCFS_UNAVAILABLE_MSG = u'''
+ATCFS_UNAVAILABLE_MSG = '''
 Извините, в настоящий момент внешнее файловое хранилище недоступно,
 сохранение приложенного файла невозможно. Пожалуйста, повторите действие позже
 или удалите приложенный файл перед сохранением.
 '''
 
 # Ссылка на файл и имя, когда недоступен сервер.
-UNAVAILABLE_FILE_NAME = u'Файл недоступен (сбой в работе файлового хранилища)'
+UNAVAILABLE_FILE_NAME = 'Файл недоступен (сбой в работе файлового хранилища)'
 
 
 class AtcfsStorage(Storage):
     """
     ATCFS Storage
     """
```

### Comparing `educommon-2.20.0/src/educommon/extjs/fields/input_params.py` & `educommon-3.0.0/src/educommon/extjs/fields/input_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# coding: utf-8
-u"""Параметры фильтрации ввода для различного типа полей (ИНН, СНИЛС и тд.).
+"""Параметры фильтрации ввода для различного типа полей (ИНН, СНИЛС и тд.).
 from __future__ import absolute_import
 
 Примеры использования:
 
     from educommon.extjs.fields.input_params import snils_field_params
 
     snils_field = ExtStringField(name='person.snils',
-                                 label=u'Номер СНИЛС',
+                                 label='Номер СНИЛС',
                                  **snils_field_params)
 """
 
 # параметры для поля ввода СНИЛС
 snils_field_params = dict(
     input_mask='###-###-### ##',
     regex=r'^\d{3}-\d{3}-\d{3} \d{2}$'
@@ -33,36 +32,36 @@
 inn12_field_params = dict(
     input_mask='############',
     regex=r'^\d{12}$'
 )
 
 children_document_series_field_params = dict(
     input_mask='****-ZZ',
-    regex=u'^[A-Za-z0-9]{1,4}-[А-ЯA-Z]{2}$'
+    regex='^[A-Za-z0-9]{1,4}-[А-ЯA-Z]{2}$'
 )
 
 children_document_number_field_params = dict(
     input_mask='#' * 6,
-    regex=u'^\d{6}$'
+    regex='^\d{6}$'
 )
 
 delegate_document_series_field_params = dict(
     input_mask='#' * 4,
-    regex=u'^\d{4}$'
+    regex='^\d{4}$'
 )
 
 delegate_document_number_field_params = dict(
     input_mask='#' * 6,
-    regex=u'^\d{6}$'
+    regex='^\d{6}$'
 )
 
 url_field_params = dict(
-    regex=u"^((http|https)\:\/\/)([^\s]*)$",
-    invalid_text=u'Адрес сайта должен начинаться с http:// '
-         u'или https:// и не должен содержать пробелов',
+    regex="^((http|https)\:\/\/)([^\s]*)$",
+    invalid_text='Адрес сайта должен начинаться с http:// '
+         'или https:// и не должен содержать пробелов',
 )
 
 # Параметры поля для ввода имён.
 name_field_params = dict(
     mask_re='[- \\\'а-яёА-ЯЁ]',
 )
```

### Comparing `educommon-2.20.0/src/educommon/importer/XLSReader.py` & `educommon-3.0.0/src/educommon/importer/XLSReader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import print_function
-
-from datetime import datetime
 import re
 import uuid
+from datetime import (
+    datetime,
+)
 
-from django.core.exceptions import ValidationError
-from six.moves import filter
-from six.moves import range
-from xlrd.xldate import XLDateAmbiguous
-from xlrd.xldate import XLDateBadDatemode
-from xlrd.xldate import XLDateNegative
-from xlrd.xldate import XLDateTooLarge
-import six
 import xlrd
+from django.core.exceptions import (
+    ValidationError,
+)
+from xlrd.xldate import (
+    XLDateAmbiguous,
+    XLDateBadDatemode,
+    XLDateNegative,
+    XLDateTooLarge,
+)
 
 
 SUBTREE_CAN_BE_EMPTY = '__grp_can_be_empty'
 START_ROW = '__start_row'
 HEADER_PARSER = '__header_parser'
 END_ROW = '__end_row_end_row'
 
@@ -40,15 +39,15 @@
 
     if not group:
         if tree.get(SUBTREE_CAN_BE_EMPTY, False):
             group = uuid.uuid4()
 
     path = ('%s/%%s' % path) if path else '%s'
     res = []
-    for key, val in six.iteritems(tree):
+    for key, val in tree.items():
         if key in _SPECIAL_KEYS:
             continue
         key = path % key
         res.extend(_fold(val, key, group))
     return res
 
 
@@ -102,21 +101,22 @@
 
 class EmptyObligatoryCellError(CellValueError):
     """
     Исключение для неверного значения ячейки
     """
     def __init__(self, message=None):
         super(EmptyObligatoryCellError, self).__init__(
-            message or u'Ячейка не может быть пустой!')
+            message or 'Ячейка не может быть пустой!')
 
 
-class BaseCell(object):
+class BaseCell:
     """
     Прототип парсера ячейки
     """
+
     _default = _NO_DEFAULT
 
     def __init__(self, default=_NO_DEFAULT):
         self._default = default
 
     def default(self):
         return (self._default, True)
@@ -124,56 +124,56 @@
     def result(self, value):
         return (value, False)
 
     def _parse(self, value):
         """
         Разбор значения
         """
-        raise NotImplementedError(u'Прототип не используется напрямую!')
+        raise NotImplementedError('Прототип не используется напрямую!')
 
     def from_cell(self, sheet, row, col):
         """
         Получение значения из ячейки в виде (значение, is_default)
         """
         try:
             value = sheet.cell(row, col).value
         except IndexError:
             if self.is_obligatory():
                 raise EmptyObligatoryCellError()
             return self.default()
 
-        if isinstance(value, six.string_types):
+        if isinstance(value, str):
             value = value.strip()
 
         if value is None or value == "":
             if self.is_obligatory():
                 raise EmptyObligatoryCellError()
             return self.default()
 
-        return self._parse(six.text_type(value))
+        return self._parse(str(value))
 
     def is_obligatory(self):
         return self._default == _NO_DEFAULT
 
 
 class StringCell(BaseCell):
     """
     Строковая ячейка
     """
 
     MSG_RECORD_TRUNCATED = (
-        u'Превышена максимально допустимая длина записи. Запись сокращена'
+        'Превышена максимально допустимая длина записи. Запись сокращена'
     )
 
-    DEFAULT_RE_MESSAGE = u'Неправильный формат записи'
+    DEFAULT_RE_MESSAGE = 'Неправильный формат записи'
 
     def __init__(
             self, default=_NO_DEFAULT, max_length=None, regex=None,
             validator=None, error_message=None, verbose=True):
-        u"""Строковая ячейка.
+        """Строковая ячейка.
 
         :param int max_length: Максимальная длина строки.
         :param regex: Регулярное выражение для проверки значения.
         :param validator: Регулярное выражение для проверки значения.
         :param error_message: Сообщение в случае провала проверки.
         :param bool verbose: Записывать ли сообщения в лог.
         """
@@ -186,54 +186,54 @@
         self._regex = regex
         self._validator = validator
         self._error_message = error_message
 
         self.message = None
 
     def set_mgs(self, msg):
-        self.message = self.message or u'' + msg
+        self.message = self.message or '' + msg
 
     def _validate(self, value):
-        u"""Выплоняет проверку по регулярному выражению.
+        """Выплоняет проверку по регулярному выражению.
 
         Если проверка не пройдена и ячейка обязательна, то райзит
         CellValueError. Если ячейка не обязательна, то она пропускается и
         пишется в лог, если verbose == True.
         """
         if self._regex:
             if not self._regex.match(value):
                 message = self._error_message or self.DEFAULT_RE_MESSAGE
 
                 if self._default is None:
                     if self._verbose:
                         self.set_mgs(message)
-                    value = u''
+                    value = ''
 
                 elif self._default is _NO_DEFAULT:
                     raise CellValueError(message)
 
         elif self._validator:
             try:
                 self._validator(value)
 
             except ValidationError as err:
                 if self._default is None:
                     if self._verbose:
                         self.set_mgs(
-                            u', '.join(err.messages)
+                            ', '.join(err.messages)
                         )
-                    value = u''
+                    value = ''
 
                 elif self._default is _NO_DEFAULT:
-                    raise CellValueError(u', '.join(err.messages))
+                    raise CellValueError(', '.join(err.messages))
 
         return value
 
     def _truncate(self, value):
-        u"""Обрезает строку до указанной в self._max_length длины."""
+        """Обрезает строку до указанной в self._max_length длины."""
         new_value = value[:self._max_length]
         if self._verbose and new_value != value:
             self.set_mgs(self.MSG_RECORD_TRUNCATED)
         return new_value
 
     def _parse(self, value):
 
@@ -247,25 +247,25 @@
 
         if self._max_length is not None:
             value = self._truncate(value)
 
         if self._regex is not None or self._validator is not None:
             value = self._validate(value)
 
-        return self.result(six.text_type(value))
+        return self.result(str(value))
 
 
 class MaybeStringCell(StringCell):
     """
     Строка или None
     """
     def __init__(
             self, default=None, max_length=None, regex=None,
             validator=None, error_message=None, verbose=True):
-        u"""Строка или None.
+        """Строка или None.
 
         :param int max_length: Максимальная длина строки.
         :param regex: Регулярное выражение для проверки значения.
         :param validator: Регулярное выражение для проверки значения.
         :param error_message: Сообщение в случае провала проверки.
         :param bool verbose: Записывать ли сообщения в лог.
         """
@@ -277,15 +277,15 @@
 class RawCell(BaseCell):
     """
     Сырая строковая ячейка "как есть",
     в том числе с добавками Excel в зависимости
     от типа ячейки
     """
     def _parse(self, value):
-        return self.result(six.text_type(value))
+        return self.result(str(value))
 
 
 class MaybeRawCell(RawCell):
     """
     Сырая строковая ячейка "как есть" или None
     """
     def __init__(self):
@@ -300,15 +300,15 @@
         try:
             result = int(value)
         except (TypeError, ValueError):
             try:
                 result = int(float(value))
             except (TypeError, ValueError):
                 raise CellValueError(
-                    u'Число имеет неверный формат! "%s"' % value)
+                    'Число имеет неверный формат! "%s"' % value)
         return self.result(result)
 
 
 class MaybeIntCell(IntCell):
     """
     Int или None
     """
@@ -321,18 +321,18 @@
     Не отрицательное целое число или None
     Не отбрасывает дробную часть (если она больше 0) и райзит ошибку
     """
     def _parse(self, value):
         result, _ = super(MaybeIntCell, self)._parse(value)
         if result < 0:
             raise CellValueError(
-                u'Число должно быть не меньше нуля! "%s"' % value)
+                'Число должно быть не меньше нуля! "%s"' % value)
         if float(value) != float(int(float(value))):
             raise CellValueError(
-                u'Число должно быть целым! "%s"' % value)
+                'Число должно быть целым! "%s"' % value)
         return self.result(result)
 
 
 class BooleanCell(BaseCell):
     """
     Bool-ячейка, получает True при совпадении с паттерном
     """
@@ -403,55 +403,54 @@
     Ячейка, которая может принимать одно из заданных значений
     """
     def __init__(self, default=_NO_DEFAULT, choices=None,
                  match_type=MATCH_IF_EXACT, blank_values=None):
         """
         choices - список вариантов вида (pattern, value)
         """
-        assert len(choices) >= 2, u'Должно быть указано хотя бы 2 варианта!'
+        assert len(choices) >= 2, 'Должно быть указано хотя бы 2 варианта!'
         super(EnumCell, self).__init__(default=default)
         self.choices = choices
         self.match_type = match_type
         self.blank_values = blank_values
 
     def _is_blank(self, value):
         if self.blank_values is not None:
             for blank_value in self.blank_values:
-                if value.lower() == six.text_type(blank_value).lower():
+                if value.lower() == str(blank_value).lower():
                     return True
         return False
 
     def _parse(self, value):
         if self._is_blank(value):
             return self.result(self._default)
         for result, pattern in self.choices:
             if _is_match(value, pattern, self.match_type):
                 return self.result(result)
-        raise CellValueError(u'Недопустимое значение!')
+        raise CellValueError('Недопустимое значение!')
 
 
-WRONG_DATE_FORMAT_MSG = u'Неправильный формат даты!'
+WRONG_DATE_FORMAT_MSG = 'Неправильный формат даты!'
 
 
 class DateCell(BaseCell):
-
-    u"""Ячейка даты."""
+    """Ячейка даты."""
 
     # различные возможные допустимые форматы дат
     possible_date_formats = ('%d.%m.%Y', '%Y.%m.%d', '%d.%m.%y')
 
     def _parse(self, value):
         result = None
         try:
             result = datetime(*xlrd.xldate_as_tuple(float(value), 0))
         except (XLDateNegative, XLDateAmbiguous, XLDateTooLarge,
                 XLDateBadDatemode):
             raise CellValueError(WRONG_DATE_FORMAT_MSG)
         except ValueError:
-            value = six.text_type(value).strip()[:10]
+            value = str(value).strip()[:10]
             value = value.replace('/', '.').replace('-', '.')
             if any(x not in '0123456789.' for x in value):
                 raise CellValueError(WRONG_DATE_FORMAT_MSG)
             for date_format in self.possible_date_formats:
                 try:
                     result = datetime.strptime(value, date_format)
                     break
@@ -468,25 +467,25 @@
     """
     Date или None
     """
     def __init__(self):
         super(MaybeDateCell, self).__init__(default=None)
 
 
-class DynamicStartRow(object):
+class DynamicStartRow:
     """
     Автоматический поиск начала таблицы по ее заголовкам ее столбцов
     """
 
     def __init__(self, table_headers,
                  order_sensetive=True,
                  case_sensitive=False,
                  search_area=[(0, 0), (50, 50)]):
         """
-        :param list table_headers: Список заголовков: [u'Фамилия' u'Имя']
+        :param list table_headers: Список заголовков: ['Фамилия' 'Имя']
         :param bool order_sensetive: Учитывать порядок списка table_headers
         :param bool case_sensitive: Учитывать регистр при сопоставлении
         :param list search_area: Область в которой будет производиться поиск
         """
 
         assert table_headers
         assert len(search_area) == 2
@@ -507,15 +506,15 @@
         max_col = min(self.max_col, sheet.ncols)
 
         for row in range(self.min_row, max_row):
             matched = {}
             for col in range(self.min_col, max_col):
                 val = sheet.cell(row, col).value
 
-                if isinstance(val, six.string_types) and not self.case_sensitive:
+                if isinstance(val, str) and not self.case_sensitive:
                     val = val.strip().upper()
 
                 if val in self.table_headers:
                     matched.setdefault(val, col)
 
             if len(matched) == len(self.table_headers):
 
@@ -529,31 +528,31 @@
 
         pos = self.find_pos(sheet)
         if pos:
             row, col = pos
             return row
 
 
-class SimpleColumnMatcher(object):
+class SimpleColumnMatcher:
     """
     Класс сопоставления столбцов таблицы
     """
 
     def __init__(self, column_name, unique_check=False,
                  strip=True, case_sensitive=False, replacer=None):
         """
-        :param unicode column_name: Название столбца
+        :param str column_name: Название столбца
         :param bool unique_check: Нужно ли проверять на то, чтобы данный
                 matcher совпал только с одним столбцом таблицы
         :param bool strip: Нужно ли удалять крайние пробельные символы
         :param bool case_sensitive: Учитывать регистр при сопоставлении
         :param callable replacer: Функция для доп. настройки значения.
             Например:
             замена нескольких пробелов одним: lambda s: re.sub(r'\s+', ' ', s)
-            замена ё на е: lambda s: s.replace(u'ё', u'е')
+            замена ё на е: lambda s: s.replace('ё', 'е')
         """
         self.column_name = column_name
         self._unique_check = unique_check
         self.strip = strip
         self.case_sensitive = case_sensitive
         if replacer:
             assert callable(replacer)
@@ -565,15 +564,15 @@
 
     @property
     def unique_check(self):
         return self._unique_check
 
     def _prepare_cell_value(self, cell_value):
         """Подготовка значения с учетом флагов настроек"""
-        cell_value = six.text_type(cell_value)
+        cell_value = str(cell_value)
         if self.strip:
             cell_value = cell_value.strip()
 
         if not self.case_sensitive:
             cell_value = cell_value.upper()
 
         if self.replacer:
@@ -598,15 +597,15 @@
 class RegexColumnMatcher(SimpleColumnMatcher):
     """
     Сопоставление столбцов по регулярному выражению
     """
 
     def __init__(self, column_name, regex, **kwargs):
 
-        if isinstance(regex, six.string_types):
+        if isinstance(regex, str):
             flags = re.UNICODE
             if not kwargs.get('case_sensitive'):
                 flags |= re.IGNORECASE
 
             regex = re.compile(regex, flags)
         self.regex = regex
         super(RegexColumnMatcher, self).__init__(column_name, **kwargs)
@@ -616,31 +615,31 @@
         return bool(self.regex.search(cell_value))
 
 
 # =============================================================================
 # XLSLoader
 # =============================================================================
 
-class XLSLoader(object):
+class XLSLoader:
     """
     Загрузчик xls-файла с разбором
     """
     config = {}
 
     """
     ..code::
 
         config = {
-            u'заголовок листа': {
+            'заголовок листа': {
                'объект_1': {
                    #SUBTREE_CAN_BE_EMPTY: True,  # вся группа м.б. пустой
-                   'поле_объекта': (u'шапка столбца', парсер_ячейки),
-                   'другое_поле_объекта': (u'шапка столбца', парсер_ячейки),
+                   'поле_объекта': ('шапка столбца', парсер_ячейки),
+                   'другое_поле_объекта': ('шапка столбца', парсер_ячейки),
                },
-               'просто параметр': (u'шапка столбца', парсер_ячейки)
+               'просто параметр': ('шапка столбца', парсер_ячейки)
             # начинать разбор с указанной строки:
             #START_ROW: 0,
             # все строки выше START_ROW передаются в HEADER_PARSER
             # в виде итератора ячеек, результаты вызовов которого можно
             # получить после загрузки файла через свойство headers
             #HEADER_PARSER: lambda cells: cells,
             }
@@ -649,15 +648,15 @@
 
     # ключ прокси в лоадере, который сообщает загрузчику, что имя листа - не
     # имеет значения
     ANY_SHEET = '*'
 
     XLS_POS = '__xls_pos__'
 
-    __RESERVED_SHEET = u'СПРАВОЧНИК'
+    __RESERVED_SHEET = 'СПРАВОЧНИК'
 
     def __init__(self, memory_mapped_file, config=None):
         self._file = memory_mapped_file
         if config is not None:
             self.config = config
 
         # основные ошибки
@@ -669,24 +668,24 @@
         self._book = xlrd.open_workbook(
             file_contents=memory_mapped_file.read())
 
         if not all((
             self._file,
             self._book.nsheets > 0
         )):
-            self._log(u"Не удалось загрузить файл!")
+            self._log("Не удалось загрузить файл!")
             self._book = None
             raise ValueError('See loader log')
 
         # древовидные парсеры листов делаются плоскими
         # накапливаются стартовые колонки и парсеры заголовка для листов
         self._start_rows, self._end_rows = {}, {}
         self._header_parsers = {}
         self._flat_config = {}
-        for k, v in six.iteritems(self.config):
+        for k, v in self.config.items():
             try:
                 k = k.strip().upper()
             except AttributeError:
                 pass
 
             self._start_rows[k] = v.pop(START_ROW, 0)
             self._end_rows[k] = v.pop(END_ROW, None)
@@ -697,15 +696,15 @@
                 # накапливает в список непустые ячейки
                 lambda x: list(filter(bool, x))
             )
             self._flat_config[k] = _fold(v)
 
         if self._XLSLoader__RESERVED_SHEET in self._flat_config:
             raise AssertionError(
-                u'Название листа "%s" зарезервировано!' %
+                'Название листа "%s" зарезервировано!' %
                 self._XLSLoader__RESERVED_SHEET
             )
 
         self._loaded_data = {}
         self._headers = {}
 
     def _log_common_error(self, *items):
@@ -765,41 +764,41 @@
             header_data = []
 
             try:
                 parsers = self._flat_config[sheet_name]
             except KeyError:
                 if sheet_name == self._XLSLoader__RESERVED_SHEET:
                     continue
-                for k, v in six.iteritems(self._flat_config):
+                for k, v in self._flat_config.items():
                     if (isinstance(k, int) and (sheet_num + 1) == k) or (
                             isinstance(k, tuple) and (sheet_num + 1) in k):
                         parsers = v
                         parser_key = k
                         break
                 else:
                     if has_default_parser:
                         parsers = default_parsers
                     else:
                         expected_sheets = (
                             key
                             for key in map(
-                                lambda x: six.text_type(x).capitalize(),
+                                lambda x: str(x).capitalize(),
                                 self._flat_config
                             )
                             if key != self.ANY_SHEET
                         )
 
                         self._log_row_error(
                             (sheet.name, sheet_num + 1, 0),
-                            u'Неверное название листа №%s: %s.\n'
-                            u'Ожидаемые названия листов: %s' %
+                            'Неверное название листа №%s: %s.\n'
+                            'Ожидаемые названия листов: %s' %
                             (
                                 sheet_num + 1,
                                 sheet.name,
-                                u', '.join(expected_sheets)
+                                ', '.join(expected_sheets)
                             ),
                         )
                         continue
 
             if not parsers:
                 continue
 
@@ -807,15 +806,15 @@
             # если функция парсинга не задана, ячейки передаются как список
             header_parser = self._header_parsers[parser_key]
             start_row = self._start_rows.get(parser_key, 0)
             if isinstance(start_row, DynamicStartRow):
                 sheet = self._book.sheet_by_index(0)
                 start_row = start_row.find_row(sheet)
                 if start_row is None:
-                    self._log_common_error(u'Таблица не найдена')
+                    self._log_common_error('Таблица не найдена')
                     continue
 
             header_data = self._headers.setdefault(parser_key, [])
             for row in range(0, start_row):
                 # парсеру заголовка передаётся итератор ячеек по строкам
                 header_data.append(
                     header_parser((
@@ -825,15 +824,15 @@
 
             # разбор шапки листа
             col_parsers = []
             errors = []
 
             for path, (col_mather, parser), grp in parsers:
 
-                if isinstance(col_mather, six.string_types):
+                if isinstance(col_mather, str):
                     col_mather = SimpleColumnMatcher(col_mather)
                 # в шапке могут быть целочисленные ячейки
                 elif isinstance(col_mather, int):
                     col_mather = SimpleColumnMatcher(str(col_mather))
                 elif isinstance(col_mather, float):
                     col_mather = SimpleColumnMatcher(str(col_mather))
 
@@ -845,32 +844,32 @@
                     try:
                         cell_value = sheet.cell(start_row, col).value
                     except IndexError:
                         break
 
                     if col_mather.match(cell_value):
                         matched_cols.append(
-                            (col, six.text_type(cell_value).strip())
+                            (col, str(cell_value).strip())
                         )
 
                 if not matched_cols:
                     if parser.is_obligatory():
                         errors.append(
-                            u'На листе "%s" (%s) отсутствует столбец "%s", '
-                            u'необходимый для импорта' % (
+                            'На листе "%s" (%s) отсутствует столбец "%s", '
+                            'необходимый для импорта' % (
                                 sheet_name, sheet_num + 1, column_name
                             )
                         )
 
                 elif col_mather.unique_check and len(matched_cols) > 1:
                     errors.append(
-                        u'На листе "%s" (%s) присутствуют взаимоисключающие '
-                        u'столбцы: %s.' % (
+                        'На листе "%s" (%s) присутствуют взаимоисключающие '
+                        'столбцы: %s.' % (
                             sheet_name, sheet_num + 1,
-                            u', '.join(u'"%s"' % x[1] for x in matched_cols)
+                            ', '.join('"%s"' % x[1] for x in matched_cols)
                         )
                     )
                 else:
                     col_pos, real_column_name = matched_cols[0]
                     col_parsers.append(
                         (col_pos, real_column_name, path, parser, grp)
                     )
@@ -905,19 +904,19 @@
                         filled_cells_counts.get(grp, 0) + 1
                     )
 
                 row_errors = {}
 
                 def add_err(grp, title, err):
                     row_errors.setdefault(grp, set()).add(
-                        u'Cтолбец "%s": %s' % (title, err)
+                        'Cтолбец "%s": %s' % (title, err)
                     )
 
                 def add_warn(grp, title, msg):
-                    message = u'Cтолбец "%s": %s' % (title, msg)
+                    message = 'Cтолбец "%s": %s' % (title, msg)
                     self._log_row_error(xls_pos, *[message])
 
                 groups = set()
 
                 for col, title, path, parser, grp in col_parsers:
                     groups.add(grp)
                     try:
@@ -964,31 +963,31 @@
                         flat_values = _unfold(flat_values)
                         flat_values[self.XLS_POS] = xls_pos
                         sheet_data.append(flat_values)
 
         non_empty = any(self._loaded_data.values())
 
         if not non_empty and not self._row_errors_log:
-            self._log_common_error(u'Файл пуст!')
+            self._log_common_error('Файл пуст!')
 
         # результат будет True, если есть хоть одна загруженная строка
         return non_empty
 
     @staticmethod
     def prepare_row_errors(log):
         """
         Преобразует словарь-лог ошибок строк в отсортированный список строк
         """
         result = []
         for pos, lines in sorted(
             log.items(), key=lambda x: (x[0][1], str(x[0][2]))
         ):
-            result.append(u'Лист "%s" (%s), строка %s:' % pos)
-            result.extend((u'  %s' % line) for line in sorted(lines))
-            result.append(u'')
+            result.append('Лист "%s" (%s), строка %s:' % pos)
+            result.extend(('  %s' % line) for line in sorted(lines))
+            result.append('')
 
         return result
 
 if __name__ == '__main__':
 
     def cells_to_pair(cells):
         cells = [c for c in cells if c]
@@ -996,57 +995,57 @@
             return cells[0], cells[1:]
         else:
             return ()
 
     config = {
         'test': {
             'date_and_int': {
-                'date': (u'date', DateCell()),
-                'int': (u'int', IntCell(default=-100)),
+                'date': ('date', DateCell()),
+                'int': ('int', IntCell(default=-100)),
             },
             'mb_true': (
-                u'mb_true',
+                'mb_true',
                 MaybeTrueCell(pattern='y', match_type=MATCH_IF_STARTS_WITH)
             ),
             'enum': (
-                u'enum',
+                'enum',
                 EnumCell(choices=((1, 'aaa'), (2, 'bbb')), default=3)
             ),
             'opt_strs': {
                 # SUBTREE_CAN_BE_EMPTY: False,
-                'date': (u'date', DateCell()),
-                'str': (u'str', StringCell()),
-                'mb_str': (u'mb_str', MaybeStringCell()),
-                'mb_int': (u'mb_int', MaybeIntCell()),
+                'date': ('date', DateCell()),
+                'str': ('str', StringCell()),
+                'mb_str': ('mb_str', MaybeStringCell()),
+                'mb_int': ('mb_int', MaybeIntCell()),
             },
             'pasport': (
                 RegexColumnMatcher(
-                    u'Номер паспорта', u'^(№|Номер) паспорта$'),
+                    'Номер паспорта', '^(№|Номер) паспорта$'),
                 StringCell(),
             ),
             # Авто определение начала таблицы
-            START_ROW: DynamicStartRow([u'Date', u'Int']),
+            START_ROW: DynamicStartRow(['Date', 'Int']),
             # Не загружать последнюю строку
             END_ROW: -1,
             HEADER_PARSER: cells_to_pair,
         }
     }
     with open('test_file.xls') as xls_file:
         ldr = XLSLoader(xls_file, config=config)
 
         print("Loaded: %s" % ldr.load())
 
         print('---- header ----')
-        print(u'\n'.join(
-            u'%s -> %r' % i
+        print('\n'.join(
+            '%s -> %r' % i
             for i in ldr.headers['TEST']
             if i
         ))
 
         print('---- data ----')
         import pprint
         pprint.pprint(ldr.data)
 
         print('---- rows_log ----')
-        print(u'\n'.join(ldr.prepare_row_errors(ldr.rows_log)))
+        print('\n'.join(ldr.prepare_row_errors(ldr.rows_log)))
         print('---- log ----')
         pprint.pprint(ldr.log)
```

### Comparing `educommon-2.20.0/src/educommon/importer/api.py` & `educommon-3.0.0/src/educommon/importer/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,53 @@
-# coding: utf-8
-from __future__ import absolute_import
+from copy import (
+    copy,
+)
 
-from copy import copy
-
-from m3.actions.exceptions import ApplicationLogicException
-from m3.actions.results import OperationResult
-from m3_django_compat import get_request_params
-from objectpack.actions import BaseAction
-from objectpack.actions import BasePack
-from objectpack.actions import BaseWindowAction
-from objectpack.actions import multiline_text_window_result
-import six
 import xlrd
-
-from .loggers import ImportLogger
-from .loggers import SeparateImportLogger
-from .proxy import fabricate_proxies
-from .proxy_import import ProxyLoader
-from .ui import BaseImportWindow
-from .ui import ConfirmImportResultWindow
-from .XLSReader import START_ROW
-from .XLSReader import XLSLoader
+from m3.actions.exceptions import (
+    ApplicationLogicException,
+)
+from m3.actions.results import (
+    OperationResult,
+)
+from m3_django_compat import (
+    get_request_params,
+)
+
+from objectpack.actions import (
+    BaseAction,
+    BasePack,
+    BaseWindowAction,
+    multiline_text_window_result,
+)
+
+from educommon.importer.loggers import (
+    ImportLogger,
+    SeparateImportLogger,
+)
+from educommon.importer.proxy import (
+    fabricate_proxies,
+)
+from educommon.importer.proxy_import import (
+    ProxyLoader,
+)
+from educommon.importer.ui import (
+    BaseImportWindow,
+    ConfirmImportResultWindow,
+)
+from educommon.importer.XLSReader import (
+    START_ROW,
+    XLSLoader,
+)
 
 
 class BaseImportPack(BasePack):
-    u"""Базовый пак, реализующий действия по импорту."""
+    """Базовый пак, реализующий действия по импорту."""
 
-    title = u''
+    title = ''
     result_window_title = None
 
     import_window = BaseImportWindow
     # result_window = BaseImportResultWindow
 
     # постраничные загрузчики
     loaders = {}
@@ -42,32 +59,32 @@
     # аргумент book, иначе пердварительного чтения не будет
     workbook_pre_reading = False
 
     default_import_logger_cls = ImportLogger
     separate_import_logger_cls = SeparateImportLogger
 
     separate_logs = False
-    u"""Необходимо ли разделять сквозные логи на ошибки и предупреждения."""
+    """Необходимо ли разделять сквозные логи на ошибки и предупреждения."""
 
     confirm_save_on_errors = False
-    u"""Вызов окна подтверждения импорта при наличии ошибок."""
+    """Вызов окна подтверждения импорта при наличии ошибок."""
 
     def __init__(self):
         super(BaseImportPack, self).__init__()
         self.import_window_action = BaseImportWindowAction()
         self.import_action = BaseImportAction()
         self.import_with_confirm_action = ImportWithConfirmAction()
         self.actions.extend([
             self.import_window_action,
             self.import_action,
             self.import_with_confirm_action,
         ])
 
     def declare_context(self, action):
-        u"""Объявлен параметр для пропуска записей с ошибками."""
+        """Объявлен параметр для пропуска записей с ошибками."""
         params = super(BaseImportPack, self).declare_context(action)
 
         if action in (self.import_action, self.import_with_confirm_action):
             params.update({
                 'ignore_bad_rows': dict(type='boolean', default=False),
                 # ID компоненты окна импорта
                 'import_window_id': dict(type='str'),
@@ -79,16 +96,16 @@
             self, memory_file, file_name, initial_context, loaders=None
     ):
         """Автогенерация прокси у загрузчиков для областей ячеек"""
         xls_loader = XLSLoader(memory_file)
         loaders = loaders or self.get_loaders()
         # только страницы, для которых определены загрузчики
         loaders = dict(  # имена сделаю большими и без пробелов
-            (six.text_type(name).strip().upper(), loader_cls)
-            for name, loader_cls in six.iteritems(loaders)
+            (str(name).strip().upper(), loader_cls)
+            for name, loader_cls in loaders.items()
         )
         sheets = (
             sheet
             for sheet in xls_loader._book.sheets()
             if sheet.name.strip().upper() in loaders
         )
         for sheet in sheets:
@@ -127,15 +144,15 @@
         # будет еще одно чтение
         memory_file.seek(0)
 
     def get_loaders(self, request=None, context=None, book=None, **kwargs):
         """
         Получение постраничных загрузчиков
         """
-        assert self.loaders, u'Не определены прокси загрузки!'
+        assert self.loaders, 'Не определены прокси загрузки!'
         loaders = self.loaders.copy()
         return loaders
 
     def set_initial_context(self, request, context):
         """
         Метод позволяет изменять начальный контекст
         прокси загрузчика в зависимости от контекста,
@@ -163,15 +180,15 @@
         # Создаем копии классов загрузчиков для текущего импорта.
         loaders = {
             name: type(
                 loader_cls.__name__ + 'SafeCopy', (loader_cls,),
                 {'proxies': copy(loader_cls.proxies)}
                 if hasattr(loader_cls, 'proxies') else {}
             ) if loader_cls else loader_cls
-            for name, loader_cls in six.iteritems(loaders)
+            for name, loader_cls in loaders.items()
         }
 
         # если загрузчик предполагает наличие прокси для областей ячеек
         # которые заранее невозможно задекларировать в описании
         self._make_proxies_config(_file, file_name, initial_context, loaders)
 
         ignore_bad_rows = (context.ignore_bad_rows
@@ -205,32 +222,32 @@
         params['extensions'] = self.extensions
         return params
 
     def get_import_result_window_params(self, params, request, context):
         """Параметры передаваемые окну результата импорта."""
         params['title'] = (
             self.result_window_title or
-            self.title + u': проверка шаблона'
+            self.title + ': проверка шаблона'
         )
 
         return params
 
     def extend_menu(self, menu):
         """Размещение в меню"""
         return menu.SubMenu(
-            u'Администрирование',
+            'Администрирование',
             menu.SubMenu(
-                u'Импорт',
+                'Импорт',
                 menu.Item(self.title, self.import_window_action)
             )
         )
 
 
 class BaseImportWindowAction(BaseWindowAction):
-    u"""Экшн показа окна импорта."""
+    """Экшн показа окна импорта."""
 
     perm_code = 'import'
 
     def create_window(self):
         self.win = self.parent.import_window()
 
     def set_window_params(self):
@@ -249,76 +266,76 @@
         )
 
     def configure_window(self):
         pass
 
 
 class BaseImportAction(BaseAction):
-    u"""Экшн выполняющий импорт."""
+    """Экшн выполняющий импорт."""
 
     perm_code = 'import'
 
     def run(self, request, context):
         try:
             log_msg, success = self.parent.make_import(request, context)
         except xlrd.XLRDError:
             raise ApplicationLogicException(
-                u'Файл имеет неверный формат или поврежден! '
-                u'Пересохраните файл в формате '
-                u'"Microsoft Excel 97/2003 (.xls)"'
+                'Файл имеет неверный формат или поврежден! '
+                'Пересохраните файл в формате '
+                '"Microsoft Excel 97/2003 (.xls)"'
             )
 
         return multiline_text_window_result(
             success=success, data=log_msg, title=self.parent.title)
 
 
 class ImportWithConfirmAction(BaseAction):
-    u"""Экшн выполняющий импорт.
+    """Экшн выполняющий импорт.
 
     При обнаружении ошибок в импорте, требует подтверждения
     пропуска строк с ошибками.
     """
 
     perm_code = 'import'
     result_window = ConfirmImportResultWindow
 
     def create_window(self, request, context, **params):
-        u"""Создание окна результата логгера."""
+        """Создание окна результата логгера."""
         win = self.result_window()
         win.set_params(self.parent.get_import_result_window_params(
             params, request, context))
 
         return win
 
     def get_window_params_by_import_result(
             self, import_was_success, import_logger, request, context):
-        u"""Формирует параметры окна результата из данных логгера."""
+        """Формирует параметры окна результата из данных логгера."""
         return dict(
             result_text=import_logger.get_pretty_log(),
             import_window_id=context.import_window_id,
             hide_confirm_button=(
                 context.ignore_bad_rows or
                 import_was_success or
                 import_logger.have_errors_in_all_rows()
             ),
             ignore_bad_rows=context.ignore_bad_rows,
             exit_from_import_on_close=import_was_success,
         )
 
     def run(self, request, context):
-        u"""Выполнение импорта и формирование окна результата."""
+        """Выполнение импорта и формирование окна результата."""
         loader = self.parent.get_import_loader(request, context)
 
         try:
             loader.load()
         except xlrd.XLRDError:
             raise ApplicationLogicException(
-                u'Файл имеет неверный формат или поврежден! '
-                u'Пересохраните файл в формате '
-                u'"Microsoft Excel 97/2003 (.xls)"'
+                'Файл имеет неверный формат или поврежден! '
+                'Пересохраните файл в формате '
+                '"Microsoft Excel 97/2003 (.xls)"'
             )
         import_was_success = not loader.result_logger.has_error()
         params = self.get_window_params_by_import_result(
             import_was_success, loader.result_logger, request, context)
         win = self.create_window(request, context, **params)
 
         return OperationResult(
```

### Comparing `educommon-2.20.0/src/educommon/importer/constants.py` & `educommon-3.0.0/src/educommon/importer/constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-
 IMPORT_SUCCESS_MSG = (
-    u'Проверка шаблона прошла успешно. '
-    u'Файл успешно загружен!'
+    'Проверка шаблона прошла успешно. '
+    'Файл успешно загружен!'
 )
 IMPORT_SUCCESS_WITH_ERRORS_MSG = (
-    u'Данные из шаблона импорта, по которым не '
-    u'выявлено ошибок, успешно загружены в систему!'
+    'Данные из шаблона импорта, по которым не '
+    'выявлено ошибок, успешно загружены в систему!'
 )
 ALL_ROWS_HAVE_ERRORS_MSG = (
-    u'Все строки файла содержат ошибки, '
-    u'скорректируйте файл и повторите импорт.'
+    'Все строки файла содержат ошибки, '
+    'скорректируйте файл и повторите импорт.'
 )
 
 IMPORT_FAIL_WITH_CRITICAL_ERROR = (
-    u'При загрузке возникла критическая ошибка, '
-    u'скорректируйте файл и повторите импорт.'
+    'При загрузке возникла критическая ошибка, '
+    'скорректируйте файл и повторите импорт.'
 )
```

### Comparing `educommon-2.20.0/src/educommon/importer/loggers.py` & `educommon-3.0.0/src/educommon/importer/loggers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# coding: utf-8
-from __future__ import absolute_import
+from functools import (
+    partial,
+)
+from itertools import (
+    chain,
+)
+
+from educommon.importer.constants import (
+    ALL_ROWS_HAVE_ERRORS_MSG,
+    IMPORT_FAIL_WITH_CRITICAL_ERROR,
+    IMPORT_SUCCESS_MSG,
+    IMPORT_SUCCESS_WITH_ERRORS_MSG,
+)
 
-from functools import partial
-from itertools import chain
 
-import six
-
-from .constants import ALL_ROWS_HAVE_ERRORS_MSG
-from .constants import IMPORT_FAIL_WITH_CRITICAL_ERROR
-from .constants import IMPORT_SUCCESS_MSG
-from .constants import IMPORT_SUCCESS_WITH_ERRORS_MSG
-
-
-class BaseImportLogger(object):
-    u"""Абстрактный логгер для импорта.
+class BaseImportLogger:
+    """Абстрактный логгер для импорта.
 
     Ключ row_info в хэндлерах: (имя_листа, № листа, № строки).
     """
 
     def on_sheet_errors(self, sheet, errors, *args, **kwargs):
         raise NotImplemented
 
@@ -40,15 +41,15 @@
         raise NotImplemented
 
     def on_save_rollback(self, *args, **kwargs):
         raise NotImplemented
 
 
 class ImportLogger(BaseImportLogger):
-    u"""Логгер для импорта.
+    """Логгер для импорта.
 
     Сохраняет необходимую информацию при импорте, для дальнейшей
     обработки.
 
     Атрибуты:
         sheets_errors   Словарь хранит названия листов excel файла и их ошибки.
         header_errors   Словарь хранит названия листов excel файла и ошибки
@@ -60,15 +61,15 @@
         rows_errors     Словарь хранит информацию об ошибках, полученных при
                         импорте.
         rows_warnings   Словарь хранит информацию о предупреждениях, полученных
                         при импорте.
     """
 
     def __init__(self, ignore_bad_rows=False, *args, **kwargs):
-        u"""Инициализация логгера."""
+        """Инициализация логгера."""
         self.ignore_bad_rows = ignore_bad_rows
         self.load_errors = []
         self.sheets_errors = {}
         self.header_errors = {}
         self.processed_rows = []
         self.saved_rows = []
         self.critical_error_msg = None
@@ -89,15 +90,15 @@
         if errors:
             self.rows_errors.setdefault(row_info, []).extend(errors)
 
         if warnings:
             self.rows_warnings.setdefault(row_info, []).extend(warnings)
 
     def on_critical_error(self, row_info, error, *args, **kwargs):
-        self.critical_error_msg = u'{0}\n {1}'.format(
+        self.critical_error_msg = '{0}\n {1}'.format(
             self._get_row_label(row_info),
             error
         )
 
     def on_row_save(self, row_info, *args, **kwargs):
         if row_info not in self.saved_rows:
             self.saved_rows.append(row_info)
@@ -108,56 +109,56 @@
         except ValueError:
             pass
 
     def on_save_rollback(self, *args, **kwargs):
         self.saved_rows = []
 
     def have_errors_in_all_rows(self):
-        u"""Проверка на ошибки во всех обработанных записях."""
+        """Проверка на ошибки во всех обработанных записях."""
         if not self.processed_rows:
             return False
 
         return sorted(self.rows_errors.keys()) == sorted(self.processed_rows)
 
     @staticmethod
     def _add_text_lines(result, lines, top_margin=0, bottom_margin=0):
-        u"""Добавление строк в массив с указанием отступов.
+        """Добавление строк в массив с указанием отступов.
 
         :param list result: Массив, куда добавляется.
         :param list or basestring lines: Массив или строка для добавления.
         :param int top_margin: Отступ сверху.
         :param int bottom_margin: Отступ снизу.
         """
         if top_margin:
-            result.extend(top_margin * [u''])
+            result.extend(top_margin * [''])
 
-        result.extend([lines] if isinstance(lines, six.string_types) else lines)
+        result.extend([lines] if isinstance(lines, str) else lines)
 
         if bottom_margin:
-            result.extend(bottom_margin * [u''])
+            result.extend(bottom_margin * [''])
 
     @staticmethod
     def _get_row_label(row_info):
-        u"""Возвращает информацию о строке в читаемом виде."""
-        return u'Лист "%s" (%s), строка %s:' % row_info
+        """Возвращает информацию о строке в читаемом виде."""
+        return 'Лист "%s" (%s), строка %s:' % row_info
 
     @staticmethod
     def _sort_rows_info(rows_info, key=lambda x: x[2]):
         return sorted(rows_info, key=key)
 
     def has_error(self):
         return bool(self.critical_error_msg or self.rows_errors)
 
     def get_pretty_log(self):
-        u"""Возвращает лог в читаемом виде."""
+        """Возвращает лог в читаемом виде."""
         result_lines = []
         add_lines = partial(self._add_text_lines, result_lines)
 
         def find_series(numbers):
-            u"""Находит интервалы номеров в списке.
+            """Находит интервалы номеров в списке.
 
             .. code-block:: python
                 >>> a = (1, 2, 3, 4, 8, 9, 10, 13)
                 >>> tuple(find_series(iter(a)))
 
                 ((1, 4), (8, 10), (13, 13))
             """
@@ -166,26 +167,26 @@
                 if cur - prev > 1:
                     yield last, prev
                     last = cur
                 prev = cur
             yield last, prev
 
         def get_saved_rows_info():
-            u"""Группированное перечисление сохранненых строк.
+            """Группированное перечисление сохранненых строк.
 
             Пример: 1-20, 43-200, 203-208.
             """
             rows_numbers = sorted([x[2] for x in self.saved_rows])
             series = find_series(iter(rows_numbers))
 
-            result = u', '.join(
+            result = ', '.join(
                 '{}-{}'.format(x, y) if x != y else str(x)
                 for x, y in series
             )
-            return u'Загружены строки : {0}.'.format(result)
+            return 'Загружены строки : {0}.'.format(result)
 
         if self.critical_error_msg is not None:
             add_lines(IMPORT_FAIL_WITH_CRITICAL_ERROR, 0, 1)
             add_lines(self.critical_error_msg)
 
         elif self.saved_rows:
             if not self.rows_errors:
@@ -195,15 +196,15 @@
                 else:
                     add_lines(IMPORT_SUCCESS_MSG)
             else:
                 add_lines(get_saved_rows_info())
 
             # Дополнительно выводим предупреждения для загруженных строк
             if self.rows_warnings:
-                add_lines(u'ПРЕДУПРЕЖДЕНИЯ:', 1, 1)
+                add_lines('ПРЕДУПРЕЖДЕНИЯ:', 1, 1)
 
                 for row in self._sort_rows_info(self.saved_rows):
                     add_lines(self._get_row_label(row), 0, 1)
                     add_lines(self.rows_warnings.get(row, []), 0, 1)
         else:
             if self.have_errors_in_all_rows():
                 add_lines(ALL_ROWS_HAVE_ERRORS_MSG, 0, 1)
@@ -219,29 +220,29 @@
                 row_errors = self.rows_errors.get(row, [])
                 row_warnings = self.rows_warnings.get(row, [])
 
                 if row_errors or row_warnings:
                     add_lines(self._get_row_label(row), 0, 1)
 
                 if row_errors:
-                    add_lines(u'ОШИБКИ:')
+                    add_lines('ОШИБКИ:')
                     add_lines(row_errors, 0, 1)
 
                 if row_warnings:
-                    add_lines(u'ПРЕДУПРЕЖДЕНИЯ:')
+                    add_lines('ПРЕДУПРЕЖДЕНИЯ:')
                     add_lines(self.rows_warnings, 0, 1)
 
-        return u'\n'.join(result_lines)
+        return '\n'.join(result_lines)
 
 
 class SeparateImportLogger(ImportLogger):
-    u"""Логгер с раздельным выводом ошибок."""
+    """Логгер с раздельным выводом ошибок."""
 
     def get_pretty_log(self):
-        u"""При наличии ошибок разделяет их на разные блоки."""
+        """При наличии ошибок разделяет их на разные блоки."""
         if (
             self.critical_error_msg is not None
             and not self.rows_errors
             or self.ignore_bad_rows
         ):
             return super(SeparateImportLogger, self).get_pretty_log()
 
@@ -251,23 +252,23 @@
         if self.have_errors_in_all_rows():
             add_lines(ALL_ROWS_HAVE_ERRORS_MSG, 0, 1)
 
         if self.load_errors:
             add_lines(self.load_errors, 0, 1)
         # Вывод ошибок по всем записям
         if self.rows_errors:
-            add_lines(u'ОШИБКИ:', 0, 1)
+            add_lines('ОШИБКИ:', 0, 1)
         else:
             add_lines(IMPORT_SUCCESS_MSG, 0, 1)
 
         for row in self._sort_rows_info(list(self.rows_errors)):
             add_lines(self._get_row_label(row))
             add_lines(self.rows_errors.get(row, []), 0, 1)
         # Вывод предупреждений по всем записям
         if self.rows_warnings:
-            add_lines(u'ПРЕДУПРЕЖДЕНИЯ:', 0, 1)
+            add_lines('ПРЕДУПРЕЖДЕНИЯ:', 0, 1)
 
             for row in self._sort_rows_info(list(self.rows_warnings)):
                 add_lines(self._get_row_label(row))
                 add_lines(self.rows_warnings.get(row, []), 0, 1)
 
-        return u'\n'.join(result_lines)
+        return '\n'.join(result_lines)
```

### Comparing `educommon-2.20.0/src/educommon/importer/proxy.py` & `educommon-3.0.0/src/educommon/importer/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import collections
 
-from django.db import transaction
-from django.db.models import Q
-from objectpack.exceptions import ValidationError
-from six.moves import map
 import django
-import six
-
-from educommon.m3 import transaction_context
-
-from .loggers import ImportLogger
-from .XLSReader import SUBTREE_CAN_BE_EMPTY
-from .XLSReader import MaybeStringCell
+from django.db import (
+    transaction,
+)
+from django.db.models import (
+    Q,
+)
+
+from objectpack.exceptions import (
+    ValidationError,
+)
+
+from educommon.importer.loggers import (
+    ImportLogger,
+)
+from educommon.importer.XLSReader import (
+    SUBTREE_CAN_BE_EMPTY,
+    MaybeStringCell,
+)
+from educommon.m3 import (
+    transaction_context,
+)
 
 
 class SafeDict(dict):
 
     @classmethod
     def _wrap(cls, value):
         if not value:
@@ -55,27 +62,26 @@
 
 
 class ProxySaveError(Exception):
     pass
 
 
 class ProxyCriticalError(Exception):
-    u"""
+    """
     Рейзится если нужно прервать процесс загрузки КТП
     в произвольном месте, с выводом ошибки
     """
-    pass
 
 
 class ProxyWarning(Exception):
-    u"""Исключение возникает, когда данные одного прокси не обработаны, но
+    """Исключение возникает, когда данные одного прокси не обработаны, но
     необходимо продолжить обработку строки в шаблоне."""
 
 
-class _ImportProxy(object):
+class _ImportProxy:
     """
     Прототип proxy для загрузки данных
     """
     # описание ячеек
     cells_config = {
         # 'key': cell
         # 'subdict': {
@@ -100,30 +106,30 @@
 
     @classmethod
     def __make_config(cls, headers):
         """
         Создание конфигурации колонок для XLSLoader`а
         """
         if headers:
-            if isinstance(headers, six.string_types):
+            if isinstance(headers, str):
                 # "шапки" могут быть переданы в виде форматирующей строки
                 fmt, headers = headers, {}
-                for key, val in six.iteritems(cls.default_headers):
+                for key, val in cls.default_headers.items():
                     headers[key] = fmt % val
             else:
                 _h = (cls.default_headers or {}).copy()
                 _h.update(headers)
                 headers = _h
         else:
             headers = cls.default_headers or {}
 
         # добавление "шапок" столбцов к конфигу ячеек
         def add_headers(src, path=''):
             result = {}
-            for key, val in six.iteritems(src):
+            for key, val in src.items():
                 path_w_key = ('%s__%s' % (path, key)) if path else key
                 try:
                     val = add_headers(val, path_w_key)
                 except AttributeError:
                     val = (headers[path_w_key], val)
                 result[key] = val
             return result
@@ -206,15 +212,15 @@
             except self.model.MultipleObjectsReturned:
                 if self.msg_multiple:
                     raise ProxySaveError(self.msg_multiple)
                 raise
 
             return None
 
-        cache_key = tuple(sorted(six.iteritems(data), key=lambda x: x[0]))
+        cache_key = tuple(sorted(data.items(), key=lambda x: x[0]))
         if cache_key not in self._cache:
             self._cache[cache_key] = default()
 
         return self._cache[cache_key]
 
 
 class ContextAdapterProxy(_ImportProxy):
@@ -296,18 +302,19 @@
         """
         Построение кэша объектов, используемых в заголовках области
         Вызывается при добавлении в лоадер
         """
         raise NotImplementedError()
 
 
-class MultiProxyLoader(object):
+class MultiProxyLoader:
     """
     Прокси загрузки нескольких моделей
     """
+
     # начальный контекст импорта
     initial_context = {
     }
 
     # proxy моделей в порядке приоритета
     proxies = [
         # (ключ_контекста, класс_обёртки)
@@ -332,30 +339,30 @@
     # откат загрузки всего листа при ошибке хотя бы в одной строке
     rollback_all = False
 
     # методы, помеченные декоратором delay_in_situations('import'),
     # будут ожидать завершения транзакций импорта
     default_delay_situation = 'import'  # по-умолчанию
 
-    LOAD_ERROR_MSG = u'Лист не был загружен!'
+    LOAD_ERROR_MSG = 'Лист не был загружен!'
 
     @classmethod
     def make_header_context(cls, header_data, context):
         """
         Преобразование данных шапки.
         При возвращении непустого списка ошибок - прекращение загрузки листа
         """
         header_context = {}
         errors = []
         return header_context, errors
 
     @classmethod
     def load_rows(cls, header_data, rows_data, parse_log, log, context,
                   warning_log=None, result_logger=None):
-        u"""Загрузка строк листа.
+        """Загрузка строк листа.
 
         Логи разделены с целью дать возможность потомку принять решение
         о дальнейшей загрузке, если были ошибки парсинга ячеек
 
         :param dict parse_log: лог парсинга типов ячеек
         :param dict log: сквозной лог импорта
         :param dict warning_log: лог с предупреждениями импорта
@@ -415,18 +422,18 @@
                         try:
                             errors, warnings = proxyloader.load(row)
                             result_logger.on_row_processed(row[xls_pos])
                             result_logger.on_row_errors(
                                 row[xls_pos], errors, warnings)
                         except ProxyCriticalError as err:
                             log.setdefault(row[xls_pos], []).extend(
-                                [six.text_type(err)])
-                            _errors.append(six.text_type(err))
+                                [str(err)])
+                            _errors.append(str(err))
                             result_logger.on_row_errors(
-                                row[xls_pos], [six.text_type(err)])
+                                row[xls_pos], [str(err)])
 
                             # XXX при данном эксепшене нужно предотвратить
                             # повторное выполнение load, поэтому откатываем
                             # НЕ через raise или inner_t.rollback
                             transaction.savepoint_rollback(inner_t._sid)
                             # откатываем внешний блок
                             transaction.rollback(outer_t._using)
@@ -473,15 +480,15 @@
     if django.VERSION[:2] >= (1, 6):
         # Для Django >= 1.6 метод загрузки строк переписан
         # с использованием transaction.atomic
         @classmethod
         @transaction.atomic
         def load_rows(cls, header_data, rows_data, parse_log, log, context,
                       warning_log=None, result_logger=None):
-            u"""
+            """
             Загрузка строк листа.
 
             Логи разделены с целью дать возможность потомку принять решение
             о дальнейшей загрузке, если были ошибки парсинга ячеек.
 
             :param dict parse_log: лог парсинга типов ячеек
             :param dict log: сквозной лог импорта
@@ -550,18 +557,18 @@
 
                 return errors
 
             for row in rows_data:
                 try:
                     rows_errors.extend(load_one_row(row))
                 except ProxyCriticalError as err:
-                    rows_errors.append(six.text_type(err))
-                    add_log(row, [six.text_type(err)])
+                    rows_errors.append(str(err))
+                    add_log(row, [str(err)])
                     result_logger.on_critical_error(
-                        row[xls_pos], six.text_type(err)
+                        row[xls_pos], str(err)
                     )
                     break
 
             # если были ошибки и нужно откатить всё
             # FIXME: Если rollback_all == True, то независимо от флага
             # FIXME: игнора, будет происходить откат
             if result_logger.has_error() and (
@@ -579,16 +586,16 @@
         """
         def prepare_headers(raw_headers):
             """
             Если на входе строка, она оборачивается в словарь-подобный объект,
             который на любой ключ возвращает эту строку.
             Если на входе словарь - он остаётся словарём.
             """
-            if isinstance(raw_headers, six.string_types):
-                class StrAsDict(object):
+            if isinstance(raw_headers, str):
+                class StrAsDict:
                     def __init__(self, value):
                         self._value = value
 
                     def __getitem__(self, key):
                         return self._value
 
                     def get(self, key, default=None):
@@ -720,21 +727,21 @@
 
                 # загрузка через proxy
                 try:
                     context[key] = proxy(key, context)._load(sub_data)
                 except ProxyWarning as err:
                     # Записать в лог и продолжить загрузку строки
                     warnings.append(
-                        (context.error_format or u'%s') % six.text_type(err)
+                        (context.error_format or '%s') % str(err)
                     )
                     raise
                 except (ProxySaveError, ValidationError) as err:
                     # такая ошибка складывается в лог
                     errors.append(
-                        (context.error_format or u'%s') % six.text_type(err)
+                        (context.error_format or '%s') % str(err)
                     )
                     if not is_layout_proxy:
                         # если обычный прокси, вся строка пропускается
                         return False
                 except (ProxyCriticalError, AssertionError) as err:
                     # AssertionError - откатит всю загрузку
                     # ProxyCriticalError - откатит с выводом сообщения
@@ -800,15 +807,15 @@
         try:
             header_info = proxy.create_header(proxy, loader_context)
             proxy.header_object = header_info.get(key)
             cls.proxies.append((key, proxy))
         except ProxySaveError as err:
             # логируем ошибку, чтобы вывалить ее в конце
             cls.add_proxy_log = add_log
-            cls.add_proxy_log.setdefault(key, six.text_type(err))
+            cls.add_proxy_log.setdefault(key, str(err))
 
     @classmethod
     def load_rows(cls, header_data, rows_data, parse_log, log, context,
                   warning_log=None):
         super(LayoutProxyLoader, cls).load_rows(
             header_data, rows_data, parse_log, log, context
         )
@@ -833,15 +840,15 @@
         {
             'was_fabricated': True,  # для фильтраци при добавлении в загрузчик
             'cells_config': cells_config,
             'default_headers': default_headers,
             # соответствие {модель: (ключ, строка)} для дальнейшего парсинга
             'layout_header': dict([(
                 AncestorCls.layout_header_model, (k, v)
-            ) for k, v in six.iteritems(default_headers)]),
+            ) for k, v in default_headers.items()]),
         }
     )
     return name, cls
 
 
 def fabricate_proxies(AncestorCls, layout_name, head_data):
     """
```

### Comparing `educommon-2.20.0/src/educommon/importer/proxy_import.py` & `educommon-3.0.0/src/educommon/importer/proxy_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,71 +1,69 @@
-# coding: utf-8
-from __future__ import absolute_import
+from educommon.importer.loggers import (
+    ImportLogger,
+)
+from educommon.importer.XLSReader import (
+    XLSLoader,
+)
 
-import six
 
-from educommon.importer.loggers import ImportLogger
+SUCCESFUL_IMPORTED = 'Файл успешно импортирован'
 
-from .XLSReader import XLSLoader
 
-
-SUCCESFUL_IMPORTED = u'Файл успешно импортирован'
-
-
-class ProxyLoader(object):
+class ProxyLoader:
     """Загрузка файла по словарю прокси-загрузчиков."""
 
     report_cls = None
-    u"""Класс отчета об ошибках."""
+    """Класс отчета об ошибках."""
 
     report_url = None
-    u"""Адрес отчета об ошибках."""
+    """Адрес отчета об ошибках."""
 
     message = None
-    u"""Сообщение о результате."""
+    """Сообщение о результате."""
 
     def __init__(self, loaders, _file, file_name, context=None,
                  separate_logs=False, ignore_bad_rows=False,
                  result_logger=None):
-        u"""Загрузка файла по словарю прокси-загрузчиков.
+        """Загрузка файла по словарю прокси-загрузчиков.
 
         :param dict loaders: словарь постраничных загрузчиков файла
         :param InMemoryUploadedFile _file: файл загрузки в оперативной памяти
-        :param unicode file_name: название файла
+        :param str file_name: название файла
         :param dict context: контекст
         :param bool separate_logs: флаг разделения логов импорта
         :param bool ignore_bad_rows: флаг для пропуска строк с ошибками
         :param result_logger: логгер для сбора информации импорта
         :type result_logger: educommon.importer.loggers.BaseImportLogger
         """
 
         config = {}
-        for key, loader in six.iteritems(loaders):
+        for key, loader in loaders.items():
             config[key] = loader.make_config() if loader else {}
 
         self.xls_loader = XLSLoader(_file, config)
         self.loaders = loaders
         self.context = context or {}
         self.context['XLS_POS'] = self.xls_loader.XLS_POS
         self.context['ignore_bad_rows'] = ignore_bad_rows
         self.separate_logs = separate_logs
         self.ignore_bad_rows = ignore_bad_rows
         self.result_logger = result_logger or ImportLogger()
 
     def make_log(self, log):
-        u"""Сбор лога для окна результата.
+        """Сбор лога для окна результата.
 
         :param dict log: лог
         :rtype str
         """
-        return u'\n'.join(
+        return '\n'.join(
             self.xls_loader.log + self.xls_loader.prepare_row_errors(log))
 
     def load(self):
-        u"""Импорт данных из файла."""
+        """Импорт данных из файла."""
         if not self.xls_loader.load():
             self.message = self.make_log(self.xls_loader.rows_log)
             # FIXME: Все очень сложно.. Так как у парсера свой лог, а
             # FIXME: в этом участке кода формируется сообщение == хак.
             self.result_logger.load_errors = self.xls_loader.log
             self.result_logger.processed_rows = list(self.xls_loader.rows_log)
             self.result_logger.rows_errors = self.xls_loader.rows_log
@@ -85,24 +83,24 @@
         parse_log = self.xls_loader.rows_log
         # сквозной лог загрузки данных проксями будет дополнен parse_log'ом в
         # методе load_rows у загрузчика листа
         import_log = {}
         # опционально - сквозной лог для предупреждений
         warning_log = {} if self.separate_logs else None
 
-        for sheet, data in six.iteritems(self.xls_loader.data):
+        for sheet, data in self.xls_loader.data.items():
             header = self.xls_loader.headers.get(sheet, [])
             # Класс загрузчика листа
             if sheet in self.loaders:
                 loader_cls = self.loaders.get(sheet)
             else:
                 loader_cls = self.loaders.get(sheet.upper())
             if not loader_cls:
                 # Если не найден загрузчик для листа
-                error_msg = u'Некорректное имя листа "%s"' % sheet
+                error_msg = 'Некорректное имя листа "%s"' % sheet
                 import_log[data[0][self.xls_loader.XLS_POS]] = error_msg
                 # Заносим запись об ошибке при обработке листа в общий лог
                 self.result_logger.on_sheet_errors(sheet, [error_msg])
                 continue
 
             # выполняет загрузку листа (с разбором шапки и логированием)
             loader_cls.load_rows(
@@ -118,24 +116,24 @@
         log = self.make_log(import_log)
         result = bool(self.result_logger.saved_rows)
 
         if self.separate_logs:
             # если задан режим разделения логов
             if log:
                 # всё же были какие-то ошибки
-                final_log = [u" ОШИБКИ:\n ", log]
+                final_log = [" ОШИБКИ:\n ", log]
             else:
                 final_log = [SUCCESFUL_IMPORTED, ]
 
             if warning_log:
                 final_log.extend([
-                    u" ПРЕДУПРЕЖДЕНИЯ:\n ", self.make_log(warning_log)
+                    " ПРЕДУПРЕЖДЕНИЯ:\n ", self.make_log(warning_log)
                 ])
 
-            self.message = u'\n'.join(final_log)
+            self.message = '\n'.join(final_log)
         else:
             self.message = log or SUCCESFUL_IMPORTED
 
         # Если произошла ошибка, составим отчет
         if not result and self.report_cls:
             report = self.report_cls(import_log)
             self.report_url = report.make()
```

### Comparing `educommon-2.20.0/src/educommon/importer/refactoring-notes.txt` & `educommon-3.0.0/src/educommon/importer/refactoring-notes.txt`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/importer/report.py` & `educommon-3.0.0/src/educommon/importer/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import os
 import sys
 import uuid
 
-from simple_report.report import SpreadsheetReport
+from simple_report.report import (
+    SpreadsheetReport,
+)
 
-from educommon.report.reporter import get_path
-from educommon.report.reporter import get_url
+from educommon.report.reporter import (
+    get_path,
+    get_url,
+)
 
 
-class BaseFailureImportReport(object):
+class BaseFailureImportReport:
     """Базовый класс отчета об импорте"""
 
     template_name = None
     reports_dir = 'reports'
     default_extension = 'xlsx'
 
     def __init__(self, data):
```

### Comparing `educommon-2.20.0/src/educommon/importer/test_file.xls` & `educommon-3.0.0/src/educommon/importer/test_file.xls`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/importer/ui.py` & `educommon-3.0.0/src/educommon/importer/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from m3_ext.ui import all_components as ext
-from objectpack.ui import BaseEditWindow
-from objectpack.ui import BaseWindow
+from m3_ext.ui import (
+    all_components as ext,
+)
+
+from objectpack.ui import (
+    BaseEditWindow,
+    BaseWindow,
+)
 
 
 class BaseImportWindow(BaseEditWindow):
-    u"""Базовое окно загрузки шаблона импорта."""
+    """Базовое окно загрузки шаблона импорта."""
 
     def _init_components(self):
         super(BaseImportWindow, self)._init_components()
         self.file_field = ext.ExtFileUploadField(
             anchor='100%',
             allow_blank=False,
             name='uploaded',
-            label=u"Файл для загрузки",
+            label="Файл для загрузки",
         )
 
     def _do_layout(self):
         super(BaseImportWindow, self)._do_layout()
         self.form.items.append(self.file_field)
 
     def set_params(self, params):
@@ -28,29 +30,29 @@
         # FIXME: При переопределении придется копипастить
         # Проброс ID окна для окна результата
         self.handler_beforesubmit = '''
             function (submit) {submit.params["import_window_id"] = win.id}
         '''
 
         self.form.file_upload = True
-        self.save_btn.text = u'Загрузить'
+        self.save_btn.text = 'Загрузить'
         self.file_field.possible_file_extensions = params.get(
             'extensions', None
         )
 
 
 class ImportResultWindow(BaseWindow):
-    u"""Окно для вывода результата импорта."""
+    """Окно для вывода результата импорта."""
 
     def _init_components(self):
         super(ImportResultWindow, self)._init_components()
         self.result_field = ext.ExtTextArea(read_only=True)
 
         self.close_btn = ext.ExtButton(
-            text=u'Закрыть',
+            text='Закрыть',
             handler='function() {win.close()}'
         )
 
         # Кнопка "Отмена" не блокируется в режиме "только для чтения"
         self._mro_exclude_list.append(self.close_btn)
 
     def _do_layout(self):
@@ -66,20 +68,20 @@
         self.layout = 'fit'
         self.modal = False
 
         self.result_field.value = params['result_text']
 
 
 class ConfirmImportResultWindow(ImportResultWindow):
-    u"""Окно для подтверждения импорта при наличии ошибок."""
+    """Окно для подтверждения импорта при наличии ошибок."""
 
     def _init_components(self):
         super(ConfirmImportResultWindow, self)._init_components()
         self.confirm_import_btn = ext.ExtButton(
-            text=u'Загрузить данные, в которых нет ошибок',
+            text='Загрузить данные, в которых нет ошибок',
         )
 
     def _do_layout(self):
         super(ConfirmImportResultWindow, self)._do_layout()
         self.buttons.insert(0, self.confirm_import_btn)
 
     def set_params(self, params):
```

### Comparing `educommon-2.20.0/src/educommon/importer/validators.py` & `educommon-3.0.0/src/educommon/importer/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-# coding: utf-8
 """
 Базовые валидаторы для импортируемых данных.
 
 Использовать только для расширения/исправления логики, реализованной с помощью
 `educommon.importer`. При написании новых классов для импорта/экспорта данных
 рекомендуется использовать пакет `data-transfer`.
 """
-from __future__ import absolute_import
+from abc import (
+    ABCMeta,
+)
 
-from abc import ABCMeta
-from abc import abstractmethod
 
-from six import with_metaclass
-
-
-class IImportDataValidator(with_metaclass(ABCMeta, object)):
+class IImportDataValidator(metaclass=ABCMeta):
     """
     Базовый класс валидатора импортируемых данных.
     """
 
     def __call__(self, data_row, errors, warnings):
         """
         Валидирует строку входных данных.
```

### Comparing `educommon-2.20.0/src/educommon/integration_entities/entities.py` & `educommon-3.0.0/src/educommon/integration_entities/entities.py`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/integration_entities/helpers.py` & `educommon-3.0.0/src/educommon/integration_entities/helpers.py`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/integration_entities/mixins.py` & `educommon-3.0.0/src/educommon/integration_entities/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/ioc/__init__.py` & `educommon-3.0.0/src/educommon/ioc/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,107 @@
-# coding: utf-8
-u"""Данный модуль является IoC-контейнером.
+"""Данный модуль является IoC-контейнером.
 
 Используется для связывания объектов и классов проекта с общей кодовой базой.
 При необходимости использования в общей кодовой базе объектов проекта,
 нужно добавить переменные со значением ``educommon.Undefined`` в данный модуль.
 """
-from __future__ import absolute_import
-
-from educommon import Undefined
+from educommon import (
+    Undefined,
+)
 
 
 observer = Undefined
-u"""Реестр слушателей системы."""
+"""Реестр слушателей системы."""
 
 main_controller = Undefined
-u"""Контроллер, обеспечивающий работу с экшенами приложений."""
+"""Контроллер, обеспечивающий работу с экшенами приложений."""
 
 auth_controller = Undefined
-u"""Контроллер, обеспечивающий работу с экшенами авторизации."""
+"""Контроллер, обеспечивающий работу с экшенами авторизации."""
 
 roles_controller = Undefined
-u"""Контроллер, обеспечивающий работу с экшенами реестра ролей RBAC."""
+"""Контроллер, обеспечивающий работу с экшенами реестра ролей RBAC."""
 
 get_current_user = Undefined
-u"""Функция для получения текущего пользователя, которому назначаются роли.
+"""Функция для получения текущего пользователя, которому назначаются роли.
 
 Должна реализовываться в проекте в связи с тем, что роли могут закрепляться за
 любыми моделями проекта (пользователями, физ. лицами, сотрудниками, учениками,
 родителями и т.д.).
 """
 
 get_user_by_email = Undefined
-u"""Функция, возвращающая учетную запись пользователя по его email'у."""
+"""Функция, возвращающая учетную запись пользователя по его email'у."""
 
 simple_auth__get_login_panel = Undefined
-u"""Функция, возвращающая панель входа в систему в виде компонента."""
+"""Функция, возвращающая панель входа в систему в виде компонента."""
 
 edureception__Specialist = Undefined
-u"""Модель специалиста приема."""
+"""Модель специалиста приема."""
 
 edureception__Office = Undefined
-u"""Модель кабинета."""
+"""Модель кабинета."""
 
 edureception__Applicant = Undefined
-u"""Модель посетителя приема."""
+"""Модель посетителя приема."""
 
 edureception__TimeTableRecord = Undefined
-u"""Модель специалиста приема."""
+"""Модель специалиста приема."""
 
 edureception__ApplicantReception = Undefined
-u"""Модель кабинета."""
+"""Модель кабинета."""
 
 edureception__SpecialistCronTab = Undefined
-u"""Модель посетителя приема."""
+"""Модель посетителя приема."""
 
 edureception__Organizations = Undefined
-u"""Модель учереждений."""
+"""Модель учереждений."""
 
 edureception__Reasons = Undefined
-u"""Модель причин записи на прием."""
+"""Модель причин записи на прием."""
 
 edureception__IdentityDocumentsTypes = Undefined
-u"""Модель типы документов, удостоверяющих личность."""
+"""Модель типы документов, удостоверяющих личность."""
 
 
 def has_value(name):
-    u"""Возвращает True, если значение *name* было установлено.
+    """Возвращает True, если значение *name* было установлено.
 
     :param str name: Имя параметра в контейнере.
 
     :rtype: bool
     """
     return globals().get(name, Undefined) is not Undefined
 
 
 def register(name, value):
-    u"""Регистрирует в контейнере значение *value* под именем *name*.
+    """Регистрирует в контейнере значение *value* под именем *name*.
 
     *name* должен быть объявлен в модуле и равен *Undefined*.
     """
     assert name in globals(), name
 
     # если в globals находится тоже самое значение,
     # то сразу возвращаем результат
     if globals()[name] is value:
         return value
 
     assert globals()[name] is Undefined, (
-        u'"{}" already registered'.format(name)
+        '"{}" already registered'.format(name)
     )
 
     globals()[name] = value
 
     return value
 
 
 def get(name):
-    u"""Возвращает содержимое с именем *name*.
+    """Возвращает содержимое с именем *name*.
 
     *name* должен быть предварительно зарегистрирован через **register**.
     """
-    assert name in globals(), u'Object {} is not registered'.format(name)
+    assert name in globals(), 'Object {} is not registered'.format(name)
     assert globals()[name] is not Undefined, (
-        u'"{}" not registered'.format(name)
+        '"{}" not registered'.format(name)
     )
 
     return globals()[name]
```

### Comparing `educommon-2.20.0/src/educommon/m3/__init__.py` & `educommon-3.0.0/src/educommon/m3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,54 @@
-# coding: utf-8
-u"""Вспомогательные средства для работы с компонентами M3."""
-from __future__ import absolute_import
-
-from collections import defaultdict
-from functools import wraps
+"""Вспомогательные средства для работы с компонентами M3."""
 import inspect
 import sys
+from functools import (
+    wraps,
+)
+
+from django.core.exceptions import (
+    NON_FIELD_ERRORS,
+    ValidationError as DjangoValidationError,
+)
+from django.db.models.base import (
+    Model,
+    ModelBase,
+)
+from django.db.transaction import (
+    atomic,
+)
+from django.utils.encoding import (
+    force_text,
+)
+from m3.actions import (
+    Action,
+    ActionPack,
+    ControllerCache,
+)
+
+from objectpack.exceptions import (
+    ValidationError as ObjectPackValidationError,
+)
+from objectpack.models import (
+    ModelProxy,
+    ModelProxyMeta,
+)
+from objectpack.observer.base import (
+    ObservableController,
+)
+
+from educommon import (
+    ioc,
+)
+from educommon.utils.misc import (
+    NoOperationCM,
+)
 
-from django.core.exceptions import NON_FIELD_ERRORS
-from django.core.exceptions import ValidationError as DjangoValidationError
-from django.db.models.base import Model
-from django.db.models.base import ModelBase
-from django.db.transaction import atomic
-from django.utils.encoding import force_text
-from m3.actions import Action
-from m3.actions import ActionPack
-from m3.actions import ControllerCache
-from objectpack.exceptions import ValidationError as ObjectPackValidationError
-from objectpack.models import ModelProxy
-from objectpack.models import ModelProxyMeta
-from objectpack.observer.base import ObservableController
-import six
-
-from educommon import ioc
-from educommon.utils.misc import NoOperationCM
 
-
-def convert_validation_error_to(exc, new_line=u'<br/>', model=None):
+def convert_validation_error_to(exc, new_line='<br/>', model=None):
     """Декоратор, преобразующий исключение
     django.core.exceptions.ValidationError, генерируемое в декорируемой
     функции, в исключение, указанное в аргументе exc путем объединения всех
     сообщений об ошибках из ValidationError.message_dict в одно сообщение, по
     одной ошибке на строку.
 
     Пример использования:
@@ -42,15 +60,15 @@
                 obj.full_clean()
                 ...
 
     :param exc: класс исключения, к которому будет преобразовываться
         ValidationError
     :type exc: subclass of Exception
 
-    :param unicode new_line: разделитель строк в сообщении об ошибке
+    :param str new_line: разделитель строк в сообщении об ошибке
 
     :param model: Модель, в которой осуществляется валидация. Должна
         использоваться в тех случаях, когда исключение ValidationError
         генерируется вне модели (например, в методе ObjectPack.save_row).
         Если аргумент указан, то данные будут извлекаться именно из этой
         модели.
     """
@@ -67,81 +85,80 @@
         if 'self' not in error_frame.f_locals:
             raise
         model_instance = error_frame.f_locals['self']
         return model_instance._meta
 
     def get_messages_from_dict(model_meta, data):
         result = []
-        for field_name, field_errors in six.iteritems(data):
+        for field_name, field_errors in data.items():
             if field_name == NON_FIELD_ERRORS:
                 result.append(
                     new_line.join(
-                        u'- {0}'.format(err) for err in field_errors
+                        '- {0}'.format(err) for err in field_errors
                     )
                 )
             else:
                 model_field = model_meta.get_field(field_name)
-                verbose_name = (model_field.verbose_name or u'')
+                verbose_name = (model_field.verbose_name or '')
                 result.append(new_line.join(
-                    u'- {0}: {1}'.format(verbose_name, err)
+                    '- {0}: {1}'.format(verbose_name, err)
                     for err in field_errors
                 ))
         return result
 
     def get_messages_from_list(messages):
         result = [
-            u'- ' + message
+            '- ' + message
             for message in messages
         ]
         return result
 
     assert issubclass(exc, Exception), type(exc)
-    new_line = six.text_type(new_line)
+    new_line = str(new_line)
 
     def decorator(func):
         assert inspect.ismethod(func) or inspect.isfunction(func)
 
         @wraps(func)
         def wrapper(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except DjangoValidationError as e:
                 model_meta = get_model_meta(e)
 
                 if hasattr(e, 'message_dict'):
-                    title = u'На форме имеются некорректно заполненные поля:'
+                    title = 'На форме имеются некорректно заполненные поля:'
                     messages = [title] + get_messages_from_dict(model_meta,
                                                                 e.message_dict)
                 else:
-                    title = u'При проверке данных найдены ошибки:'
+                    title = 'При проверке данных найдены ошибки:'
                     messages = [title] + get_messages_from_list(e.messages)
-                messages.insert(1, u'')
+                messages.insert(1, '')
 
                 raise exc(new_line.join(messages))
 
         return wrapper
 
     return decorator
 
 
-class ModelProxyValidationMixin(object):
-
-    u"""Примесь для составных прокси-моделей objectpack'а.
+class ModelProxyValidationMixin:
+    """Примесь для составных прокси-моделей objectpack'а.
 
     Добавляет к *objectpack.models.ModelProxy* возможность валидации данных
     перед сохранением. Валидация осуществляется, как и в моделях Django, путем
     запуска метода *full_clean()* для каждой зависимой модели, порядок запуска
     соответствует порядку указания моделей в *relations*. После выполнения
     валидации зависимых моделей запускается *full_clean()* основной модели.
     """
 
     def __update_error_dict(self, error, errors, model_name):
         model_errors = error.update_error_dict({})
 
-        for field_name, messages in six.iteritems(model_errors):
+        for field_name, messages in model_errors.items():
 
             # В зависимости от версии Django в messages могут быть
             # как сообщения в виде строк, так и экземпляры ValidationError,
             # поэтому приводим его к списку, содержащему только строки
             messages = sum([m.messages if isinstance(
                 m, DjangoValidationError) else [m] for m in messages], [])
 
@@ -170,15 +187,15 @@
                 errors.setdefault(full_field_name, []).extend(messages)
             else:
                 errors.setdefault(NON_FIELD_ERRORS, []).extend(messages)
 
         return errors
 
     def full_clean(self, exclude=None):
-        u"""Валидация данных составной модели.
+        """Валидация данных составной модели.
 
         :param list exclude: Список полей составной модели, исключаемых из
             проверки. Например: 'relation', 'relation1.relation2.name'.
 
             .. note::
                При многоуровневой вложенности вложенная составная модель также
                должна поддерживать валидацию данных (иметь метод
@@ -240,26 +257,24 @@
                         model.__dict__[valid_key] = True
 
         if errors:
             raise DjangoValidationError(errors)
 
 
 class BaseModelProxy(ModelProxyValidationMixin, ModelProxy):
-
-    u"""Базовый класс для составных прокси моделей с валидацией.
+    """Базовый класс для составных прокси моделей с валидацией.
 
     .. seealso::
         - :py:class: objectpack.models.ModelProxy
         - :py:class: ModelProxyValidationMixin
     """
 
 
-class PackValidationMixin(object):
-
-    u"""Примесь к пакам из objectpack, добавляющая валидацию моделей.
+class PackValidationMixin:
+    """Примесь к пакам из objectpack, добавляющая валидацию моделей.
 
     Перед сохранением объекта в методе *save_row()* пака выполняется проверка
     данных путем вызова метода *full_clean()* сохраняемого объекта.
 
     .. note::
        При использовании в паке составной модели
        (*objectpack.models.ModelProxy*) в такой модели должен быть реализован
@@ -273,16 +288,18 @@
 
        class PeriodPack(PackValidationMxin, ObjectPack):
            ....
     """
 
     @convert_validation_error_to(ObjectPackValidationError)
     def save_row(self, obj, create_new, request, context):
-        u"""Вызывает проверку данных перед их сохранением в БД."""
-        from objectpack.slave_object_pack.actions import SlavePack
+        """Вызывает проверку данных перед их сохранением в БД."""
+        from objectpack.slave_object_pack.actions import (
+            SlavePack,
+        )
         if isinstance(self, SlavePack):
             obj.__dict__.update(
                 self._get_parents_dict(context, key_fmt='%s_id')
             )
             save_row = super(SlavePack, self).save_row
         else:
             save_row = super(PackValidationMixin, self).save_row
@@ -294,15 +311,15 @@
 
         with cm:
             obj.full_clean()
             save_row(obj, create_new, request, context)
 
 
 def get_pack(pack_or_model):
-    u"""Возвращает экземпляр указанного пака.
+    """Возвращает экземпляр указанного пака.
 
     Пак может быть задан:
         - именем класса в пакете: 'extedu.unit.actions.Pack'
         - классом пака: Pack
         - именем класса модели: 'Unit'
         - классом модели: Unit
         - экземпляром класса модели: unit
@@ -342,15 +359,15 @@
 
     assert result is not None, repr(pack_or_model)
 
     return result
 
 
 def get_pack_id(pack_or_model):
-    u"""Возвращает имя параметра, идентифицирующего объект.
+    """Возвращает имя параметра, идентифицирующего объект.
 
     .. note::
        Вызов get_pack_id('Unit') аналогичен вызову
        get_pack('Unit').id_param_name.
 
     :param pack_or_model: Аргумент, определяющий пак, из которого будет
         получено имя параметра, идентифицирующего объект (*id_param_name*).
@@ -359,15 +376,15 @@
     """
     pack = get_pack(pack_or_model)
     result = pack.id_param_name
     return result
 
 
 def get_id_value(context, pack_or_model):
-    u"""Возвращает значение параметра, идентифицирующего объект.
+    """Возвращает значение параметра, идентифицирующего объект.
 
     Значение извлекается из контекста запроса *context*, имя параметра
     определяется свойством *id_param_name* пака. Пак определяется аргументом
     *pack_or_model*.
 
     .. note::
         Вызов get_id_value(context, 'Unit') аналогичен вызову
```

### Comparing `educommon-2.20.0/src/educommon/m3/extensions/listeners/__init__.py` & `educommon-3.0.0/src/educommon/m3/extensions/listeners/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-# coding: utf-8
-u"""Расширение поведения экшнов."""
-from __future__ import absolute_import
+"""Расширение поведения экшнов."""
+from m3.actions import (
+    OperationResult,
+)
+from m3.actions.context import (
+    ActionContext,
+    ContextBuildingError,
+    CriticalContextBuildingError,
+    RequiredFailed,
+)
+from m3_ext.ui.results import (
+    ExtUIScriptResult,
+)
+
+from educommon.m3.extensions.ui import (
+    BaseEditWinExtender,
+)
 
-from m3.actions import OperationResult
-from m3.actions.context import ActionContext
-from m3.actions.context import ContextBuildingError
-from m3.actions.context import CriticalContextBuildingError
-from m3.actions.context import RequiredFailed
-from m3_ext.ui.results import ExtUIScriptResult
-import six
 
-from ..ui import BaseEditWinExtender
-
-
-class DeclareContextListener(object):
-
-    u"""
+class DeclareContextListener:
+    """
     Предок листенеров.
 
     Предоставляет возможность задекларировать дополнительный контекст
     выполнения экшна
     """
 
     def before(self, request, context):
-        u"""Действия перед вызовом экшна."""
+        """Действия перед вызовом экшна."""
         # получение контекста по "обновленным правилам", если они были
         rebuilt_context = self._rebuild_context(request, context)
         rebuilt_context_dict = rebuilt_context.__dict__
         if rebuilt_context_dict:
             # этот же страх делается и внутри метода ``ActionContext.combine``
             context.__dict__.update(rebuilt_context_dict)
 
     def _declare_additional_context(self):
-        u"""Дополнительная декларация контекста."""
+        """Дополнительная декларация контекста."""
         return {}
 
     def _rebuild_context(self, request, context):
-        u"""Пересбор контекста с учетом дополнительных правил."""
+        """Пересбор контекста с учетом дополнительных правил."""
         rules = self.action.context_declaration()
         additional_rules = self._declare_additional_context()
 
         if not additional_rules:
             # дополнительно ничего не задекларировали, возврат пустого контекст
             return ActionContext()
         else:
@@ -52,50 +55,49 @@
         try:
             context.build(request, rules)
         except CriticalContextBuildingError:
             # критическая ошибка сбора контекста - должна валиться
             raise
         except ContextBuildingError as e:
             # некритичную ошибку - показываем пользователю
-            return OperationResult.by_message(six.text_type(e))
+            return OperationResult.by_message(str(e))
         except RequiredFailed as e:
             # если контекст неправильный, то возвращаем
             # фейльный результат операции
             return OperationResult.by_message(
-                u'Не удалось выполнить операцию. '
-                u'Не задан обязательный<br>параметр: ' + e.reason
+                'Не удалось выполнить операцию. '
+                'Не задан обязательный<br>параметр: ' + e.reason
             )
         return context
 
 
 class BaseEditWinListener(DeclareContextListener):
-
-    u"""
+    """
     Базовый листенер для расширения окна редактирования доп.полями и данными.
 
     Окно редактирования связано с определенной моделью, она - расширяемая и ее
     данные требуется дополнить с помощью доп.полей.
     """
 
     # класс-наследник BaseEditWinExtender
     # отвечает за расширение интерфейса окна и биндинг
     ui_extender_cls = None
     # имя поля, которое ссылается на расширяемую модель
     parent_model_field = None
 
     def _get_id(self, context):
-        u"""
+        """
         Получение из контекста параметра, определяющего id расширяемой модели.
 
         :rype: int
         """
         raise NotImplementedError()
 
     def _get_instance(self, row_id):
-        u"""
+        """
         Получение модели, которая расширяет основную ``ui_extender_cls.model``.
 
         :param row_id: идентификатор расширяемой модели
         :rtype: object
         """
         try:
             instance = self.ui_extender_cls.model.objects.get(**{
@@ -103,21 +105,21 @@
             })
         except self.ui_extender_cls.model.DoesNotExist:
             # расширяющая модель еще только создается
             return
         return instance
 
     def _get_params(self, instance, context):
-        u"""Дополнение параметров."""
+        """Дополнение параметров."""
         return {
             'instance': instance
         }
 
     def after(self, request, context, response):
-        u"""
+        """
         Получение истанса модели, которая расширяет и биндинг ее в окно.
 
         :param request: Request
         :type request: django.http.HttpRequest
         :param context: Context
         :type context: m3.actions.context.DeclarativeActionContext
         """
@@ -145,16 +147,15 @@
         extender.bind_from_object(instance)
         # установка параметров
         params = self._get_params(instance, context)
         extender.set_params(params)
 
 
 class BaseSaveListener(DeclareContextListener):
-
-    u"""
+    """
     Базовый класс листенеров сохранения доп.данных.
 
     Обращение к данному листенеру из экшна делается через
 
     ..code::
 
         self.handle('post_save', (obj, context))
@@ -165,15 +166,15 @@
 
     # класс-наследник BaseEditWinExtender
     ui_extender_cls = None
     # имя поля, ссылающуюся на родительскую модель
     parent_model_field = None
 
     def _get_instance(self, parent_model_instance, context):
-        u"""
+        """
         Получение инстанса расширяющей модели.
 
         Метод вынесен для возможности инстанцирования дополнительных
         зависимых моделей (относительно расширяющей модели ``instance``)
 
         :param parent_model_instance: инстанс расширяемой модели
         :param context: Context
@@ -187,15 +188,15 @@
         except self.ui_extender_cls.model.DoesNotExist:
             instance = self.ui_extender_cls.model(**{
                 self.parent_model_field: parent_model_instance
             })
         return instance
 
     def post_save(self, arguments):
-        u"""
+        """
         Точка входа для расширения из экшна self.handle('post_save', *).
 
         :param parent_model_instance: инстанс расширяемой модели
         :param context: Context
         :type context: m3.actions.context.DeclarativeActionContext
         """
         parent_model_instance, context = arguments
@@ -207,14 +208,14 @@
         self.ui_extender_cls.bind_to_object(instance, context)
 
         self._save_instance(instance)
 
         return parent_model_instance, context
 
     def _save_instance(self, instance):
-        u"""
+        """
         Сохранение расширяющей модели.
 
         Вынесено для возможности сохранения связанных/зависимых сущностей
         """
         instance.full_clean()
         instance.save()
```

### Comparing `educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js` & `educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/listeners.py` & `educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/listeners.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,39 @@
-# coding: utf-8
-from __future__ import absolute_import
+from collections import (
+    defaultdict,
+)
+
+from django.dispatch import (
+    Signal,
+)
+from m3.actions import (
+    OperationResult,
+)
+
+from objectpack.actions import (
+    ObjectDeleteAction,
+)
+from objectpack.models import (
+    ModelProxy,
+)
+
+from educommon.m3.extensions.listeners.delete_check.mixins import (
+    CascadeDeleteMixin,
+)
+from educommon.m3.extensions.listeners.delete_check.ui import (
+    CancelConfirmWindow,
+)
+from educommon.utils.db import (
+    get_non_block_relations,
+    get_related_instances_proxy,
+)
 
-from collections import defaultdict
 
-from django.dispatch import Signal
-from m3.actions import OperationResult
-from objectpack.actions import ObjectDeleteAction
-from objectpack.models import ModelProxy
-import six
-
-from educommon.utils.db import get_non_block_relations
-from educommon.utils.db import get_related_instances_proxy
-
-from .mixins import CascadeDeleteMixin
-from .ui import CancelConfirmWindow
-
-
-class DeleteCheck(object):
-
-    u"""Проверяет объекты перед удалением на наличие зависимостей.
+class DeleteCheck:
+    """Проверяет объекты перед удалением на наличие зависимостей.
 
     В случае, если в системе есть объекты, зависимые от удаляемого объекта и
     не отмеченные для каскадного удаления через cascade_delete_objects, то
     отменяет удаление и выводит окно с предупреждением и списком зависимых
     объектов.
     Если в системе есть только зависимые объекты, помеченные
     cascade_delete_objects, то выводится сообщение с кнопкой Удалить, для
@@ -42,36 +53,36 @@
     collect_implicit = Signal(
         providing_args=['objects_to_delete', 'related_objects']
     )
 
     def _get_message(self, objects):
         """Возвращает сообщение в правильном склонении."""
         return (
-            u'объекта' if len(objects) == 1 else u'объектов',
-            u'него' if len(objects) == 1 else u'них'
+            'объекта' if len(objects) == 1 else 'объектов',
+            'него' if len(objects) == 1 else 'них'
         )
 
     def _setup_window(self, objects, related_objects, blocked=True,
                       grid_id=None):
         """Возвращает окно с сообщением о связанных объектах.
 
         :param objects: удаляемые объекты
         :param related_objects: связанные объекты
         :param bool blocked: режим показа окна блокирующее/не блокирующее
         :param str grid_id: id грида, из которого происходит удаление
         :return: CancelConfirmWindow
         """
         if blocked:
             title = (
-                u'Удаление {} невозможно, т.к. на {} есть ссылки:'
+                'Удаление {} невозможно, т.к. на {} есть ссылки:'
                 .format(*self._get_message(objects))
             )
         else:
             title = (
-                u'При удалении {} будут удалены следующие связи:'
+                'При удалении {} будут удалены следующие связи:'
                 .format(self._get_message(objects)[0])
             )
 
         win = CancelConfirmWindow()
         win.set_params(dict(
             title=title,
             objects=objects,
```

### Comparing `educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/mixins.py` & `educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-# coding: utf-8
-from __future__ import absolute_import
+from m3.db import (
+    safe_delete,
+)
+from m3_django_compat import (
+    atomic,
+    get_model,
+)
+
+from educommon.m3.extensions.listeners.delete_check.signals import (
+    post_cascade,
+    pre_cascade,
+)
+from educommon.m3.extensions.listeners.delete_check.utils import (
+    get_related_instances_and_handlers,
+)
 
-from m3.db import safe_delete
-from m3_django_compat import atomic
-from m3_django_compat import get_model
 
-from .signals import post_cascade
-from .signals import pre_cascade
-from .utils import get_related_instances_and_handlers
+class CascadeDeletePackMixin:
 
-
-class CascadeDeletePackMixin(object):
-
-    u"""Mixin определяющий исключаемые поля модели при проверке DeleteCheck.
+    """Mixin определяющий исключаемые поля модели при проверке DeleteCheck.
 
     Поскольку DeleteCheck срабатывает до вызова delete_row возникают ситуации,
     когда нам требуется при работе с этим паком исключить определенные
     поля модели, из которых имеются ссылки на модель. Для решения данных
     ситуаций используется атрибут cascade_delete_objects.
 
     .. code-block:: python
@@ -55,17 +60,16 @@
     @atomic
     def delete_row(self, obj_id, request, context):
         self._cascade_delete(obj_id, request, context)
         return super(CascadeDeletePackMixin, self).delete_row(
             obj_id, request, context)
 
 
-class CascadeDeleteMixin(object):
-
-    u"""Определяет связи, исключаемые при проверке в ``DeleteCheck``.
+class CascadeDeleteMixin:
+    """Определяет связи, исключаемые при проверке в ``DeleteCheck``.
 
     Перед удалением объекта модели обеспечивает удаление или изменение
     зависимых от него объектов, если настройки зависимых объектов
     (``cascade_delete_for``) позволяют это делать.
 
     (``cascade_delete_for``) может быть как кортежем с перечислением полей,
     так и словарем, ключем в котором выступает поле, а значением словарь с
@@ -148,15 +152,15 @@
 
     @staticmethod
     def skip_field(field):
         return field in getattr(field.model, 'cascade_delete_for', ())
 
     @atomic
     def safe_delete(self):
-        u"""Выполнение действий над связанными объектами перед удалением."""
+        """Выполнение действий над связанными объектами перед удалением."""
         for obj, handler in get_related_instances_and_handlers(
             self, skip_func=lambda field: not self.skip_field(field)
         ):
             params = dict(
                 sender=self._meta.model,
                 instance=obj,
                 initiator=self
```

### Comparing `educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/ui.py` & `educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from django.template.loader import render_to_string
-from m3_ext.ui import all_components as ext
-from m3_ext.ui.containers.forms import ExtPanel
-from objectpack.ui import BaseWindow
-import six
-
-from educommon.django.db.model_view import registries
-from educommon.utils.ui import local_template
+from django.template.loader import (
+    render_to_string,
+)
+from m3_ext.ui import (
+    all_components as ext,
+)
+from m3_ext.ui.containers.forms import (
+    ExtPanel,
+)
+
+from objectpack.ui import (
+    BaseWindow,
+)
+
+from educommon.django.db.model_view import (
+    registries,
+)
+from educommon.utils.ui import (
+    local_template,
+)
 
 
 class RelatedObjectsWindow(BaseWindow):
 
-    u"""Окно с информацией о зависимых объектах.
+    """Окно с информацией о зависимых объектах.
 
     Используется для отображения информации об объектах, зависящих от
     удаляемых.
 
     В параметрах окна должен быть указан список удаляемых объектов и список
     объектов, зависимых от удаляемых.
     """
 
     #: Шаблон HTML-страницы с представлениями моделей.
     html_template = local_template('related-objects-window.html')
 
     @property
     def model_view_registry(self):
-        u"""Реестр представлений моделей."""
+        """Реестр представлений моделей."""
         return registries['related_objects']
 
     def _init_components(self):
         super(RelatedObjectsWindow, self)._init_components()
 
         self.panel = ExtPanel(
             auto_scroll=True,
@@ -45,29 +54,29 @@
         self.height = 600
 
         self.layout = 'fit'
 
     def _get_html(self, title, objects, related_objects):
         views = tuple(
             self.model_view_registry.get(model).get_view(objects)
-            for model, objects in six.iteritems(related_objects)
+            for model, objects in related_objects.items()
         )
 
         return render_to_string(
             template_name=self.html_template,
             context=dict(
                 title=title,
                 views=views,
             ),
         )
 
     def set_params(self, params):
         super(RelatedObjectsWindow, self).set_params(params)
 
-        self.title = u'Внимание!'
+        self.title = 'Внимание!'
 
         self.panel.html = self._get_html(
             params.get('title'),
             params['objects'],
             params['related_objects'],
         )
```

### Comparing `educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/utils.py` & `educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from django.db.models import SET_DEFAULT
-from django.db.models import SET_NULL
-from educommon.utils.db import get_related_fields
-from m3.db import safe_delete
-from m3_django_compat import get_related
+from django.db.models import (
+    SET_DEFAULT,
+    SET_NULL,
+)
+from m3.db import (
+    safe_delete,
+)
+from m3_django_compat import (
+    get_related,
+)
+
+from educommon.utils.db import (
+    get_related_fields,
+)
 
 
 def get_related_instances_and_handlers(obj, skip_func=None):
-    u"""Возвращает генератор связанных объектов с функциями-обработчиками."""
+    """Возвращает генератор связанных объектов с функциями-обработчиками."""
     for field in get_related_fields(obj.__class__, skip_func=skip_func):
         related_model = field.model
         field_name = field.name
         if field.many_to_many:
             related_model = field.remote_field.through
             field_name = field.m2m_reverse_name()
 
@@ -23,40 +29,40 @@
 
         on_delete_function = get_on_relation_delete_function(field)
         for related_obj in related_objects.iterator():
             yield related_obj, on_delete_function
 
 
 def get_on_relation_delete_function(field):
-    u"""Возвращает функцию, которая будет вызыватся при удалении связи.
+    """Возвращает функцию, которая будет вызыватся при удалении связи.
 
     Если в `cascade_delete_for` модели, для поля в параметре `on_delete`
     указана функция то возвращается именно она, в противном случае
     возвращается функция, соответсвующая поведению, указанному в атрибуте
     `on_delete` поля.
     """
     return (
         get_custom_on_delete_function(field) or
         get_field_on_delete_function(field)
     )
 
 
 def get_custom_on_delete_function(field):
-    u"""Возвращает функцию, указанную в cascade_delete_for для поля."""
+    """Возвращает функцию, указанную в cascade_delete_for для поля."""
     if (
         not hasattr(field.model, 'cascade_delete_for') or
         not isinstance(field.model.cascade_delete_for, dict)
     ):
         return None
     on_delete_params = field.model.cascade_delete_for[field]
     return on_delete_params.get('on_delete')
 
 
 def get_field_on_delete_function(field):
-    u"""Возвращает функцию, которая соответсвует поведению on_delete поля."""
+    """Возвращает функцию, которая соответсвует поведению on_delete поля."""
     model = field.model
     on_delete_function = get_related(field).on_delete
 
     if field.many_to_many:
         return safe_delete
 
     if on_delete_function == SET_NULL:
```

### Comparing `educommon-2.20.0/src/educommon/m3/extensions/ui.py` & `educommon-3.0.0/src/educommon/m3/extensions/ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# coding: utf-8
-u"""Расширение поведения интерфейсов."""
-from __future__ import absolute_import
+"""Расширение поведения интерфейсов."""
+from m3_ext.ui import (
+    all_components as ext,
+)
 
-from m3_ext.ui import all_components as ext
-from objectpack.ui import model_fields_to_controls
+from objectpack.ui import (
+    model_fields_to_controls,
+)
 
 
-class BaseEditWinExtender(object):
-
-    u"""
+class BaseEditWinExtender:
+    """
     Базовый объект для расширения окон редактирования.
 
     ``_extend_edit_win`` - добавление и размещение контролов
     ``bind_to_object`` - заполнение объекта данными из полей формы
     ``bind_from_object`` - заполнение полей формы из объекта
     """
 
@@ -26,41 +27,41 @@
 
     def __init__(self, win):
         # ожидается окно
         self._win = win
         self._extend_edit_win()
 
     def _extend_edit_win(self):
-        u"""
+        """
         Расширение формы окна.
 
         ..code::
 
             for fld in self.model_fields_to_controls(self.model_fields):
                 self._win.form.items.append(fld)
 
         """
         raise NotImplementedError()
 
     def model_fields_to_controls(self, fields):
-        u"""Шорткат для генерации контролов."""
-        assert self.model, u'No model defined in Extender!'
+        """Шорткат для генерации контролов."""
+        assert self.model, 'No model defined in Extender!'
         return model_fields_to_controls(
             self.model,
             self._win,
             field_list=fields,
             model_register=self.model_register
         )
 
     # -------------------------------------------------------------------------
     # Биндинг из формы в объект
 
     @classmethod
     def set_value(cls, instance, field_names, value):
-        u"""
+        """
         Установка значения поля (полей).
 
         :param instance: инстанс модели, которая расширяет основную ``model``
         :param list field_names: список связаных полей (либо одно поле)
         :raise: DoesNotExist если предварительно не инстанцировали зависимые
         сущности (для случая связанных полей)
         """
@@ -71,53 +72,53 @@
             # есть связанные поля, достаются связанные сущности
             # связанные сущности должны быть получены
             nested = getattr(instance, field_names[0])
             cls.set_value(nested, field_names[1:], value)
 
     @classmethod
     def bind_to_object(cls, instance, context):
-        u"""
+        """
         Заполнение полей ``model_fields`` модели instance по полям формы.
 
         :param instance: инстанс модели, которая расширяет основную ``model``
         :param context: контекст
         :type context: m3.actions.context.DeclarativeActionContext
         """
         assert cls.model_fields is not None, (
-            u'No model_fields defined in Extender')
+            'No model_fields defined in Extender')
 
         for field_name in cls.model_fields:
             try:
                 value = getattr(context, field_name)
             except AttributeError:
                 value = None
 
             field_names = field_name.split('.')
             cls.set_value(instance, field_names, value)
 
     # -------------------------------------------------------------------------
     # Биндинг из объекта в форму
 
     def bind_from_object(self, instance):
-        u"""
+        """
         Заполнение полей ``model_fields`` формы по полям модели instance.
 
         :param instance: инстанс модели, которая расширяет основную ``model``
         """
         assert self.model_fields is not None, (
-            u'No model_fields defined in Extender')
+            'No model_fields defined in Extender')
         for name in self.model_fields:
             field = self._win.find_by_name(name)
             field_names = field.name.split('.')
             value = self._get_value(instance, field_names)
             if value:
                 self._set_value_to_field(field, value)
 
     def _get_value(self, instance, field_names):
-        u"""
+        """
         Получение значение поля (полей).
 
         :param instance: инстанс модели, которая расширяет основную ``model``
         :param list field_names: список связаных полей (либо одно поле)
         :raise: DoesNotExist если предварительно не инстанцировали зависимые
         сущности (для случая связанных полей)
         """
@@ -127,15 +128,15 @@
         else:
             # есть связанные поля, достаются связанные сущности
             nested = getattr(instance, field_names[0], None)
             return self._get_value(nested, field_names[1:])
 
     @staticmethod
     def _set_value_to_field(field, value):
-        u"""
+        """
         Установка значения в поле.
 
         :param field: наследник BaseExtField
         :param value: значение для установки в поле
         """
         field.value = value
         if isinstance(field, ext.ExtDictSelectField):
@@ -146,15 +147,15 @@
                 else:
                     field.default_text = pack.get_display_text(
                         value, field.display_field)
         elif isinstance(field, ext.ExtCheckBox):
             field.checked = bool(value)
 
     def set_params(self, params):
-        u"""
+        """
         Установка параметров компонентам.
 
         Выполняется по завершению создания компонент, размещению на форме и
         после биндинга значений в форму.
 
         ..code::
```

### Comparing `educommon-2.20.0/src/educommon/m3/transaction_context.py` & `educommon-3.0.0/src/educommon/m3/transaction_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding: utf-8
 """
 Модуль позволяющий реализовать управление порядком выполнения
 обработчиков сигналов возбужденных в контексте некой операции,
 "завернутой" в транзакцию.
 
 Типичный сценарий:
 
@@ -26,21 +25,27 @@
 with TransactionCM('user_import'):
     for login, pwd in source:
         with SavePointCM():
             user = User(username=login)
             user.set_password(pwd)
             user.save()
 """
-from __future__ import absolute_import
-
-from functools import wraps
-from threading import local as _local
-from uuid import uuid4
-
-from django.db import transaction
+from functools import (
+    wraps,
+)
+from threading import (
+    local as _local,
+)
+from uuid import (
+    uuid4,
+)
+
+from django.db import (
+    transaction,
+)
 
 
 _state = _local()
 
 
 def _reset_state():
     _state.rolled_back = set()
@@ -61,22 +66,22 @@
     Исключение, прерывающее текущий CM (SavePointCM/TransactionCM).
     Поймав это исключение CM откатывает изменения,
     произошедшие с момента входа в него и корректно завершается.
     """
     pass
 
 
-class SavePointCM(object):
+class SavePointCM:
     """
     Context Manager создающий на время своего действия savepoint
     """
 
     def __init__(self):
         assert _state.situation, (
-            u'Must be nested in TransactionCM!'
+            'Must be nested in TransactionCM!'
         )
         cookie = uuid4()
         _state.cookies.append(cookie)
         self._cookie = cookie
         self._sid = None
 
     def __enter__(self):
@@ -93,22 +98,23 @@
             _state.rolled_back.add(self._cookie)
             return ex_type is AbortTransaction
 
     def rollback(self):
         raise AbortTransaction()
 
 
-class TransactionCM(object):
+class TransactionCM:
     """
     ContextManager создающий "ручную" транзакцию
     """
+
     def __init__(self, situation, rollback_all=True, using=None):
         _prepare_state()
         assert not _state.situation, (
-            u'Nested contexts not supported!'
+            'Nested contexts not supported!'
         )
         _reset_state()
         _state.situation = self._situation = situation
 
         self._using = using
 
     def __enter__(self):
```

### Comparing `educommon-2.20.0/src/educommon/objectpack/actions.py` & `educommon-3.0.0/src/educommon/objectpack/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,73 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from collections import OrderedDict
-
-from django.template.loader import render_to_string
-from m3.actions import OperationResult
-from m3_django_compat import ModelOptions
-from m3_ext.ui.results import ExtUIComponentResult
-from objectpack.actions import BaseAction
-from objectpack.actions import BasePack
-from objectpack.actions import BaseWindowAction
-from objectpack.models import ModelProxy
-import six
-
-from educommon.utils.ui import reconfigure_grid_by_access
-
-from . import ui
-from .ui import BaseGridWindow
+from collections import (
+    OrderedDict,
+)
+
+from django.template.loader import (
+    render_to_string,
+)
+from m3.actions import (
+    OperationResult,
+)
+from m3_django_compat import (
+    ModelOptions,
+)
+from m3_ext.ui.results import (
+    ExtUIComponentResult,
+)
+
+from objectpack.actions import (
+    BaseAction,
+    BasePack,
+    BaseWindowAction,
+)
+from objectpack.models import (
+    ModelProxy,
+)
+
+from educommon.objectpack import (
+    ui,
+)
+from educommon.objectpack.ui import (
+    BaseGridWindow,
+)
+from educommon.utils.ui import (
+    reconfigure_grid_by_access,
+)
 
 
 class BaseGridPack(BasePack):
-    u"""
+    """
     Пак умеющий строить динамический грид с изменяющимся
     количеством колонок в зависимости от значений полей фильтрации.
-
     """
+
     window = BaseGridWindow
 
     # аттрибуты грида
     column_param_name = None
-    u"""
+    """
     Например, для колонок из классов можно определить
 
     column_param_name = 'classyear_id'
     """
     row_id_name = None
-    u"""
+    """
     Например, для строк из звонков расписания можно определить
 
     row_id_name = 'call_id'
     """
 
     @property
     def id_param_name(self):
         return '%s_id' % self.short_name
 
     @property
     def grid_panel(cls):
-        u"""
+        """
         Класс панели с гридом.
 
         .. note::
             Вынесено в метод для случая, когда пак работает с гридом,
             размещенным не в окне, а, например, в табе
         """
         return cls.window.grid_panel_cls
@@ -59,35 +75,35 @@
     def __init__(self):
         super(BaseGridPack, self).__init__()
         self.grid_action = BaseGridCreateAction()
         self.window_action = BaseGridWinAction()
         self.actions.extend([self.grid_action, self.window_action])
 
     def create_columns(self, request, context):
-        u"""
+        """
         Метод возвращающий колонки.
 
         .. seealso:: objectpack.actions.ObjectPack.columns
 
         :rtype: list
         """
         return []
 
     def create_grid(self, columns):
-        u"""
+        """
         Создание грида.
 
         :param list columns: список колонок
         :rtype: m3_ext.ui.ExtObjectGrid
         """
         grid = self.grid_panel.create_grid(pack=self, columns=columns)
         return grid
 
     def set_grid_params(self, grid, request, context):
-        u"""
+        """
         Настройка параметров для конфигурации грида.
 
         Параметры грида передаются панели с гридом в метод configure_grid.
         :param grid: грид
         :type grid: m3_ext.ui.ExtObjectGrid
         :param request: Запрос
         :type request: django.http.HttpRequest
@@ -97,52 +113,52 @@
         :returns: словарь параметров для создания грида
         """
         # пак для настройки грида (column_param_name, id_param_name, url_data)
         params = {'pack': self}
         return params
 
     def configure_grid(self, grid, request, context):
-        u"""
+        """
         Метод конфигурирования грида после его создания.
         :param grid: грид
         :type grid: m3_ext.ui.ExtObjectGrid
         :param request: Запрос
         :type request: django.http.HttpRequest
         :param context: Контекст
         :type context: m3.actions.context.DeclarativeActionContext
         """
         params = self.set_grid_params(grid, request, context)
         grid = self.grid_panel.configure_grid(grid, params)
         return grid
 
     def get_grid_action_url(self):
-        u"""
+        """
         Получение адреса экшна построения грид.
 
         :rtype: str
         """
         return self.grid_action.get_absolute_url()
 
     def get_rows_url(self):
-        u"""
+        """
         Получение адреса экшна, возвращающего строки грида.
 
         Должен быть определен в потомке.
         :rtype: str
         """
         raise NotImplementedError(
-            u"Не определен метод get_rows_url() "
-            u"в %s!" % self.__class__.__name__)
+            "Не определен метод get_rows_url() "
+            "в %s!" % self.__class__.__name__)
 
     def create_window(self, request, context):
-        u"""Получение окна."""
+        """Получение окна."""
         return self.window()
 
     def get_window_params(self, request, context):
-        u"""
+        """
         Параметры для показа окна
         :param request: Запрос
         :type request: django.http.HttpRequest
         :param context: Контекст
         :type context: m3.actions.context.DeclarativeActionContext
         :rtype: dict
 
@@ -155,60 +171,59 @@
             # пак отвечающий за получения грида окном
             "grid_pack": self
         }
         return params
 
 
 class BaseGridCreateAction(BaseAction):
-    u"""Базовый экшн построения грида."""
+    """Базовый экшн построения грида."""
 
     perm_code = 'view'
 
     def run(self, request, context):
         pack = self.parent
         columns = pack.create_columns(request, context)
         grid = pack.create_grid(columns)
         pack.configure_grid(grid, request, context)
         return ExtUIComponentResult(grid)
 
 
 class BaseGridWinAction(BaseWindowAction):
-    u"""Экшн показа окна."""
+    """Экшн показа окна."""
 
     perm_code = 'view'
 
     def create_window(self):
         self.win = self.parent.create_window(self.request, self.context)
 
     def set_window_params(self):
         super(BaseGridWinAction, self).set_window_params()
         self.win_params = self.parent.get_window_params(
             self.request, self.context)
 
 
-class RelationsCheckMixin(object):
-
-    u"""
+class RelationsCheckMixin:
+    """
     Миксин для экшенов удаления и редактирования, проверяющий наличие
     ссылок на редактируемый/удаляемый объект и выводящий данную информацию
     в табличном виде.
     """
 
     # Описание настроек отображения информации для каждой модели.
     rel_conf = {}
     # Список с именами моделей, которые должны проверяться
     rel_list = []
     # Список с именами моделей, которые нужно исключить из проверки
     rel_ignore_list = []
-    err_msg = u'На объект "{obj}" есть ссылки:'
+    err_msg = 'На объект "{obj}" есть ссылки:'
     render_template_name = 'relations-check-mixin-template.html'
 
     def __init__(self, rel_conf=None, rel_list=None,
                  rel_ignore_list=None, err_msg=None, *args, **kwargs):
-        u"""
+        """
         :param rel_conf: настройки отображения
         :type dict
         :param rel_list: список моделей
         :type: list
         :param rel_ignore_list: список игнорироемых моделей
         :type list
         :param err_msg: сообщение об ошибке
@@ -237,15 +252,15 @@
         if rel_ignore_list:
             self.rel_ignore_list = rel_ignore_list
         if err_msg:
             self.err_msg = err_msg
         super(RelationsCheckMixin, self).__init__(*args, **kwargs)
 
     def _get_relations_to_check(self):
-        u"""Получение всех связанных моделей для проверки."""
+        """Получение всех связанных моделей для проверки."""
         model = self._get_check_model()
         opts = ModelOptions(model)
         all_related_objects = [
             rel_obj.relation for rel_obj in opts.get_all_related_objects()
         ]
         result = all_related_objects[:]
 
@@ -260,18 +275,18 @@
                 rel for rel in all_related_objects
                 if rel.field.model.__name__ in self.rel_list
             ]
 
         return result
 
     def _get_check_model(self):
-        u"""Получение модели для проверки."""
+        """Получение модели для проверки."""
 
         def _extract_proxy_from_model(model):
-            u"""Если получена не модель, а прокси, то извлекает из него модель.
+            """Если получена не модель, а прокси, то извлекает из него модель.
             Функция рекурсивна, т.к. возможны прокси на прокси.
             """
             if issubclass(model, ModelProxy) and hasattr(
                 model, 'model'
             ):
                 model = _extract_proxy_from_model(model.model)
             elif model._meta.proxy:
@@ -279,22 +294,22 @@
                 model = _extract_proxy_from_model(model._meta.proxy_for_model)
 
             return model
 
         return _extract_proxy_from_model(self.parent.model)
 
     def _get_objects_to_check(self, request, context):
-        u"""Получение списка проверяемых объектов."""
+        """Получение списка проверяемых объектов."""
         ids = getattr(context, self.parent.id_param_name, [])
         if isinstance(ids, int):
             ids = [ids]
         return self._get_check_model().objects.filter(id__in=ids)
 
     def collect_related_objects(self, request, context):
-        u"""
+        """
         Получение списка связанных объектов
         :param request: Запрос
         :type request: django.http.HttpRequest
         :param context: Контекст
         :type context: m3.actions.context.DeclarativeActionContext
 
         """
@@ -332,34 +347,34 @@
                 if conf.get('get_query'):
                     query = conf['get_query'](query, obj)
 
                 count = query.count()
                 objects_limit = conf.get('objects_limit', 100)
                 query = query[:objects_limit]
 
-                display = conf.get('display', lambda obj: [six.text_type(obj)])
+                display = conf.get('display', lambda obj: [str(obj)])
                 objects = [display(o) for o in query]
 
                 if count:
                     object_relations['relations'].append({
                         'model': rel.field.model,
                         'title': (conf.get('title') or
                                   rel.field.model._meta.verbose_name),
                         'columns': conf.get('columns'),
                         'objects': objects,
                         'count': count,
                     })
 
         return dict(
-            items=[v for v in six.itervalues(result) if v['relations']],
+            items=[v for v in result.values() if v['relations']],
             model_name=model._meta.verbose_name,
         )
 
     def pre_run(self, request, context):
-        u"""
+        """
         Вывод окна отчета
         :param request: Запрос
         :type request: django.http.HttpRequest
         :param context: Контекст
         :type context: m3.actions.context.DeclarativeActionContext
 
         """
@@ -381,16 +396,16 @@
 
             return OperationResult(
                 success=False,
                 code=win.get_script()
             )
 
 
-class ViewWindowPackMixin(object):
-    u"""Примесь к паку с окном просмотра.
+class ViewWindowPackMixin:
+    """Примесь к паку с окном просмотра.
 
     Добавляет кнопку просмотра в ListWindow, запрещает редактирование.
     """
 
     def create_edit_window(self, create_new, request, context):
         window = super(ViewWindowPackMixin, self).create_edit_window(
             create_new, request, context
```

### Comparing `educommon-2.20.0/src/educommon/objectpack/templates/filter-panel.js` & `educommon-3.0.0/src/educommon/objectpack/templates/filter-panel.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/objectpack/templates/grid-panel.js` & `educommon-3.0.0/src/educommon/objectpack/templates/grid-panel.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/objectpack/templates/multiSelectWindow.js` & `educommon-3.0.0/src/educommon/objectpack/templates/multiSelectWindow.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/objectpack/templates/multiselect-page-fix.js` & `educommon-3.0.0/src/educommon/objectpack/templates/multiselect-page-fix.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/objectpack/templates/relations-check-mixin-template.html` & `educommon-3.0.0/src/educommon/objectpack/templates/relations-check-mixin-template.html`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/objectpack/ui.py` & `educommon-3.0.0/src/educommon/objectpack/ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,42 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from m3_ext.ui import all_components as ext
-from m3_ext.ui import render_component
-from m3_ext.ui.containers.grids import ExtGridGroupingView
-from m3_ext.ui.misc import store as ext_store
-from m3_ext.ui.misc.store import ExtJsonWriter
-from objectpack.ui import BaseEditWindow as OPBaseEditWindow
-from objectpack.ui import BaseListWindow as OPBaseListWindow
-from objectpack.ui import BaseMultiSelectWindow as OPBaseMultiSelectWindow
-from objectpack.ui import BaseSelectWindow as OPBaseSelectWindow
-from objectpack.ui import BaseWindow
-from objectpack.ui import ColumnsConstructor
-from objectpack.ui import ComboBoxWithStore
-from objectpack.ui import ModelEditWindow as OPModelEditWindow
-from objectpack.ui import TabbedEditWindow as OPTabbedEditWindow
-import six
-
-from educommon.utils.ui import local_template
-from educommon.utils.ui import reconfigure_grid_by_access
-from educommon.utils.ui import switch_window_in_read_only_mode
+from m3_ext.ui import (
+    all_components as ext,
+    render_component,
+)
+from m3_ext.ui.containers.grids import (
+    ExtGridGroupingView,
+)
+from m3_ext.ui.misc import (
+    store as ext_store,
+)
+from m3_ext.ui.misc.store import (
+    ExtJsonWriter,
+)
+
+from objectpack.ui import (
+    BaseEditWindow as OPBaseEditWindow,
+    BaseListWindow as OPBaseListWindow,
+    BaseMultiSelectWindow as OPBaseMultiSelectWindow,
+    BaseSelectWindow as OPBaseSelectWindow,
+    BaseWindow,
+    ColumnsConstructor,
+    ComboBoxWithStore,
+    ModelEditWindow as OPModelEditWindow,
+    TabbedEditWindow as OPTabbedEditWindow,
+)
+
+from educommon.utils.ui import (
+    local_template,
+    reconfigure_grid_by_access,
+    switch_window_in_read_only_mode,
+)
 
 
 class GridPanel(ext.ExtPanel):
-    u"""
+    """
     Панель, имеющая grid_url, по которому получает грид и вставляет в себя
     """
 
     grid_url = None
     template = 'grid-panel.js'
     grid_class = ext.ExtObjectGrid
 
@@ -35,15 +44,15 @@
         # в инитах затирается темплейт
         t = self.template
         super(GridPanel, self).__init__(*args, **kwargs)
         self.template = t
 
     @staticmethod
     def _create_grid(pack, columns, grid_cls, group_by=None, **kwargs):
-        u"""
+        """
         Метод возвращает грид
         :param grid_cls: класс грида
         :type grid_cls: ExtObjectGrid
         :param str group_by: темплейт для группирования
         """
         grid = grid_cls(
             region='north',
@@ -82,15 +91,15 @@
             configure_reader = lambda col: None
 
         def populate(root, columns):
             for c in columns:
                 sub_cols = c.pop('columns', None)
                 params = {}
                 params.update(c)
-                params['header'] = six.text_type(params.pop('header', ''))
+                params['header'] = str(params.pop('header', ''))
                 # TODO - сомнительная проверка
                 if sub_cols is not None:
                     if sub_cols:
                         new_root = cc.BandedCol(**params)
                         root.add(new_root)
                         populate(new_root, sub_cols)
                 else:
@@ -110,15 +119,15 @@
         # список исключений для make_read_only
         grid._mro_exclude_list = []
 
         return grid
 
     @classmethod
     def configure_grid(cls, grid, params):
-        u"""Конфигурирование грида"""
+        """Конфигурирование грида"""
 
         pack = params['pack']
         # обычное поведение
         grid.sm = ext.ExtGridCellSelModel()
         grid.row_id_name = pack.row_id_name
         grid.url_data = pack.get_rows_url()
         # кнопка "Обновить" не участвует в блокировке грида при make_read_only
@@ -128,45 +137,45 @@
 
     @classmethod
     def create_grid(cls, pack, columns, **kwargs):
         grid = cls._create_grid(pack, columns, cls.grid_class, **kwargs)
         return grid
 
     def pre_render(self):
-        assert self.grid_url, u'grid url must be defined in gridpanel!'
+        assert self.grid_url, 'grid url must be defined in gridpanel!'
         self._put_config_value('grid_url', self.grid_url)
 
     def render(self):
         self.pre_render()
         self.cmp_code = super(GridPanel, self).render()
         return render_component(self)
 
 
 class FilterPanel(ext.ExtPanel):
-    u"""
+    """
     Панель, умеющая fireevent'ить об изменении контрола,
     входящего в список filters
     """
 
     def __init__(self, *args, **kwargs):
         super(FilterPanel, self).__init__(*args, **kwargs)
         self.filters = []
 
     def configure_redirect(self, control, event):
-        u"""
+        """
         Связывает текущую панель с контролом control
         посредством fireevent'а event
         """
         self._listeners["changed"] = """
             function(params) {
                 Ext.getCmp('%s').fireEvent('%s', params)
             }""" % (control.client_id, event)
 
     def configure_events(self):
-        u"""
+        """
         Дополнение рендера fireevent'ом изменения значения контролов,
         входящих в список filters панели
         """
         for control in self.filters:
             # определяется что за контрол и приделываются разные events
             if isinstance(control, ComboBoxWithStore):
                 control.events = [
@@ -189,30 +198,30 @@
         self.cmp_code = super(FilterPanel, self).render()
         # где-то в инитах затирается темплейт, опишем еще раз
         self.template = 'filter-panel.js'
         return render_component(self)
 
 
 class BaseGridWindow(BaseWindow):
-    u"""
+    """
     Базовое окно с фильтрующей панелью и панелью с гридом
     Клиент получает панель с гридом с сервера при изменении
     полей фильтрации на фильтрующей панели
     """
     grid_panel_cls = GridPanel  # панель грида
 
     def _init_grid_panel(self):
-        u"""Панель для грида."""
+        """Панель для грида."""
         self.grid_panel = self.grid_panel_cls(
             region='center', layout='hbox', flex=1,
             layout_config={"align": "stretch"}
         )
 
     def _init_filter_panel(self):
-        u"""Панель с фильтрами."""
+        """Панель с фильтрами."""
         self.filter_cnt = FilterPanel(
             body_cls='x-window-mc',
             padding='5px 7px',
             border=False,
             body_border=False,
             region='north',
             layout='column',
@@ -235,16 +244,16 @@
         self.minimizable = True
         self.width, self.min_width = 870, 870
         self.height = 600
         self.grid_panel.layout_config['align'] = 'stretch'
 
         # добавление фильтрующих полей в фильтрующую панель
         assert self.filter_cnt.filters, (
-            u'Необходимо добавить элементы в список фильтров '
-            u'(self.filter_cnt.filters)!')
+            'Необходимо добавить элементы в список фильтров '
+            '(self.filter_cnt.filters)!')
 
         self.items.extend([
             self.filter_cnt, self.grid_panel
         ])
 
     def set_params(self, params):
 
@@ -261,37 +270,36 @@
         self.column_prefix = self.pack.column_param_name
 
         # заголовок окна
         self.title = self.pack.title
 
 
 class RelatedErrorWindow(BaseWindow):
-    u"""Окно с ошибкой.
+    """Окно с ошибкой.
 
     Показывается, если невозможно удаление записи из-за наличия ссылок
     на удаляемый объект.
     """
     def _init_components(self):
         super(RelatedErrorWindow, self)._init_components()
-        self.title = u"Внимание!"
+        self.title = "Внимание!"
         self.layout = 'fit'
         self.panel = ext.ExtPanel(
             auto_scroll=True
         )
         self.items.append(self.panel)
 
     def set_params(self, params):
         super(RelatedErrorWindow, self).set_params(params)
         assert 'html' in params
         self.panel.html = params['html']
 
 
-class _ListWindowMixin(object):
-
-    u"""Класс-примесь к окнам на базе objectpack.ui.BaseListWindow.
+class _ListWindowMixin:
+    """Класс-примесь к окнам на базе objectpack.ui.BaseListWindow.
 
     В отличии от BaseListWindow с read_only оставляет в гриде возможность
     просмотра по даблклику на строку, а также переделывает кнопку `изменить`
     в кнопку `просмотр`.
     """
 
     def __init__(self):
@@ -310,46 +318,42 @@
         super(_ListWindowMixin, self).set_params(params)
 
         if params.get('read_only'):
             reconfigure_grid_by_access(self.grid)
 
 
 class BaseListWindow(_ListWindowMixin, OPBaseListWindow):
-
-    u"""Окно с гридом с возможностью просмотра в режиме read_only.
+    """Окно с гридом с возможностью просмотра в режиме read_only.
 
     В отличии от :class:`~objectpack.ui.BaseListWindow` с ``read_only``
     оставляет в гриде возможность просмотра по даблклику на строку, а также
     меняет текст кнопки "Изменить" на "Просмотр".
     """
 
 
 class _SelectWindowMixin(_ListWindowMixin):
-
-    u"""Класс-примесь для окон выбора объектов."""
+    """Класс-примесь для окон выбора объектов."""
 
     def set_params(self, params):
         super(_SelectWindowMixin, self).set_params(params)
 
         reconfigure_grid_by_access(self.grid, can_view=False)
 
 
 class BaseSelectWindow(_SelectWindowMixin, OPBaseSelectWindow):
-
-    u"""Окно выбора из списка объектов.
+    """Окно выбора из списка объектов.
 
     В отличии от :class:`~objectpack.ui.BaseSelectWindow` оставляет в гриде
     возможность просмотра по даблклику на строку, а также меняет текст кнопки
     "Изменить"  на "Просмотр".
     """
 
 
 class BaseMultiSelectWindow(_SelectWindowMixin, OPBaseMultiSelectWindow):
-
-    u"""Окно множественного выбора из списка объектов.
+    """Окно множественного выбора из списка объектов.
 
     В отличии от :class:`~objectpack.ui.BaseMultiSelectWindow` оставляет в
     гриде возможность просмотра по даблклику на строку, а также меняет текст
     кнопки "Изменить"  на "Просмотр".
     """
 
     def set_params(self, params):
@@ -359,17 +363,16 @@
             'templates/multiselect-page-fix.js'
         )
         self.template_globals = local_template(
             'templates/multiSelectWindow.js'
         )
 
 
-class EditWindowMixin(object):
-
-    u"""Класс-примесь к окнам редактирования.
+class EditWindowMixin:
+    """Класс-примесь к окнам редактирования.
 
     Дополняет окно следующим функционалом:
 
         - скрывает кнопку "Сохранить" в режиме только для чтения;
         - кнопку "Отмена" переименовывает в "Закрыть".
     """
 
@@ -378,31 +381,28 @@
 
         if params.get('read_only'):
             # TODO: Выпилить эту функцию, а ее код перенести сюда
             switch_window_in_read_only_mode(self)
 
 
 class BaseEditWindow(EditWindowMixin, OPBaseEditWindow):
-
-    u"""Базовый класс окон просмотра/редактирования.
+    """Базовый класс окон просмотра/редактирования.
 
     Отличия от :class:``objectpack.ui.BaseEditWindow`` описаны в
     :class:`educommon.objectpack.ui.EditWindowMixin`.
     """
 
 
 class ModelEditWindow(EditWindowMixin, OPModelEditWindow):
-
-    u"""Базовый класс для окон просмотра/редактирования объекта модели.
+    """Базовый класс для окон просмотра/редактирования объекта модели.
 
     Отличия от :class:``objectpack.ui.ModelEditWindow`` описаны в
     :class:`educommon.objectpack.ui.EditWindowMixin`.
     """
 
 
 class TabbedEditWindow(EditWindowMixin, OPTabbedEditWindow):
-
-    u"""Базовый класс для окон просмотра/редактирования с вкладками.
+    """Базовый класс для окон просмотра/редактирования с вкладками.
 
     Отличия от :class:``objectpack.ui.TabbedEditWindow`` описаны в
     :class:`educommon.objectpack.ui.EditWindowMixin`.
     """
```

### Comparing `educommon-2.20.0/src/educommon/report/__init__.py` & `educommon-3.0.0/src/educommon/report/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# coding: utf-8
-u"""Шаблон для построения отчётной системы.
+"""Шаблон для построения отчётной системы.
 
 Представляет собой набор абстрактных базовых и вспомогательных классов для
 различных элементов отчётной подсистемы: провайдера данных, построителя отчёта
 и собственно отчёта.
 """
-from __future__ import absolute_import
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
+from collections import (
+    Mapping,
+)
 
-from abc import ABCMeta
-from abc import abstractmethod
-from collections import Mapping
 
-import six
-
-
-class AbstractDataProvider(six.with_metaclass(ABCMeta, object)):
-
-    u"""Абстрактный класс провайдера данных.
+class AbstractDataProvider(metaclass=ABCMeta):
+    """Абстрактный класс провайдера данных.
 
     Данный класс является базовым для всех классов, реализующих функционал
     провайдера данных. Идеология провайдера данных следующая:
         - провайдер обеспечивает доступ к данным через свойства
           (которые могут быть кешированы через декоратор @cached_property),
         - все кастомные артибуты класса, которые могут быть вызваны извне,
           при обращению к экземпляру провайдера для извлечения данных - не
@@ -36,45 +34,44 @@
           кроме как последовательным вызовом методов init() и load_data().
     """
 
     # Имя провайдера, используемое в композитном провайдере
     provider_name = None
 
     def init(self, **params):
-        u"""Инициализация провайдера.
+        """Инициализация провайдера.
 
         Используется вместо конструктора.
         """
 
     def load_data(self):
-        u"""Загрузка данных.
+        """Загрузка данных.
 
         Данный метод может быть описан и использоваться для подготовки
         данных или реализации каких-либо необходимых общих расчётов.
         Метод не должен иметь никаких входных параметров.
         """
 
     @property
     def name(self):
-        u"""Имя провайдера для применения в композитном провайдере."""
+        """Имя провайдера для применения в композитном провайдере."""
         if self.provider_name is not None:
             return self.provider_name
         else:
             return self.__class__.__name__
 
 
 class CompositeDataProvider(AbstractDataProvider):
-
-    u"""Композитный провайдер данных.
+    """Композитный провайдер данных.
 
     Используется для объединения нескольких провайдеров в один.
     """
 
     def __init__(self, provider_classes):
-        u"""Конструктор композитного провайдера.
+        """Конструктор композитного провайдера.
 
         Здесь инстанцируются все подпровайдеры.
 
         :param provider_classes: список классов провайдеров
         """
         # словарь экземпляров провайдеров
         self.providers = {}
@@ -85,50 +82,49 @@
                 self.providers[provider_class.name] = provider_class
             else:
                 # пришёл просто класс провайдера
                 _provider = provider_class()
                 self.providers[_provider.name] = _provider
 
     def init(self, **params):
-        u"""Здесь инициализируются все подпровайдеры."""
-        for provider in six.itervalues(self.providers):
+        """Здесь инициализируются все подпровайдеры."""
+        for provider in self.providers.values():
             if hasattr(provider, 'init'):
                 provider.init(**params)
 
     def load_data(self):
-        u"""Загрузка данных во всех подпровайдерах."""
-        for provider in six.itervalues(self.providers):
+        """Загрузка данных во всех подпровайдерах."""
+        for provider in self.providers.values():
             if hasattr(provider, 'load_data'):
                 provider.load_data()
 
 
 class DependentCompositeProvider(AbstractDataProvider):
-
-    u"""
+    """
     Композитный провайдер с описанием подпровайдеров, порядка их загрузки.
 
     'Прокидывает' данные между подпровайдерами в процессе загрузки данных
     """
 
     providers_order = None
-    u"""
+    """
     Описание провайдеров в порядке их загрузки.
     Следует использовать "_" перед коротким именем провайдера,
     чтобы эти аттрибуты не уходили в адаптер
 
     ..code::
 
         providers_order = (
             ('_provider_name', ProviderClass),
             ('_provider_name2', ProviderClass2),
             ('_provider_name3', ProviderClass3),
         )
     """
     _dependence_map = None
-    u"""
+    """
     Описание карты дополнительных данных (между подпровайдерами).
     См. метод _extend_provider_data
 
     ..code::
 
         _dependence_map = {
             '_provider_name': {
@@ -153,136 +149,133 @@
         for shortname, provider_class in self.providers_order:
             provider = provider_class()
             self._set_provider_to_loader(provider, shortname)
             # для поддержки работы с адаптерами
             self.providers[provider.name] = provider
 
     def _set_provider_to_loader(self, provider, shortname):
-        u"""
+        """
         Установка зависимого подпровайдера в список для загрузки.
 
         :param provider: провайдер данных, наследник AbstractDataProvider
         :param str shortname: ключ из словаря self._dependence
         """
         provider._shortname = shortname
         self._providers.append(provider)
         setattr(self, shortname, provider)
 
     def init(self, **params):
-        u"""Инициализация подпровайдеров."""
+        """Инициализация подпровайдеров."""
         for provider in self._providers:
             if hasattr(provider, 'init'):
                 provider.init(**params)
 
     def load_data(self):
-        u"""Загрузка данных во всех подпровайдерах."""
+        """Загрузка данных во всех подпровайдерах."""
         for provider in self._providers:
             if hasattr(provider, 'load_data'):
                 self._extend_provider_data(provider)
                 provider.load_data()
 
     def _extend_provider_data(self, provider):
-        u"""
+        """
         Дополнение данных провайдера данными предыдущих загруженных провайдеров
         согласно карте зависимостей self._dependence_map
 
         :type provider: AbstractDataProvider
         :param provider: провайдер данных, наследник AbstractDataProvider
         """
         # дополнение параметров результатами предыдущих провайдеров
         additional = self._dependence_map.get(provider._shortname, {})
-        for param, (dependent_provider_name, att) in six.iteritems(additional):
+        for param, (dependent_provider_name, att) in additional.items():
             dependent_provider = getattr(self, dependent_provider_name)
             setattr(provider, param, getattr(dependent_provider, att))
 
 
-class AbstractReportBuilder(six.with_metaclass(ABCMeta, object)):
-
-    u"""Абстрактный класс построителя отчётов.
+class AbstractReportBuilder(metaclass=ABCMeta):
+    """Абстрактный класс построителя отчётов.
 
     Имеет обязательный атрибут build(), вызов которого производит
     непосредственную генерацию отчёта.
     Принимает данные от провайдера "как есть", через его свойства или целиком
     через специальный адаптер.
     """
 
     def __init__(self, provider=None, adapter=None, *args, **kwargs):
-        u"""Конструктор класса билдера.
+        """Конструктор класса билдера.
 
         :param provider: Провайдер данных.
         :param adapter: Адаптер для извлечения данных из провайдера.
         """
 
     @abstractmethod
     def build(self):
-        u""" Метод, осуществляющий построение отчёта.
+        """ Метод, осуществляющий построение отчёта.
 
         Должен возвращать результат в виде файла или иной структуры данных.
         """
 
 
 class BaseProviderAdapter(Mapping, dict):
-
-    u"""Базовый класс для адаптеров, извлекающих данные из провайдера."""
+    """Базовый класс для адаптеров, извлекающих данные из провайдера."""
 
     # список атрибутов провайдера, которые не должны быть "видны" через адаптер
     _attrs_stop_list = (
         'init',
         'load_data',
         'name',
         'provider_name',
         'providers',
     )
 
     def __init__(self, provider):
-        u"""Конструктор адаптера.
+        """Конструктор адаптера.
 
         :param provider: провайдер данных
         """
         assert isinstance(provider, AbstractDataProvider), type(provider)
         self.provider = provider
         self._cache = {}
 
     def _check_provider_attr(self, attr):
-        u"""Проверка атрибута - можно ли его брать из провайдера.
+        """Проверка атрибута - можно ли его брать из провайдера.
 
         'Магические' и некоторые отдельные методы будут игнорироваться.
         """
         return not(attr.startswith('_') or attr in self._attrs_stop_list)
 
 
 class FlatDataProviderAdapter(BaseProviderAdapter):
-
-    u"""Данные провайдера в 'плоском' виде.
+    """Данные провайдера в 'плоском' виде.
 
     Класс адаптера, получающего все данные из провайдера и представляющего их
     в "плоском" виде (словарь с единичной глубиной):
         {
             'MainDataProvider__Provider01__param01': 16,
             'MainDataProvider__Provider01__param02': 54,
             'MainDataProvider__Provider01__param03': 80
         }
     Обращение к такому адаптеру - как и к обычному словарю, через "[]",
     """
 
     def __init__(self, provider, splitter):
-        u"""Конструктор адаптера.
+        """Конструктор адаптера.
 
         :param provider: провайдер данных
         :param splitter: строка-разделитель.
         """
-        assert isinstance(splitter, six.string_types), type(splitter)
+        assert isinstance(splitter, str), type(splitter)
 
         super(FlatDataProviderAdapter, self).__init__(provider)
 
         self.level_splitter = splitter
         self._all_keys = self._get_all_keys(self.provider)
 
     def _get_all_keys(self, provider, key_level=None):
-        u"""все ключи в иерархии провайдеров."""
+        """Все ключи в иерархии провайдеров."""
         result = []
         if key_level is None:
             key_level = ""
         else:
             if key_level:
                 key_level += self.level_splitter + provider.name
             else:
@@ -304,16 +297,16 @@
             # если есть вложенные провайдеры
             for p in provider.providers.values():
                 result.extend(self._get_all_keys(p, key_level))
 
         return result
 
     def __getitem__(self, item):
-        u"""Поиск элемента с ключом item в словаре данных адаптера."""
-        if not isinstance(item, six.string_types):
+        """Поиск элемента с ключом item в словаре данных адаптера."""
+        if not isinstance(item, str):
             raise KeyError(item)
         if item not in self._all_keys:
             raise KeyError(item)
         key_parts = item.split(self.level_splitter)
         # указатель на объект, где будет искаться атрибут
         obj = self.provider
         for part in key_parts[:-1]:
@@ -331,28 +324,27 @@
         else:
             # атрибут
             value = attr
 
         return value
 
     def __len__(self):
-        u"""Магический метод для поддержки операции len()."""
+        """Магический метод для поддержки операции len()."""
         return len(self._all_keys)
 
     def __bool__(self):
         return bool(self._all_keys)
     __nonzero__ = __bool__
 
     def __iter__(self):
         return iter(self._all_keys)
 
 
 class NestedDataProviderAdapter(BaseProviderAdapter):
-
-    u"""Данные провайдера в 'иерархическом' (вложенные словари) виде.
+    """Данные провайдера в 'иерархическом' (вложенные словари) виде.
 
     Класс адаптера, получающего все данные провайдера и представляющего их
     в виде вложенных словарей:
         {
             'MainDataProvider': {
                 'Provider01': {
                     'param01': 16,
@@ -361,23 +353,23 @@
                 }
             }
         }
     Обращение к такому адаптеру - как и к обычному словарю, через "[]".
     """
 
     def __init__(self, provider):
-        u"""Конструктор адаптера.
+        """Конструктор адаптера.
 
         :param provider: провайдер данных
         """
         super(NestedDataProviderAdapter, self).__init__(provider)
         self._all_keys = self._get_top_keys(self.provider)
 
     def _get_top_keys(self, provider):
-        u"""все необходимые атрибуты адаптируемого провайдера."""
+        """все необходимые атрибуты адаптируемого провайдера."""
         result = []
         for attr_name in dir(provider):
             # цикл по всем атрибутам провайдера
             if not self._check_provider_attr(attr_name):
                 continue
             result.append(attr_name)
 
@@ -385,16 +377,16 @@
             # если есть вложенные провайдеры
             for p in provider.providers.values():
                 result.append(p.name)
 
         return result
 
     def __getitem__(self, item):
-        u"""Поиск элемента с ключом item в словаре данных адаптера."""
-        if not isinstance(item, six.string_types):
+        """Поиск элемента с ключом item в словаре данных адаптера."""
+        if not isinstance(item, str):
             raise KeyError(item)
         if not self._check_provider_attr(item):
             raise KeyError(item)
         if hasattr(self.provider, item):
             attr = getattr(self.provider, item)
             if callable(attr):
                 value = attr()
@@ -409,15 +401,15 @@
             if provider_key not in self._cache:
                 self._cache[provider_key] = NestedDataProviderAdapter(provider)
             return self._cache[provider_key]
         else:
             raise KeyError(item)
 
     def __len__(self):
-        u"""Магический метод для поддержки операции len()."""
+        """Магический метод для поддержки операции len()."""
         return len(self._all_keys)
 
     def __bool__(self):
         return bool(self._all_keys)
     __nonzero__ = __bool__
 
     def __iter__(self):
```

### Comparing `educommon-2.20.0/src/educommon/report/actions.py` & `educommon-3.0.0/src/educommon/report/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-# coding: utf-8
-u"""Генерация отчётов средствами платформы M3."""
-from __future__ import absolute_import
-
-from m3 import ApplicationLogicException
-from m3.actions import OperationResult
-from objectpack.actions import BaseAction
-from objectpack.actions import BasePack
-from objectpack.actions import BaseWindowAction
-from objectpack.ui import BaseEditWindow
-import six
+"""Генерация отчётов средствами платформы M3."""
+from m3 import (
+    ApplicationLogicException,
+)
+from m3.actions import (
+    OperationResult,
+)
+
+from objectpack.actions import (
+    BaseAction,
+    BasePack,
+    BaseWindowAction,
+)
+from objectpack.ui import (
+    BaseEditWindow,
+)
 
 
 class BaseReportPack(BasePack):
 
-    u"""Базовый класс отчёта.
+    """Базовый класс отчёта.
 
     Отчёты на любых движках могут быть описаны на основе этого класса.
     """
 
-    title = u'Отчёт'
+    title = 'Отчёт'
 
     # дефолтное окно отчёта
     report_window = BaseEditWindow
 
     # признак асинхронного выполнения
     is_async = False
 
@@ -35,45 +40,45 @@
     # экземпляр класса провайдера
     data_provider = None
 
     # экземпляр класса построителя отчёта
     report_builder = None
 
     def create_provider(self, context):
-        u"""Кастомный метод для создания экземпляра класса провайдера.
+        """Кастомный метод для создания экземпляра класса провайдера.
 
         Используется в случае необходимости явного вызова конструктора
         провайдера, например для композитного провайдера.
 
         Внимание! Экземпляр созданного провайдера должен быть присвоен
         атрибуту data_provider
         """
 
     def init_provider(self, context):
-        u"""Кастомный метод для инициации провайдера.
+        """Кастомный метод для инициации провайдера.
 
         Данный метод должен извлечь параметры из контекста, а затем
         вызывать метод провайдера init().
         """
 
     def create_builder(self, context, *args, **kwargs):
-        u"""Специальный метод для создания билдера.
+        """Специальный метод для создания билдера.
 
         Извлекает параметры создания билдера из контекста или из *args/**kwargs
         затем инстанцирует билдер, присваивая его атрибуту self.report_builder
         """
 
 
 def download_result(url):
-    u"""функция для скачивания файла отчёта."""
-    if not isinstance(url, six.text_type):
-        url = six.text_type(url, 'utf-8')
+    """Функция для скачивания файла отчёта."""
+    if not isinstance(url, str):
+        url = str(url, 'utf-8')
     return OperationResult(
         success=True,
-        code=u"""
+        code="""
             (function(){
                 var hiddenIFrameID = 'hiddenDownloader',
                     iframe = document.getElementById(hiddenIFrameID);
                 if (iframe === null) {
                     iframe = document.createElement('iframe');
                     iframe.id = hiddenIFrameID;
                     iframe.style.display = 'none';
@@ -82,67 +87,64 @@
                 iframe.src = "%s";
             })()
         """ % url
     )
 
 
 class CommonReportWindowAction(BaseWindowAction):
-
-    u"""Экшн показа окна параметров отчёта (перед выполнением отчёта)."""
+    """Экшн показа окна параметров отчёта (перед выполнением отчёта)."""
 
     perm_code = 'report'
 
     def create_window(self):
-        u"""создание окна параметров отчёта."""
+        """Создание окна параметров отчёта."""
         self.win = self.parent.create_report_window(self.request, self.context)
 
     def configure_window(self):
-        u"""конфигурирование окна параметров отчёта."""
-        self.win.save_btn.text = u'Сформировать'
+        """Конфигурирование окна параметров отчёта."""
+        self.win.save_btn.text = 'Сформировать'
 
     def set_window_params(self):
-        u"""Задание параметров окна."""
+        """Задание параметров окна."""
         super(CommonReportWindowAction, self).set_window_params()
         params = self.win_params.copy()
         params['title'] = self.parent.title
         params['form_url'] = self.parent.get_reporting_url()
         self.win_params = self.parent.set_report_window_params(
             params, self.request, self.context)
 
 
 class CommonReportAction(BaseAction):
-
-    u"""Экшн, выполняющий отчёт."""
+    """Экшн, выполняющий отчёт."""
 
     perm_code = 'report'
 
     def run(self, request, context):
-        u"""Выполнение запроса."""
+        """Выполнение запроса."""
         pack = self.parent
         # проверка параметров отчёта
         pack.check_report_params(request, context)
         provider_params = pack.get_provider_params(request, context)
         builder_params = pack.get_builder_params(request, context)
 
         if 'title' not in builder_params and hasattr(pack, 'title'):
             builder_params.update(title=pack.title)
         # генерация отчёта
         out_file_url = pack.make_report(provider_params, builder_params)
         return download_result(out_file_url.encode('utf-8'))
 
 
 class CommonReportPack(BasePack):
-
-    u"""
+    """
     Пак, реализующий генерацию отчётов.
 
     Использует класс-построитель reporter.
     """
 
-    title = u'Отчёт'
+    title = 'Отчёт'
 
     # дефолтное окно отчёта
     report_window = BaseEditWindow
 
     # признак асинхронного выполнения
     is_async = False
 
@@ -152,95 +154,95 @@
 
     ..code:
 
         reporter = MySimpleReporter
     """
 
     def __init__(self):
-        u"""Конструктор пака генерации отчётов."""
+        """Конструктор пака генерации отчётов."""
         super(CommonReportPack, self).__init__()
 
         self.report_window_action = CommonReportWindowAction()
         self.report_action = CommonReportAction()
         self.actions.extend([
             self.report_window_action,
             self.report_action,
         ])
 
     def get_reporting_url(self):
-        u"""Отдаёт адрес форме, куда передавать данные для обработки."""
+        """Отдаёт адрес форме, куда передавать данные для обработки."""
         return self.report_action.get_absolute_url()
 
     @staticmethod
     def context2dict(context):
-        u"""преобразование контекста в словарь."""
+        """преобразование контекста в словарь."""
         result = {}
-        for key, value in six.iteritems(context.__dict__):
+        for key, value in context.__dict__.items():
             try:
                 if callable(value):
                     value = value()
                 result[key] = value
             except TypeError:
                 continue
 
         return result
 
     def check_report_params(self, request, context):
-        u"""
+        """
         Проверка передаваемых параметров для формирования отчёта.
 
         :raise: ApplicationLogicException
         """
         pass
 
     def get_provider_params(self, request, context):
-        u"""
+        """
         Преобразование request, context к словарю для создания провайдера.
 
         :param request:
         :param context:
         """
         return {}
 
     def get_builder_params(self, request, context):
-        u"""
+        """
         Преобразование request, context к словарю для создания билдера.
 
         :param request:
         :param context:
         """
         return {}
 
     def init_reporter(self, provider_params, builder_params):
-        u"""
+        """
         Инициализация построителя с передачей параметров билдеру и провайдеру.
 
         Не требует переопределения.
         """
         return self.reporter_class(provider_params, builder_params)
 
     def make_report(self, provider_params, builder_params):
-        u"""Синхронное построение отчёта. Не требует переопределения."""
+        """Синхронное построение отчёта. Не требует переопределения."""
         reporter = self.init_reporter(provider_params, builder_params)
         url = reporter.make_report()
         return url
 
     def set_report_window_params(self, params, request, context):
-        u"""Дополнение параметров окна отчёта."""
+        """Дополнение параметров окна отчёта."""
         if self.reporter_class.extension not in (
             self.reporter_class._available_extensions
         ):
-            raise ApplicationLogicException(u'Расширение указано неверно!')
+            raise ApplicationLogicException('Расширение указано неверно!')
         params['extension'] = self.reporter_class.extension
         return params
 
     def create_report_window(self, request, context):
-        u"""
+        """
         Cоздание окна настройки параметров отчёта.
 
         Не требует переопределения.
         """
         return self.report_window()
 
     def extend_menu(self, menu):
-        u"""Размещение в меню."""
+        """Размещение в меню."""
         pass
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/README.rst` & `educommon-3.0.0/src/educommon/report/constructor/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/report/constructor/__init__.py` & `educommon-3.0.0/src/educommon/report/constructor/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# coding: utf-8
-u"""Конструктор отчетов.
+"""Конструктор отчетов.
 
 Поддерживает конструирование пользователем простых отчетов в формате Excel.
 """
-from __future__ import absolute_import
-
-from pkg_resources import get_distribution
 import django
+from pkg_resources import (
+    get_distribution,
+)
 
 
 # -----------------------------------------------------------------------------
 
 
 default_app_config = __name__ + '.apps.AppConfig'
 # -----------------------------------------------------------------------------
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/base.py` & `educommon-3.0.0/src/educommon/report/constructor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,46 @@
-# coding: utf-8
 # pylint: disable=protected-access
-from __future__ import absolute_import
-
-from django.core.exceptions import FieldDoesNotExist
-from django.core.exceptions import ValidationError
-from django.db import models
-from django.db.models.fields import Field
-from django.db.models.fields.related import RelatedField
-from django.db.models.fields.reverse_related import ForeignObjectRel
-from django.db.models.fields.reverse_related import OneToOneRel
-from django.utils.encoding import force_text
-from m3_django_compat import ModelOptions
-from m3_django_compat import get_related
-
-from educommon.django.db.utils import LazyModel
-from educommon.report.constructor.utils import get_data_type
-from educommon.utils.misc import cached_property
-
-from . import constants
-from .utils import get_field
+from django.core.exceptions import (
+    FieldDoesNotExist,
+    ValidationError,
+)
+from django.db import (
+    models,
+)
+from django.db.models.fields import (
+    Field,
+)
+from django.db.models.fields.related import (
+    RelatedField,
+)
+from django.db.models.fields.reverse_related import (
+    ForeignObjectRel,
+    OneToOneRel,
+)
+from django.utils.encoding import (
+    force_text,
+)
+from m3_django_compat import (
+    ModelOptions,
+    get_related,
+)
+
+from educommon.django.db.utils import (
+    LazyModel,
+)
+from educommon.report.constructor import (
+    constants,
+)
+from educommon.report.constructor.utils import (
+    get_data_type,
+    get_field,
+)
+from educommon.utils.misc import (
+    cached_property,
+)
 
 
 def _get_accessor_name(field):
     """Возвращает название поля модели.
 
     :rtype: str
     """
@@ -55,15 +73,15 @@
         return False
 
     params = model.report_constructor_params
     assert isinstance(params, dict), params
     assert sum(
         1 if param in params else 0
         for param in ('skip', 'except', 'only')
-    ) <= 1, (u'Должен быть указан только один параметр.', model, params)
+    ) <= 1, ('Должен быть указан только один параметр.', model, params)
 
     if 'extra' in params and accessor_name in params['extra']:
         return False
 
     if 'skip' in params and params['skip']:
         return True
 
@@ -82,15 +100,15 @@
                 return False
         return True
 
     return False
 
 
 def skip_field(model, field, accessor_name):
-    u"""Возвращает True, если поле модели должно игнорироваться конструктором.
+    """Возвращает True, если поле модели должно игнорироваться конструктором.
 
     Игнорируются:
         - поля с типами ``AutoField`` и ``FileField``;
         - поля, исключенные параметром ``model.report_constructor_params``;
 
     :param model: Модель в рамках которой происходит проверка.
     :type model: django.db.models.Model
@@ -103,23 +121,22 @@
     """
     if isinstance(field, (models.AutoField, models.FileField)):
         return True
 
     return field_ignored_by_model_params(model, accessor_name)
 
 
-class ColumnDescriptor(object):
-
-    u"""Дескриптор поля модели, входящего в состав столбца отчета.
+class ColumnDescriptor:
+    """Дескриптор поля модели, входящего в состав столбца отчета.
 
     Предназначен для извлечения из моделей необходимой информации.
     """
 
     def __init__(self, data_source, parent, field, level=0):
-        u"""Инициализация экземпляра класса.
+        """Инициализация экземпляра класса.
 
         :param data_source: Источник данных.
 
         :param parent: Дескриптор верхнего уровня. Определяет дескриптор для
             поля, из которого модель ссылается на поле данного дейскриптора.
         :type parent: ColumnDescriptor or None
 
@@ -147,15 +164,15 @@
     @staticmethod
     def create(model, field_name, data_source, parent=None, level=0):
         model_params = getattr(model, 'report_constructor_params', {})
         assert sum(
             1 if param in model_params else 0
             for param in ('skip', 'except', 'only')
         ) <= 1, (
-            u'Может быть указан только один параметр.', model, model_params
+            'Может быть указан только один параметр.', model, model_params
         )
 
         attr_name, _, nested_attr = field_name.partition('.')
 
         for field in getattr(model, '_meta').get_fields():
             accessor_name = _get_accessor_name(field)
 
@@ -255,28 +272,28 @@
                 (self.parent.full_lookup, self.lookup)
             )
         else:
             return self.lookup
 
     @property
     def data_type(self):
-        u"""Тип данных в столбце.
+        """Тип данных в столбце.
 
         :rtype: str
         """
         if not isinstance(self.field, (Field, ForeignObjectRel, RelatedField)):
             result = self.field.data_type
         else:
             result = get_data_type(self.field)
 
         return result
 
     @property
     def choices(self):
-        u"""Допустимые значения столбца с описанием."""
+        """Допустимые значения столбца с описанием."""
         return self.field.choices or None
 
     @property
     def title(self):
         if (
             self.data_source.field_titles and
             self.full_accessor_name in self.data_source.field_titles
@@ -290,20 +307,20 @@
             else:
                 result = options.verbose_name_plural
         else:
             result = self.field.verbose_name
 
         return force_text(result)
 
-    def get_full_title(self, delimiter=u' → '):
-        u"""Возвращает полное наименование с учетом иерархии.
+    def get_full_title(self, delimiter=' → '):
+        """Возвращает полное наименование с учетом иерархии.
 
-        :param unicode delimiter: Разделитель наименований.
+        :param str delimiter: Разделитель наименований.
 
-        :rtype: unicode
+        :rtype: str
         """
         if self.parent:
             return delimiter.join((
                 self.parent.get_full_title(delimiter), self.title
             ))
         else:
             return self.title
@@ -361,66 +378,64 @@
                         yield ColumnDescriptor(
                             self.data_source,
                             self, field,
                             level=self.level + 1
                         )
 
     def validate_value(self, value):
-        u"""Проверяет текстовое представление значения на соотв-е типу поля.
+        """Проверяет текстовое представление значения на соотв-е типу поля.
 
         :param unicode value: Текстовое представление значения для проверки.
 
         :raises django.core.exceptions.ValidationError: если значение аргумента
             value не прошло проверку. Описание ошибки будет в исключении.
         """
         if self.data_type == constants.CT_REVERSE_RELATION:
-            raise ValidationError(u'Обратная связь не доступна для сравнения.')
+            raise ValidationError('Обратная связь не доступна для сравнения.')
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
         elif self.data_type == constants.CT_DIRECT_RELATION:
-            raise ValidationError(u'Ключевые поля не доступны для сравнения.')
+            raise ValidationError('Ключевые поля не доступны для сравнения.')
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
         elif self.data_type == constants.CT_CHOICES:
             lower_case_value = value.lower()
             for _, choice_display in self.field.choices:
                 if choice_display.lower() == lower_case_value:
                     break
             else:
                 raise ValidationError(
-                    u'Недопустимое значение для сравнения: {}.'
+                    'Недопустимое значение для сравнения: {}.'
                     .format(value)
                 )
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
         else:
             form_field = self.field.formfield()
             if form_field:
                 form_field.validate(value)
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
 
-class FakeField(object):
-
-    u"""Класс несуществующего поля модели для отчета.
+class FakeField:
+    """Класс несуществующего поля модели для отчета.
 
     Предназначен для подмены реальных полей при отображении в отчете.
     """
 
     def __init__(self, name):
         self.id = None
         self.name = name
         self.verbose_name = name
         self.concrete = False
         self.data_type = constants.CT_OTHER
 
 
-class ExtraField(object):
-
-    u"""Класс дополнительного поля модели.
+class ExtraField:
+    """Класс дополнительного поля модели.
 
     Используется для доступа к атрибутам объектов моделей, а также результатам
     вызова функций с объектом модели в качестве аргумента.
     """
 
     def __init__(self, name, field):
         """Инициализация экземпляра.
@@ -460,20 +475,19 @@
         return self._field.model
 
     @property
     def formfield(self):
         return self._field.formfield
 
 
-class _ModelDataSourceInfo(object):
-
-    u"""Клас-примесь для работы с информацией об источнике данных."""
+class _ModelDataSourceInfo:
+    """Клас-примесь для работы с информацией об источнике данных."""
 
     def __init__(self, model, filter_func=None, field_titles=None):
-        u"""Инициализация экземпляра.
+        """Инициализация экземпляра.
 
         :param model: Модель, для источника данных которой определяются
             параметры. См. :class:`educommon.django.db.utils.LazyModel`
 
         :param filter_func: Фильтрующая функция. Накладывает дополнительные
             ограничения для данных в источнике.
 
@@ -483,67 +497,65 @@
             модели.
 
             .. code:: python
 
                _ModelDataSourceInfo(
                    ...,
                    field_titles={
-                       'restored_to': u'Сведения до восстановления',
-                       'person.surname': u'Фамилия физ. лица',
+                       'restored_to': 'Сведения до восстановления',
+                       'person.surname': 'Фамилия физ. лица',
                    }
                )
         """
         self._model = LazyModel(model)
         self._filter_func = filter_func
         self.field_titles = field_titles
 
     @cached_property
     def model(self):
         return self._model.get_model()
 
     @cached_property
     def name(self):
-        u"""Внутрисистемное имя источника данных."""
+        """Внутрисистемное имя источника данных."""
         result = '.'.join((self._model.app_label, self._model.model_name))
 
         return force_text(result)
 
     @cached_property
     def title(self):
-        u"""Отображаемое пользователю наименование источника данных."""
+        """Отображаемое пользователю наименование источника данных."""
         result = getattr(self.model, '_meta').verbose_name
         return force_text(result)
 
 
 class ModelDataSourceParams(_ModelDataSourceInfo):
-
-    u"""Параметры для дескриптора источника данных в шаблоне отчета."""
+    """Параметры для дескриптора источника данных в шаблоне отчета."""
 
     def get_data_source_descriptor(self):
-        u"""Возвращает дескриптор источника данных."""
+        """Возвращает дескриптор источника данных."""
         return ModelDataSourceDescriptor(
             self._model.get_model(), self._filter_func, self.field_titles
         )
 
 
 class ModelDataSourceDescriptor(_ModelDataSourceInfo):
-
-    u"""Дескриптор модели, являющейся источником данных в шаблоне отчета."""
+    """Дескриптор модели, являющейся источником данных в шаблоне отчета."""
 
     def __init__(self, *args, **kwargs):
         super(ModelDataSourceDescriptor, self).__init__(*args, **kwargs)
 
         self.column_descriptors_cache = {}
 
     @cached_property
     def _options(self):
         return ModelOptions(self._model.get_model())
 
     def add_source_filter(self, query, include_available_units, user):
-        u"""Добавление фильтра к источнику данных."""
+        """Добавление фильтра к источнику данных."""
         if self._filter_func:
             return self._filter_func(query, include_available_units, user)
         return query
 
     def get_available_columns(self):
         model = self._model.get_model()
 
@@ -558,15 +570,15 @@
             extra = model.report_constructor_params['extra']
             for accessor_name, params in extra.items():
                 field = ExtraField(accessor_name, params['field'])
                 yield ColumnDescriptor(self, None, field)
 
     @staticmethod
     def _get_model_field_by_name(model, field_name):
-        u"""Получает поле модели и модель связанную с ним по его имени.
+        """Получает поле модели и модель связанную с ним по его имени.
 
         Рейзит FieldDoesNotExist если поле с таким именем не найдено.
         """
         for field in getattr(model, '_meta').get_fields():
             if skip_field(model, field, field_name):
                 continue
 
@@ -596,15 +608,15 @@
                 raise FieldDoesNotExist(
                     '{}.{}'.format(model.__name__, field_name)
                 )
 
         return column_field, model
 
     def is_column_ignored(self, accessor_name):
-        u"""Проверяет исключение модели ``model.report_constructor_params``.
+        """Проверяет исключение модели ``model.report_constructor_params``.
 
         :param str accessor_name: путь, через ".", до поля от указанной модели.
 
         :rtype: bool
         """
         level_names = []
         model = self.model
@@ -614,15 +626,15 @@
 
             if field_ignored_by_model_params(model, full_accessor_name):
                 return True
 
         return False
 
     def is_column_exist(self, accessor_name):
-        u"""Проверяет существование поля в моделе.
+        """Проверяет существование поля в моделе.
 
         :param str accessor_name: путь, через ".", до поля от указанной модели.
 
         :rtype: bool
         """
         model = self.model
         for name in accessor_name.split('.'):
@@ -630,15 +642,15 @@
                 _, model = self._get_model_field_by_name(model, name)
             except FieldDoesNotExist:
                 return False
 
         return True
 
     def get_column_descriptor(self, accessor_name):
-        u"""Возвращает дескриптор столбца по его имени.
+        """Возвращает дескриптор столбца по его имени.
 
         .. code-block:: python
 
            data_source.get_column_descriptor('person.surname')
 
         :rtype: ColumnDescriptor
         """
@@ -668,15 +680,15 @@
                 )
                 self.column_descriptors_cache[full_accessor_name] = result
             # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
         return result
 
     def get_fake_column_descriptor(self, column_name):
-        u"""Возвращает дескриптор отсутствующего столбца по его имени.
+        """Возвращает дескриптор отсутствующего столбца по его имени.
 
         .. code-block:: python
 
            data_source.get_fake_column_descriptor('person.surname')
 
         :rtype: FakeColumnDescriptor
         """
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/builders/excel/_base.py` & `educommon-3.0.0/src/educommon/report/constructor/builders/excel/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,95 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from collections import defaultdict
-from functools import partial
-from functools import reduce
-from functools import total_ordering
-from operator import gt
 import abc
 import itertools
 import operator
-
-from django.db import models
-from django.db.models import Q
-from django.db.models.fields.related import RelatedField
-from django.db.models.fields.reverse_related import ForeignObjectRel
-from django.db.models.manager import Manager
-from django.forms.fields import BooleanField
-from django.utils.encoding import force_text
-from m3.actions.exceptions import ApplicationLogicException
-from six.moves import map
-from six.moves import range
-from xlsxwriter import Workbook
-import six
-
-from educommon.report.constructor.builders.excel.constants import COUNT
-from educommon.report.constructor.builders.excel.constants import SUM
-from educommon.report.constructor.constants import FALSE
-from educommon.report.constructor.constants import TRUE
-from educommon.report.constructor.utils import get_field
-from educommon.report.constructor.utils import get_field_value_by_display
-from educommon.utils.misc import cached_property
-
-from ... import constants
-from ...base import ColumnDescriptor
-from ...constants import BY_VALUE_COUNT
-from ...constants import BY_VALUE_SUM
-from ...constants import DIRECTION_ASC
-from ...constants import TOTAL_COUNT
-from ...constants import TOTAL_SUM
-from ...constants import TOTAL_UNIQUE_COUNT
-from ...exceptions import DataSourceParamsNotFound
-from ...exceptions import FilterError
-from ...exceptions import ReportConstructorException
-from ...models import ReportFilter
-from ...models import ReportFilterGroup
-from ...models import ReportTemplate
-from ...registries import registry
-from ...utils import get_columns_hierarchy
+from collections import (
+    defaultdict,
+)
+from functools import (
+    partial,
+    reduce,
+    total_ordering,
+)
+from operator import (
+    gt,
+)
+
+from django.db import (
+    models,
+)
+from django.db.models import (
+    Q,
+)
+from django.db.models.fields.related import (
+    RelatedField,
+)
+from django.db.models.fields.reverse_related import (
+    ForeignObjectRel,
+)
+from django.db.models.manager import (
+    Manager,
+)
+from django.forms.fields import (
+    BooleanField,
+)
+from django.utils.encoding import (
+    force_text,
+)
+from m3.actions.exceptions import (
+    ApplicationLogicException,
+)
+from xlsxwriter import (
+    Workbook,
+)
+
+from educommon.report.constructor import (
+    constants,
+)
+from educommon.report.constructor.base import (
+    ColumnDescriptor,
+)
+from educommon.report.constructor.builders.excel.constants import (
+    COUNT,
+    SUM,
+)
+from educommon.report.constructor.constants import (
+    BY_VALUE_COUNT,
+    BY_VALUE_SUM,
+    DIRECTION_ASC,
+    FALSE,
+    TOTAL_COUNT,
+    TOTAL_SUM,
+    TOTAL_UNIQUE_COUNT,
+    TRUE,
+)
+from educommon.report.constructor.exceptions import (
+    DataSourceParamsNotFound,
+    FilterError,
+    ReportConstructorException,
+)
+from educommon.report.constructor.models import (
+    ReportFilter,
+    ReportFilterGroup,
+    ReportTemplate,
+)
+from educommon.report.constructor.registries import (
+    registry,
+)
+from educommon.report.constructor.utils import (
+    get_columns_hierarchy,
+    get_field,
+    get_field_value_by_display,
+)
+from educommon.utils.misc import (
+    cached_property,
+)
 
 
-class FilterValuesProvider(object):
-
-    u"""Поставщик данных фильтра.
+class FilterValuesProvider:
+    """Поставщик данных фильтра.
 
     Используется как для формирования Q-фильтра для ORM, так и для
         последующей фильтрации полученных данных.
 
     Возвращает значение из фильтра, преобразованное к объекту Python.
 
     Тип возвращаемого значения определяется оператором сравнения, который
@@ -74,56 +108,56 @@
 
        Под значением фильтра подразумевается значение поля ``values`` модели
        :class:`~educommon.report.constructor.models.ReportFilter`.
 
     """
 
     def __init__(self, as_orm_filter=True):
-        u"""Инициализация провайдера.
+        """Инициализация провайдера.
 
         :param bool as_orm_filter: преобразовать значения к типам ORM
             или к типам отчёта (например, True/False или Да/Нет).
         """
 
         self._as_orm_filter = as_orm_filter
 
     def to_python(self, value, report_filter, column_descriptor):
-        u"""Возвращает значение из фильтра, приведенное к объекту Python.
+        """Возвращает значение из фильтра, приведенное к объекту Python.
 
         В параметрах фильтра значение хранится в виде текстовой строки.
         """
 
         if column_descriptor.data_type == constants.CT_CHOICES:
             return get_field_value_by_display(
                 column_descriptor.field,
                 value
             ) if self._as_orm_filter else value
         else:
             if isinstance(column_descriptor.field.formfield(), BooleanField):
                 if (
-                    isinstance(value, six.string_types) and
-                    value.lower() in (u'false', u'0', u'нет')
+                    isinstance(value, str) and
+                    value.lower() in ('false', '0', 'нет')
                 ):
                     return False if self._as_orm_filter else FALSE
 
                 elif (
-                    isinstance(value, six.string_types) and
-                    value.lower() in (u'true', u'1', u'да')
+                    isinstance(value, str) and
+                    value.lower() in ('true', '1', 'да')
                 ):
                     return True if self._as_orm_filter else TRUE
 
                 else:
                     raise FilterError(
-                        report_filter, u'неправильно задано значение фильтра'
+                        report_filter, 'неправильно задано значение фильтра'
                     )
 
             return column_descriptor.field.formfield().to_python(value)
 
     def __call__(self, report_filter, column_descriptor):
-        u"""Возвращает значение из фильтра, преобразованное к объекту Python.
+        """Возвращает значение из фильтра, преобразованное к объекту Python.
 
         :param report_filter: Фильтр шаблона отчетов.
         :type report_filter: educommon.report.constructor.models.ReportFilter
 
         :param column_descriptor: Дескриптор поля модели, входящего в состав
             столбца отчета.
         :type column_descriptor:
@@ -142,57 +176,57 @@
             result = tuple(
                 self.to_python(value, report_filter, column_descriptor)
                 for value in report_filter.values
             )
 
             if len(result) != 2:
                 raise FilterError(
-                    report_filter, u'не правильно заданы границы диапазона'
+                    report_filter, 'не правильно заданы границы диапазона'
                 )
 
         elif report_filter.values:
             result = self.to_python(
                 report_filter.values[0],
                 report_filter,
                 column_descriptor
             )
 
         else:
             raise FilterError(
-                report_filter, u'не указано значение для сравнения.'
+                report_filter, 'не указано значение для сравнения.'
             )
 
         return result
 
 
 def is_row(data):
-    u"""Возвращает True, если в ``data`` содержится строка с данными.
+    """Возвращает True, если в ``data`` содержится строка с данными.
 
     :rtype: bool
     """
     return (
         isinstance(data, (tuple, list)) and
         any(not isinstance(cell, (tuple, list)) for cell in data)
     )
 
 
 def is_block(data):
-    u"""Возвращает True, если в ``data`` содержится блок записей.
+    """Возвращает True, если в ``data`` содержится блок записей.
 
     :rtype: bool
     """
     return (
         data and
         isinstance(data, (tuple, list)) and
         all(isinstance(row, (tuple, list)) for row in data)
     )
 
 
 def get_data_width(data):
-    u"""Возвращает количество колонок, занимаемое данными.
+    """Возвращает количество колонок, занимаемое данными.
 
     :param list data: Данные блока, строки или ячейки.
         - Ячейка --- это простые данные (строка, число, дата и т.п.).
         - Строка --- это кортеж из данных ячеек и вложенных блоков.
         - Блок --- это кортеж из строк. Содержит только строки.
 
     :rtype: int
@@ -201,20 +235,19 @@
         return max(map(get_data_width, data))
     elif is_row(data):
         return sum(map(get_data_width, data))
     else:
         return 1
 
 
-class _FilterBuilder(object):
-
-    u"""Построитель фильтров для выборки данных из БД."""
+class _FilterBuilder:
+    """Построитель фильтров для выборки данных из БД."""
 
     def __init__(self, report_filter, column_descriptor):
-        u"""Инициализация экземпляра.
+        """Инициализация экземпляра.
 
         :param report_filter: Фильтр шаблона отчетов.
         :type report_filter: educommon.report.constructor.models.ReportFilter
 
         :param column_descriptor: Дескриптор поля модели, входящего в состав
             столбца отчета.
         ::type column_descriptor:
@@ -225,15 +258,15 @@
             column_descriptor
         )
 
         self._report_filter = report_filter
         self._column_descriptor = column_descriptor
 
     def _get_lookup(self, field_lookup):
-        u"""Возвращает lookup-выражение, соответствующее параметрам фильтра.
+        """Возвращает lookup-выражение, соответствующее параметрам фильтра.
 
         При формировании lookup-выражения учитываются параметры фильтра
         ``case_sensitive``, ``operator``, а также тип данных столбца, по
         которому выполняется фильтрация.
 
         :param str field_lookup: lookup-выражение для доступа к значению поля
         """
@@ -279,51 +312,50 @@
             values = FilterValuesProvider()(
                 self._report_filter, self._column_descriptor
             )
 
         return values
 
     def get_orm_filter(self):
-        u"""Возвращает условия выборки из шаблона отчета.
+        """Возвращает условия выборки из шаблона отчета.
 
         :rtype: django.db.models.Q
         """
         field_lookup = self._column_descriptor.full_lookup
 
         filter_values = self._get_values()
 
         if self._report_filter.operator == constants.IS_NULL:
             if self._column_descriptor.data_type == constants.CT_TEXT:
                 result = Q(
                     Q(**{field_lookup + '__isnull': True}) |
-                    Q(**{field_lookup: u''})
+                    Q(**{field_lookup: ''})
                 )
             else:
                 result = Q(**{field_lookup + '__isnull': True})
 
         else:
             try:
                 result = Q(**{
                     self._get_lookup(field_lookup): filter_values,
                 })
             except ValueError as error:
-                raise FilterError(self._report_filter, six.text_type(error))
+                raise FilterError(self._report_filter, str(error))
 
         if self._report_filter.exclude:
             result = ~result
 
         return result
 
 
-class _FilterGroupBuilder(object):
-
-    u"""Построитель Q-выражений и фильтрующих функций для групп фильтров."""
+class _FilterGroupBuilder:
+    """Построитель Q-выражений и фильтрующих функций для групп фильтров."""
 
     def __init__(self, data_filterer, filter_group):
-        u"""Инициализация экземпляра класса.
+        """Инициализация экземпляра класса.
 
         :param data_filterer: Фильтратор данных отчета.
         :type data_filterer: _DataFilterer
 
         :param filter_group: Группа фильтров.
         :type filter_group:
             educommon.report.constructor.models.ReportFilterGroup
@@ -336,45 +368,45 @@
         self._data_filterer = data_filterer
         self._filter_group = filter_group
 
     def _get_nested_orm_filters(self):
         for nested_group in self._filter_group.nested_groups.all():
             if any(
                 report_filter
-                for report_filter in six.itervalues(self._data_filterer)
+                for report_filter in self._data_filterer.values()
                 if report_filter.group_id == nested_group.id
             ):
                 yield nested_group.get_orm_filter()
 
         data_source = self._data_filterer.data_source_descriptor
 
-        for report_filter in six.itervalues(self._data_filterer.filters_by_id):
+        for report_filter in self._data_filterer.filters_by_id.values():
             if report_filter.group_id == self._filter_group.id:
                 column_descriptor = data_source.get_column_descriptor(
                     report_filter.column.name
                 )
                 if isinstance(column_descriptor.field, models.Field):
                     filter_builder = _FilterBuilder(
                         report_filter, column_descriptor
                     )
                     yield filter_builder.get_orm_filter()
 
     def get_orm_filter(self):
-        u"""Возвращает Q-выражение для данной группы фильтров.
+        """Возвращает Q-выражение для данной группы фильтров.
 
         :rtype: django.db.models.Q
         """
         operators = {
             ReportFilterGroup.OPERATOR_AND: operator.and_,
             ReportFilterGroup.OPERATOR_OR: operator.or_,
         }
 
         if self._filter_group.operator not in operators:
             raise ApplicationLogicException(
-                u'Неподдерживаемый оператор: {}'
+                'Неподдерживаемый оператор: {}'
                 .format(self._filter_group.operator)
             )
 
         orm_filters = tuple(self._get_nested_orm_filters())
 
         if orm_filters:
             result = reduce(
@@ -383,27 +415,26 @@
             )
         else:
             result = Q()
 
         return result
 
 
-class _DataFilterer(object):
-
-    u"""Фильтратор данных отчета.
+class _DataFilterer:
+    """Фильтратор данных отчета.
 
     Фильтрация данных выполняется в два этапа:
 
         1. Наложение фильтров на запрос.
         2. Фильтрация полученных данных в приложении.
     """
 
     def __init__(self, report_template, data_source_descriptor,
                  report_columns, ignored_columns_ids):
-        u"""Инициализация экземпляра класса.
+        """Инициализация экземпляра класса.
 
         :param report_template: Шаблон фильтра.
         :type report_template:
             educommon.report.constructor.models.ReportTemplate
 
         :param data_source_descriptor: Дескриптор источника данных..
         :type data_source_descriptor:
@@ -422,15 +453,15 @@
         self._report_template = report_template
         self.data_source_descriptor = data_source_descriptor
         self._report_columns = report_columns
         self._ignored_columns_ids = ignored_columns_ids
 
     @cached_property
     def filters_by_id(self):
-        u"""Все фильтры шаблона по id фильтра.
+        """Все фильтры шаблона по id фильтра.
 
         :rtype: dict
         """
         query = ReportFilter.objects.filter(
             group__report_template=self._report_template,
         ).exclude(
             column_id__in=self._ignored_columns_ids
@@ -438,15 +469,15 @@
 
         return {
             report_filter.id: report_filter
             for report_filter in query
         }
 
     def get_orm_filters(self):
-        u"""Возвращает фильтры для формирования SQL-запроса.
+        """Возвращает фильтры для формирования SQL-запроса.
 
         .. note::
 
            Предназначена для предварительной фильтрации данных на уровне СУБД.
            Т.к. данные загружаются только для модели источника данных без
            данных зависимых объектов, эти фильтры не срабатывают при загрузке
            зависимых объектов. Поэтому дополнительно нужно применять функцию
@@ -460,15 +491,15 @@
 
         if filter_group:
             return _FilterGroupBuilder(self, filter_group).get_orm_filter()
         else:
             return Q()
 
     def _get_function_for_filter(self, report_filter):
-        u"""Возвращает функцию для фильтрации данных в соответствии с фильтром.
+        """Возвращает функцию для фильтрации данных в соответствии с фильтром.
 
         :rtype: callable
         """
         data_source = self.data_source_descriptor
         column_descriptor = data_source.get_column_descriptor(
             report_filter.column.name
         )
@@ -497,42 +528,42 @@
                 return value is not None and value >= filter_values
 
         elif report_filter.operator == constants.IS_NULL:
             def function(value):
                 return value is None or value == ''
 
         elif report_filter.operator == constants.CONTAINS:
-            assert isinstance(filter_values, six.string_types), type(
+            assert isinstance(filter_values, str), type(
                 filter_values
             )
 
             if report_filter.case_sensitive:
                 def function(value):
                     return value is not None and filter_values in value
             else:
                 def function(value):
                     return value is not None and any(
                         v.lower() in value
                         for v in filter_values
                     )
 
         elif report_filter.operator == constants.STARTS_WITH:
-            assert isinstance(filter_values, six.string_types), type(
+            assert isinstance(filter_values, str), type(
                 filter_values
             )
 
             if report_filter.case_sensitive:
                 def function(value):
                     return value is not None and value.startswith(filter_values)
             else:
                 def function(value):
                     return value is not None and value.lower().startswith(filter_values.lower())
 
         elif report_filter.operator == constants.ENDS_WITH:
-            assert isinstance(filter_values, six.string_types), type(
+            assert isinstance(filter_values, str), type(
                 filter_values
             )
 
             if report_filter.case_sensitive:
                 def function(value):
                     return value is not None and value.endswith(filter_values)
             else:
@@ -544,15 +575,15 @@
                 def function(value):
                     return (
                         value is not None and
                         filter_values[0] <= value <= filter_values[1]
                     )
             else:
                 def function(value):
-                    if isinstance(value, six.text_type):
+                    if isinstance(value, str):
                         value = value.lower()
                         values = tuple(v.lower() for v in filter_values)
                     else:
                         values = filter_values
 
                     return (
                         value is not None and
@@ -568,48 +599,48 @@
             else:
                 def function(value):
                     return value.lower() in (v.lower() for v in filter_values)
 
         else:
             raise FilterError(
                 report_filter,
-                u'Неподдерживаемый оператор ({})'.format(
+                'Неподдерживаемый оператор ({})'.format(
                     report_filter.operator
                 )
             )
 
         if report_filter.exclude:
             return lambda value: not function(value)
         else:
             return function
 
     def get_filter_function(self):
-        u"""Возвращает функцию для фильтрации данных.
+        """Возвращает функцию для фильтрации данных.
 
         Эта функция для каждого набора данных возвращает новый набор данных,
         которые отфильтрованы в соответствии с параметрами фильтрации,
         указанными в шаблоне отчета.
 
         Запись может быть отфильтрована полностью, либо отфильтрованы только
         вложенные блоки. В первом случае функция возвращает ``None``. Во
         втором случае --- будут удалены записи во внутренних блоках.
         """
         filter_functions = {
             report_filter.column_id: self._get_function_for_filter(
                 report_filter
             )
-            for report_filter in six.itervalues(self.filters_by_id)
+            for report_filter in self.filters_by_id.values()
         }
         filter_functions_by_column = tuple(
             filter_functions.get(report_column.pk)
             for report_column in self._report_columns
         )
 
         def filter_function(row_data, column_functions=None):
-            u"""Возвращает отфильтрованные данные записи отчета."""
+            """Возвращает отфильтрованные данные записи отчета."""
             if column_functions is None:
                 column_functions = filter_functions_by_column
 
             result = []
             for cell in row_data:
                 cell_width = get_data_width(cell)
                 column_filter_functions = column_functions[:cell_width]
@@ -631,44 +662,42 @@
                     ):
                         return None
                     result.append(cell)
 
             return result
 
         def _filter_block_or_row(block_or_row, column_filter_functions):
-            u"""Возвращет отфильтрованный блок/строку или None."""
+            """Возвращет отфильтрованный блок/строку или None."""
             if is_row(block_or_row):
                 return filter_function(block_or_row, column_filter_functions)
             filtered = [_filter_block_or_row(item, column_filter_functions)
                         for item in block_or_row]
             filtered = [item for item in filtered if item is not None]
             return filtered or None
 
         return filter_function
 
 
 @total_ordering
-class _OrderInverter(object):
-
+class _OrderInverter:
     """Класс-обёртка для смены направления сортировки."""
 
     # pylint: disable=eq-without-hash
 
     def __init__(self, value):
         self.value = value
 
     def __eq__(self, other):
         return self.value == other.value
 
     def __lt__(self, other):
         return gt(self.value, other.value)
 
 
-class _DataSorter(object):
-
+class _DataSorter:
     """Сортировщик данных отчёта.
 
     Структура данных для отчёта представляет из себя набор кортежей (см.
     описание класса ``DataLoader``). Все кортежи можно разделить на два типа:
     строка и блок. Блок --- это набор строк, строка, в свою очередь, может
     содержать как данные ячеек, так и другие блоки. Если строка содержит блоки,
     это означает, что объекты-источники, содержащие соответствующие данные,
@@ -795,17 +824,16 @@
 
         :rtype: bool
         """
         values_to_sort = (i in row and row[i] for i in self._params)
         return None in values_to_sort
 
 
-class DataLoader(object):
-
-    u"""Загрузчик данных для шаблона отчета.
+class DataLoader:
+    """Загрузчик данных для шаблона отчета.
 
     Данные каждой строки отчета представлены в виде кортежа. Элементами кортежа
     могут быть значения простых типов (числа, строки и т.п.), а также
     кортежи кортежей (вложенные блоки). Вложенные блоки добавляются в тех
     случаях, когда в параметрах отчета указаны т.н. обратные связи (связь "один
     ко многим"), когда одной записи в модели источника данных соответствует
     несколько записей в связанных моделях. В таких вложенных кортежах также
@@ -857,15 +885,15 @@
         self._user = user
 
     @staticmethod
     def _get_column_count(columns):
         # Для иерархии столбцов возвращает количество занимаемых столбцов.
         if columns:
             return sum(map(
-                DataLoader._get_column_count, six.itervalues(columns)
+                DataLoader._get_column_count, columns.values()
             ))
         else:
             return 1
 
     @staticmethod
     def _get_field_display(field, field_value):
         for value, name in field.flatchoices:
@@ -943,15 +971,15 @@
                 yield list(itertools.takewhile(bool, related_obj_data_gen))
             else:
                 yield [[None] * DataLoader._get_column_count(nested)]
 
         # Прямая связь (ForeignKey или OneToOneField).
         elif nested:
             if attr_value:
-                for k, v in six.iteritems(nested):
+                for k, v in nested.items():
                     for object_data in (
                         DataLoader._get_object_data(attr_value, k, v)
                     ):
                         yield object_data
             else:
                 for _ in range(DataLoader._get_column_count(nested)):
                     yield None
@@ -966,42 +994,42 @@
                             DataLoader._get_field_display(
                                 field.base_field, inner_value
                             )
                         )
                     else:
                         inner_values.append(inner_value)
                 yield list(
-                    (six.text_type(value),) for value in inner_values
+                    (str(value),) for value in inner_values
                 )
 
             # Поле с choices.
             elif getattr(field, 'flatchoices', False):
                 yield DataLoader._get_field_display(
                     field, attr_value
                 )
 
             # Поле с данными.
             else:
                 yield attr_value
 
     @cached_property
     def _data_filterer(self):
-        u"""Фильтратор данных отчета."""
+        """Фильтратор данных отчета."""
         return _DataFilterer(
             self._report_template, self._data_source, self._report_columns,
             self._ignored_columns_ids
         )
 
     @cached_property
     def _data_aggregator(self):
-        u"""Агрегатор данных отчета."""
+        """Агрегатор данных отчета."""
         return DataAggregator(self._report_columns)
 
     def _available_units_filter(self, query):
-        u"""Фильтратор данных отчета по доступности учреждений."""
+        """Фильтратор данных отчета по доступности учреждений."""
         return self._data_source.add_source_filter(
             query, self._report_template.include_available_units,
             self._user
         )
 
     def _get_objects(self):
         result = self._data_source.model.objects.all()
@@ -1042,248 +1070,245 @@
             visible=True,
         ).exclude(
             pk__in=self._ignored_columns_ids
         ).values_list('name', flat=True)
 
         if not column_names:
             raise ReportConstructorException(
-                u'В шаблоне нет ни одного отображаемого столбца.'
+                'В шаблоне нет ни одного отображаемого столбца.'
             )
 
         columns_hierarchy = get_columns_hierarchy(*column_names)
 
         result = list(self._get_rows_data(columns_hierarchy))
 
         sorter = _DataSorter(self._report_template, self._ignored_columns_ids)
         result = sorter.sort(result)
 
         result.extend(self._data_aggregator.get_rows())
 
         return iter(result)
 
 
-class ReportBuilderBase(six.with_metaclass(abc.ABCMeta, object)):
-    u"""Базовый класс построителя отчета."""
+class ReportBuilderBase(metaclass=abc.ABCMeta):
+    """Базовый класс построителя отчета."""
 
     def __init__(self, report_template, file_path, user):
-        u"""Инициализация класса.
+        """Инициализация класса.
 
         :param report_template: Шаблон отчета.
         :type report_template:
             educommon.report.constructor.models.ReportTemplate
 
-        :param unicode file_path: Путь к файлу отчета.
+        :param str file_path: Путь к файлу отчета.
         """
         assert isinstance(report_template, ReportTemplate), type(
             report_template
         )
 
         if report_template.data_source_name not in registry:
             raise DataSourceParamsNotFound(report_template.data_source_name)
 
         self._report_template = report_template
         self._file_path = file_path
         self._user = user
 
     @cached_property
     def _data_source(self):
-        u"""Имя источника данных, указанного в шаблоне.
+        """Имя источника данных, указанного в шаблоне.
 
-        :rtype: unicode
+        :rtype: str
         """
         return self._report_template.data_source
 
     @cached_property
     def _report_columns(self):
-        u"""Столбцы отчета.
+        """Столбцы отчета.
 
         :rtype: tuple
         """
         return tuple(
             self._report_template.columns.exclude(
                 pk__in=self._ignored_columns_ids
             )
         )
 
     @cached_property
     def _ignored_columns_ids(self):
-        u"""Исключенные из отчета колонки
+        """Исключенные из отчета колонки
 
         :rtype: set
         """
         ignored_columns = set()
         for col_id, col_name in self._report_template.columns.values_list(
                 'id', 'name'):
             if self._data_source.is_column_ignored(col_name):
                 ignored_columns.add(col_id)
 
         return ignored_columns
 
     @cached_property
     def _data(self):
-        u"""Отфильтрованные и отсортированные данные отчета.
+        """Отфильтрованные и отсортированные данные отчета.
 
         :rtype: list
         """
         return list(
             DataLoader(
                 self._report_template, self._data_source, self._report_columns,
                 self._ignored_columns_ids, self._user
             )
         )
 
     @cached_property
     def _workbook(self):
-        u"""Книга Excel, в которой формируется отчет."""
+        """Книга Excel, в которой формируется отчет."""
         result = Workbook(self._file_path, dict(
             default_date_format='dd.mm.yyyy',
         ))
 
         for cell_format in (result.default_date_format,
                             result.default_url_format):
             cell_format.set_border()
             cell_format.set_align('vcenter')
 
         return result
 
     @cached_property
     def _worksheet(self):
-        u"""Страница в книге Excel."""
-        return self._workbook.add_worksheet(u'Отчет')
+        """Страница в книге Excel."""
+        return self._workbook.add_worksheet('Отчет')
 
     @abc.abstractmethod
     def _flush_header(self):
-        u"""Запись заголовка отчета."""
+        """Запись заголовка отчета."""
 
     @abc.abstractmethod
     def _flush_data(self):
-        u"""Запись данных в отчет."""
+        """Запись данных в отчет."""
 
     def build(self):
-        u"""Формирование отчета."""
+        """Формирование отчета."""
         self._flush_header()
         self._flush_data()
 
         self._workbook.close()
 
 
-class BaseColumnAggregator(six.with_metaclass(abc.ABCMeta, object)):
-
-    u"""Базовый класс агрегатора данных для колонки."""
+class BaseColumnAggregator(metaclass=abc.ABCMeta):
+    """Базовый класс агрегатора данных для колонки."""
 
     @abc.abstractmethod
     def type(self):
-        u"""Тип агрегатора."""
+        """Тип агрегатора."""
 
     @abc.abstractmethod
     def title(self):
-        u"""Название агрегатора."""
+        """Название агрегатора."""
 
     def __init__(self, column_index, by_value, total, **kwargs):
-        u"""Инициализирует агрегатор.
+        """Инициализирует агрегатор.
 
         :param column_name: Название колонки.
         :param column_index: Порядковый номер колонки в отчете.
         :param by_value: Требуется вывод промежуточного итога в отчет.
         :param total: Требуется вывод итога в отчет.
         :param kwargs: Дополнительные параметры.
         """
         self.__column_idx = column_index
         self.__data = defaultdict(int)
         self.__is_total = total
         self.__is_by_value = by_value
 
     @abc.abstractmethod
     def aggregate(self, value):
-        u"""Реализует правила подсчета по значению колонки."""
+        """Реализует правила подсчета по значению колонки."""
 
     def get(self, value):
-        u"""Возвращает результат подсчета для определенного элемента."""
+        """Возвращает результат подсчета для определенного элемента."""
         return self.__data[value]
 
     @property
     def data(self):
-        u"""Возвращает текущий результат выполнения подсчета."""
+        """Возвращает текущий результат выполнения подсчета."""
         return self.__data
 
     @property
     def is_by_value(self):
-        u"""Требуется вывод промежуточного итога в отчет."""
+        """Требуется вывод промежуточного итога в отчет."""
         return self.__is_by_value
 
     @property
     def is_total(self):
-        u"""Требуется вывод итога в отчет"""
+        """Требуется вывод итога в отчет"""
         return self.__is_total
 
     @property
     def total(self):
-        u"""Считает итоговое значение по собранным промежуточным итогам."""
-        return sum(six.itervalues(self.__data))
+        """Считает итоговое значение по собранным промежуточным итогам."""
+        return sum(self.__data.values())
 
     @property
     def column_index(self):
-        u"""Позиция колонки в отчете."""
+        """Позиция колонки в отчете."""
         return self.__column_idx
 
 
 class ColumnCounter(BaseColumnAggregator):
-
-    u"""Счетчик данных для колонки."""
+    """Счетчик данных для колонки."""
 
     type = COUNT
-    title = u'Количество'
+    title = 'Количество'
 
     def __init__(self, column_index, by_value, total, **kwargs):
         super(ColumnCounter, self).__init__(
             column_index, by_value, total, **kwargs
         )
         # Требуется ли вывод в итоге количества уникальных значений.
         self.__is_total_unique = kwargs.get('total_unique', False)
 
     def aggregate(self, value):
-        u"""Считает количество элементов."""
+        """Считает количество элементов."""
         self.data[value] += 1
 
     @property
     def is_total_unique(self):
-        u"""Требуется вывод количества уникальных значений."""
+        """Требуется вывод количества уникальных значений."""
         return self.__is_total_unique
 
     @property
     def total_unique(self):
-        u"""Количество уникальных значений."""
-        return sum(count for count in six.itervalues(self.data) if count == 1)
+        """Количество уникальных значений."""
+        return sum(count for count in self.data.values() if count == 1)
 
 
 class ColumnSum(BaseColumnAggregator):
-
-    u"""Сумматор данных для колонки."""
+    """Сумматор данных для колонки."""
 
     type = SUM
-    title = u'Сумма'
+    title = 'Сумма'
 
     def aggregate(self, value):
-        u"""Считает сумму элементов."""
-        if isinstance(value, six.string_types):
+        """Считает сумму элементов."""
+        if isinstance(value, str):
             # Если число, то пробуем привести к int.
             if value.isdigit():
                 value = int(value)
             # Иначе, пробуем привести к float.
             else:
                 try:
                     value = float(value)
                 except ValueError:
                     value = 0
 
         self.data[value] += value
 
 
 def get_column_aggregator_info(column):
-    u"""Возвращает информацию об агрегаторе колонки.
+    """Возвращает информацию об агрегаторе колонки.
 
     :param column: Колонка отчета
     :type column: educommon.report.constructor.models.ReportColumn
     :return: Тип агрегатора, (промежуточный итог, итог, количество уникальных)
     :rtype: tuple
     """
     if (
@@ -1301,38 +1326,37 @@
             column.total == TOTAL_SUM,
             None
         )
     else:
         return None, (None, None, None)
 
 
-class DataAggregator(object):
-
-    u"""Агрегатор данных полученных при формировании отчета."""
+class DataAggregator:
+    """Агрегатор данных полученных при формировании отчета."""
 
     def __init__(self, report_columns):
         self._report_columns = report_columns
 
         self._aggregators = dict()
         self.set_aggregators((ColumnCounter, ColumnSum))
 
     def set_aggregators(self, aggregators):
-        u"""Добавляет последовательность агрегаторов."""
+        """Добавляет последовательность агрегаторов."""
         for aggregator in aggregators:
             self.set_aggregator(aggregator)
 
     def set_aggregator(self, aggregator):
-        u"""Добавляет агрегатор."""
+        """Добавляет агрегатор."""
         self._aggregators[aggregator.type] = dict(
             cls=aggregator,
             instances=dict()
         )
 
     def get_column_aggregator(self, column, column_idx):
-        u"""Возвращает агрегатор для колонки."""
+        """Возвращает агрегатор для колонки."""
         aggregator_type, (by_value, total, total_unique) = (
             get_column_aggregator_info(column)
         )
         aggregator = self._aggregators.get(aggregator_type)
         if not aggregator:
             return
 
@@ -1349,92 +1373,92 @@
                 params['total_unique'] = total_unique
             instance = aggregator_cls(**params)
             aggregator['instances'][column.name] = instance
 
         return instance
 
     def _process_cell_value(self, col_idx, col_value):
-        u"""Считает промежуточный результат для значения в ячейке."""
+        """Считает промежуточный результат для значения в ячейке."""
         column = self._report_columns[col_idx]
         column_aggregator = self.get_column_aggregator(column, col_idx)
         if col_value and column_aggregator:
             column_aggregator.aggregate(col_value)
 
     def aggregate(self, row_data):
-        u"""Считает промежуточный результат по элементам строки отчета."""
+        """Считает промежуточный результат по элементам строки отчета."""
         for idx, value in enumerate(row_data):
             if isinstance(value, (list, tuple)):
                 for nested_data in value:
                     for nested_idx, nested_value in enumerate(nested_data):
                         col_idx = idx + nested_idx
                         self._process_cell_value(col_idx, nested_value)
             else:
                 self._process_cell_value(idx, value)
 
     def get_empty_row(self):
-        u"""Формирует пустую строку по количеству колонок в отчете."""
+        """Формирует пустую строку по количеству колонок в отчете."""
         return ['' for _ in range(len(self._report_columns))]
 
     def _extend_rows(self, aggregators, rows):
         """Добавляет строки с промежуточными итогами."""
         aggregators_data = (
             (
                 aggregator.title,
                 aggregator.column_index,
-                six.iteritems(aggregator.data),
+                aggregator.data.items(),
             )
             for aggregator in aggregators if aggregator.is_by_value
         )
         for title, col_idx, data in aggregators_data:
             for idx, (value, value_data) in enumerate(data):
                 try:
                     row_data = rows[idx]
                 except IndexError:
                     row_data = self.get_empty_row()
                     rows.append(row_data)
 
                 row_data[col_idx] = (
-                    u'{} "{}": {}'.format(title, value, value_data)
+                    '{} "{}": {}'.format(title, value, value_data)
                 )
 
     def _extend_rows_by_count(self, rows):
-        u"""Добавляет строки с количеством элементов."""
+        """Добавляет строки с количеством элементов."""
         counters = sorted(
-            six.itervalues(self._aggregators[COUNT]['instances']),
+            self._aggregators[COUNT]['instances'].values(),
             key=lambda c: c.column_index
         )
         self._extend_rows(counters, rows)
 
     def _extend_rows_by_sum(self, rows):
-        u"""Добавляет строки с суммой элементов."""
+        """Добавляет строки с суммой элементов."""
         summators = sorted(
-            six.itervalues(self._aggregators[SUM]['instances']),
+            self._aggregators[SUM]['instances'].values(),
             key=lambda c: c.column_index
         )
         self._extend_rows(summators, rows)
 
     def get_total_row(self):
-        u"""Возвращает строку с итоговыми значениями."""
+        """Возвращает строку с итоговыми значениями."""
         row = self.get_empty_row()
-        for aggregator in six.itervalues(self._aggregators):
-            for instance in six.itervalues(aggregator['instances']):
+        for aggregator in self._aggregators.values():
+            for instance in aggregator['instances'].values():
                 if instance.is_total:
-                    row[instance.column_index] = u'Итог({}): {}'.format(
+                    row[instance.column_index] = 'Итог({}): {}'.format(
                         instance.title,
                         instance.total
                     )
                 elif instance.is_total_unique:
                     row[instance.column_index] = (
-                        u'Итог(Уникальных): {}'.format(instance.total_unique)
+                        'Итог(Уникальных): {}'.format(instance.total_unique)
                     )
 
         return row
 
     def get_rows(self):
-        u"""Возвращает строки отчета с результатами подсчета значений."""
+        """Возвращает строки отчета с результатами подсчета значений."""
         rows = list()
         self._extend_rows_by_count(rows)
         self._extend_rows_by_sum(rows)
 
         # Добавляем итоговые значения
         total_row = self.get_total_row()
         if any(total_row):
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/builders/excel/_header.py` & `educommon-3.0.0/src/educommon/report/constructor/builders/excel/_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# coding: utf-8
-from __future__ import absolute_import
+from educommon.utils.misc import (
+    cached_property,
+)
 
-from six.moves import range
 
-from educommon.utils.misc import cached_property
-
-
-class HierarchicalHeaderMixin(object):
-    u"""Класс-примесь к построителям отчетов для формирования заголовка."""
+class HierarchicalHeaderMixin:
+    """Класс-примесь к построителям отчетов для формирования заголовка."""
 
     @cached_property
     def __column_descriptors(self):
         result = []
 
         for report_column in self._report_columns:
             if not report_column.visible:
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/builders/excel/product.py` & `educommon-3.0.0/src/educommon/report/constructor/builders/excel/product.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-# coding: utf-8
-from __future__ import absolute_import
+from datetime import (
+    date,
+    datetime,
+    time,
+)
+from functools import (
+    partial,
+)
+from itertools import (
+    chain,
+    product,
+)
+
+from educommon.report.constructor.builders.excel._base import (
+    ReportBuilderBase,
+    is_block,
+)
+from educommon.report.constructor.builders.excel._header import (
+    HierarchicalHeaderMixin,
+)
+from educommon.utils.misc import (
+    cached_property,
+)
 
-from datetime import date
-from datetime import datetime
-from datetime import time
-from functools import partial
-from itertools import chain
-from itertools import product
 
-from six.moves import map
-from six.moves import zip
-
-from educommon.utils.misc import cached_property
-
-from ._base import ReportBuilderBase
-from ._base import is_block
-from ._header import HierarchicalHeaderMixin
-
-
-class _Cell(object):
+class _Cell:
     # Класс для хранения значения ячейки отчета и порядкового номера ячейки.
     # Позволяет сортировать ячейки в соответстии с их порядковым номером.
 
     def __init__(self, index, value):
         self.index = index
         self.value = value
 
     def __lt__(self, other):
         return self.index < other.index
 
 
 def _join(simple_data, block_indexes, block_row_data):
-    u"""Объединяет данные основной записи и данные строки блока"""
+    """Объединяет данные основной записи и данные строки блока"""
 
     # Проставление порядковых номеров
     block_row_data = tuple(
         _Cell(index, data)
         for index, data in zip(block_indexes, block_row_data)
     )
 
@@ -50,15 +55,15 @@
             else (cell.value,)
         )
         for cell in block_row_data
     )))
 
 
 class ReportBuilder(HierarchicalHeaderMixin, ReportBuilderBase):
-    u"""Построитель отчета в формате Excel без объединения ячеек.
+    """Построитель отчета в формате Excel без объединения ячеек.
 
     В случае, если столбцы формируемого отчета связаны отношением один ко
     многим (обратные связи), формируется декартово произведение связанных
     записей как при объединении таблиц в SQL.
     """
 
     @cached_property
@@ -69,15 +74,15 @@
         result.set_text_wrap()
         result.set_align('vcenter')
 
         return result
 
     @staticmethod
     def _data_to_rows(data):
-        u"""Возвращает данные отчета в виде декартова произведения.
+        """Возвращает данные отчета в виде декартова произведения.
 
         В зависимости от значения аргумента :arg:`data` выполняет следующие
         преобразования данных:
 
             * *Блоки записей*: для каждой записи блока рекурсивно вызывает
               функцию :meth:`_data_to_rows`, полученные строки объединяет в
               новый блок и возвращает его в качестве результата. Записи
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/builders/excel/with_merged_cells.py` & `educommon-3.0.0/src/educommon/report/constructor/builders/excel/with_merged_cells.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# coding: utf-8
-u"""Реализация построителя отчетов ."""
-from __future__ import absolute_import
+"""Реализация построителя отчетов ."""
+from datetime import (
+    date,
+    datetime,
+    time,
+)
+
+from educommon.report.constructor.builders.excel._base import (
+    ReportBuilderBase,
+)
+from educommon.report.constructor.builders.excel._header import (
+    HierarchicalHeaderMixin,
+)
+from educommon.utils.misc import (
+    cached_property,
+)
 
-from datetime import date
-from datetime import datetime
-from datetime import time
 
-from six.moves import map
-from six.moves import range
-
-from educommon.utils.misc import cached_property
-
-from ._base import ReportBuilderBase
-from ._header import HierarchicalHeaderMixin
-
-
-class Frame(object):
+class Frame:
 
     def __init__(self, worksheet, top, left, style):
         self._worksheet = worksheet
         self._top = top
         self._left = left
         self._style = style
 
@@ -138,15 +139,15 @@
         elif isinstance(data, list):
             self._write_row(data)
         else:
             self._write_cell(data, height=1)
 
 
 class ReportBuilder(HierarchicalHeaderMixin, ReportBuilderBase):
-    u"""Построитель отчетов, основанных на пользовательских шаблонах."""
+    """Построитель отчетов, основанных на пользовательских шаблонах."""
 
     @cached_property
     def _data_cell_style(self):
         result = self._workbook.add_format()
 
         result.set_border()
         result.set_text_wrap()
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/config.py` & `educommon-3.0.0/src/educommon/report/constructor/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# coding: utf-8
-u"""Конфигурация асинхронной сборки отчета."""
-from __future__ import absolute_import
+"""Конфигурация асинхронной сборки отчета."""
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
 
-import abc
 
-import six
+class ConstructorConfig(metaclass=ABCMeta):
+    """Конфигурация конструктора отчетов."""
 
-
-class ConstructorConfig(six.with_metaclass(abc.ABCMeta, object)):
-
-    u"""Конфигурация конструктора отчетов."""
-
-    @abc.abstractproperty
+    @property
+    @abstractmethod
     def async_task(self):
-        u"""Асинхронная задача, в которой будет выполняться построение отчета.
+        """Асинхронная задача, в которой будет выполняться построение отчета.
 
         :rtype: :class:`celery.app.task.Task`
         """
-    @abc.abstractproperty
+    @property
+    @abstractmethod
     def current_user_func(self):
-        u"""Функция, возвращающая текущего пользователя."""
+        """Функция, возвращающая текущего пользователя."""
 
 
 # : Конфигурация конструктора отчетов.
 # :
 # : В проекте, который использует конструктор отчетов, в этой переменной должен
 # : быть сохранен экземпляр потомка класса :class:`
 #  ~constructor.config.ConstructorConfig`.
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/editor/actions.py` & `educommon-3.0.0/src/educommon/report/constructor/editor/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,86 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from collections import OrderedDict
-from collections import defaultdict
-from itertools import chain
-from itertools import repeat
-
-from django.contrib.contenttypes.models import ContentType
-from django.core.exceptions import FieldDoesNotExist
-from django.db.transaction import atomic
-from m3.actions.exceptions import ApplicationLogicException
-from m3.actions.results import OperationResult
-from m3.actions.results import PreJsonResult
-from m3_ext.ui.results import ExtUIScriptResult
-from objectpack.actions import BaseAction
-from objectpack.actions import ObjectPack
-from objectpack.exceptions import ValidationError
-from objectpack.ui import BaseEditWindow
-from objectpack.ui import make_combo_box
-from six.moves import map
-from six.moves import zip
-import six
-
-from educommon.m3 import PackValidationMixin
-from educommon.m3 import convert_validation_error_to
-from educommon.m3 import get_id_value
-from educommon.report.constructor.config import report_constructor_config
-from educommon.utils.misc import cached_property
-from educommon.utils.ui import anchor100
-
-from .. import constants
-from ..base import ColumnDescriptor
-from ..models import ReportColumn
-from ..models import ReportFilter
-from ..models import ReportFilterGroup
-from ..models import ReportSorting
-from ..models import ReportTemplate
-from ..registries import registry
-from .ui import EditWindow
-from .ui import ListWindow
+from collections import (
+    OrderedDict,
+    defaultdict,
+)
+from itertools import (
+    chain,
+    repeat,
+)
+
+from django.contrib.contenttypes.models import (
+    ContentType,
+)
+from django.core.exceptions import (
+    FieldDoesNotExist,
+)
+from django.db.transaction import (
+    atomic,
+)
+from m3.actions.exceptions import (
+    ApplicationLogicException,
+)
+from m3.actions.results import (
+    OperationResult,
+    PreJsonResult,
+)
+from m3_ext.ui.results import (
+    ExtUIScriptResult,
+)
+
+from objectpack.actions import (
+    BaseAction,
+    ObjectPack,
+)
+from objectpack.exceptions import (
+    ValidationError,
+)
+from objectpack.ui import (
+    BaseEditWindow,
+    make_combo_box,
+)
+
+from educommon.m3 import (
+    PackValidationMixin,
+    convert_validation_error_to,
+    get_id_value,
+)
+from educommon.report.constructor import (
+    constants,
+)
+from educommon.report.constructor.base import (
+    ColumnDescriptor,
+)
+from educommon.report.constructor.config import (
+    report_constructor_config,
+)
+from educommon.report.constructor.editor.ui import (
+    EditWindow,
+    ListWindow,
+)
+from educommon.report.constructor.models import (
+    ReportColumn,
+    ReportFilter,
+    ReportFilterGroup,
+    ReportSorting,
+    ReportTemplate,
+)
+from educommon.report.constructor.registries import (
+    registry,
+)
+from educommon.utils.misc import (
+    cached_property,
+)
+from educommon.utils.ui import (
+    anchor100,
+)
 
 
 class ColumnsAction(BaseAction):
-
-    u"""Действие, предоставляющее данные для дерева столбцов."""
+    """Действие, предоставляющее данные для дерева столбцов."""
 
     def context_declaration(self):
         return dict(
             data_source_name=dict(type='str'),
             parent_column_name=dict(type='str_or_none', default=None),
         )
 
@@ -64,17 +97,17 @@
         if result['data_type'] == constants.CT_CHOICES:
             result['choices'] = column.choices
 
         return result
 
     def run(self, request, context):
         if context.data_source_name not in registry:
-            raise ApplicationLogicException(u'Не выбран источник данных.')
+            raise ApplicationLogicException('Не выбран источник данных.')
 
-        if context.parent_column_name == u'-1':
+        if context.parent_column_name == '-1':
             context.parent_column_name = None
 
         data_source = registry.get(
             context.data_source_name
         ).get_data_source_descriptor()
 
         if context.parent_column_name:
@@ -92,16 +125,15 @@
         ))
 
 
 _BUILDERS_PACKAGE = 'educommon.report.constructor.builders'
 
 
 class BuildAction(BaseAction):
-
-    u"""Сборка отчета на основе указанного шаблона."""
+    """Сборка отчета на основе указанного шаблона."""
 
     _builders = {
         ReportTemplate.EXCEL_SIMPLE:
             _BUILDERS_PACKAGE + '.excel.product.ReportBuilder',
         ReportTemplate.EXCEL_MERGED:
             _BUILDERS_PACKAGE + '.excel.with_merged_cells.ReportBuilder',
     }
@@ -122,42 +154,42 @@
             raise ApplicationLogicException(self.parent.MSG_DOESNOTEXISTS)
 
     def _check_report_template(self, report_template):
         # Проверка наличия в системе источника данных с именем, указанным в
         # шаблоне.
         if report_template.data_source_name not in registry:
             raise ApplicationLogicException(
-                u'Источник данных {} не существует.'
+                'Источник данных {} не существует.'
                 .format(report_template.data_source_name)
             )
 
         data_source = registry.get(
             report_template.data_source_name
         ).get_data_source_descriptor()
 
         if ReportInfo(report_template).ignored_columns_ids:
             raise ApplicationLogicException(
-                u'Некоторые колонки шаблона неактуальны, '
-                u'требуется редактирование'
+                'Некоторые колонки шаблона неактуальны, '
+                'требуется редактирование'
             )
 
         # Проверка доступности данных для всех столбцов шаблона отчета.
         try:
             for col_name in report_template.columns.values_list(
                     'name', flat=True):
                 if data_source.is_column_ignored(col_name):
                     continue
                 data_source.get_column_descriptor(col_name)
         except FieldDoesNotExist as error:
             raise ApplicationLogicException(
-                u'Колонка {} недоступна'.format(six.text_type(error))
+                'Колонка {} недоступна'.format(str(error))
             )
 
     def _check_params(self, request, context, report_template):
-        u"""Возвращает True, если параметры сборки указаны верно."""
+        """Возвращает True, если параметры сборки указаны верно."""
         if context.format is None:
             return report_template.format in self._builders
 
         if (
             report_template.format == ReportTemplate.USER_DEFINED and
             context.format in self._builders
         ):
@@ -165,34 +197,34 @@
 
         return False
 
     def _get_params_window(self, request, context, report_template):
         win = BaseEditWindow()
 
         win.field__format = make_combo_box(
-            label=u'Формат отчета',
+            label='Формат отчета',
             name='format',
             data=ReportTemplate.FORMAT_CHOICES[1:],
         )
 
         win.form.items.extend(anchor100(
             win.field__format,
         ))
 
         win.set_params(dict(
             form_url=self.get_absolute_url(),
             height=100,
-            title=u'Параметры сборки',
+            title='Параметры сборки',
         ))
 
         return ExtUIScriptResult(win, context)
 
     def _check_format(self, report_format):
         if report_format not in self._builders:
-            raise ApplicationLogicException(u'Указан неверный формат отчета.')
+            raise ApplicationLogicException('Указан неверный формат отчета.')
 
     def _build_report(self, request, context):
         report_template_id = get_id_value(context, self.parent)
         current_user_func = report_constructor_config.current_user_func
         user = current_user_func(request)
         content_type = ContentType.objects.get_for_model(user)
         params = {
@@ -200,61 +232,60 @@
             'content_type': content_type,
             'report_template_id': report_template_id,
             'format': context.format or None
         }
         report_constructor_config.async_task.apply_async(None, params)
 
         return OperationResult(
-            message=u'Внимание! Задача поставлена в очередь! Результаты '
-                    u'будут доступны в реестре Асинхронных задач.'
+            message='Внимание! Задача поставлена в очередь! Результаты '
+                    'будут доступны в реестре Асинхронных задач.'
         )
 
     def run(self, request, context):
         report_template = self._get_report_template(request, context)
         self._check_report_template(report_template)
         if context.format:
             self._check_format(context.format)
 
         if self._check_params(request, context, report_template):
             return self._build_report(request, context)
         else:
             return self._get_params_window(request, context, report_template)
 
 
-class ReportInfo(object):
-
-    u"""Сведения о столбцах отчета, подготовленные к сериализации в JSON."""
+class ReportInfo:
+    """Сведения о столбцах отчета, подготовленные к сериализации в JSON."""
 
     def __init__(self, report_template):
-        u"""Инициализация экземпляра класса.
+        """Инициализация экземпляра класса.
 
         :param report_template: Шаблон отчета.
         :type report_template:
             educommon.report.constructor.models.ReportTemplate
         """
         assert isinstance(report_template, ReportTemplate), type(
             report_template
         )
 
         self.report_template = report_template
 
     @cached_property
     def _data_source(self):
-        u"""Источник данных шаблона.
+        """Источник данных шаблона.
 
         :rtype: educommon.report.constructor.base.ModelDataSourceDescriptor
         """
         data_source = registry.get(
             self.report_template.data_source_name
         ).get_data_source_descriptor()
         return data_source
 
     @cached_property
     def ignored_columns_ids(self):
-        u"""Список колонок исключенных из конструктора отчетов.
+        """Список колонок исключенных из конструктора отчетов.
 
         Исключается параметром ``model.report_constructor_params``.
 
         :rtype: set
         """
         ignored_columns = set()
         for col_id, col_name in self.report_template.columns.values_list(
@@ -263,68 +294,68 @@
                     not self._data_source.is_column_exist(col_name)):
                 ignored_columns.add(col_id)
 
         return ignored_columns
 
     @cached_property
     def _report_columns_by_id(self):
-        u"""Колонки отчета по id.
+        """Колонки отчета по id.
 
         :rtype: collections.OrderedDict
         """
         columns = self.report_template.columns.order_by('index')
 
         return OrderedDict(
             (report_column.id, report_column)
             for report_column in columns
         )
 
     @cached_property
     def _report_columns_by_name(self):
-        u"""Колонки отчета по имени.
+        """Колонки отчета по имени.
 
         :rtype: collections.OrderedDict
         """
         return OrderedDict(
             (report_column.name, report_column)
-            for report_column in six.itervalues(self._report_columns_by_id)
+            for report_column in self._report_columns_by_id.values()
         )
 
     @cached_property
     def _field_descriptors(self):
-        u"""Дескрипторы полей в источнике данных.
+        """Дескрипторы полей в источнике данных.
 
         :rtype: collections.OrderedDict
         """
         get_descriptor = self._data_source.get_column_descriptor
         get_fake_descriptor = self._data_source.get_fake_column_descriptor
 
         descriptors = OrderedDict()
 
-        for report_column in six.itervalues(self._report_columns_by_name):
+        for report_column in self._report_columns_by_name.values():
             if report_column.id in self.ignored_columns_ids:
                 descriptor = get_fake_descriptor(report_column.title)
             else:
                 descriptor = get_descriptor(report_column.name)
             while descriptor:
                 if descriptor.full_accessor_name not in descriptors:
                     descriptors[descriptor.full_accessor_name] = descriptor
                 descriptor = descriptor.parent
 
         return descriptors
 
     @cached_property
     def _fields_hierarchy(self):
-        u"""Иерархия полей в источнике данных.
+        """Иерархия полей в источнике данных.
 
         :rtype: collections.defaultdict
         """
         hierarchy = defaultdict(list)
 
-        for descriptor in six.itervalues(self._field_descriptors):
+        for descriptor in self._field_descriptors.values():
             if not descriptor.is_root():
                 hierarchy[descriptor.parent.full_accessor_name].append(
                     descriptor
                 )
 
         return hierarchy
 
@@ -349,15 +380,15 @@
         result['is_fake'] = (
             not column_id or column_id in self.ignored_columns_ids
         )
         if full_accessor_name in self._report_columns_by_name:
             result['visible'] = (
                 self._report_columns_by_name[full_accessor_name].visible
             )
-            result['visible_title'] = u'Да' if result['visible'] else u'Нет'
+            result['visible_title'] = 'Да' if result['visible'] else 'Нет'
 
             # "Количество"
             result['by_value'] = column.by_value
             if column.by_value:
                 title = column.get_by_value_display()
             else:
                 title = ''
@@ -374,29 +405,29 @@
         if descriptor.accessor_name in self._report_columns_by_name:
             report_column = self._report_columns_by_name[accessor_name]
             result['overridden_title'] = report_column.title
 
         return result
 
     def get_columns_data(self):
-        u"""Возвращает параметры столбцов шаблона."""
+        """Возвращает параметры столбцов шаблона."""
         return tuple(
             self._get_descriptor_data(descriptor)
-            for descriptor in six.itervalues(self._field_descriptors)
+            for descriptor in self._field_descriptors.values()
             if descriptor.is_root()
         )
 
     _OPERATOR_MAP = {
         ReportFilterGroup.OPERATOR_AND: 'AND',
         ReportFilterGroup.OPERATOR_OR: 'OR',
     }
 
     @cached_property
     def _filter_groups(self):
-        u"""Группы фильтров.
+        """Группы фильтров.
 
         :rtype: collections.OrderedDict
         """
         tree_manager = getattr(ReportFilterGroup, '_tree_manager')
         filter_groups_query = tree_manager.get_queryset_descendants(
             self.report_template.filter_groups.exclude(
                 filters__column_id__in=self.ignored_columns_ids
@@ -406,15 +437,15 @@
 
         return OrderedDict(
             (filter_group.pk, filter_group)
             for filter_group in filter_groups_query
         )
 
     def _get_filter_data(self, report_filter):
-        u"""Возвращает параметры фильтра.
+        """Возвращает параметры фильтра.
 
         :rtype: dict
         """
         column = self._report_columns_by_id[report_filter.column_id]
 
         return dict(
            column=column.name,
@@ -423,21 +454,21 @@
            exclude=report_filter.exclude,
            case_sensitive=report_filter.case_sensitive,
            values=report_filter.values or [],
            comment=report_filter.comment,
         )
 
     def _get_filter_group_data(self, filter_group):
-        u"""Возвращает парамеры группы фильтров.
+        """Возвращает парамеры группы фильтров.
 
         :rtype: dict
         """
         nested_groups = (
             nested_group
-            for nested_group in six.itervalues(self._filter_groups)
+            for nested_group in self._filter_groups.values()
             if nested_group.parent_id == filter_group.pk
         )
 
         return {
             self._OPERATOR_MAP[filter_group.operator]: tuple(
                 (
                     self._get_filter_group_data(obj)
@@ -445,15 +476,15 @@
                     self._get_filter_data(obj)
                 )
                 for obj in chain(nested_groups, filter_group.filters.all())
             )
         }
 
     def get_filters_data(self):
-        u"""Возвращает параметры фильтров.
+        """Возвращает параметры фильтров.
 
         Т.к. в БД фильтры хранятся в виде дерева (синтаксическое дерево), а в
         окне редактирования фильтры организованы в виде плоского списка (так
         сделано из-за того, что на этапе анализа было решено делать фильтры
         в виде плоского списка, но позднее появилось понимание того, что должно
         быть дерево, но чтобы не тратить время на переработку окна
         редактирования, решили в UI сделать ограниченный функционал, а на
@@ -467,21 +498,21 @@
                {
                    'AND': (
                        {
                            'OR': (
                                {
                                    'column': 'group.unit.short_name',
                                    'operator': 3,
-                                   'value': u'СДЮШОР1',
+                                   'value': 'СДЮШОР1',
                                    ...
                                },
                                {
                                    'column': 'group.unit.short_name',
                                    'operator': 3,
-                                   'value': u'СДЮШОР2',
+                                   'value': 'СДЮШОР2',
                                    ...
                                },
                            ),
                        {
                            'column': 'person.date_of_birth',
                            'operator': 6,
                            'value': '01.01.2016',
@@ -500,21 +531,21 @@
         Но поскольку в окне фильтры организованы в плоский список, ожидается,
         что иерархия фильтров будет только одноуровневой.
 
         :rtype: tuple
         """
         return tuple(
             self._get_filter_group_data(filter_group)
-            for filter_group in six.itervalues(self._filter_groups)
+            for filter_group in self._filter_groups.values()
             if filter_group.parent_id is None
         )
 
     @cached_property
     def _sorting_params_by_column_name(self):
-        u"""Параметры сортировки.
+        """Параметры сортировки.
 
         :rtype: tuple
         """
         result = tuple(
             ReportSorting.objects.filter(
                 column__report_template=self.report_template
             ).exclude(
@@ -525,38 +556,37 @@
         for sorting_params in result:
             column_id = sorting_params.column_id
             sorting_params.column = self._report_columns_by_id[column_id]
 
         return result
 
     def _get_sorting_data(self, report_sorting):
-        u"""Возвращает парамеры сортировки в пригодном для сериализации виде.
+        """Возвращает парамеры сортировки в пригодном для сериализации виде.
 
         :rtype: dict
         """
         return dict(
             column=report_sorting.column.name,
             direction=report_sorting.direction,
         )
 
     def get_sorting_data(self):
-        u"""Возвращает параметры сортировки."""
+        """Возвращает параметры сортировки."""
         return tuple(
             self._get_sorting_data(sorting_params)
             for sorting_params in self._sorting_params_by_column_name
         )
 
 
-class ReportTemplateWriter(object):
-
-    u"""Класс, сохраняющий в БД данные шаблона отчета."""
+class ReportTemplateWriter:
+    """Класс, сохраняющий в БД данные шаблона отчета."""
 
     def __init__(self, report_template, columns_data, filters_data,
                  sorting_data):
-        u"""Инициализация экземпляра класса.
+        """Инициализация экземпляра класса.
 
         :param report_template: Шаблон отчета
         :type report_template:
             educommon.report.constructor.models.ReportTemplate
 
         :param list columns_data: Параметры столбцов, полученные в
             HTTP-запросе из окна редактирования шаблона.
@@ -576,32 +606,32 @@
 
         self.errors = []
 
         self._column_descriptors = OrderedDict()
         self._report_columns = {}
 
     def _is_report_template_valid(self, report_template):
-        u"""Возвращает True, если шаблон отчета корректный.
+        """Возвращает True, если шаблон отчета корректный.
 
         Перечень проверок:
 
             1. Источник данных зарегистрирован в Системе.
 
         :rtype: bool
         """
         if report_template.data_source_name not in registry:
             self.errors.append(
-                u'Источник данных "{}" не существует.'
+                'Источник данных "{}" не существует.'
                 .format(report_template.data_source_name)
             )
 
         return not self.errors
 
     def _is_columns_data_valid(self, columns_data):
-        u"""Возвращает True, если параметры столбцов корректны.
+        """Возвращает True, если параметры столбцов корректны.
 
         Перечень проверок:
 
             1. В источнике данных шаблона отчета должны быть все столбцы
                шаблона.
 
         :rtype: bool
@@ -611,56 +641,56 @@
 
         data_source = registry.get(
             self._report_template.data_source_name
         ).get_data_source_descriptor()
 
         for column_params in columns_data:
             if 'accessor_name' not in column_params:
-                self.errors.append(u'Колонки отчета заданы неверно.')
+                self.errors.append('Колонки отчета заданы неверно.')
                 break
 
             full_accessor_name = column_params['accessor_name']
             if full_accessor_name in self._column_descriptors:
                 self.errors.append(
-                    u'Колонка {} указана более одного раза.'
+                    'Колонка {} указана более одного раза.'
                     .format(full_accessor_name)
                 )
             else:
                 try:
                     column_descriptor = data_source.get_column_descriptor(
                         full_accessor_name
                     )
                 except FieldDoesNotExist:
                     self.errors.append(
-                        u'Колонки "{}" нет в источнике данных "{}".'
+                        'Колонки "{}" нет в источнике данных "{}".'
                         .format(full_accessor_name, data_source.title)
                     )
                 else:
                     self._column_descriptors[full_accessor_name] = (
                         column_descriptor
                     )
 
         if not any(
             column_params.get('visible', False)
             for column_params in columns_data
         ):
-            self.errors.append(u'В отчете нет ни одного видимого столбца.')
+            self.errors.append('В отчете нет ни одного видимого столбца.')
         # ---------------------------------------------------------------------
 
         return not self.errors
 
     def _is_filters_data_valid(self, filters_data):
-        u"""Возвращает True, если параметры фильтров корректны.
+        """Возвращает True, если параметры фильтров корректны.
 
         :rtype: bool
         """
         if not isinstance(filters_data, dict):
             return False
 
-        for operator, filters in six.iteritems(filters_data):
+        for operator, filters in filters_data.values():
             if operator not in ('AND', 'OR'):
                 return False
 
             for filter_params in filters:
                 if not isinstance(filter_params, dict):
                     return False
 
@@ -689,15 +719,15 @@
                     )
                 ):
                     return False
 
         return True
 
     def _is_sorting_data_valid(self, sorting_data):
-        u"""Возвращает True, если параметры сортировки корректны.
+        """Возвращает True, если параметры сортировки корректны.
 
         :rtype: bool
         """
         if not isinstance(sorting_data, list):
             return False
 
         for sorting_params in sorting_data:
@@ -711,45 +741,45 @@
                 for param_name in param_names
             ):
                 return False
 
         return True
 
     def validate(self):
-        u"""Выполняет проверку параметров отчета перед его сохранением.
+        """Выполняет проверку параметров отчета перед его сохранением.
 
         :raises objectpack.exceptions.ValidationError: если во время проверки
             найдены ошибки.
         """
         if not self._is_report_template_valid(self._report_template):
             raise ValidationError(
-                u'Параметры шаблона указаны некорректно.'
+                'Параметры шаблона указаны некорректно.'
             )
         if not self._is_columns_data_valid(self._columns_data):
             raise ValidationError(
-                u'Параметры столбцов указаны некорректно.'
+                'Параметры столбцов указаны некорректно.'
             )
         if not self._is_filters_data_valid(self._filters_data):
             raise ValidationError(
-                u'Параметры фильтров указаны некорректно.'
+                'Параметры фильтров указаны некорректно.'
             )
         if not self._is_sorting_data_valid(self._sorting_data):
             raise ValidationError(
-                u'Параметры сортировки указаны некорректно.'
+                'Параметры сортировки указаны некорректно.'
             )
 
     def _write_template(self):
-        u"""Сохранение в БД шаблона отчета."""
+        """Сохранение в БД шаблона отчета."""
         self._report_template.clean_and_save()
 
     def _write_columns(self):
-        u"""Сохранение в БД столбцов."""
+        """Сохранение в БД столбцов."""
         column_descriptor_names = set(
             column_descriptor.full_accessor_name
-            for column_descriptor in six.itervalues(self._column_descriptors)
+            for column_descriptor in self._column_descriptors.values()
         )
 
         columns_query = self._report_template.columns.order_by('index')
         report_columns = OrderedDict(
             (report_column.name, report_column)
             for report_column in columns_query
         )
@@ -764,15 +794,15 @@
         for accessor_name in set(report_columns) - column_descriptor_names:
             report_column = report_columns.pop(accessor_name)
             report_column.delete()
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
         created_report_columns = []
         for index, column_descriptor in enumerate(
-            six.itervalues(self._column_descriptors), 1
+            self._column_descriptors.values(), 1
         ):
             report_column = report_columns.get(
                 column_descriptor.full_accessor_name
             )
 
             column_data = columns_data[column_descriptor.full_accessor_name]
             visible = column_data.get('visible', False)
@@ -807,21 +837,21 @@
                 report_column.by_value = by_value
                 report_column.total = total
 
                 report_column.clean_and_save()
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         # Сохранение столбцов для дальнейшего использования.
 
-        for report_column in chain(six.itervalues(report_columns),
+        for report_column in chain(report_columns.values(),
                                    created_report_columns):
             self._report_columns[report_column.name] = report_column
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def _write_filter_group(self, parent_group, operator, filters):
-        u"""Сохранение в БД групп фильтров."""
+        """Сохранение в БД групп фильтров."""
         report_filter_group = ReportFilterGroup(
             report_template=self._report_template,
             parent=parent_group,
             operator=operator,
         )
         report_filter_group.clean_and_save()
 
@@ -852,32 +882,32 @@
                     exclude=filter_params.get('exclude', False),
                     case_sensitive=filter_params.get('case_sensitive'),
                     values=filter_params['values'],
                     comment=filter_params.get('comment'),
                 )
 
     def _write_filters(self):
-        u"""Сохранение в БД фильтров."""
+        """Сохранение в БД фильтров."""
         # Чтобы не разбираться с имеющимся деревом фильтров, удалим его и
         # создадим заново.
 
         self._report_template.filter_groups.all().delete()
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
-        for operator, filters in six.iteritems(self._filters_data):
+        for operator, filters in self._filters_data.items():
             if operator == 'OR':
                 operator = ReportFilterGroup.OPERATOR_OR
             else:
                 operator = ReportFilterGroup.OPERATOR_AND
 
             self._write_filter_group(None, operator, filters)
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def _write_sorting(self):
-        u"""Сохранение в БД параметров сортировки."""
+        """Сохранение в БД параметров сортировки."""
         sorting_params = chain(self._sorting_data, repeat(None))
         sorting_objs = chain(
             ReportSorting.objects.filter(
                 column__report_template=self._report_template,
             ).order_by('index'),
             repeat(None),
         )
@@ -899,24 +929,23 @@
                 obj.delete()
             else:
                 break
 
     @convert_validation_error_to(ValidationError)
     @atomic
     def write(self):
-        u"""Сохранение в БД данных шаблона отчета."""
+        """Сохранение в БД данных шаблона отчета."""
         self._write_template()
         self._write_columns()
         self._write_filters()
         self._write_sorting()
 
 
 class Pack(PackValidationMixin, ObjectPack):
-
-    u"""Пак реестра шаблонов отчетов."""
+    """Пак реестра шаблонов отчетов."""
 
     model = ReportTemplate
     _is_primary_for_model = False
 
     columns = (
         dict(
             data_index='title',
@@ -953,15 +982,15 @@
         return obj
 
     def declare_context(self, action):
         result = super(Pack, self).declare_context(action)
 
         if action is self.save_action:
             result.update(
-                title=dict(type='unicode'),
+                title=dict(type='str'),
                 data_source_name=dict(type='str'),
                 columns=dict(type='json'),
                 filters=dict(type='json', default={}),
                 sorting=dict(type='json', default={}),
             )
 
         return result
@@ -1011,17 +1040,17 @@
             filters_data=context.filters,
             sorting_data=context.sorting,
         )
 
         try:
             writer.validate()
         except ValidationError as error:
-            raise ValidationError(u'\n'.join((
-                six.text_type(error),
-                u'\n'.join(writer.errors)
+            raise ValidationError('\n'.join((
+                str(error),
+                '\n'.join(writer.errors)
             )))
 
         writer.write()
 
     @atomic
     def delete_row(self, obj_id, request, context):
         for report_sorting in ReportSorting.objects.filter(
@@ -1044,13 +1073,13 @@
         ).iterator():
             report_column.safe_delete()
 
         super(Pack, self).delete_row(obj_id, request, context)
 
     def extend_menu(self, menu):
         return menu.SubMenu(
-            u'Отчеты',
+            'Отчеты',
             menu.SubMenu(
-                u'Конструктор отчетов',
-                menu.Item(u'Редактор шаблонов', self.list_window_action),
+                'Конструктор отчетов',
+                menu.Item('Редактор шаблонов', self.list_window_action),
             )
         )
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/editor/edit-window.js` & `educommon-3.0.0/src/educommon/report/constructor/editor/edit-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/report/constructor/editor/list-window.js` & `educommon-3.0.0/src/educommon/report/constructor/editor/list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/report/constructor/editor/ui.py` & `educommon-3.0.0/src/educommon/report/constructor/editor/ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,80 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from m3_ext.ui.containers import ExtContextMenu
-from m3_ext.ui.containers import ExtContextMenuItem
-from m3_ext.ui.containers.container_complex import ExtContainerTable
-from m3_ext.ui.containers.containers import ExtContainer
-from m3_ext.ui.containers.containers import ExtToolBar
-from m3_ext.ui.containers.containers import ExtToolbarMenu
-from m3_ext.ui.containers.forms import ExtFieldSet
-from m3_ext.ui.containers.grids import ExtGrid
-from m3_ext.ui.containers.trees import ExtTree
-from m3_ext.ui.controls.buttons import ExtButton
-from m3_ext.ui.fields.simple import ExtCheckBox
-from m3_ext.ui.fields.simple import ExtStringField
-from m3_ext.ui.fields.simple import ExtTextArea
-from m3_ext.ui.misc.store import ExtDataStore
-from objectpack.ui import ColumnsConstructor
-from objectpack.ui import ComboBoxWithStore
-from objectpack.ui import WindowTab
-from objectpack.ui import _create_control_for_field
-from objectpack.ui import make_combo_box
-
-from educommon.objectpack.ui import BaseListWindow
-from educommon.objectpack.ui import TabbedEditWindow
-from educommon.utils.ui import local_template
-
-from .. import constants
-from .. import models
-from ..models import ReportTemplate
+from m3_ext.ui.containers import (
+    ExtContextMenu,
+    ExtContextMenuItem,
+)
+from m3_ext.ui.containers.container_complex import (
+    ExtContainerTable,
+)
+from m3_ext.ui.containers.containers import (
+    ExtContainer,
+    ExtToolBar,
+    ExtToolbarMenu,
+)
+from m3_ext.ui.containers.forms import (
+    ExtFieldSet,
+)
+from m3_ext.ui.containers.grids import (
+    ExtGrid,
+)
+from m3_ext.ui.containers.trees import (
+    ExtTree,
+)
+from m3_ext.ui.controls.buttons import (
+    ExtButton,
+)
+from m3_ext.ui.fields.simple import (
+    ExtCheckBox,
+    ExtStringField,
+    ExtTextArea,
+)
+from m3_ext.ui.misc.store import (
+    ExtDataStore,
+)
+
+from objectpack.ui import (
+    ColumnsConstructor,
+    ComboBoxWithStore,
+    WindowTab,
+    _create_control_for_field,
+    make_combo_box,
+)
+
+from educommon.objectpack.ui import (
+    BaseListWindow,
+    TabbedEditWindow,
+)
+from educommon.report.constructor import (
+    constants,
+    models,
+)
+from educommon.report.constructor.models import (
+    ReportTemplate,
+)
+from educommon.utils.ui import (
+    local_template,
+)
 
 
 # -----------------------------------------------------------------------------
 # Окно просмотра списка шаблонов.
 class ListWindow(BaseListWindow):
-
-    u"""Окно просмотра списка шаблонов отчетов."""
+    """Окно просмотра списка шаблонов отчетов."""
 
     def _init_components(self):
         super(ListWindow, self)._init_components()
 
         self.grid.top_bar.button__build = ExtButton(
-            text=u'Собрать отчет',
+            text='Собрать отчет',
             icon_cls='database_table',
             handler='buildReport',
             disabled=True,
         )
         self.grid.context_menu_row.menuitem__build = ExtContextMenuItem(
-            text=u'Собрать отчет',
+            text='Собрать отчет',
             icon_cls='database_table',
             handler='buildReport',
         )
 
     def _do_layout(self):
         super(ListWindow, self)._do_layout()
 
@@ -66,129 +90,127 @@
 
         self.build_action_url = params['build_action_url']
 # -----------------------------------------------------------------------------
 # Вкладка "Столбцы" окна редактирования шаблона.
 
 
 class AvailableColumnsTree(ExtTree):
-
-    u"""Дерево доступных для использования в отчете столбцов."""
+    """Дерево доступных для использования в отчете столбцов."""
 
     class ToolBar(ExtToolBar):
 
         def __init__(self, *args, **kwargs):
             super(AvailableColumnsTree.ToolBar, self).__init__(*args, **kwargs)
 
             self.button__add = ExtButton(
-                text=u'Добавить в шаблон',
+                text='Добавить в шаблон',
                 icon_cls='add_item',
                 handler='addColumnToReport',
                 disabled=True,
             )
 
             self.items[:] = (
                 self.button__add,
             )
 
     def __init__(self, *args, **kwargs):
         kwargs.update(
-            title=u'Доступные наименования столбцов',
+            title='Доступные наименования столбцов',
             header=True,
             read_only=True,
         )
         super(AvailableColumnsTree, self).__init__(*args, **kwargs)
 
         self.style = {'border-width': '1px'}
 
         ColumnsConstructor.from_config((
             dict(
                 data_index='title',
-                header=u'Наименование',
+                header='Наименование',
                 sortable=False,
             ),
         )).configure_grid(self)
 
         self.top_bar = self.ToolBar()
 
     def set_params(self, params):
         self.available_columns_url = params['available_columns_action_url']
 
 
 class ReportColumnsTree(ExtTree):
-
-    u"""Дерево используемых в шаблоне отчета столбцов."""
+    """Дерево используемых в шаблоне отчета столбцов."""
 
     class ToolBar(ExtToolBar):
 
         def __init__(self, *args, **kwargs):
             super(ReportColumnsTree.ToolBar, self).__init__(*args, **kwargs)
 
             self.button__remove = ExtButton(
-                text=u'Убрать столбец',
+                text='Убрать столбец',
                 icon_cls='delete_item',
                 handler='removeColumnFromReport',
                 disabled=True,
             )
 
             self.button__switch_visibility = ExtButton(
-                text=u'Скрывать',
+                text='Скрывать',
                 icon_cls='report-constructor-switch-visible',
                 handler='switchColumnVisibility',
                 hidden=True,
             )
 
             # Промежуточный итог
             self.button__by_value_count = ExtContextMenuItem(
-                text=u'Количество',
+                text='Количество',
                 icon_cls='icon-report-add',
                 handler='setByValueCountAggregator'
             )
             self.button__by_value_sum = ExtContextMenuItem(
-                text=u'Сумма',
+                text='Сумма',
                 icon_cls='icon-report-add',
                 handler='setByValueSumAggregator'
             )
             self.button__by_value_none = ExtContextMenuItem(
-                text=u'Очистить',
+                text='Очистить',
                 icon_cls='icon-report-delete',
                 handler='setByValueNoneAggregator'
             )
             context_menu__by_value = ExtContextMenu()
             context_menu__by_value.items.extend(
                 (
                     self.button__by_value_count,
                     self.button__by_value_sum,
                     self.button__by_value_none,
                 )
             )
             self.menu__by_value = ExtToolbarMenu(
                 icon_cls="icon-report",
                 menu=context_menu__by_value,
-                text=u'Промежуточный итог',
+                text='Промежуточный итог',
                 hidden=True,
             )
 
             # Итог
             self.button__total_count = ExtContextMenuItem(
-                text=u'Количество',
+                text='Количество',
                 icon_cls='icon-calculator-add',
                 handler='setTotalCountAggregator'
             )
             self.button__total_uniq_count = ExtContextMenuItem(
-                text=u'Количество уникальных',
+                text='Количество уникальных',
                 icon_cls='icon-calculator-add',
                 handler='setTotalCountUniqueAggregator'
             )
             self.button__total_sum = ExtContextMenuItem(
-                text=u'Сумма',
+                text='Сумма',
                 icon_cls='icon-calculator-add',
                 handler='setTotalSumAggregator'
             )
             self.button__total_none = ExtContextMenuItem(
-                text=u'Очистить',
+                text='Очистить',
                 icon_cls='icon-calculator-delete',
                 handler='setTotalNoneAggregator'
             )
             context_menu__total = ExtContextMenu()
             context_menu__total.items.extend(
                 (
                     self.button__total_count,
@@ -196,88 +218,87 @@
                     self.button__total_sum,
                     self.button__total_none,
                 )
             )
             self.menu__total = ExtToolbarMenu(
                 icon_cls="icon-calculator",
                 menu=context_menu__total,
-                text=u'Итог',
+                text='Итог',
                 hidden=True,
             )
 
             self.items[:] = (
                 self.button__remove,
                 self.button__switch_visibility,
                 self.menu__by_value,
                 self.menu__total,
             )
 
     def __init__(self, *args, **kwargs):
         kwargs.update(
-            title=u'Столбцы в отчете',
+            title='Столбцы в отчете',
             header=True,
         )
         super(ReportColumnsTree, self).__init__(*args, **kwargs)
 
         self.enable_sort = False
 
         self.style = {'border-width': '1px'}
 
         ColumnsConstructor.from_config((
             dict(
                 data_index='title',
-                header=u'Наименование',
+                header='Наименование',
                 sortable=False,
             ),
             dict(
                 data_index='visible',
                 hidden=True
             ),
             dict(
                 data_index='visible_title',
-                header=u'Отображать',
+                header='Отображать',
                 sortable=False,
                 width=20,
                 fixed=True,
             ),
             dict(
                 data_index='by_value',
                 hidden=True
             ),
             dict(
                 data_index='by_value_title',
-                header=u'Промежуточный итог',
+                header='Промежуточный итог',
                 sortable=False,
                 width=20,
                 fixed=True,
             ),
             dict(
                 data_index='total',
                 hidden=True,
             ),
             dict(
                 data_index='total_title',
-                header=u'Итог',
+                header='Итог',
                 sortable=False,
                 width=20,
                 fixed=True,
             ),
         )).configure_grid(self)
 
         self.top_bar = self.ToolBar()
 
     def set_params(self, params):
         pass
 
 
 class ColumnsTab(WindowTab):
+    """Вкладка "Колонки" окна редактирования шаблона отчета."""
 
-    u"""Вкладка "Колонки" окна редактирования шаблона отчета."""
-
-    title = u'Столбцы'
+    title = 'Столбцы'
 
     def init_components(self, win):
         super(ColumnsTab, self).init_components(win)
 
         self.grid__available_columns = AvailableColumnsTree()
         self.grid__report_columns = ReportColumnsTree()
         # ---------------------------------------------------------------------
@@ -308,95 +329,93 @@
         self.grid__report_columns.drag_drop = True
         self.grid__report_columns.handler_beforedrop = 'onBeforeDrop'
 # -----------------------------------------------------------------------------
 # Вкладка "Фильтры" окна редактирования шаблона.
 
 
 class OperatorPanel(ExtFieldSet):
-
-    u"""Панель для поля "Оператор" на вкладке "Фильтры"."""
+    """Панель для поля "Оператор" на вкладке "Фильтры"."""
 
     def __init__(self, *args, **kwargs):
         super(OperatorPanel, self).__init__(*args, **kwargs)
 
         self.label_width = 55
         self.style = {
             'border': 0,
             'padding': 0,
         }
 
         self.field__operator = ComboBoxWithStore(
             name='operator',
             display_field='title',
-            label=u'Условие',
+            label='Условие',
             width=70,
         )
         self.field__operator.data = (
-            ('AND', u'И'),
-            ('OR', u'ИЛИ'),
+            ('AND', 'И'),
+            ('OR', 'ИЛИ'),
         )
 
         # Решили временно ограничить возможность выбора оператора, но
         # контрол не убирать.
         self.hidden = True
         self.field__operator.value = 'AND'
 
         self.items[:] = (
             self.field__operator,
         )
 
 
 class FilterParamsPanel(ExtContainerTable):
-
-    u"""Панель ввода параметров фильтра."""
+    """Панель ввода параметров фильтра."""
 
     def __init__(self, *args, **kwargs):
         super(FilterParamsPanel, self).__init__(columns=3, rows=4)
 
-        self.title = u'Параметры фильтра'
+        self.title = 'Параметры фильтра'
         self.style['padding-top'] = '5px'
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         self.field__column = ComboBoxWithStore(
             name='column',
             value_field='name',
             display_field='title',
-            label=u'Столбец',
+            label='Столбец',
         )
 
         self.field__operator = ComboBoxWithStore(
             name='operator',
             display_field='title',
-            label=u'Условие',
+            label='Условие',
             data=(),  # ReportFilter.OPERATOR_CHOICES,
         )
         self.field__operator.store.id_property = (
             self.field__operator.value_field
         )
 
         self.field__exclude = ExtCheckBox(
             name='exclude',
-            label=u'Обратное условие',
+            label='Обратное условие',
             disabled=True,
         )
 
         self.field__case_sensitive = ExtCheckBox(
             name='case_sensitive',
-            label=u'Учет регистра',
+            label='Учет регистра',
             disabled=True,
         )
 
         self.field__value = ExtStringField(
             name='values',
-            label=u'Значение',
+            label='Значение',
             disabled=True,
         )
 
         self.field__comment = ExtTextArea(
             name='comment',
-            label=u'Описание',
+            label='Описание',
             height=35,
             disabled=True,
         )
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
         self.set_item(0, 0, self.field__column, 3)
         self.set_item(1, 0, self.field__operator)
@@ -414,41 +433,39 @@
 
         self.set_rows_height(25)
         self.set_row_height(3, 40)
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
 
 class FiltersGridTopBar(ExtToolBar):
-
-    u"""Верхняя панель грида с параметрами фильтрации."""
+    """Верхняя панель грида с параметрами фильтрации."""
 
     def __init__(self, *args, **kwargs):
         super(FiltersGridTopBar, self).__init__(*args, **kwargs)
 
         self.button__add = ExtButton(
-            text=u'Добавить',
+            text='Добавить',
             icon_cls='add_item',
             handler='addFilter',
         )
         self.button__delete = ExtButton(
-            text=u'Удалить',
+            text='Удалить',
             icon_cls='delete_item',
             handler='deleteFilter',
             disabled=True,
         )
 
         self.items[:] = (
             self.button__add,
             self.button__delete,
         )
 
 
 class FiltersGrid(ExtGrid):
-
-    u"""Грид с параметрами фильтрации данных в отчете."""
+    """Грид с параметрами фильтрации данных в отчете."""
 
     def __init__(self, *args, **kwargs):
         super(FiltersGrid, self).__init__(*args, **kwargs)
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
         self.cls = 'word-wrap-grid'
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -462,54 +479,53 @@
 
         self.add_column(
             data_index='column',
             hidden=True,
         )
         self.add_column(
             data_index='column_title',
-            header=u'Столбец',
+            header='Столбец',
         )
         self.add_column(
             data_index='operator',
             hidden=True,
         )
         self.add_column(
             data_index='operator_title',
-            header=u'Условие',
+            header='Условие',
             width=110,
             fixed=True,
         )
         self.add_check_column(
             data_index='exclude',
-            header=u'Обратное условие',
+            header='Обратное условие',
             width=90,
             fixed=True,
         )
         self.add_check_column(
             data_index='case_sensitive',
-            header=u'Учет регистра',
+            header='Учет регистра',
             width=85,
             fixed=True,
         )
         self.add_column(
             data_index='values',
-            header=u'Значение',
+            header='Значение',
         )
         self.add_column(
             data_index='comment',
-            header=u'Описание',
+            header='Описание',
         )
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
 
 class FiltersTab(WindowTab):
+    """Вкладка "Фильтры" окна редактирования шаблона отчета."""
 
-    u"""Вкладка "Фильтры" окна редактирования шаблона отчета."""
-
-    title = u'Фильтры'
+    title = 'Фильтры'
 
     def init_components(self, win):
         super(FiltersTab, self).init_components(win)
 
         self.panel__operator = OperatorPanel()
         self.panel__filter_params = FilterParamsPanel()
         self.grid__filters = FiltersGrid()
@@ -534,27 +550,26 @@
         self.panel__filter_params.height = 120
         self.grid__filters.flex = 1
 # -----------------------------------------------------------------------------
 # Вкладка "Сортировка" окна редактирования шаблона.
 
 
 class SortingGridTopBar(ExtToolBar):
-
-    u"""Верхняя панель грида с параметрами сортировки."""
+    """Верхняя панель грида с параметрами сортировки."""
 
     def __init__(self, *args, **kwargs):
         super(SortingGridTopBar, self).__init__(*args, **kwargs)
 
         self.button__add = ExtButton(
-            text=u'Добавить',
+            text='Добавить',
             icon_cls='add_item',
             handler='addSort',
         )
         self.button__delete = ExtButton(
-            text=u'Удалить',
+            text='Удалить',
             icon_cls='delete_item',
             handler='deleteSort',
             disabled=True,
         )
 
         self.button__move_up = ExtButton(
             icon_cls='report-constructor-arrow-up',
@@ -572,16 +587,15 @@
             self.button__delete,
             self.button__move_up,
             self.button__move_down,
         )
 
 
 class SortingGrid(ExtGrid):
-
-    u"""Грид для отображения параметров сортировки."""
+    """Грид для отображения параметров сортировки."""
 
     def __init__(self, *args, **kwargs):
         super(SortingGrid, self).__init__(*args, **kwargs)
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
         self.cls = 'word-wrap-grid'
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -595,53 +609,52 @@
 
         self.add_column(
             data_index='column',
             hidden=True,
         )
         self.add_column(
             data_index='column_title',
-            header=u'Столбец',
+            header='Столбец',
             width=1,
         )
         self.add_column(
             data_index='direction',
             hidden=True,
         )
         self.add_column(
             data_index='direction_title',
-            header=u'Направление сортировки',
+            header='Направление сортировки',
             width=150,
             fixed=True,
         )
 
 
 class SortingParamsPanel(ExtFieldSet):
-
-    u"""Панель ввода параметров сортировки."""
+    """Панель ввода параметров сортировки."""
 
     def __init__(self, *args, **kwargs):
         super(SortingParamsPanel, self).__init__(*args, **kwargs)
 
-        self.title = u'Параметры сортировки'
+        self.title = 'Параметры сортировки'
         self.label_width = 150
         self.style['padding'] = '5px'
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
         self.field__column = ComboBoxWithStore(
             name='column',
             value_field='name',
             display_field='title',
-            label=u'Столбец',
+            label='Столбец',
             anchor='100%',
         )
 
         self.field__direction = ComboBoxWithStore(
             name='direction',
             display_field='title',
-            label=u'Направление сортировки',
+            label='Направление сортировки',
             data=constants.DIRECTION_CHOICES,
             anchor='100%',
         )
         self.field__direction.store.id_property = (
             self.field__direction.value_field
         )
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -649,18 +662,17 @@
         self.items[:] = (
             self.field__column,
             self.field__direction,
         )
 
 
 class SortingTab(WindowTab):
+    """Вкладка "Сортировка" окна редактирования шаблона отчета."""
 
-    u"""Вкладка "Сортировка" окна редактирования шаблона отчета."""
-
-    title = u'Сортировка'
+    title = 'Сортировка'
 
     def init_components(self, win):
         super(SortingTab, self).init_components(win)
 
         self.grid__sorting = SortingGrid()
         self.panel__sorting_params = SortingParamsPanel()
 
@@ -681,16 +693,15 @@
         self.grid__sorting.flex = 1
         self.panel__sorting_params.flex = 0
         self.panel__sorting_params.height = 80
 # -----------------------------------------------------------------------------
 
 
 class EditWindow(TabbedEditWindow):
-
-    u"""Окно добавления/редактирования шаблона отчета."""
+    """Окно добавления/редактирования шаблона отчета."""
 
     tabs = (
         ColumnsTab,
         FiltersTab,
         SortingTab,
     )
 
@@ -703,15 +714,15 @@
         self.field__title = _create_control_for_field(
             getattr(ReportTemplate, '_meta').get_field('title'),
             allow_blank=False,
             anchor='100%',
         )
         self.field__data_source_name = make_combo_box(
             name='data_source_name',
-            label=u'Источник данных',
+            label='Источник данных',
             display_field='title',
             value_field='name',
             allow_blank=False,
             anchor='100%',
         )
         self.field__format = _create_control_for_field(
             getattr(ReportTemplate, '_meta').get_field('format'),
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/exceptions.py` & `educommon-3.0.0/src/educommon/report/constructor/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-
 class ReportConstructorException(Exception):
-
-    u"""Базовый класс для исключений конструктора отчетов."""
+    """Базовый класс для исключений конструктора отчетов."""
 
 
 class DataSourceParamsNotFound(ReportConstructorException):
-    u"""Исключение при отсутствии в реестре параметров источника данных."""
+    """Исключение при отсутствии в реестре параметров источника данных."""
 
     def __init__(self, data_source_name):
         self.data_source_name = data_source_name
 
         super(DataSourceParamsNotFound, self).__init__(
-            u'"Параметры для источника данных с именем "{}" не '
-            u'зарегистрированы в системе.'.format(self.data_source_name.name)
+            '"Параметры для источника данных с именем "{}" не '
+            'зарегистрированы в системе.'.format(self.data_source_name.name)
         )
 
 
 class FilterError(ReportConstructorException):
-
-    u"""Ошибка в фильтре."""
+    """Ошибка в фильтре."""
 
     def __init__(self, report_filter, message):
         self.report_filter = report_filter
 
         if not message:
             message = (
-                u'Ошибка в фильтре для столбца {}'
+                'Ошибка в фильтре для столбца {}'
                 .format(self.report_filter.column.title)
             )
 
         super(FilterError, self).__init__(
-            u'Ошибка в фильтре для столбца {}: {}'.format(
+            'Ошибка в фильтре для столбца {}: {}'.format(
                 self.report_filter.column.title, message
             )
         )
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/migrations/0001_initial.py` & `educommon-3.0.0/src/educommon/report/constructor/migrations/0001_initial.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# coding: utf-8
 # Generated by Django 1.10.4 on 2016-12-27 11:37
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
 import django.db.models.deletion
+from django.db import (
+    migrations,
+    models,
+)
 
 import educommon.m3.extensions.listeners.delete_check.mixins
 import educommon.report.constructor.validators
 
 
 class Migration(migrations.Migration):
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/migrations/0002_report_filters.py` & `educommon-3.0.0/src/educommon/report/constructor/migrations/0002_report_filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# coding: utf-8
 # Generated by Django 1.10.5 on 2017-02-07 10:16
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
 import django.contrib.postgres.fields
 import django.db.models.deletion
 import mptt.fields
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [('report_constructor', '0001_initial'), ]
 
     operations = [
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py` & `educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
-import django.contrib.postgres.fields
+import django.db.models.deletion
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
-    dependencies = [('report_constructor', '0003_reportfilter_exclude'), ]
+    dependencies = [
+        ('contenttypes', '0002_remove_content_type_name'),
+        ('contingent_plugin', '0001_initial'),
+    ]
 
     operations = [
-        migrations.AlterField(
-            model_name='reportfilter',
-            name='operator',
-            field=models.PositiveSmallIntegerField(
-                choices=[(1, 'Меньше или равно'),
-                         (2, 'Меньше'),
-                         (3, 'Равно'),
-                         (4, 'Больше'),
-                         (5, 'Больше или равно'),
-                         (6, 'Пусто'),
-                         (7, 'Содержит'),
-                         (8, 'Начинается с'),
-                         (9, 'Заканчивается на'),
-                         (10, 'Между'),
-                         (11, 'Равно одному из')],
-                verbose_name='Оператор сравнения'), ),
-        migrations.AlterField(
-            model_name='reportfilter',
-            name='values',
-            field=django.contrib.postgres.fields.ArrayField(
-                base_field=models.TextField(verbose_name='Значение'),
-                blank=True,
-                null=True,
-                size=None), ),
+        migrations.CreateModel(
+            name='ContingentModelDeleted',
+            fields=[
+                ('id',
+                 models.AutoField(auto_created=True,
+                                  primary_key=True,
+                                  serialize=False,
+                                  verbose_name='ID')),
+                ('object_id', models.PositiveIntegerField()),
+                ('data',
+                 models.TextField(verbose_name='Данные об удалённом объекте')),
+                ('content_type',
+                 models.ForeignKey(on_delete=django.db.models.deletion.CASCADE,
+                                   to='contenttypes.ContentType')),
+            ],
+        ),
+        migrations.AlterUniqueTogether(
+            name='contingentmodeldeleted',
+            unique_together=set([('content_type', 'object_id')]),
+        ),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/migrations/0006_reportsorting.py` & `educommon-3.0.0/src/educommon/report/constructor/migrations/0007_include_available_units.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,44 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
+import django.contrib.postgres.fields
 import django.db.models.deletion
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
-    dependencies = [('report_constructor', '0005_reportcolumn_visible'), ]
+    dependencies = [('report_constructor', '0006_reportsorting'), ]
 
     operations = [
-        migrations.CreateModel(
-            name='ReportSorting',
-            fields=[
-                ('id', models.AutoField(
-                    auto_created=True,
-                    primary_key=True,
-                    serialize=False,
-                    verbose_name='ID')),
-                ('direction', models.PositiveSmallIntegerField(
-                    choices=[(1, 'По возрастанию'), (2, 'По убыванию')],
-                    verbose_name='Направление сортировки')),
-                ('index', models.PositiveSmallIntegerField(
-                    verbose_name='Порядковый номер')),
-                ('column', models.OneToOneField(
-                    on_delete=django.db.models.deletion.CASCADE,
-                    to='report_constructor.ReportColumn',
-                    verbose_name='Колонка')),
-            ],
+        migrations.AlterModelOptions(
+            name='reportsorting',
             options={
+                'ordering': ('index', ),
                 'verbose_name': 'Сортировка',
-                'verbose_name_plural': 'Сортировка',
+                'verbose_name_plural': 'Сортировка'
             }, ),
+        migrations.AddField(
+            model_name='reporttemplate',
+            name='include_available_units',
+            field=models.BooleanField(
+                default=False,
+                verbose_name='Отображать данные по дочерним учреждениям'), ),
+        migrations.AlterField(
+            model_name='reportfilter',
+            name='values',
+            field=django.contrib.postgres.fields.ArrayField(
+                base_field=models.TextField(
+                    blank=True, null=True, verbose_name='Значение'),
+                blank=True,
+                null=True,
+                size=None), ),
+        migrations.AlterField(
+            model_name='reportsorting',
+            name='column',
+            field=models.OneToOneField(
+                on_delete=django.db.models.deletion.CASCADE,
+                related_name='sorting',
+                to='report_constructor.ReportColumn',
+                verbose_name='Колонка'), ),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/migrations/0007_include_available_units.py` & `educommon-3.0.0/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
+import datetime
 
-from django.db import migrations
-from django.db import models
-import django.contrib.postgres.fields
-import django.db.models.deletion
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
-    dependencies = [('report_constructor', '0006_reportsorting'), ]
+    dependencies = [
+        ('ws_log', '0004_auto_20160727_1600'),
+    ]
 
     operations = [
-        migrations.AlterModelOptions(
-            name='reportsorting',
-            options={
-                'ordering': ('index', ),
-                'verbose_name': 'Сортировка',
-                'verbose_name_plural': 'Сортировка'
-            }, ),
-        migrations.AddField(
-            model_name='reporttemplate',
-            name='include_available_units',
-            field=models.BooleanField(
-                default=False,
-                verbose_name='Отображать данные по дочерним учреждениям'), ),
         migrations.AlterField(
-            model_name='reportfilter',
-            name='values',
-            field=django.contrib.postgres.fields.ArrayField(
-                base_field=models.TextField(
-                    blank=True, null=True, verbose_name='Значение'),
-                blank=True,
-                null=True,
-                size=None), ),
+            model_name='smevlog',
+            name='consumer_type',
+            field=models.PositiveSmallIntegerField(blank=True, choices=[(0, 'Юридическое лицо'), (1, 'Физическое лицо')], default=1, null=True, verbose_name='Потребитель сервиса'),
+        ),
+        migrations.AlterField(
+            model_name='smevlog',
+            name='result',
+            field=models.TextField(blank=True, null=True, verbose_name='Результат'),
+        ),
+        migrations.AlterField(
+            model_name='smevlog',
+            name='target_name',
+            field=models.CharField(blank=True, max_length=100, null=True, verbose_name='Наименование электронного сервиса'),
+        ),
+        migrations.AlterField(
+            model_name='smevlog',
+            name='time',
+            field=models.DateTimeField(db_index=True, default=datetime.datetime.now, verbose_name='Время СМЭВ запроса'),
+        ),
         migrations.AlterField(
-            model_name='reportsorting',
-            name='column',
-            field=models.OneToOneField(
-                on_delete=django.db.models.deletion.CASCADE,
-                related_name='sorting',
-                to='report_constructor.ReportColumn',
-                verbose_name='Колонка'), ),
+            model_name='smevprovider',
+            name='source',
+            field=models.PositiveSmallIntegerField(choices=[(0, 'ЕПГУ'), (1, 'РПГУ'), (2, 'Межведомственное взаимодействие')], verbose_name='Источник взаимодействия'),
+        ),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py` & `educommon-3.0.0/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
+from django.db import (
+    migrations,
+)
 
 
 def delete_reports(apps, schema_editor):
-    u"""Удаляет отчеты с несуществующими источниками данных."""
+    """Удаляет отчеты с несуществующими источниками данных."""
     ReportTemplate = apps.get_model('report_constructor', 'ReportTemplate')
     ReportTemplate.objects.filter(
-        data_source_name__in=(u'unit.Unit', u'person.Person')
+        data_source_name__in=('unit.Unit', 'person.Person')
     ).delete()
 
 
 class Migration(migrations.Migration):
 
     dependencies = [('report_constructor', '0007_include_available_units'), ]
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py` & `educommon-3.0.0/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# coding: utf-8
-from django.db import migrations
-from django.db import models
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('report_constructor', '0009_auto_20180405_0642'),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/mixins.py` & `educommon-3.0.0/src/educommon/report/constructor/mixins.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from importlib import import_module
-from uuid import uuid4
 import os
-
-from django.conf import settings
-from django.utils.text import slugify
-import six
-
-from educommon.report.constructor.models import ReportTemplate
+from importlib import (
+    import_module,
+)
+from uuid import (
+    uuid4,
+)
+
+from django.conf import (
+    settings,
+)
+from django.utils.text import (
+    slugify,
+)
+
+from educommon.report.constructor.models import (
+    ReportTemplate,
+)
 
 
 _BUILDERS_PACKAGE = 'educommon.report.constructor.builders'
 
 
-class BuildReportTaskMixin(object):
+class BuildReportTaskMixin:
 
     _builders = {
         ReportTemplate.EXCEL_SIMPLE:
             _BUILDERS_PACKAGE + '.excel.product.ReportBuilder',
         ReportTemplate.EXCEL_MERGED:
             _BUILDERS_PACKAGE + '.excel.with_merged_cells.ReportBuilder',
     }
@@ -32,37 +38,37 @@
 
         builder_name = self._builders[report_format]
         module_name, _, class_name = builder_name.rpartition('.')
         module = import_module(module_name)
         return getattr(module, class_name)
 
     def make_report(self, *args, **kwargs):
-        u"""Совершает сборку отчета."""
+        """Совершает сборку отчета."""
         result = dict()
         report_template_id = kwargs['report_template_id']
         report_template = ReportTemplate.objects.get(pk=report_template_id)
         reports_dir = os.path.join(settings.MEDIA_ROOT, 'report_constructor')
         if not os.path.exists(reports_dir):
             os.mkdir(reports_dir)
         while True:
-            report_id = six.text_type(uuid4().hex)
+            report_id = str(uuid4().hex)
             report_dir = os.path.join(reports_dir, report_id)
             if not os.path.exists(report_dir):
                 os.mkdir(report_dir)
                 break
         file_name = (
-            slugify(report_template.title, allow_unicode=True) + u'.xlsx'
+            slugify(report_template.title, allow_unicode=True) + '.xlsx'
         )
         file_path = os.path.join(report_dir, file_name)
         builder_class = self._get_builder(report_template, kwargs['format'])
         user = kwargs['content_type'].get_object_for_this_type(
             id=kwargs['object_id']
         )
         builder = builder_class(report_template, file_path, user)
         builder.build()
         link = os.path.join(
-            settings.MEDIA_URL, u'report_constructor', report_id, file_name
+            settings.MEDIA_URL, 'report_constructor', report_id, file_name
         )
-        download_link = u'<a href="{}" target="_blank" download>{}</a>'.format(
+        download_link = '<a href="{}" target="_blank" download>{}</a>'.format(
             link, file_name)
         result['download_link'] = download_link
         return result
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/models.py` & `educommon-3.0.0/src/educommon/report/constructor/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,162 +1,177 @@
-# coding: utf-8
-from __future__ import absolute_import
+from django.contrib.postgres.fields.array import (
+    ArrayField,
+)
+from django.db import (
+    models,
+)
+from mptt.models import (
+    MPTTModel,
+    TreeForeignKey,
+)
+
+from objectpack.exceptions import (
+    ValidationError,
+)
+
+from educommon.django.db.mixins.validation import (
+    post_clean,
+)
+from educommon.django.db.models import (
+    BaseModel,
+)
+from educommon.m3.extensions.listeners.delete_check.mixins import (
+    CascadeDeleteMixin,
+)
+from educommon.report.constructor import (
+    constants,
+)
+from educommon.report.constructor.registries import (
+    registry,
+)
+from educommon.report.constructor.validators import (
+    validate_data_source_name,
+)
+from educommon.utils.misc import (
+    cached_property,
+)
 
-from django.contrib.postgres.fields.array import ArrayField
-from django.db import models
-from mptt.models import MPTTModel
-from mptt.models import TreeForeignKey
-from objectpack.exceptions import ValidationError
-
-from educommon.django.db.mixins.validation import post_clean
-from educommon.django.db.models import BaseModel
-from educommon.m3.extensions.listeners.delete_check.mixins import \
-    CascadeDeleteMixin
-from educommon.utils.misc import cached_property
-
-from . import constants
-from .registries import registry
-from .validators import validate_data_source_name
 
-
-# -----------------------------------------------------------------------------
 class ReportTemplate(CascadeDeleteMixin, BaseModel):
-
-    u"""Модель "Шаблон отчета"."""
+    """Модель "Шаблон отчета"."""
 
     USER_DEFINED = constants.FORMAT_USER_DEFINED
     EXCEL_SIMPLE = constants.FORMAT_EXCEL_SIMPLE
     EXCEL_MERGED = constants.FORMAT_EXCEL_MERGED
     FORMAT_CHOICES = constants.FORMAT_CHOICES
 
     title = models.CharField(
-        u'Наименование шаблона отчета',
+        'Наименование шаблона отчета',
         max_length=1000,
         unique=True,
     )
     data_source_name = models.CharField(
-        u'Имя источника данных',
+        'Имя источника данных',
         max_length=500,
         validators=[validate_data_source_name],
     )
     format = models.PositiveSmallIntegerField(
-        u'Формат сборки',
+        'Формат сборки',
         choices=FORMAT_CHOICES,
         default=USER_DEFINED,
     )
     include_available_units = models.BooleanField(
-        u'Отображать данные по дочерним организациям', default=False
+        'Отображать данные по дочерним организациям', default=False
     )
 
     class Meta:
-        verbose_name = u'Отчет'
-        verbose_name_plural = u'Отчеты'
+        verbose_name = 'Отчет'
+        verbose_name_plural = 'Отчеты'
 
     def simple_clean(self, errors):
         # ---------------------------------------------------------------------
         # Проверка уникальности наименования шаблона отчета.
         if self.title:
             query = ReportTemplate.objects.filter(
                 title__smart_iexact=self.title,
             )
             if self.pk:
                 query = query.exclude(pk=self.pk)
 
             if query.exists():
                 errors['title'].append(
-                    u'Шаблон отчета с подобным именем уже существует.'
+                    'Шаблон отчета с подобным именем уже существует.'
                 )
         # ---------------------------------------------------------------------
         super(ReportTemplate, self).simple_clean(errors)
 
     @cached_property
     def data_source(self):
         if self.data_source_name not in registry:
             raise ValidationError(
-                u'В шаблоне отчета указан несуществующий источник данных ({}).'
+                'В шаблоне отчета указан несуществующий источник данных ({}).'
                 .format(self.data_source_name)
             )
         data_source = registry.get(
             self.data_source_name
         ).get_data_source_descriptor()
         return data_source
 
     def __str__(self):
         return 'Шаблон отчета: {}'.format(self.title)
 # -----------------------------------------------------------------------------
 
 
 class ReportColumn(BaseModel):
-
-    u"""Модель "Столбец отчета"."""
+    """Модель "Столбец отчета"."""
 
     # Направления сортировки.
     ASCENDING = constants.SORT_ASCENDING
     DESCENDING = constants.SORT_DESCENDING
     SORT_CHOICES = constants.SORT_CHOICES
 
     report_template = models.ForeignKey(
         ReportTemplate,
-        verbose_name=u'Отчет',
+        verbose_name='Отчет',
         related_name='columns',
         on_delete=models.CASCADE,
     )
     name = models.CharField(
-        u'Имя столбца в источнике данных',
+        'Имя столбца в источнике данных',
         max_length=300,
     )
     index = models.PositiveSmallIntegerField(
-        u'Порядковый номер',
+        'Порядковый номер',
     )
     visible = models.BooleanField(
-        u'Видимость колонки в отчете',
+        'Видимость колонки в отчете',
         default=True,
     )
     title = models.CharField(
-        u'Отображаемое имя',
+        'Отображаемое имя',
         max_length=300,
         null=True, blank=True,
     )
     by_value = models.PositiveSmallIntegerField(
-        u'Промежуточный итог',
+        'Промежуточный итог',
         choices=constants.BY_VALUE_CHOICES,
         blank=True,
         null=True
     )
     total = models.PositiveSmallIntegerField(
-        u'Итог',
+        'Итог',
         choices=constants.TOTAL_CHOICES,
         blank=True,
         null=True
     )
 
     cascade_delete_for = (report_template,)
 
     class Meta:
-        verbose_name = u'Столбец отчета'
-        verbose_name_plural = u'Столбцы отчетов'
+        verbose_name = 'Столбец отчета'
+        verbose_name_plural = 'Столбцы отчетов'
         unique_together = (
             ('report_template', 'name'),
         )
         ordering = (
             'index',
         )
 
     def _clean_aggregator_type(self, errors):
-        u"""Проверяет на соответствие типов итогов."""
+        """Проверяет на соответствие типов итогов."""
         if not (
             (self.by_value == self.total) or
             (any(not bool(item) for item in (self.by_value, self.total)))
         ):
             errors['by_value'].append(
-                u'Тип для "Промежуточный итог" и "Итог" должен совпадать.'
+                'Тип для "Промежуточный итог" и "Итог" должен совпадать.'
             )
 
     def _clean_aggregator_data_type(self, errors):
-        u"""Проверяет тип данных для итогов."""
+        """Проверяет тип данных для итогов."""
         # Определяем тип данных в колонке.
         data_source_descriptor = registry.get(
             self.report_template.data_source_name
         ).get_data_source_descriptor()
         column_descriptor = data_source_descriptor.get_column_descriptor(
             self.name
         )
@@ -170,34 +185,33 @@
         aggregator_info = (
             ('by_value', is_sum_by_value),
             ('total', is_total_sum)
         )
         for aggregator_type, is_sum in aggregator_info:
             if is_sum and not is_num_data_type:
                 errors[aggregator_type].append(
-                    u'Подсчет суммы недопустим для колонки "{}".'.format(
+                    'Подсчет суммы недопустим для колонки "{}".'.format(
                         column_descriptor.get_full_title(),
                     )
                 )
 
     def simple_clean(self, errors):
-        u"""Добавляет проверку для подсчета итогов."""
+        """Добавляет проверку для подсчета итогов."""
         self._clean_aggregator_type(errors)
         self._clean_aggregator_data_type(errors)
 
         super(ReportColumn, self).simple_clean(errors)
 
     def __str__(self):
         return self.title
 # -----------------------------------------------------------------------------
 
 
 class ReportFilterGroup(MPTTModel, BaseModel):
-
-    u"""Группа фильтров.
+    """Группа фильтров.
 
     Фильтры объединяются в группы с помощью логических операторов "И" и "ИЛИ".
     При этом группы фильтров также могут быть объединены в группы. В итоге
     получается древовидная структура, представляющая собой подобие
     синтаксического дерева. Модели ``ReportFilterGroup`` и ``ReportFilter``
     используются для формирования таких деревьев.
     """
@@ -209,49 +223,49 @@
     # возможности не предусматрено. В случае, если у пользователей в будущем
     # возникнет потребность в создании более сложных фильтров, понадобится
     # переработка только интерфейсной части (окна редактирования шаблона).
 
     OPERATOR_AND = 1
     OPERATOR_OR = 2
     OPERATOR_CHOICES = (
-        (OPERATOR_AND, u'И'),
-        (OPERATOR_OR, u'ИЛИ'),
+        (OPERATOR_AND, 'И'),
+        (OPERATOR_OR, 'ИЛИ'),
     )
 
     report_template = models.ForeignKey(
         ReportTemplate,
-        verbose_name=u'Отчет',
+        verbose_name='Отчет',
         related_name='filter_groups',
         on_delete=models.CASCADE,
     )
     parent = TreeForeignKey(
         'self',
         blank=True, null=True,
-        verbose_name=u'Родительская группа',
+        verbose_name='Родительская группа',
         related_name='nested_groups',
         on_delete=models.CASCADE,
     )
     operator = models.PositiveSmallIntegerField(
-        u'Логический оператор',
-        help_text=u'Логический оператор, объединяющий фильтры в группе',
+        'Логический оператор',
+        help_text='Логический оператор, объединяющий фильтры в группе',
         choices=OPERATOR_CHOICES,
     )
 
     cascade_delete_for = (report_template,)
 
     class Meta:
-        verbose_name = u'Группа фильтров'
-        verbose_name_plural = u'Группы фильтров'
+        verbose_name = 'Группа фильтров'
+        verbose_name_plural = 'Группы фильтров'
 
     def __str__(self):
         return self.get_operator_display()
 
     @staticmethod
     def check_filter(instance, errors, **kwargs):
-        u"""Проверка фильтров в контексте группы фильтров.
+        """Проверка фильтров в контексте группы фильтров.
 
             1. Группа фильтра и столбца фильтра должны быть в одном и том же
                шаблоне.
 
         Вызывается через сигнал ``post_clean`` для объектов модели
         ``ReportFilter``.
 
@@ -274,16 +288,16 @@
         column = report_filter.column
         group = report_filter.group
         # ---------------------------------------------------------------------
         # Колонка фильтра должна быть в том же шаблоне, что и группа.
 
         if column.report_template_id != group.report_template_id:
             errors['column'].append(
-                u'Шаблон, к которому относится столбец фильтра "{}" '
-                u'отличается от шаблона, к которому относится группа фильтров.'
+                'Шаблон, к которому относится столбец фильтра "{}" '
+                'отличается от шаблона, к которому относится группа фильтров.'
                 .format(column.name)
             )
         # ---------------------------------------------------------------------
 
     def simple_clean(self, errors):
         super(ReportFilterGroup, self).simple_clean(errors)
         # ---------------------------------------------------------------------
@@ -294,98 +308,97 @@
             self.pk and
             self.report_template_id and
             self.filters.exclude(
                 column__report_template=self.report_template_id,
             ).exists()
         ):
             errors['report_template'].append(
-                u'В данной группе есть фильтры, ссылающиеся на столбцы из '
-                u'другого шаблона.'
+                'В данной группе есть фильтры, ссылающиеся на столбцы из '
+                'другого шаблона.'
             )
         # ---------------------------------------------------------------------
         # Шаблоны данной группы и родительской должны совпадать.
 
         if (
             self.pk and self.report_template_id and
             self.parent and self.parent.report_template_id and
             self.report_template_id != self.parent.report_template_id
         ):
             errors['parent'].append(
-                u'Шаблон данной группы фильтров ("{}") отличается от шаблона '
-                u'родительской группы ("{}").'.format(
+                'Шаблон данной группы фильтров ("{}") отличается от шаблона '
+                'родительской группы ("{}").'.format(
                     self.report_template.title,
                     self.parent.report_template.title,
                 )
             )
 # -----------------------------------------------------------------------------
 
 
 class ReportFilter(BaseModel):
-
-    u"""Модель "Параметр фильтрации данных отчета"."""
+    """Модель "Параметр фильтрации данных отчета"."""
 
     group = models.ForeignKey(
         ReportFilterGroup,
-        verbose_name=u'Группа фильтров',
+        verbose_name='Группа фильтров',
         related_name='filters',
         on_delete=models.CASCADE,
     )
     column = models.ForeignKey(
         ReportColumn,
-        verbose_name=u'Столбец',
+        verbose_name='Столбец',
         related_name='filters',
         on_delete=models.CASCADE,
     )
     index = models.PositiveSmallIntegerField(
-        u'Порядковый номер',
+        'Порядковый номер',
     )
     operator = models.PositiveSmallIntegerField(
-        u'Оператор сравнения',
+        'Оператор сравнения',
         choices=constants.OPERATOR_CHOICES,
     )
     exclude = models.BooleanField(
-        u'Исключать записи, удовлетворяющие условию',
+        'Исключать записи, удовлетворяющие условию',
         default=False,
     )
     case_sensitive = models.NullBooleanField(
-        u'Учет регистра',
+        'Учет регистра',
     )
     values = ArrayField(
         models.TextField(
-            u'Значение',
+            'Значение',
             blank=True, null=True,
         ),
         blank=True, null=True,
     )
     comment = models.TextField(
-        u'Описание фильтра',
+        'Описание фильтра',
         blank=True, null=True,
     )
 
     cascade_delete_for = (group, column)
 
     def __str__(self):
         """Возвращает строку вида:
         `Поле "<название_поля>" [не ]<оператор:меньше или равно|меньше|...>
         "<значение>", <без учета|с учетом> регистра`
         :return:
         """
         template = (
-            u'Поле "{col}"{invert__op:10}{operator} '
-            u'"{value}", {case} регистра'
+            'Поле "{col}"{invert__op:10}{operator} '
+            '"{value}", {case} регистра'
         )
-        invert__op = u' не ' if self.exclude else u' '
-        case = u'с учетом' if self.case_sensitive else u'без учета'
+        invert__op = ' не ' if self.exclude else ' '
+        case = 'с учетом' if self.case_sensitive else 'без учета'
         return template.format(col=self.column, invert__op=invert__op,
                                operator=self.get_operator_display().lower(),
-                               value=u', '.join(self.values), case=case)
+                               value=', '.join(self.values), case=case)
 
     class Meta:
-        verbose_name = u'Фильтр'
-        verbose_name_plural = u'Фильтры'
+        verbose_name = 'Фильтр'
+        verbose_name_plural = 'Фильтры'
         unique_together = (
             ('column', 'index'),
         )
         ordering = (
             'index',
         )
 
@@ -401,85 +414,84 @@
             self.operator == constants.BETWEEN and
             (
                 not self.values or
                 len(self.values) != 2
             )
         ):
             errors['values'].append(
-                u'Для оператора "{}" должно быть указано два значения.'
+                'Для оператора "{}" должно быть указано два значения.'
                 .format(self.get_operator_display())
             )
 
         elif (
             self.operator not in (constants.IN, constants.BETWEEN,) and
             (
                 not self.values or
                 len(self.values) > 1
             )
         ):
             errors['values'].append(
-                u'Должно быть указано только одно значение.'
+                'Должно быть указано только одно значение.'
             )
 
         elif not self.values:
-            errors['values'].append(u'Не указано значение для сравнения.')
+            errors['values'].append('Не указано значение для сравнения.')
         # ---------------------------------------------------------------------
 
         if (
             self.group and self.column and
             self.group.report_template_id != self.column.report_template_id
         ):
             errors['column'].append(
-                u'Группа и колонка принадлежат разным шаблонам.'
+                'Группа и колонка принадлежат разным шаблонам.'
             )
         # ---------------------------------------------------------------------
 
         data_source_descriptor = registry.get(
             self.group.report_template.data_source_name
         ).get_data_source_descriptor()
         column_descriptor = data_source_descriptor.get_column_descriptor(
             self.column.name
         )
         data_type = column_descriptor.data_type
         valid_operators = constants.VALID_OPERATORS[data_type]
         if self.operator and self.operator not in valid_operators:
             errors['operator'].append(
-                u'Оператор "{}" недопустим для колонки "{}".'.format(
+                'Оператор "{}" недопустим для колонки "{}".'.format(
                     self.get_operator_display(),
                     column_descriptor.get_full_title(),
                 )
             )
 # -----------------------------------------------------------------------------
 
 
 class ReportSorting(BaseModel):
-
-    u"""Модель "Параметр сортировки данных отчета"."""
+    """Модель "Параметр сортировки данных отчета"."""
 
     column = models.OneToOneField(
         ReportColumn,
-        verbose_name=u'Колонка',
+        verbose_name='Колонка',
         related_name='sorting',
         on_delete=models.CASCADE,
     )
     direction = models.PositiveSmallIntegerField(
-        u'Направление сортировки',
+        'Направление сортировки',
         choices=constants.DIRECTION_CHOICES,
     )
     index = models.PositiveSmallIntegerField(
-        u'Порядковый номер',
+        'Порядковый номер',
     )
 
     class Meta:
-        verbose_name = u'Сортировка'
-        verbose_name_plural = u'Сортировка'
+        verbose_name = 'Сортировка'
+        verbose_name_plural = 'Сортировка'
         ordering = ('index',)
 
     def __str__(self):
-        return u'{col} ({direction})'.format(
+        return '{col} ({direction})'.format(
             col=self.column, direction=self.get_direction_display().lower()
         )
 # -----------------------------------------------------------------------------
 
 
 post_clean.connect(ReportFilterGroup.check_filter, ReportFilter,
                    dispatch_uid='ReportFilterGroup.check_filter')
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/registries.py` & `educommon-3.0.0/src/educommon/report/constructor/registries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,50 @@
-# coding: utf-8
-from __future__ import absolute_import
+from educommon.report.constructor.base import (
+    ModelDataSourceParams,
+)
 
-import six
 
-from .base import ModelDataSourceParams
-
-
-class DataSourceParamsRegistry(object):
-
-    u"""Реестр параметров данных.
+class DataSourceParamsRegistry:
+    """Реестр параметров данных.
 
     При первом чтении из реестра отправляет сигнал ``init`` для добавления
     в реестр параметров для источников данных системы. Каждое django-приложение
     должно в обработчике этого сигнала зарегистрировать свои параметры
     источников данных.
     """
 
     def __init__(self):
-        u"""Инициализация реестра.
+        """Инициализация реестра.
 
         По завершении инициализации отправляет сигнал ``post_init``.
         """
         self._data_sources_params = {}
 
     def register(self, data_source_params):
-        u"""Регистрация параметров источника данных."""
+        """Регистрация параметров источника данных."""
         assert isinstance(data_source_params, ModelDataSourceParams)
         assert data_source_params.name
         assert data_source_params.name not in self._data_sources_params
 
         self._data_sources_params[data_source_params.name] = data_source_params
 
     def get(self, data_source_name):
-        u"""Возвращает параметры источника данных по имени.
+        """Возвращает параметры источника данных по имени.
 
         :param str data_source_name: Имя источника данных.
         """
         return self._data_sources_params[data_source_name]
 
     def __contains__(self, key):
         return key in self._data_sources_params
 
     def iterkeys(self):
-        return six.iterkeys(self._data_sources_params)
+        return self._data_sources_params.keys()
 
     def itervalues(self):
-        return six.itervalues(self._data_sources_params)
+        return self._data_sources_params.values()
 
     def iteritems(self):
-        return six.iteritems(self._data_sources_params)
+        return self._data_sources_params.items()
 
 
 registry = DataSourceParamsRegistry()
```

### Comparing `educommon-2.20.0/src/educommon/report/constructor/utils.py` & `educommon-3.0.0/src/educommon/report/constructor/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,56 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from collections import OrderedDict
-from inspect import isclass
-
-from django.core.exceptions import FieldDoesNotExist
-from django.db.models.fields import BooleanField
-from django.db.models.fields import CharField
-from django.db.models.fields import DateField
-from django.db.models.fields import DateTimeField
-from django.db.models.fields import DecimalField
-from django.db.models.fields import FloatField
-from django.db.models.fields import IntegerField
-from django.db.models.fields import NullBooleanField
-from django.db.models.fields import TextField
-from django.db.models.fields import TimeField
-from django.db.models.fields.related import ForeignKey
-from django.db.models.fields.reverse_related import ForeignObjectRel
-from m3_django_compat import get_related
-
-from .constants import CT_BOOLEAN
-from .constants import CT_CHOICES
-from .constants import CT_DATE
-from .constants import CT_DATETIME
-from .constants import CT_DIRECT_RELATION
-from .constants import CT_NULL_BOOLEAN
-from .constants import CT_NUMBER
-from .constants import CT_OTHER
-from .constants import CT_REVERSE_RELATION
-from .constants import CT_TEXT
-from .constants import CT_TIME
+from collections import (
+    OrderedDict,
+)
+from inspect import (
+    isclass,
+)
+
+from django.core.exceptions import (
+    FieldDoesNotExist,
+)
+from django.db.models.fields import (
+    BooleanField,
+    CharField,
+    DateField,
+    DateTimeField,
+    DecimalField,
+    FloatField,
+    IntegerField,
+    NullBooleanField,
+    TextField,
+    TimeField,
+)
+from django.db.models.fields.related import (
+    ForeignKey,
+)
+from django.db.models.fields.reverse_related import (
+    ForeignObjectRel,
+)
+from m3_django_compat import (
+    get_related,
+)
+
+from educommon.report.constructor.constants import (
+    CT_BOOLEAN,
+    CT_CHOICES,
+    CT_DATE,
+    CT_DATETIME,
+    CT_DIRECT_RELATION,
+    CT_NULL_BOOLEAN,
+    CT_NUMBER,
+    CT_OTHER,
+    CT_REVERSE_RELATION,
+    CT_TEXT,
+    CT_TIME,
+)
 
 
 def get_field(model, name):
-    u"""Возвращает поле с именем :arg:`name` модели :arg:`model`.
+    """Возвращает поле с именем :arg:`name` модели :arg:`model`.
 
     Для обратных зависимостей в :arg:`name` нужно указывать имя атрибута
     объекта модели (см. :attr:`~django.db.models.ForeignKey.related_name`).
 
     :rtype: django.db.models.fields.Field or
         django.db.models.fields.related.RelatedField
     """
@@ -51,25 +64,27 @@
         if name == field_name:
             return field
 
     # Поиск среди дополнительных полей модели.
     extra = getattr(model, 'report_constructor_params', {}).get('extra', {})
     for accessor_name, params in extra.items():
         if name == accessor_name:
-            from .base import ExtraField
+            from educommon.report.constructor.base import (
+                ExtraField,
+            )
             field = params['field']
             field.model = model if isclass(model) else model.__class__
             field.name = name
             return ExtraField(accessor_name, field)
 
     raise FieldDoesNotExist(name)
 
 
 def get_nested_field(model, field_name):
-    u"""Возвращает поле модели с учетом вложенности связей.
+    """Возвращает поле модели с учетом вложенности связей.
 
     Например, такой вызов вернет поле ``surname`` модели ``Person``, на которую
     есть внешний ключ из модели ``Employee`` через поле ``person``.
 
     .. code-block:: python
 
        >>> get_nested_field(Employee, 'person.surname')
@@ -105,15 +120,15 @@
                 .format(model.__name__, field_name)
             )
     else:
         return attr_value
 
 
 def get_columns_hierarchy(*columns):
-    u"""Формирует иерахию полей по списку колонок.
+    """Формирует иерахию полей по списку колонок.
 
     .. code-block:: python
 
        >>> get_columns_hierarchy('person.surname', 'person.firstname')
        {
            'person': {
                'surname': {},
@@ -134,42 +149,42 @@
                 nodes[level_name] = OrderedDict()
             nodes = nodes[level_name]
 
     return result
 
 
 def get_field_value_by_display(field, display_value):
-    u"""Возвращает значение поля с вариантами, соответствующее представлению.
+    """Возвращает значение поля с вариантами, соответствующее представлению.
 
     :param field: Поле модели.
     :type field: django.db.models.fields.Field
 
     :param display_value: Текстовое представление, соответствующее искомому
         значению поля.
     :type display_value: unicode
 
     :raises ValueError: если поле ``field`` не содержит вариантов допустимых
         значений, либо значения ``display_value`` нет среди допустимых
         вариантов.
     """
     if not field.choices:
-        raise ValueError(u'Поле не содержит варианты выбора.')
+        raise ValueError('Поле не содержит варианты выбора.')
 
     for value, display in field.choices:
         if display.lower() == display_value.lower():
             return value
 
     raise ValueError(
-        u'Значения "{}" нет среди вариантов выбора.'
+        'Значения "{}" нет среди вариантов выбора.'
         .format(display_value)
     )
 
 
 def get_data_type(field):
-    u"""Возвращает тип данных поля.
+    """Возвращает тип данных поля.
 
     :param field: поле модели.
     :type field: django.db.models.fields.Field
 
     :rtype: str
     """
     if field.concrete and field.choices:
```

### Comparing `educommon-2.20.0/src/educommon/report/reporter.py` & `educommon-3.0.0/src/educommon/report/reporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-# coding: utf-8
-u"Модуль с построителями отчетов"
-from __future__ import absolute_import
-
+"Модуль с построителями отчетов"
 import os
 import sys
 import uuid
 
-from django.conf import settings
-from simple_report.converter.abstract import FileConverter
-from simple_report.report import DocumentReport
-from simple_report.report import SpreadsheetReport
-from simple_report.xls.document import DocumentXLS
+from django.conf import (
+    settings,
+)
+from simple_report.converter.abstract import (
+    FileConverter,
+)
+from simple_report.report import (
+    DocumentReport,
+    SpreadsheetReport,
+)
+from simple_report.xls.document import (
+    DocumentXLS,
+)
 
 
 path_dir = settings.REPORTS_DIR
 if not os.path.exists(path_dir):
     os.makedirs(path_dir)
 
 
 def get_path(filename):
-    u"""Путь до временного файла отчёта.
+    """Путь до временного файла отчёта.
 
     :param str filename: имя файла (с раcширением, без пути до файла)
     :rtype: str
     """
     return os.path.abspath(os.path.join(path_dir, filename))
 
 
 def get_url(filename):
-    u"""URL до временного файла отчёта.
+    """URL до временного файла отчёта.
 
     :param str filename: имя файла (с раcширением, без пути до файла)
     :rtype: str
     """
     return '/'.join((settings.REPORTS_URL, filename))
 
 
-class SimpleReporter(object):
-    u"""
+class SimpleReporter:
+    """
     Объект занимающийся комплексным построением отчета на основе simple_report:
     1) инстанцированием и загрузкой данных провайдера
     2) инстанцированием билдера
     3) построением отчета
 
     Можно использовать вне паков и экшнов
 
@@ -54,15 +59,15 @@
     _available_extensions = ['.xls', '.xlsx', '.docx']
 
     # формат по-умолчанию
     extension = '.xls'
 
     # путь где лежит файл шаблона отчета
     template_file_path = None
-    u"""
+    """
     будет искать шаблон report.{extension} в директори отчета
     template_file_path = None
     custom_report.{extension} по абсолютному пути
     template_file_path = '/tmp/some/custom_report.{extension}'
     по относительному ./templates в директории отчета
     template_file_path = './templates/custom_report.{extension}'
     report.{extension} в ./templates/somedir/
@@ -75,20 +80,20 @@
     # класс билдера
     builder_class = None
 
     # класс адаптера
     adapter_class = None
 
     def __init__(self, provider_params, builder_params):
-        assert self.builder_class, u''
+        assert self.builder_class, ''
         self.provider_params = provider_params
         self.builder_params = builder_params
 
     def get_template(self, default_base_name='report'):
-        u"""Возвращает путь к шаблону отчета.
+        """Возвращает путь к шаблону отчета.
 
         :param default_base_name: базовое имя шаблона,
             если определить не удалось
         :type default_base_name: str
         :returns: str - полный путь к шаблону
         """
         if (self.template_file_path is not None and
@@ -115,20 +120,20 @@
 
         auto_report_name = '{0}{1}{2}'.format(
             base_name, os.path.extsep, self.extension.strip('.'))
         auto_report_path = os.path.join(
             report_dir, rel_sub_path, auto_report_name)
 
         assert os.path.isfile(auto_report_path), (
-            u"Report template '{0}' not found at {1}".format(
+            "Report template '{0}' not found at {1}".format(
                 auto_report_name, auto_report_path))
         return auto_report_path
 
     def set_up_report(self):
-        u"""Настройка формата отчёта."""
+        """Настройка формата отчёта."""
         template_path = self.get_template()
 
         if self.extension == '.xls':
             report = SpreadsheetReport(
                 template_path, wrapper=DocumentXLS, type=FileConverter.XLS)
         elif self.extension == '.xlsx':
             report = SpreadsheetReport(template_path)
@@ -136,57 +141,57 @@
             report = DocumentReport(template_path)
         else:
             raise Exception('Unknown template extension')
 
         return report
 
     def set_file_and_url(self):
-        u"""
+        """
         Возвращает кортеж из абс. пути отчёта и url для скачивания.
         Не требует переопределения.
         """
         title = self.builder_params.get('title')
         title = title + '_' if title else ''
         base_name = title + str(uuid.uuid4())[0:16] + self.extension
         out_file_path = get_path(base_name)
         out_file_url = get_url(base_name)
 
         return (out_file_path, out_file_url)
 
     def create_provider(self):
-        u"""
+        """
         Кастомный метод для создания экземпляра класса провайдера.
 
         Используется в случае необходимости явного вызова конструктора
         провайдера, например, для композитного провайдера.
         :returns: инстанс дата-провайдера
         """
 
     def init_provider(self, data_provider):
-        u"""
+        """
         Инициализирует дата-провайдер с параметрами self.provider_params
         """
         data_provider.init(**self.provider_params)
 
     def create_builder(self, data_provider, report):
-        u"""
+        """
         Создание билдера.
         Если требуется, можно использовать адаптер self.adapter_class
 
         :returns: билдер с параметрами self.builder_params
         """
         return self.builder_class(
             data_provider,
             adapter=self.adapter_class,
             report=report,
             params=self.builder_params
         )
 
     def get_data_provider(self):
-        u"""
+        """
         Создание провайдера и взятие данных.
 
         :return: Provider с уже сформированным результатом
         """
         # создание провайдера
         # для случая композитного провайдера
         data_provider = self.create_provider()
@@ -196,57 +201,57 @@
 
         self.init_provider(data_provider)
         data_provider.load_data()
 
         return data_provider
 
     def _get_report_builder(self, data_provider, report):
-        u"""
+        """
         Создание билдера и построение отчета.
 
         :param data_provider: Provider с уже сформированным результатом.
         :param report: Отчет форматов .xls, .xlsx или .docx
         :returns: Результат выполнения метода build
         """
         # создание билдера, который будет строить кастомный отчёт
         report_builder = self.create_builder(data_provider, report=report)
         return report_builder.build()
 
     def create_dir(self, out_file):
-        u"""
+        """
         Создание директории для сохранения файла
 
         :param out_file:  str, путь к файлу.
         :raise: OsError
         :return: None
         """
         # Если пытаемся сохранить файл в несуществующую директорию,
         # то попробуем её предварительно создать
         cat = os.path.dirname(out_file)
         if not os.path.exists(cat):
             # здесь может быть OsError
             os.makedirs(cat)
 
     def build_report(self, report, out_file, params):
-        u"""
+        """
         Построение отчета.
 
         :param report: Отчет форматов .xls, .xlsx или .docx
         :param out_file: str, путь к файлу.
         :param params: Результат выполение работы билдера.
         :return: None
         """
         # построение отчёта
         if isinstance(report, DocumentReport):
             report.build(out_file, params)
         else:
             report.build(out_file)
 
     def make_report(self):
-        u"""
+        """
         Основной метод, выполняющий построение отчета
         """
         # получение абс. пути отчёта
         out_file, out_url = self.set_file_and_url()
         # настройка формата отчета
         report = self.set_up_report()
```

### Comparing `educommon-2.20.0/src/educommon/report/utils.py` & `educommon-3.0.0/src/educommon/report/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from six.moves import range
-
-from educommon.utils.fonts import ARIAL
-from educommon.utils.fonts import get_font
-from educommon.utils.fonts import split_text
+from educommon.utils.fonts import (
+    ARIAL,
+    get_font,
+    split_text,
+)
 
 
 # Высота и ширина символа "0" шрифта по умолчанию в xlwt.
 DEFAULT_CHAR_SIZE = 256
 
 
 def cm_to_inch(value):
-    u"""Переводит значение из сантиметров в дюймы."""
+    """Переводит значение из сантиметров в дюймы."""
     return value / 2.54
 
 
 def inch_to_cm(value):
-    u"""Переводит значение из дюймов в сантиметры."""
+    """Переводит значение из дюймов в сантиметры."""
     return value * 2.54
 
 
 def get_cell_bounds(section, row_index, column_index):
-    u"""Возвращает границы ячейки, находящейся на пересечении строки и столбца.
+    """Возвращает границы ячейки, находящейся на пересечении строки и столбца.
 
     .. note::
 
        Индексы строк и колонок начинаются с нуля.
 
     :param section: Секция, в которой находится строка.
     :type section: :class:`simple_report.xls.section.Section`
@@ -48,15 +45,15 @@
         ):
             return first_row, last_row, first_column, last_column
 
     return row_index, row_index, column_index, column_index
 
 
 def get_cell_width(section, row_index, column_index):
-    u"""Возвращает ширину ячейки с учётом объединения.
+    """Возвращает ширину ячейки с учётом объединения.
 
     .. note ::
 
        Ширина ячейки определяется, как 1/256 от ширины символа "0" первого
        попавшегося шрифта в файле, т.е. единицы изменения достаточно условны.
 
     .. note::
@@ -78,15 +75,15 @@
     return sum(
         section.writer.wtsheet.col(i).width
         for i in range(first_column, last_column + 1)
     )
 
 
 def get_cell_height(section, row_index, column_index):
-    u"""Возвращает высоту ячейки с учётом объединения.
+    """Возвращает высоту ячейки с учётом объединения.
 
     .. note::
 
        Индексы строк и колонок начинаются с нуля.
 
     :param section: Секция, в которой находится строка.
     :type section: :class:`simple_report.xls.section.Section`
@@ -105,15 +102,15 @@
         section.writer.wtsheet.row(i).height
         for i in range(first_row, last_row + 1)
     )
 
 
 def adjust_row_height(section, row_idx, col_idx, text, font,
                       adjusted_row_index=None):
-    u"""Увеличивает высоту строки, если необходимо.
+    """Увеличивает высоту строки, если необходимо.
 
     Высота строки устанавливается такая, чтобы текст `text`
     поместился в ячейку с индексами `row_idx`, `col_idx`.
 
     Можно применять для нескольких ячеек одной строки. Тогда строке будет
     установлена максимальная высота.
 
@@ -124,26 +121,26 @@
     :param section: Секция, в которой находится строка.
     :type section: :class:`simple_report.xls.section.Section`
 
     :param int row_idx: Индекс строки в таблице excel.
 
     :param int col_idx: Индекс столбца в таблице excel.
 
-    :param unicode text: Строка, которая будет записана в ячейку.
+    :param str text: Строка, которая будет записана в ячейку.
 
     :param font: Шрифт.
     :type font: :class:`PIL.ImageFont.FreeTypeFont`
 
     :param int adjusted_row_index: Номер строки, размер которой будет увеличен.
         Если не указывается (``None``), то высота всех строк объединенной
         ячейки будет увеличена равномерно. Номер указывается относительно
         ячейки, нумерация начинается с нуля.
     """
     def get_text_height(column_width):
-        u"""Вычисляет высоту строки отчета в зависимости от текста."""
+        """Вычисляет высоту строки отчета в зависимости от текста."""
         # Т.к. высота и ширина ячейки измеряется в единицах относительно
         # дефолтного шрифта, берем его параметры.
         normal_font = get_font(ARIAL, 10)
 
         # Количество символов "0", которое входит в одну ячейку без переносов.
         # DEFAULT_CHAR_SIZE * 0.8 определяет ширину отступов слева и справа (в
         # сумме, а не каждого отступа по отдельности). Источник точной
@@ -205,27 +202,27 @@
         else:
             row = section.writer.wtsheet.row(row_idx)
             add_row_height(row, height_delta)
 
 
 def adjust_row_height_arial(section, row_idx, col_idx, text, font_size=10,
                             adjusted_row_index=None):
-    u"""Устанавливает высоту строки автоматически.
+    """Устанавливает высоту строки автоматически.
 
     Высота строки устанавливается такая, чтобы текст text
     поместился в ячейку с индексами row_idx, col_idx.
 
     Расчет ведется для шрифта Arial, и соответствует отображению ячеек в
     MS Excel.
 
     :param section: Секция, в которой находится строка
     :type section: :class:`simple_report.xls.section.Section`
     :param int row_idx: Индекс строки в таблице excel
     :param int col_idx: Индекс столбца в таблице excel
-    :param unicode text: Строка, которая будет записана в ячейку
+    :param str text: Строка, которая будет записана в ячейку
     :param int font_size: Размер шрифта в пунктах
     :param int adjusted_row_index: Номер строки, размер которой будет увеличен.
         Если не указывается (``None``), то высота всех строк объединенной
         ячейки будет увеличена равномерно. Номер указывается относительно
         ячейки, нумерация начинается с нуля.
     """
     font = get_font(ARIAL, font_size)
```

### Comparing `educommon-2.20.0/src/educommon/rest/actions.py` & `educommon-3.0.0/src/educommon/rest/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# coding: utf-8
-from objectpack.actions import BasePack
-
-from . import mixins
+from objectpack.actions import (
+    BasePack,
+)
+
+from educommon.rest import (
+    mixins,
+)
 
 
 class BaseRestPack(BasePack):
-
     """Базовый пак для всех REST пакокв."""
 
 
 class RestPack(
     mixins.ListModelMixin,
     mixins.RetrieveModelMixin,
     mixins.CreateModelMixin,
```

### Comparing `educommon-2.20.0/src/educommon/rest/context.py` & `educommon-3.0.0/src/educommon/rest/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-# coding: utf-8
 import json
 
-from m3.actions import context
-import six
-
-from .controllers import ObservableController
-from .misc import get_request_params
+from m3.actions import (
+    context,
+)
+
+from educommon.rest.controllers import (
+    ObservableController,
+)
+from educommon.rest.misc import (
+    get_request_params,
+)
 
 
 class RestDeclarativeActionContext(
     ObservableController.VerboseDeclarativeContext
 ):
 
     def build(self, request, rules):
@@ -40,15 +44,15 @@
             self._mode = mode
 
         # аккумуляторы ошибок, связанных с нехваткой и неправильным форматом
         requiremets = []
         errors = []
         only_noncritical = True
 
-        for key, parser_data in six.iteritems(rules):
+        for key, parser_data in rules.items():
             parser = parser_data['type']
             if not callable(parser):
                 try:
                     parser = self._parsers[parser]
                 except KeyError:
                     raise TypeError(
                         'Неизвестный парсер контекста: "%s"' %
```

### Comparing `educommon-2.20.0/src/educommon/rest/controllers.py` & `educommon-3.0.0/src/educommon/rest/controllers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-# coding: utf-8
 import json
 import re
 
-from m3 import actions as m3_actions
-from objectpack.observer.base import ObservableController
-from objectpack.observer.base import _warn
-import six
-
-from .context import RestDeclarativeActionContext
-from .misc import get_request_params
+from m3 import (
+    actions as m3_actions,
+)
+
+from objectpack.observer.base import (
+    ObservableController,
+    _warn,
+)
+
+from educommon.rest.context import (
+    RestDeclarativeActionContext,
+)
+from educommon.rest.misc import (
+    get_request_params,
+)
 
 
 class RestObservableController(ObservableController):
-
     """Контроллер для REST."""
 
     api = None
     object_id_regex = re.compile(r'/(?P<id>\d+)$')
 
     class VerboseDeclarativeContext(
         RestDeclarativeActionContext
@@ -28,23 +34,23 @@
                 RestDeclarativeActionContext.build(self, request, rules)
             except m3_actions.CriticalContextBuildingError as e:
                 if self.__debug:
                     raise
                 else:
                     _warn('%r, url="%s"' % (e, request.path_info))
 
-            for k, v in list(six.iteritems(get_request_params(request))):
+            for k, v in list(get_request_params(request).items()):
                 if not hasattr(self, k):
                     setattr(self, k, v)
 
             # Если метод запроса не GET соберем контекст из body
             if request.method != 'GET':
                 try:
                     json_params = json.loads(request.body)
-                    for k, v in six.iteritems(json_params):
+                    for k, v in json_params.items():
                         if not hasattr(self, k):
                             setattr(self, k, v)
                 except ValueError:
                     pass
 
     def __init__(self, observer, *args, **kwargs):
         super(RestObservableController, self).__init__(
```

### Comparing `educommon-2.20.0/src/educommon/rest/mixins.py` & `educommon-3.0.0/src/educommon/rest/mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# coding: utf-8
-from m3.actions.results import PreJsonResult
-from objectpack.actions import BaseAction
+from m3.actions.results import (
+    PreJsonResult,
+)
+
+from objectpack.actions import (
+    BaseAction,
+)
 
 
 class BaseRestAction(BaseAction):
-
     """Базовый экшен для экшенов REST."""
 
 
-class ListModelMixin(object):
-
+class ListModelMixin:
     """
     Примесь для REST паков, обработка запросов метода GET.
     Получения списка объектов.
     """
 
     def __init__(self):
         super(ListModelMixin, self).__init__()
@@ -25,16 +27,15 @@
         """
         Метод отвечает за обработку запроса методом GET.
         Получение списка объектов.
         """
         raise NotImplementedError
 
 
-class RetrieveModelMixin(object):
-
+class RetrieveModelMixin:
     """
     Примесь для REST паков, обработка запросов метода GET.
     Получение конкретно объекта по context.id.
     """
 
     def __init__(self):
         super(RetrieveModelMixin, self).__init__()
@@ -47,15 +48,14 @@
         Метод отвечает за обработку запроса методом GET.
         Получение конкретного объекта по context.id.
         """
         raise NotImplementedError
 
 
 class GetAction(BaseRestAction):
-
     """
     Экшен обработки запроса методом GET.
     Делегирует обработку методам пака.
     """
 
     url = '/get'
 
@@ -63,44 +63,41 @@
         if not request.object_id and hasattr(self.parent, 'list'):
             result = self.parent.list(request, context)
         else:
             result = self.parent.retrieve(request, context)
         return result
 
 
-class CreateModelMixin(object):
-
+class CreateModelMixin:
     """Примесь для REST паков, обработка запросов методом POST."""
 
     def __init__(self):
         super(CreateModelMixin, self).__init__()
         self.post_action = PostAction()
         self.actions.append(self.post_action)
 
     def create(self, request, context):
         """Метод отвечает за создание объекта."""
         raise NotImplementedError
 
 
 class PostAction(BaseRestAction):
-
     """
     Экшен обработки запроса методом POST.
     Делегирует обработку методам пака.
     """
 
     url = '/post'
 
     def run(self, request, context):
         result = self.parent.create(request, context)
         return PreJsonResult(result)
 
 
-class UpdateModelMixin(object):
-
+class UpdateModelMixin:
     """Примесь для REST паков, обработка запросов методом PUT и PATCH."""
 
     def __init__(self):
         super(UpdateModelMixin, self).__init__()
         self.put_action = PutAction()
         self.patch_action = PatchAction()
         self.actions.extend([
@@ -110,57 +107,53 @@
 
     def update(self, request, context):
         """Метод отвечает за изменение объекта."""
         raise NotImplementedError
 
 
 class PutAction(BaseRestAction):
-
     """
     Экшен обработки запроса методом PUT.
     Делегирует обработку методам пака.
     """
 
     url = '/put'
 
     def run(self, request, context):
         result = self.parent.update(request, context)
         return PreJsonResult(result)
 
 
 class PatchAction(BaseRestAction):
-
     """
     Экшен обработки запроса методом PATCH.
     Делегирует обработку методам пака.
     """
 
     url = '/patch'
 
     def run(self, request, context):
         result = self.parent.update(request, context)
         return PreJsonResult(result)
 
 
-class DestroyModelMixin(object):
-
+class DestroyModelMixin:
     """Примесь для REST паков, обработка запросов методом DELETE."""
 
     def __init__(self):
         super(DestroyModelMixin, self).__init__()
         self.delete_action = DeleteAction()
         self.actions.append(self.delete_action)
 
     def destroy(self, request, context):
         """Метод отвечает за удаление объекта."""
         raise NotImplementedError
 
 
 class DeleteAction(BaseRestAction):
-
     """
     Экшен обработки запроса методом PATCH.
     Делегирует обработку методам пака.
     """
 
     url = '/delete'
```

### Comparing `educommon-2.20.0/src/educommon/secure_media/README.rst` & `educommon-3.0.0/src/educommon/secure_media/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/secure_media/app_meta.py` & `educommon-3.0.0/src/educommon/secure_media/app_meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,43 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import os
 
-from django import http
-from django.conf import settings
-from django.conf.urls import url
-from m3 import M3JSONEncoder
-from m3_django_compat import is_authenticated
-from sendfile import sendfile
+from django import (
+    http,
+)
+from django.conf import (
+    settings,
+)
+from django.conf.urls import (
+    url,
+)
+from m3 import (
+    M3JSONEncoder,
+)
+from m3_django_compat import (
+    is_authenticated,
+)
+from sendfile import (
+    sendfile,
+)
 
 
 def check_autorization(request, path):
 
     # Если файл в media/public, то отдаем сразу без проверки
     # Вообще это делается соответствующим конфигурированием NGINX
     path_list = path.split(os.path.sep)
     if path_list and path_list[0] == "public":
         return sendfile(request, os.path.join(settings.MEDIA_ROOT, path))
 
     if not is_authenticated(request.user):
         result = M3JSONEncoder().encode(
             {'success': False,
-             'message': u'Вы не авторизованы. Возможно, закончилось время '
-                        u'пользовательской сессии. Для повторной '
-                        u'аутентификации обновите страницу.'})
+             'message': 'Вы не авторизованы. Возможно, закончилось время '
+                        'пользовательской сессии. Для повторной '
+                        'аутентификации обновите страницу.'})
         return http.HttpResponse(result, content_type='application/json')
 
     return sendfile(request, os.path.join(settings.MEDIA_ROOT, path))
 
 
 urlpatterns = [
     url(r'^media/(?P<path>.*)$', check_autorization)
```

### Comparing `educommon-2.20.0/src/educommon/utils/__init__.py` & `educommon-3.0.0/src/educommon/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# coding: utf-8
-u"""Вспомогательные средства."""
-from __future__ import absolute_import
+"""Вспомогательные средства."""
 
 
 def is_ranges_intersected(range1, range2):
-    u"""Возвращает True, если указанные интервалы значений пересекаются.
+    """Возвращает True, если указанные интервалы значений пересекаются.
 
     Интервалы задаются в виде двухэлементных кортежей, первый элемент кортежа
     определяет начало интервала, а второй - конец интервала. None определяет
     открытый с соответствующей стороны интервал.
 
     Типы данных в интервалах должны поддерживать сравнение значений с помощью
     оператора <=.
@@ -42,24 +40,23 @@
         else:  # from2 is not None and to2 is not None
             result = from2 <= to1 and from1 <= to2
 
     return result
 
 
 class SingletonMeta(type):
-
-    u"""Метакласс для классов-одиночек.
+    """Метакласс для классов-одиночек.
 
     Потомки класса с данным метаклассом также будут одиночками. Инициализация
     классов-одиночек (вызов метода ``__init__``) будет выполняться один раз
     при создании.
 
     .. code-block:: python
 
-       class SingleClass(object):
+       class SingleClass:
            __metaclass__ = SingletonMeta
     """
 
     def __init__(cls, name, bases, attrs):
         super(SingletonMeta, cls).__init__(name, bases, attrs)
         cls.instance = None
```

### Comparing `educommon-2.20.0/src/educommon/utils/caching.py` & `educommon-3.0.0/src/educommon/utils/caching.py`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/conversion.py` & `educommon-3.0.0/src/educommon/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/crypto.py` & `educommon-3.0.0/src/educommon/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/date.py` & `educommon-3.0.0/src/educommon/utils/date.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 WED_IDX = 2
 THU_IDX = 3
 FRI_IDX = 4
 SAT_IDX = 5
 SUN_IDX = 6
 
 WEEKDAYS = (
-    (MON_IDX, u'Понедельник'),
-    (TUE_IDX, u'Вторник'),
-    (WED_IDX, u'Среда'),
-    (THU_IDX, u'Четверг'),
-    (FRI_IDX, u'Пятница'),
-    (SAT_IDX, u'Суббота'),
-    (SUN_IDX, u'Воскресенье')
+    (MON_IDX, 'Понедельник'),
+    (TUE_IDX, 'Вторник'),
+    (WED_IDX, 'Среда'),
+    (THU_IDX, 'Четверг'),
+    (FRI_IDX, 'Пятница'),
+    (SAT_IDX, 'Суббота'),
+    (SUN_IDX, 'Воскресенье')
 )
 WEEKDAYS_DICT = dict(WEEKDAYS)
 
 
 def date_range_to_str(date_from, date_to, can_be_one_day_long=False):
     """
     Возвращает строку формата "с дд.мм.гггг [по дд.мм.гггг]",
@@ -64,22 +64,22 @@
     date_from = validate_year(date_from)
     date_to = validate_year(date_to)
     if date_from and date_to:
         assert date_from <= date_to
         if date_from == date_to:
             result = fmt(date_from)
         else:
-            result = u'с %s по %s' % (fmt(date_from), fmt(date_to))
+            result = 'с %s по %s' % (fmt(date_from), fmt(date_to))
     else:
         if can_be_one_day_long:
             result = fmt(date_from or date_to or None)
         elif date_from:
-            result = u'с %s' % fmt(date_from)
+            result = 'с %s' % fmt(date_from)
         elif date_to:
-            result = u'по %s' % fmt(date_to)
+            result = 'по %s' % fmt(date_to)
     return result
 
 
 def iter_days_between(date_from, date_to, odd_weeks_only=False):
     """
     Генератор дат в промежутке между указанными (включая границы).
 
@@ -162,15 +162,15 @@
     :param date: Дата, определяющая неделю. Значение по умолчанию - текущая
         дата.
     :type date: datetime.date or None
 
     :param weekday_names: Список или словарь наименований дней недели.
     :type weekday_names: dict, list
 
-    :return: Кортеж из кортежей вида (u'Название дня недели', дата).
+    :return: Кортеж из кортежей вида ('Название дня недели', дата).
     :rtype: tuple
     """
     weekday_names = weekday_names or WEEKDAYS_DICT
 
     return tuple(
         (weekday_names[day.weekday()], day)
         for day in get_week_dates(date)
```

### Comparing `educommon-2.20.0/src/educommon/utils/db/__init__.py` & `educommon-3.0.0/src/educommon/utils/db/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,67 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from functools import reduce
-from itertools import groupby
-from operator import or_
-
-from django.apps import apps
-from django.db import models
-from django.db import router
-from django.db.models.base import Model
-from django.db.models.deletion import Collector
-from django.db.models.fields.related import RelatedField
-from django.db.models.query_utils import Q
-from m3_django_compat import get_related
-from objectpack.models import ModelProxy
-import six
+from functools import (
+    reduce,
+)
+from itertools import (
+    groupby,
+)
+from operator import (
+    or_,
+)
+
+from django.apps import (
+    apps,
+)
+from django.db import (
+    models,
+    router,
+)
+from django.db.models.base import (
+    Model,
+)
+from django.db.models.deletion import (
+    Collector,
+)
+from django.db.models.fields.related import (
+    RelatedField,
+)
+from django.db.models.query_utils import (
+    Q,
+)
+from m3_django_compat import (
+    get_related,
+)
+
+from objectpack.models import (
+    ModelProxy,
+)
 
 
 def get_field(obj, field_name):
-    u"""Возвращает поле модели c учетом внешних ключей.
+    """Возвращает поле модели c учетом внешних ключей.
 
     ::
 
       get_field(obj, 'person.user.username')
 
     :param basestring field_name: Имя поля.
 
     :rtype: django.db.model.fields.Field
     """
-    name, _, nested = field_name.partition(u'.')
+    name, _, nested = field_name.partition('.')
     field = obj._meta.get_field(name)
     if nested:
         assert isinstance(field, models.ForeignKey)
         return get_field(get_related(field).parent_model, nested)
     else:
         return field
 
 
 def get_related_fields(model, skip_func=None):
-    u"""Возвращает поля моделей системы, ссылающихся на указанную модель.
+    """Возвращает поля моделей системы, ссылающихся на указанную модель.
 
     :param model: Модель, для которой будут найдены все зависимые поля.
     :type model: django.db.models.base.Model
 
     :param skip_func: Функция исключения, в которой будет определяться
         исключаемые поля.
     :type skip_func: lambda
@@ -60,15 +79,15 @@
                     issubclass(model, get_related(field).parent_model) and
                     (not skip_func or not skip_func(field))
                 ):
                     yield field
 
 
 def get_related_instances(obj, collapse=True, skip_func=None):
-    u"""Возвращает связанные с ``obj`` объекты.
+    """Возвращает связанные с ``obj`` объекты.
 
     :param obj: Объект, для которого будет осуществляться поиск связанных
         объектов.
     :type obj: django.db.models.base.Model
 
     :param bool collapse: Флаг, указывающий на необходимость "объединения"
         ссылок на объект. В тех случаях, когда в объекте модели есть несколько
@@ -172,15 +191,15 @@
     collector = Collector(
         using=router.db_for_write(obj.__class__, instance=obj)
     )
     collector.collect((obj,))
     # Коллектор содержит ссылку на obj, удалим сам объект из коллектора
     collector.data[obj.__class__].remove(obj)
 
-    for model, related_objects in six.iteritems(collector.data):
+    for model, related_objects in collector.data.items():
         if all((
             getattr(model, 'display_related_error', True),
             related_objects
         )):
             key = '.'.join((
                 model._meta.app_label,
                 model._meta.object_name,
```

### Comparing `educommon-2.20.0/src/educommon/utils/db/postgresql.py` & `educommon-3.0.0/src/educommon/utils/db/postgresql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from contextlib import closing
-
-from django.db import connections
-from django.db.utils import ProgrammingError
-import six
+from contextlib import (
+    closing,
+)
+
+from django.db import (
+    connections,
+)
+from django.db.utils import (
+    ProgrammingError,
+)
 
 
 def is_extension_exists(alias, name):
-    u"""Возвращает True, если в БД доступно расширение с указанным именем.
+    """Возвращает True, если в БД доступно расширение с указанным именем.
 
     :param str alias: Алиас базы данных (напр. ``'default'``).
     :param str name: Имя расширения.
 
     :rtype: bool
     """
     with closing(connections[alias].cursor()) as cursor:
@@ -21,15 +23,15 @@
             "SELECT 1 FROM pg_extension WHERE extname = %s",
             (name,)
         )
         return cursor.fetchone() is not None
 
 
 def create_extension(alias, name, quite=False):
-    u"""Создает в БД расширение PostgreSQL.
+    """Создает в БД расширение PostgreSQL.
 
     :param str alias: Алиас базы данных (напр. ``'default'``).
     :param str name: Имя расширения.
     :param bool quite: Флаг, указывающий на необходимость генерации исключения
         при невозможности создания расширения (отсутствии соответствующих
         прав).
 
@@ -44,37 +46,36 @@
                 return False
             else:
                 raise
         else:
             return True
 
 
-class Lock(object):
-
-    u"""Блокировка с помощью функции PostgreSQL ``pg_advisory_lock``.
+class Lock:
+    """Блокировка с помощью функции PostgreSQL ``pg_advisory_lock``.
 
     .. seealso::
 
        `Функции управления рекомендательными блокировками <https://postgrespro\
        .ru/docs/postgrespro/9.5/functions-admin.html#FUNCTIONS-ADVISORY-LOCKS>`
     """
 
     def __init__(self, alias, key):
-        u"""Инициализация экземпляра.
+        """Инициализация экземпляра.
 
         :param str alias: Алиас базы данных.
 
         :param key: Идентификатор блокировки.
         :type key: str or int
         """
         assert alias in connections, alias
 
         self.alias = alias
 
-        if isinstance(key, six.string_types):
+        if isinstance(key, str):
             self.key = hash(key)
         else:
             self.key = int(key)
 
     @property
     def _connection(self):
         return connections[self.alias]
```

### Comparing `educommon-2.20.0/src/educommon/utils/fonts/Arial.ttf` & `educommon-3.0.0/src/educommon/utils/fonts/Arial.ttf`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/fonts/Calibri.ttf` & `educommon-3.0.0/src/educommon/utils/fonts/Calibri.ttf`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/fonts/Tahoma.ttf` & `educommon-3.0.0/src/educommon/utils/fonts/Tahoma.ttf`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/fonts/__init__.py` & `educommon-3.0.0/src/educommon/utils/fonts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# coding: utf-8
-u"""Средства для работы со шрифтами."""
-from __future__ import absolute_import
-
+"""Средства для работы со шрифтами."""
 import os.path
 
-from PIL import ImageFont
+from PIL import (
+    ImageFont,
+)
 
 
 # Мнемоники для шрифтов
 ARIAL = 1
 TAHOMA = 2
 CALIBRI = 3
 
@@ -20,52 +19,52 @@
         (CALIBRI, 'Calibri.ttf'),
         (TAHOMA, 'Tahoma.ttf'),
     )
 }
 
 
 def get_font(font, size=10):
-    u"""Возвращает шрифт указанного семейства.
+    """Возвращает шрифт указанного семейства.
 
     :param int font: Поддерживаемое модулем семейство шрифтов.
     :param int size: Размер шрифта.
 
     :rtype: :class:`PIL.ImageFont.FreeTypeFont`
     """
     assert font in _FONT_FILES, font
 
     file_path = _FONT_FILES[font]
 
     return ImageFont.truetype(file_path, size, encoding='utf-8')
 
 
 def _split_word(font, word, max_width):
-    u"""Разбивает слово на две части.
+    """Разбивает слово на две части.
 
     Причем первая часть слова содержит наибольшее количество символов
     шрифта font от начала слова, которое умещается в max_width пикселей.
 
     :param font: Шрифт.
     :type font: :class:`PIL.ImageFont.FreeTypeFont`
 
-    :param unicode word: Слово, которое требуется разбить.
+    :param str word: Слово, которое требуется разбить.
     :param int max_width: Максимальная длина строки в пикселях.
 
     :rtype: tuple: (<Часть слова, умещающаяся в max_width>, <остаток>).
     """
     def _split_index(index, max_index=None):
-        u"""Рекурсивно разбивает слово на две части.
+        """Рекурсивно разбивает слово на две части.
 
         :param int index: Индекс текущего символа.
         :param int max_index: Индекс символа, до которого ширина строки
                               больше максимальной.
         """
         index = int(index)
-        assert index > 0, (u'Ширины строки не хватает, '
-                           u'чтобы поместить один символ')
+        assert index > 0, ('Ширины строки не хватает, '
+                           'чтобы поместить один символ')
 
         # определяем ширину слова в пикселях
         width, _ = font.getsize(word[:index])
 
         if width > max_width:
 
             if index == max_index:
@@ -94,15 +93,15 @@
         return index
 
     idx = _split_index(len(word))
     return word[:idx], word[idx:]
 
 
 def split_text(text, font, max_width):
-    u"""Разбивает текст на строки с учетом максимальной ширины строки.
+    """Разбивает текст на строки с учетом максимальной ширины строки.
 
     Разбиение осуществляется по словам. Если очередное слово не входит в
     строку, то выполняется перенос строки.
 
     :param unicode text: Текст, подлежащий разбиению на строки.
 
     :param font: Шрифт.
@@ -113,23 +112,23 @@
     :rtype: list
     """
     words = text.split(' ')
     string = []
     strings = [string]
     while words:
         string.append(words[0])
-        width, _ = font.getsize(u' '.join(string))
+        width, _ = font.getsize(' '.join(string))
         if width >= max_width:
             if len(string) == 1:
                 word, tail = _split_word(font, words[0], max_width)
                 if len(tail) > 0:
                     words[0] = tail
                 else:
                     words.pop(0)
                 string[0] = word
             else:
                 string.pop()
             string = []
             strings.append(string)
         else:
             words.pop(0)
-    return tuple(u' '.join(s) for s in strings if s)
+    return tuple(' '.join(s) for s in strings if s)
```

### Comparing `educommon-2.20.0/src/educommon/utils/licence/__init__.py` & `educommon-3.0.0/src/educommon/utils/licence/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
 import os.path
 
-from django.core.exceptions import ImproperlyConfigured
-from lxml import etree
-import six
-
-from educommon.utils.misc import cached_property
-from educommon.utils.xml import get_text
-from educommon.utils.xml import load_xml_document
+from django.core.exceptions import (
+    ImproperlyConfigured,
+)
+from lxml import (
+    etree,
+)
+
+from educommon.utils.misc import (
+    cached_property,
+)
+from educommon.utils.xml import (
+    get_text,
+    load_xml_document,
+)
 
 
 class LicenceError(Exception):
+    """Ошибка проверки файла лицензии."""
 
-    u"""Ошибка проверки файла лицензии."""
-
-
-class Licence(object):
 
-    u"""Базовый класс лицензии."""
+class Licence:
+    """Базовый класс лицензии."""
 
     def __init__(self, licence_file_path, schema_file_path, config,
                  params_root='//BarsLicence/LicenceData'):
-        u"""Инициализация экземпляра класса.
+        """Инициализация экземпляра класса.
 
         :param basestring licence_file_path: Путь к файлу лицензии.
         :param basestring schema_file_path: Путь к файлу c XML-схемой.
             Если указан, то файл лицензии будет проверяться на соответсвие этой
             схеме.
         :param basestring params_root: XPath-выражение для извлечения корневого
             элемента с параметрами лицензии.
@@ -63,40 +64,40 @@
         :param basestring file_path: Путь к файлу.
 
         :raises django.core.exceptions.ImproperlyConfigured: если файл не
             существует, либо к нему нет доступа.
         """
         if not os.path.exists(file_path):
             raise ImproperlyConfigured(
-                u'Licence file not found: ' + file_path
+                'Licence file not found: ' + file_path
             )
 
         if not os.access(file_path, os.R_OK):
             raise ImproperlyConfigured(
-                u"Can't read licence file: " + file_path
+                "Can't read licence file: " + file_path
             )
 
     @cached_property
     def _params_elements(self):
         """Возвращает XML-дерево файла лицензии.
 
         :rtype: list of lxml.etree._Element
 
         :raises LicenceError: Если при проверке возникли ошибки.
         """
         self._check_file(self.licence_file_path)
         if self.schema_file_path:
             self._check_file(self.schema_file_path)
-            schema_uri = u'file://' + self.schema_file_path
+            schema_uri = 'file://' + self.schema_file_path
         else:
             schema_uri = None
 
         try:
             document_tree = load_xml_document(
-                document_uri=u'file://' + self.licence_file_path,
+                document_uri='file://' + self.licence_file_path,
                 schema_uri=schema_uri,
             )
         except etree.XMLSyntaxError as error:
             raise LicenceError(
                 'Error parsing licence XML document {}:\n{}'
                 .format(self.licence_file_path, str(error))
             )
@@ -115,15 +116,15 @@
 
         :rtype: dict
         """
         params_root_element = self._params_elements.pop()
 
         return {
             param_name: converter(get_text(params_root_element.xpath(xpath)))
-            for param_name, (xpath, converter) in six.iteritems(self._config)
+            for param_name, (xpath, converter) in self._config.items()
         }
 
     @cached_property
     def plugins(self):
         """Список разрешенных к использованию плагинов.
 
         :rtype: set
```

### Comparing `educommon-2.20.0/src/educommon/utils/licence/converters.py` & `educommon-3.0.0/src/educommon/utils/licence/converters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from datetime import datetime
+from datetime import (
+    datetime,
+)
 
 
 def get_string_value(text):
-    u"""Возвращает строковое значение."""
-    text = text.replace(u'\n', u' ')
-    while text.find(u'  ') != -1:
-        text = text.replace(u'  ', u' ')
+    """Возвращает строковое значение."""
+    text = text.replace('\n', ' ')
+    while text.find('  ') != -1:
+        text = text.replace('  ', ' ')
     return text
 
 
 def get_int_value(text):
-    u"""Возвращает числовое значение."""
+    """Возвращает числовое значение."""
     text = get_string_value(text)
     result = None
     if text:
         try:
             result = int(text)
         except ValueError:
             pass
     return result
 
 
 def get_date_value(text, xml_format=False):
-    u"""Возвращает значение даты.
+    """Возвращает значение даты.
 
     :param text basestring: Строковое значение поля.
     :param boolean xml_format: Флаг формата даты, принятой для типа данных
         date в XML Schema.
     """
     text = get_string_value(text)
     date_format = '%Y.%m.%d' if xml_format else '%d.%m.%Y'
     return datetime.strptime(text, date_format).date()
 
 
 def get_bool_value(text):
-    u"""Возвращает булевое значение."""
+    """Возвращает булевое значение."""
     text = get_string_value(text)
     return True if text.lower() == 'true' else False
```

### Comparing `educommon-2.20.0/src/educommon/utils/misc.py` & `educommon-3.0.0/src/educommon/utils/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import hashlib
 
-from six import text_type
-
-from educommon import Undefined
+from educommon import (
+    Undefined,
+)
 
 
 class cached_property(property):
-
-    u"""Кешируемое свойство.
+    """Кешируемое свойство.
 
     В отличие от :class:`django.utils.functional.cached_property`, наследуется
     от property и копирует строку документации, что актуально при генерации
     документации средствами Sphinx.
     """
 
     def __init__(self, method):
@@ -29,15 +25,15 @@
         if self.fget.__name__ not in instance.__dict__:
             instance.__dict__[self.fget.__name__] = self.fget(instance)
 
         return instance.__dict__[self.fget.__name__]
 
 
 def get_nested_attr(obj, attr, default=Undefined):
-    u"""Возвращает значение вложенного атрибута объекта.
+    """Возвращает значение вложенного атрибута объекта.
 
     .. code-block:: python
 
        obj = datetime(2015, 1, 1, 0, 0, 0)
        get_nested_attr(obj, 'date().year')  # 2015
        get_nested_attr(obj, 'date().year.__class__')  # int
     """
@@ -71,34 +67,33 @@
                     )
                 )
 
     return nested_object
 
 
 def md5sum(filepath):
-    u"""Возвращает контрольную сумму MD5 указанного файла.
+    """Возвращает контрольную сумму MD5 указанного файла.
 
     :param basestring filepath: Путь к файлу.
 
     :rtype: str
     """
     md5 = hashlib.md5()
     with open(filepath, 'r') as infile:
         while True:
             data = infile.read(1024)
             if not data:
                 break
-            if isinstance(data, text_type):
+            if isinstance(data, str):
                 data = data.encode('utf-8')
             md5.update(data)
     return md5.hexdigest()
 
 
-class NoOperationCM(object):
-
+class NoOperationCM:
     """Менеджер контекта, не выполняющий никаких действий."""
 
     def __enter__(self):
         return self
 
     def __exit__(self, ex_type, ex_inst, traceback):
         pass
```

### Comparing `educommon-2.20.0/src/educommon/utils/patches.py` & `educommon-3.0.0/src/educommon/utils/patches.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-# coding: utf-8
-u"""Патчи для встроенных и библиотечных объектов."""
-from __future__ import absolute_import
-
+"""Патчи для встроенных и библиотечных объектов."""
 import sys
 
-import six
-
 
 class AssertionError(__builtins__['AssertionError']):
 
     __doc__ = __builtins__['AssertionError'].__doc__
 
     def __init__(self, message='', *args, **kwargs):
-        u"""Кодирует unicode сообщение в utf-8."""
-        if isinstance(message, six.text_type):
+        """Кодирует unicode сообщение в utf-8."""
+        if isinstance(message, str):
             message = message.encode('utf-8')
         super(AssertionError, self).__init__(message, *args, **kwargs)
 
 
 def patch_utf8_assertion_error():
-    u"""Кодирует сообщения AssertionError в utf-8.
+    """Кодирует сообщения AssertionError в utf-8.
 
     Т.к. обычно используемая кодировка в терминале utf-8, а python по
     какой-то причине не кодирует сообщения в кодировку stderr, то сообщения
     исключений выводятся в виде кодов символов.
 
     Чтобы избежать этого, мы принудительно конвертируем unicode строки
     в utf-8.
```

### Comparing `educommon-2.20.0/src/educommon/utils/plugins.py` & `educommon-3.0.0/src/educommon/utils/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,38 @@
-# coding: utf-8
-from collections import defaultdict
-from functools import wraps
-from inspect import isclass
-from types import FunctionType
-from types import MethodType
-
-from django.apps import apps
-from django.core.exceptions import ImproperlyConfigured
-from six import PY3
-from six import with_metaclass
-
-from educommon.utils import SingletonMeta
+from collections import (
+    defaultdict,
+)
+from functools import (
+    lru_cache,
+    wraps,
+)
+from inspect import (
+    isclass,
+)
+from types import (
+    FunctionType,
+    MethodType,
+)
+
+from django.apps import (
+    apps,
+)
+from django.core.exceptions import (
+    ImproperlyConfigured,
+)
+
+from educommon.utils import (
+    SingletonMeta,
+)
 
 
 __all__ = ['extender_for']
 
 
-class _ExtenderRegistry(object, with_metaclass(SingletonMeta)):
+class _ExtenderRegistry(metaclass=SingletonMeta):
 
     """Реестр расширителей классов.
 
     Обеспечивает работу декораторов
     :func:`~educommon.utils.plugins.extender_for` и
     :func:`~educommon.utils.plugins.extendable`.
 
@@ -68,30 +80,30 @@
 
 
 _extender_registry = _ExtenderRegistry()
 
 
 def _function_types():
     """Возвращает типы функций и методов, доступных для расширения."""
-    from m3_django_compat import WrapperDescriptorType
-    from m3_django_compat import MethodWrapperType
-    from m3_django_compat import MethodDescriptorType
+    from m3_django_compat import (
+        MethodDescriptorType,
+        MethodWrapperType,
+        WrapperDescriptorType,
+    )
 
     return (
         FunctionType,
         MethodType,
         WrapperDescriptorType,
         MethodWrapperType,
         MethodDescriptorType
     )
 
 
-if PY3:
-    from functools import lru_cache
-    _function_types = lru_cache(maxsize=1)(_function_types)
+_function_types = lru_cache(maxsize=1)(_function_types)
 
 
 def extender_for(*extendables):
     """Помечает класс, как расширитель для указанных классов.
 
     Имена расширяемых методов должны быть указаны в ``extends_methods``. Эти
     методы будут обернуты декоратором. Расширение staticmethod и classmethod
@@ -109,15 +121,15 @@
         3. Результат работы последнего расширителя класса возвращается в
            качестве результата расширяемого метода.
 
     .. code-block:: python
        :caption: Пример использования
 
        @extender_for(ListWindow, AddWindow, EditWindow):
-       class WindowExtender(object):
+       class WindowExtender:
 
            extends_methods = ('set_params',)
 
            @staticmethod
            def set_params(window, result, params):
                window.width, window.height = 1000, 1000
                return result
@@ -165,15 +177,17 @@
            def set_params(self, params):
                ...
     """
     assert isinstance(func, _function_types()), func
 
     @wraps(func)
     def wrapper(self, *args, **kwargs):
-        from m3_django_compat import WrapperDescriptorType
+        from m3_django_compat import (
+            WrapperDescriptorType,
+        )
         unbound_types = (FunctionType, WrapperDescriptorType,)
 
         assert all((
             isinstance(func, unbound_types),
             not isclass(self))
         ), 'Нельзя расширить staticmethod и classmethod'
```

### Comparing `educommon-2.20.0/src/educommon/utils/registry.py` & `educommon-3.0.0/src/educommon/utils/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# coding: utf-8
-
-
-class ModelHandlerRegistry(object):
+class ModelHandlerRegistry:
     """Класс для хранения обработчиков модели."""
 
     def __init__(self, handlers):
         """
         :param handlers: Словарь с обработчиками модели, т.е.
             словарь, где ключ - django модель, значение -
             функция-обработчик (вызываемый объект) для данной модели
```

### Comparing `educommon-2.20.0/src/educommon/utils/seqtools.py` & `educommon-3.0.0/src/educommon/utils/seqtools.py`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/serializer.py` & `educommon-3.0.0/src/educommon/utils/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-# coding: utf-8
-u"""Инструменты для сериализации моделей."""
-from __future__ import absolute_import
+"""Инструменты для сериализации моделей."""
+from collections import (
+    defaultdict,
+)
+
+from django.core import (
+    serializers,
+)
+from django.db.models import (
+    ForeignKey,
+)
+from django.db.models.query import (
+    QuerySet,
+)
+from m3_django_compat import (
+    ModelOptions,
+    get_related,
+)
 
-from collections import defaultdict
 
-from django.core import serializers
-from django.db.models import ForeignKey
-from django.db.models.query import QuerySet
-from m3_django_compat import ModelOptions
-from m3_django_compat import get_related
-
-
-class SerializeQueue(object):
-
-    u"""Выборочная сериализация данных из разных моделей в JSON.
+class SerializeQueue:
+    """Выборочная сериализация данных из разных моделей в JSON.
 
     Производит сериализацию моделей со всеми зависимостями от них в фикстуру,
     которую затем можно загрузить через команду loaddata
 
     Пример применения:
 
     # всё, что было раньше этой даты не будет сохранено и восстановлено
@@ -72,53 +78,53 @@
     ForeignKey и не попасть под фильтрацию.
     Например, в ЭШ, модель SubjectPlan (КТП) может иметь ссылку на ClassYear,
     а может и нет.
 
     """
 
     def __init__(self, include=None, exclude=None, **kwargs):
-        u"""Накопление и сериализация
+        """Накопление и сериализация
 
         :param include: модели и объекты для условия "__in"
         :param exclude: модели и объекты для операции ".exclude()"
         """
         # контейнер для добавляемых объектов
         self._objects = []
         # кеш уже добавленных моделей и объектов, чтобы избежать повторов
         self._model_cache = defaultdict(list)
         # условия вхождения - список моделей и инстансов
         self._include_conditions = {} if include is None else include
         # условия исключения - список моделей и инстансов
         self._exclude_conditions = {} if exclude is None else exclude
 
     def _object_in_cache(self, model_name, obj_id):
-        u"""Проверить наличие объекта в кеше."""
+        """Проверить наличие объекта в кеше."""
         objects = self._model_cache.get(model_name)
         if objects:
             return obj_id in objects
         else:
             return False
 
     def _add_object_to_cache(self, model_name, obj_id):
-        u"""Добавить объект в кеш."""
+        """Добавить объект в кеш."""
         self._model_cache[model_name].append(obj_id)
 
     def _ext_filter(self, query_set):
-        u"""Фильтрация кверисета c учётом условий вхождения и исключения
+        """Фильтрация кверисета c учётом условий вхождения и исключения
 
         :param query_set:
         :return:
         """
         fields = self.all_foreign_keys(query_set.model)
         for field, rel_model in fields:
             # добавление условий по внешним ключам
             attname = field.attname
             if attname.endswith('_id'):
-                attname = attname.replace(u'_id', u'')
-                attname = u'%s__in' % attname
+                attname = attname.replace('_id', '')
+                attname = '%s__in' % attname
             # добавление фильтра вхождения
             objects = self._include_conditions.get(rel_model._meta.object_name)
             if objects:
                 query_set = query_set.filter(
                     **{attname: objects}
                 )
             # добавление фильтра исключения
@@ -128,51 +134,51 @@
                     **{attname: objects}
                 )
 
         return query_set
 
     @staticmethod
     def all_foreign_keys(model):
-        u"""Возвращает список внешних ссылок для заданной модели
+        """Возвращает список внешних ссылок для заданной модели
 
         :param model: Класс модели
         :return: список кортежей вида [(поле, ссылочная модель), ...]
         """
         return [
             (field, get_related(field).parent_model) for
             field in model._meta.fields
             if isinstance(field, ForeignKey)
         ]
 
     @staticmethod
     def related_objects(obj):
-        u""" Возвращает список кверисетов зависимых моделей
+        """ Возвращает список кверисетов зависимых моделей
 
         :param obj:
         :return:
         """
         _relations = ModelOptions(obj).get_all_related_objects()
         result = []
 
         for rel in _relations:
             _attname = rel.field.attname
             if _attname.endswith('_id'):
-                _attname = _attname.replace(u'_id', u'')
-            _attname = u'%s__pk' % _attname
+                _attname = _attname.replace('_id', '')
+            _attname = '%s__pk' % _attname
             # Пытаемся определить наличие зависимых объектов:
             rel_qs = rel.field.model.objects.filter(
                 **{str(_attname): obj.id}
             )
             if rel_qs.exists():
                 result.append(rel_qs)
 
         return result
 
     def add_objects(self, query_set, filtered=True):
-        u"""добавить объекты пачкой.
+        """Добавить объекты пачкой.
 
         :param query_set: Кверисет, возвращающий объекты моделей
         :param filtered: флаг, применять или нет общую фильтрацию
         :return:
         """
         assert isinstance(query_set, QuerySet), type(query_set)
 
@@ -181,15 +187,15 @@
         for obj in query_set:
             # добавить объект
             if not self._object_in_cache(str(obj.__class__), obj.id):
                 self._objects.append(obj)
                 self._add_object_to_cache(str(obj.__class__), obj.id)
 
     def add_related_objects(self, query_set, filtered=True):
-        u"""добавить объекты пачкой с учётом зависимых.
+        """Добавить объекты пачкой с учётом зависимых.
 
         :param query_set: Кверисет, возвращающий объекты моделей
         :param filtered: флаг, применять или нет общую фильтрацию
         """
         assert isinstance(query_set, QuerySet), type(query_set)
 
         if filtered:
@@ -202,14 +208,14 @@
                 self._add_object_to_cache(str(obj.__class__), obj.id)
             # затем добавить всех, кто на него ссылается
             for new_query_set in self.related_objects(obj):
                 # рекурсивно позвать себя
                 self.add_related_objects(new_query_set, filtered)
 
     def serialize(self, filename):
-        u"""Собственно, сериализация в файл
+        """Собственно, сериализация в файл
 
         :param filename: имя файла
         """
         data = serializers.serialize("json", self._objects, indent=4)
         with open(filename, 'wb') as json_out:
             json_out.write(data)
```

### Comparing `educommon-2.20.0/src/educommon/utils/storage.py` & `educommon-3.0.0/src/educommon/utils/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# coding: utf-8
-from abc import ABCMeta, abstractmethod
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
 
-import six
+from educommon.utils.registry import (
+    ModelHandlerRegistry,
+)
 
-from educommon.utils.registry import ModelHandlerRegistry
 
-
-class AbstractInstanceStorage(six.with_metaclass(ABCMeta, object)):
+class AbstractInstanceStorage(metaclass=ABCMeta):
     @abstractmethod
     def save(self, instance, **kwargs):
         """Сохранение данных для объекта модели."""
 
 
 class AbstractInstanceDataStorage(AbstractInstanceStorage):
     """Абстрактный класс для сохранения данных объекта модели.
```

### Comparing `educommon-2.20.0/src/educommon/utils/system.py` & `educommon-3.0.0/src/educommon/utils/system.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from importlib import import_module
-from inspect import currentframe
 import platform
+from importlib import (
+    import_module,
+)
+from inspect import (
+    currentframe,
+)
 
 import distro
 
 
 def is_in_migration_command():
-    u"""Возвращает True, если код выполняется в рамках миграций Django.
+    """Возвращает True, если код выполняется в рамках миграций Django.
 
     :rtype: bool
     """
-    from django.core.management import ManagementUtility
+    from django.core.management import (
+        ManagementUtility,
+    )
 
     def is_in_command(command):
         frame = currentframe()
         while frame:
             if 'self' in frame.f_locals:
                 self_object = frame.f_locals['self']
                 if isinstance(self_object, command):
@@ -43,15 +46,15 @@
         if is_in_command(import_module(module_name).Command):
             return True
 
     return False
 
 
 def get_postgresql_version(connection):
-    u"""Возвращает версию PostgreSQL.
+    """Возвращает версию PostgreSQL.
 
     :param connection: :class:`django.db.DefaultConnectionProxy`
     :rtype: tuple
     """
     with connection.cursor() as cursor:
         if cursor.db.vendor != 'postgresql':
             raise RuntimeError(
@@ -62,28 +65,28 @@
             cursor.db.pg_version // 10000,
             cursor.db.pg_version % 10000 // 100,
             cursor.db.pg_version % 100,
         )
 
 
 def get_os_version():
-    u"""Возвращает строку с описанием дистрибутива (релиза) и версии ОС."""
+    """Возвращает строку с описанием дистрибутива (релиза) и версии ОС."""
     result = 'Unknown'
     system = platform.system()
 
     if system == 'Linux':
         name, version, codename = distro.linux_distribution()
-        result = u'{} {}'.format(name, version)
+        result = '{} {}'.format(name, version)
         if codename:
-            result = u'{} ({})'.format(result, codename)
+            result = '{} ({})'.format(result, codename)
 
     elif system == 'Windows':
         release, version, sp, _ = platform.win32_ver()
-        result = u'{} {}'.format(release, version)
+        result = '{} {}'.format(release, version)
         if sp:
-            result = u'{}, SP {}'.format(result, sp)
+            result = '{}, SP {}'.format(result, sp)
 
     elif system == 'Darwin':
         release, version, arch = platform.mac_ver()
-        result = u'MacOS {} ({})'.format(release, arch)
+        result = 'MacOS {} ({})'.format(release, arch)
 
     return result
```

### Comparing `educommon-2.20.0/src/educommon/utils/system_app/management/commands/delete_objects.py` & `educommon-3.0.0/src/educommon/utils/system_app/management/commands/delete_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,39 @@
-# coding: utf-8
-u"""Management-команда для удаления обьектов."""
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from collections import defaultdict
+"""Management-команда для удаления обьектов."""
 import sys
-
-from django.apps import apps
-from django.core import serializers
-from django.core.management import BaseCommand
-from django.core.management import CommandError
-from django.core.management import get_commands
-from django.core.management import handle_default_options
-from django.core.management import load_command_class
-from django.core.management.base import SystemCheckError
-from django.db import connections
-from django.utils.encoding import force_text
-import six
+from collections import (
+    defaultdict,
+)
+
+from django.apps import (
+    apps,
+)
+from django.core import (
+    serializers,
+)
+from django.core.management import (
+    BaseCommand,
+    CommandError,
+    get_commands,
+    handle_default_options,
+    load_command_class,
+)
+from django.core.management.base import (
+    SystemCheckError,
+)
+from django.db import (
+    connections,
+)
+from django.utils.encoding import (
+    force_text,
+)
 
 
 def call_custom_command(command_name, *args, **options):
-    u"""Осуществляет вызов команды с регистрацией неизвестных аргументов."""
+    """Осуществляет вызов команды с регистрацией неизвестных аргументов."""
     if isinstance(command_name, BaseCommand):
         # Command object passed in.
         command = command_name
         command_name = command.__class__.__module__.split('.')[-1]
     else:
         # Load the command object by name.
         try:
@@ -47,15 +56,15 @@
             '-', '_'): s_opt.dest
         for s_opt in parser._actions if s_opt.option_strings
     }
     arg_options = {opt_mapping.get(key, key): value
                    for key, value in options.items()}
     options, un_options = parser.parse_known_args(args)
     for opt in un_options:
-        if not isinstance(opt, six.text_type):
+        if not isinstance(opt, str):
             opt = opt.decode(sys.stdout.encoding)
         com = opt.split('=')
         com = com[0]
         if '__in' in com:
             parser.add_argument(com, action='append')
         elif '__isnull' in com:
             parser.add_argument(com, action='store')
@@ -68,26 +77,25 @@
     if 'skip_checks' not in options:
         defaults['skip_checks'] = True
 
     return command.execute(*args, **defaults)
 
 
 class Command(BaseCommand):
-
-    u"""Удаление групп и учащихся за заданный период в заданном ОУ."""
+    """Удаление групп и учащихся за заданный период в заданном ОУ."""
 
     def run_from_argv(self, argv):
         # переопределен в связи с регистрацией аргументов
         # при вызове самой команды
         self._called_from_command_line = True
         parser = self.create_parser(argv[0], argv[1])
 
         options, un_options = parser.parse_known_args(argv[2:])
         for opt in un_options:
-            if not isinstance(opt, six.text_type):
+            if not isinstance(opt, str):
                 opt = opt.decode(sys.stdout.encoding)
             com = opt.split('=')
             com = com[0]
             if '__in' in com:
                 parser.add_argument(com, action='append')
             elif '__isnull' in com:
                 parser.add_argument(com, action='store')
@@ -111,50 +119,50 @@
                 self.stderr.write('%s: %s' % (e.__class__.__name__, e))
             sys.exit(1)
         finally:
             connections.close_all()
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '--count', action='count', help=u'Количество удаляемых обьектов'
+            '--count', action='count', help='Количество удаляемых обьектов'
         )
         parser.add_argument(
-            '--model', type=str, required=True, help=u'Модель для удаления'
+            '--model', type=str, required=True, help='Модель для удаления'
         )
         parser.add_argument(
-            '--data', action='count', help=u'Вернуть json удаляемых обьектов'
+            '--data', action='count', help='Вернуть json удаляемых обьектов'
         )
 
     @staticmethod
     def find_filter(options, ignore_opt=()):
-        u"""Возвращает lookup для поиска по модели.
+        """Возвращает lookup для поиска по модели.
 
         :param options: Опции, переданные в команду.
         :type request: dict
         :param ignore_opt: Кортеж игнорируемых значений при построении фильтра.
         :type ignore_opt: tuple
         :rtype : dict
         """
         lookup = dict()
-        for key, value in six.iteritems(options):
+        for key, value in options.items():
             if key and key not in ignore_opt and value:
                 if '__in' in key:
                     lookup[key] = value[0].split(',')
                 elif '__isnull' in key:
                     if value == 'False':
                         lookup[key] = False
                     else:
                         lookup[key] = True
                 else:
                     lookup[key] = value
         return lookup
 
     @staticmethod
     def find_model(model_name, app_name=None):
-        u"""Возвращает модель, либо список моделей для приложения.
+        """Возвращает модель, либо список моделей для приложения.
 
         А также вернет сообщение об ошибке, если такая возникла.
 
         :param model_name: Название искомой модели.
         :type request: str
         :param app_name: Название приложения.
         :type ignore_opt: str
@@ -166,51 +174,51 @@
         message = None
         model = None
         if app_name:
             try:
                 model = apps.get_model(app_name, model_name)
             except LookupError:
                 message = (
-                    u'Модели {} в приложении '
-                    u'{} не найдено.'.format(model_name, app_name)
+                    'Модели {} в приложении '
+                    '{} не найдено.'.format(model_name, app_name)
                 )
             return model, message
         for app_config in apps.get_app_configs():
             try:
                 model = app_config.get_model(model_name)
                 models.append(model)
             except LookupError:
                 pass
 
         if len(models) > 1:
             model = None
             message = (
-                u'Невозможно однозначно определить модель, '
-                u'найдены похожие модели: \n'
+                'Невозможно однозначно определить модель, '
+                'найдены похожие модели: \n'
             )
-            message += u'\n'.join(str(model._meta) for model in models)
+            message += '\n'.join(str(model._meta) for model in models)
         elif not model:
-            message = u'Модели {} не найдено.'.format(model_name)
+            message = 'Модели {} не найдено.'.format(model_name)
         return model, message
 
     def process_count(self, deleted_objects):
-        u"""Выводит в stdout количество зависимых обьектов."""
+        """Выводит в stdout количество зависимых обьектов."""
         uniq_dict = defaultdict(set)
         for del_obj in deleted_objects:
             for model, model_objects in del_obj.get_related_objects():
                 for o in model_objects:
                     uniq_dict[
                         model.__name__ + ' ' + model._meta.verbose_name
                     ].add(o)
-        for model, objs in six.iteritems(uniq_dict):
-            display_mes = u'{} {}'.format(model, len(objs))
+        for model, objs in uniq_dict.items():
+            display_mes = '{} {}'.format(model, len(objs))
             self.stdout.write(display_mes)
 
     def process_data(self, deleted_objects):
-        u"""Выводит в stdout json зависимых обьектов."""
+        """Выводит в stdout json зависимых обьектов."""
         objs = []
         for instance in deleted_objects:
             for rel_model, rel_objs in instance.get_related_objects():
                 for obj in rel_objs:
                     objs.append(obj)
         data = serializers.serialize(
             'json', objs)
```

### Comparing `educommon-2.20.0/src/educommon/utils/ui.py` & `educommon-3.0.0/src/educommon/utils/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,90 +1,114 @@
-# coding: utf-8
-u"""Утилиты для работы с элементами управления (интерфейсами)."""
-from __future__ import absolute_import
-
-from datetime import datetime
-from datetime import time
+"""Утилиты для работы с элементами управления (интерфейсами)."""
 import inspect
 import os
-
-from django.conf import settings
-from django.db.models import TextField
-from django.db.models import Q
-from m3.actions.context import ActionContext
-from m3_ext.ui import all_components as ext
-from m3_ext.ui.icons import Icons
-from m3_ext.ui.panels.grids import ExtObjectGrid
-from objectpack.filters import CustomFilter
-from objectpack.filters import FilterByField as _FilterByField
-from objectpack.tools import modify
-from objectpack.tree_object_pack.ui import BaseObjectTree
-from objectpack.ui import BaseEditWindow
-from objectpack.ui import _create_control_for_field
-from objectpack.ui import anchor100 as obj_anchor100
-from objectpack.ui import deny_blank as obj_deny_blank
-from objectpack.ui import make_combo_box
-
-from educommon import ioc
-from educommon.utils.misc import cached_property
+from datetime import (
+    datetime,
+    time,
+)
+
+from django.conf import (
+    settings,
+)
+from django.db.models import (
+    Q,
+    TextField,
+)
+from m3.actions.context import (
+    ActionContext,
+)
+from m3_ext.ui import (
+    all_components as ext,
+)
+from m3_ext.ui.icons import (
+    Icons,
+)
+from m3_ext.ui.panels.grids import (
+    ExtObjectGrid,
+)
+
+from objectpack.filters import (
+    CustomFilter,
+    FilterByField as _FilterByField,
+)
+from objectpack.tools import (
+    modify,
+)
+from objectpack.tree_object_pack.ui import (
+    BaseObjectTree,
+)
+from objectpack.ui import (
+    BaseEditWindow,
+    _create_control_for_field,
+    anchor100 as obj_anchor100,
+    deny_blank as obj_deny_blank,
+    make_combo_box,
+)
+
+from educommon import (
+    ioc,
+)
+from educommon.utils.misc import (
+    cached_property,
+)
 
 
 def anchor100(*elements):
-    u"""Установка anchor='100%' для перечня компонент."""
+    """Установка anchor='100%' для перечня компонент."""
     return list(
         obj_anchor100(element)
         for element in elements
     )
 
 
 def deny_blank(*elements):
-    u"""Установка allow_blank=False для перечня компонент."""
+    """Установка allow_blank=False для перечня компонент."""
     return list(
         obj_deny_blank(element)
         for element in elements
     )
 
 
 def make_button(title, icon_cls, event, client_id):
-    u"""Создает кнопку, оповещающую компонент с client_id на событие event."""
+    """Создает кнопку, оповещающую компонент с client_id на событие event."""
     handler = "function() {Ext.getCmp('%s').fireEvent('%s');}" % (
         client_id, event)
 
     return ext.ExtButton(text=title, icon_cls=icon_cls, handler=handler)
 
 
 def formed(ctl, width=-1, label_width=100, **kwargs):
-    u"""Возращает control в контейнере."""
+    """Возращает control в контейнере."""
     cont = ext.ExtContainer(layout='form')
     cont.items.append(ctl)
     ctl.anchor = '100%'
     if width > 0:
         cont.width = width
     else:
         cont.flex = -width
     cont.label_width = label_width
     cont.anchor = '100%'
     return modify(cont, **kwargs)
 
 
 class ChoicesFilter(CustomFilter):
-    u"""Колоночный фильтр с выпадающим списком."""
+    """Колоночный фильтр с выпадающим списком."""
 
     def __init__(self, choices, *args, **kwargs):
-        u"""Метод инициализации.
+        """Метод инициализации.
 
         Добавляем значения для выбора и тип компонента.
         """
         self._choices = choices
         kwargs['xtype'] = 'combo'
 
         super(ChoicesFilter, self).__init__(*args, **kwargs)
 
     def get_script(self):
-        u"""Генерация кода компонента."""
+        """Генерация кода компонента."""
         if callable(self._choices):
             choices = self._choices()
         else:
             choices = self._choices
         control = make_combo_box(data=list(choices))
         control._put_config_value('filterName', self._uid)
         control._put_config_value('tooltip', self._tooltip or control.label)
@@ -110,15 +134,15 @@
         # Закомментировано, чтобы проставлять значение по-умолчанию
         # control.value = None
         return [control.render()]
 
 
 def reconfigure_grid_by_access(grid, can_add=False, can_edit=False,
                                can_delete=False, can_view=True):
-    u"""Перенастраивает грид в зависимости от прав доступа.
+    """Перенастраивает грид в зависимости от прав доступа.
 
     :param grid: Перенастраиваемый грид.
     :type grid: m3_ext.ui.panels.grids.ExtObjectGrid
 
     :param bool can_add: Определяет доступность функции добавления объектов.
     :param bool can_edit: Определяет доступность функции изменения объектов.
     :param bool can_delete: Определяет доступность функции удаления объектов.
@@ -127,28 +151,28 @@
     """
     assert isinstance(grid, ExtObjectGrid), type(grid)
     grid.read_only = False
     if not can_add:
         grid.url_new = None
     if not can_edit:
         if can_view:
-            grid.top_bar.button_edit.text = u'Просмотр'
+            grid.top_bar.button_edit.text = 'Просмотр'
             grid.top_bar.button_edit.icon_cls = Icons.APPLICATION_VIEW_DETAIL
 
             grid.top_bar.items.remove(grid.top_bar.button_edit)
             grid.top_bar.items.insert(0, grid.top_bar.button_edit)
         else:
             grid.url_edit = None
     if not can_delete:
         grid.url_delete = None
 
 
 def reconfigure_object_tree_by_access(grid, can_add=False, can_edit=False,
                                       can_delete=False, can_view=True):
-    u"""Перенастраивает древовидный грид в зависимости от прав доступа.
+    """Перенастраивает древовидный грид в зависимости от прав доступа.
 
     :param grid: Перенастраиваемый грид.
     :type grid: objectpack.tree_object_pack.ui.BaseObjectTree
 
     :param bool can_add: Определяет доступность функции добавления объектов.
     :param bool can_edit: Определяет доступность функции изменения объектов.
     :param bool can_delete: Определяет доступность функции удаления объектов.
@@ -157,25 +181,24 @@
     """
     assert isinstance(grid, BaseObjectTree), type(grid)
 
     if not can_add:
         grid.action_new = None
     if not can_edit:
         if can_view:
-            grid.top_bar.button_edit.text = u'Просмотр'
+            grid.top_bar.button_edit.text = 'Просмотр'
             grid.top_bar.button_edit.icon_cls = Icons.APPLICATION_VIEW_DETAIL
         else:
             grid.action_edit = None
     if not can_delete:
         grid.action_delete = None
 
 
 class FilterByField(_FilterByField):
-
-    u"""FilterByField c возможностью расширения контрола фильтра.
+    """FilterByField c возможностью расширения контрола фильтра.
 
     Дополнительно добавляет ActionContext, необходимый в случае если
     контролом является ExtDictSelectField.
     """
 
     def __init__(self, *args, **kwargs):
         self._control_creator = kwargs.pop('control_creator', None)
@@ -204,24 +227,23 @@
         control.hide_clear_trigger = False
         return control
 
     def get_script(self):
         return [self.get_control().render()]
 
 
-class DatetimeFilterCreator(object):
-
-    u"""Класс, создающий колоночный фильтр по интервалу для datetime поля.
+class DatetimeFilterCreator:
+    """Класс, создающий колоночный фильтр по интервалу для datetime поля.
 
     Поддерживает значения по умолчанию.
     """
 
     def __init__(self, model, field_name,
                  get_from=lambda: None, get_to=lambda: None):
-        u"""Фильтр по интервалу для datetime поля.
+        """Фильтр по интервалу для datetime поля.
 
         :param django.db.models.Model model: модель для фильтра.
         :param str field_name: имя поля модели.
         :param callable get_from: возвращает дату по умолчанию для фильтра "С".
         :param callable get_to: возвращает дату по умолчанию для фильтра "По".
 
         Значения по умолчанию передаются в качестве callable, чтобы они
@@ -237,15 +259,15 @@
         self.defaults = {
             'from': get_from,
             'to': get_to,
         }
 
     @cached_property
     def filter(self):
-        u"""Фильтр для колонки.
+        """Фильтр для колонки.
 
         :return Группа колоночных фильтров для грида
         :rtype objectpack.filters.FilterGroup
         """
         observer = ioc.get('observer')
 
         return (
@@ -255,36 +277,36 @@
                 control_creator=lambda: ext.ExtDateField(
                     value=self.defaults['from']()
                 ),
                 field_name=self.field_name,
                 lookup=lambda dt: Q(**{
                     self.field_name + '__gte': datetime.combine(dt, time(0))
                 }),
-                tooltip=u'С',
+                tooltip='С',
             ) & FilterByField(
                 self.model,
                 model_register=observer,
                 control_creator=lambda: ext.ExtDateField(
                     value=self.defaults['to']()
                 ),
                 field_name=self.field_name,
                 lookup=lambda dt: Q(**{
                     self.field_name + '__lte': datetime.combine(
                         dt, time(
                             hour=23, minute=59, second=59, microsecond=999999
                         )
                     )
                 }),
-                tooltip=u'По',
+                tooltip='По',
             )
         )
 
     @property
     def base_params(self):
-        u"""Базовые параметры для store грида.
+        """Базовые параметры для store грида.
 
         :rtype: dict
         """
         result = {}
 
         value = self.defaults['from']()
         if value is not None:
@@ -293,32 +315,32 @@
         value = self.defaults['to']()
         if value is not None:
             result[self.filter._items[1]._uid] = str(value)
         return result
 
 
 def switch_window_in_read_only_mode(window):
-    u"""Переводит окно редактирования в режим "Только для чтения".
+    """Переводит окно редактирования в режим "Только для чтения".
 
     Удаляет кнопку "Сохранить", на кнопке "Отмена" меняет текст на "Закрыть".
 
     :param window: Окно редактирования.
     :type window: :class:`objectpack.ui.BaseEditWindow`
     """
     assert isinstance(window, BaseEditWindow), type(window)
 
-    if window.title.endswith(u': Редактирование'):
-        window.title = window.title[:-len(u'Редактирование')] + u'Просмотр'
+    if window.title.endswith(': Редактирование'):
+        window.title = window.title[:-len('Редактирование')] + 'Просмотр'
 
     window.buttons.remove(window.save_btn)
-    window.cancel_btn.text = u'Закрыть'
+    window.cancel_btn.text = 'Закрыть'
 
 
 def local_template(file_name):
-    u"""Возвращает абсолютный путь к файлу относительно модуля.
+    """Возвращает абсолютный путь к файлу относительно модуля.
 
     Основное предназначение -- формирование значений полей ``template`` и
     ``template_globals`` окон, вкладок и других компонент пользовательского
     интерфейса в тех случаях, когда файл шаблона размещен в той же папке, что
     и модуль с компонентом.
 
     :param str file_name: Имя файла.
```

### Comparing `educommon-2.20.0/src/educommon/utils/xml/__init__.py` & `educommon-3.0.0/src/educommon/utils/xml/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from lxml import etree
-import six
-
-from .resolver import Resolver
+from lxml import (
+    etree,
+)
+
+from educommon.utils.xml.resolver import (
+    Resolver,
+)
 
 
 def load_xml_schema(uri):
-    u"""Возвращает XML-схему по указанному URI.
+    """Возвращает XML-схему по указанному URI.
 
     При создании объекта схемы используется ``.resolver.Resolver``.
 
     :rtype: lxml.etree.XMLSchema
     """
     parser = etree.XMLParser(load_dtd=True)
     parser.resolvers.add(Resolver())
@@ -21,36 +21,36 @@
 
     schema = etree.XMLSchema(schema_doc)
 
     return schema
 
 
 def load_xml_document(document_uri, schema_uri):
-    u"""Возвращает XML-документ, проверенный на соответствие XML-схеме.
+    """Возвращает XML-документ, проверенный на соответствие XML-схеме.
 
     :rtype: lxml.etree._ElementTree
 
     :raises lxml.etree.DocumentInvalid: Если документ не соответствует
         XML-схеме.
     """
     document = etree.parse(document_uri)
     if schema_uri:
         schema = load_xml_schema(schema_uri)
         schema.assertValid(document)
     return document
 
 
 def parse_xml(xml):
-    u"""Возвращает дерево XML-документа.
+    """Возвращает дерево XML-документа.
 
     :param basestring xml: Текст XML-документа.
     :rtype: lxml.etree.ElementTree or None
     """
     if xml:
-        if isinstance(xml, six.text_type):
+        if isinstance(xml, str):
             xml = xml.encode('utf-8')
 
         try:
             root = etree.fromstring(xml)
         except etree.XMLSyntaxError:
             result = None
         else:
@@ -58,25 +58,25 @@
     else:
         result = None
 
     return result
 
 
 def get_text(elements):
-    u"""Возвращает текст первого элемента найденного
+    """Возвращает текст первого элемента найденного
         с помощью make_xpath_query
     """
-    return elements[0].text if elements else u''
+    return elements[0].text if elements else ''
 
 
 def make_xpath_query(*tags):
-    u"""Возвращает запрос, извлекающий элементы дерева XML-документа.
+    """Возвращает запрос, извлекающий элементы дерева XML-документа.
 
     :param tags: Имена тэгов XML-документа в порядке иерархии (без учета
         пространств имен).
     """
-    result = u'/' + u''.join(
-        u"/*[local-name()='{}']".format(tag)
+    result = '/' + ''.join(
+        "/*[local-name()='{}']".format(tag)
         for tag in tags
     )
 
     return result
```

### Comparing `educommon-2.20.0/src/educommon/utils/xml/catalog.json` & `educommon-3.0.0/src/educommon/utils/xml/catalog.json`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/xml/resolver.py` & `educommon-3.0.0/src/educommon/utils/xml/resolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import json
 import os.path
 import warnings
 
-from lxml import etree
+from lxml import (
+    etree,
+)
 
 
 def _load_catalog():
     file_path = os.path.join(os.path.dirname(__file__), 'catalog.json')
     with open(file_path, 'r') as infile:
         result = json.load(infile)
     return result
 
 
 _catalog = _load_catalog()
 
 
 class Resolver(etree.Resolver):
-
-    u"""Резолвер для предварительно загруженных XML-схем.
+    """Резолвер для предварительно загруженных XML-схем.
 
     Может использоваться в случаях, когда в XML-схемах используются внешние
     документы (<include> и <import>). Для корректной обработки XML-схем
     средствами lxml (по сути, LibXML2), использующих внешние документы,
     необходима настройка каталога, но поскольку этого не делается,
     альтернативой может служить данный резолвер.
 
@@ -32,15 +30,17 @@
 
         from lxml import etree
         parser = etree.XMLParser(load_dtd=True)
         parser.resolvers.add(Resolver())
     """
 
     def resolve(self, url, public_id, context):
-        from ..misc import md5sum
+        from educommon.utils.misc import (
+            md5sum,
+        )
 
         if url in _catalog:
             meta = _catalog[url]
             filepath = os.path.join(os.path.dirname(__file__), meta['file'])
             if meta['md5'] != md5sum(filepath):
                 warnings.warn('File {} corrupted.'.format(filepath))
                 result = self.resolve_empty(context)
```

### Comparing `educommon-2.20.0/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd` & `educommon-3.0.0/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd` & `educommon-3.0.0/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/xml/xenc-schema.xsd` & `educommon-3.0.0/src/educommon/utils/xml/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/utils/xml/xmldsig-core-schema.xsd` & `educommon-3.0.0/src/educommon/utils/xml/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/ws_log/README.rst` & `educommon-3.0.0/src/educommon/ws_log/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/ws_log/__init__.py` & `educommon-3.0.0/src/educommon/ws_log/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
 
-import abc
-
-import six
-
-
-class IConfig(six.with_metaclass(abc.ABCMeta, object)):
 
+class IConfig(metaclass=ABCMeta):
     """Класс интерфейс для конфигурации менеджера логгеров веб-сервисов."""
 
-    @abc.abstractproperty
+    @property
+    @abstractmethod
     def loggers(self):
         """Список логгеров Системы.
 
         :return: Кортеж из строк, содержащих полные наименования
             модулей (с наименованием пакета), содержащих класс логгера.
         :type: tuple of strings
         """
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/actions.py` & `educommon-3.0.0/src/educommon/ws_log/actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-# coding: utf-8
-u"""Экшены и паки приложения логирования СМЭВ."""
-from __future__ import absolute_import
-
+"""Экшены и паки приложения логирования СМЭВ."""
 import datetime
 import functools
 
-from django.db.models import Q
-from educommon.m3 import PackValidationMixin
-from educommon.utils.ui import ChoicesFilter
-from educommon.utils.ui import ColumnFilterWithDefaultValue
-from educommon.utils.ui import FilterByTextField
-from objectpack.actions import ObjectPack
-from objectpack.filters import ColumnFilterEngine
-from objectpack.filters import FilterByField
-
-from . import models
-from . import ui
+from django.db.models import (
+    Q,
+)
+
+from objectpack.actions import (
+    ObjectPack,
+)
+from objectpack.filters import (
+    ColumnFilterEngine,
+    FilterByField,
+)
+
+from educommon.m3 import (
+    PackValidationMixin,
+)
+from educommon.utils.ui import (
+    ChoicesFilter,
+    ColumnFilterWithDefaultValue,
+    FilterByTextField,
+)
+from educommon.ws_log import (
+    models,
+    ui,
+)
 
 
 ALL_TYPES = -1  # Тип "Все", выбираемого значения в фильтре.
 
 
 class SmevLogPack(ObjectPack):
-    u"""Лог запросов СМЭВ."""
+    """Лог запросов СМЭВ."""
 
     model = models.SmevLog
     edit_window = ui.SmevLogEditWindow
     list_window = ui.SmevLogListWindow
 
     column_name_on_select = 'method_name'
     list_sort_order = ['-time']
@@ -36,229 +46,228 @@
     filter_field = functools.partial(FilterByField, model)
     date_field = functools.partial(ColumnFilterWithDefaultValue, model)
     text_field_filter = functools.partial(FilterByTextField, model)
 
     columns = [
         {
             'data_index': 'time',
-            'header': u'Дата время',
+            'header': 'Дата время',
             'filter': date_field(
                 'time',
                 lookup=lambda d: Q(
                     time__range=(
                         datetime.datetime.combine(d, datetime.time.min),
                         datetime.datetime.combine(d, datetime.time.max)
                     )
                 ) if d else Q(),
-                tooltip=u'Дата время',
+                tooltip='Дата время',
                 value=datetime.date.today(),
                 allow_blank=False
             ),
             'sortable': True,
             'sort_fields': ('time',),
         },
         {
             'data_index': 'service_address',
-            'header': u'Адрес сервиса',
+            'header': 'Адрес сервиса',
             'filter': filter_field(
                 'service_address', 'service_address__icontains'),
             'sortable': True,
             'sort_fields': ('service_address',),
         },
         {
             'data_index': 'consumer_type_verbose',
-            'header': u'Потребитель сервиса',
+            'header': 'Потребитель сервиса',
             'filter': ChoicesFilter(
-                choices=models.SmevLog.CONSUMER_TYPES + ((ALL_TYPES, u'Все'),),
+                choices=models.SmevLog.CONSUMER_TYPES + ((ALL_TYPES, 'Все'),),
                 parser=int,
                 lookup=lambda index: Q(
                     consumer_type=index) if index != ALL_TYPES else Q(),
-                tooltip=u'Потребитель сервиса',
+                tooltip='Потребитель сервиса',
             ),
             'sortable': True,
             'sort_fields': ('consumer_type',),
         },
         {
             'data_index': 'consumer_name',
-            'header': u'Наименование потребителя',
+            'header': 'Наименование потребителя',
             'filter': filter_field(
                 'consumer_name', 'consumer_name__icontains'),
             'sortable': True,
             'sort_fields': ('consumer_name',),
         },
         {
             'data_index': 'source_verbose',
-            'header': u'Источник взаимодействия',
+            'header': 'Источник взаимодействия',
             'filter': ChoicesFilter(
-                choices=models.SmevLog.SOURCE_TYPES + ((ALL_TYPES, u'Все'),),
+                choices=models.SmevLog.SOURCE_TYPES + ((ALL_TYPES, 'Все'),),
                 parser=int,
                 lookup=lambda index: Q(
                     source=index) if index != ALL_TYPES else Q(),
-                tooltip=u'Источник взаимодействия',
+                tooltip='Источник взаимодействия',
             ),
             'sortable': True,
             'sort_fields': ('source',),
         },
         {
             'data_index': 'target_name',
-            'header': u'Наименование электронного сервиса',
+            'header': 'Наименование электронного сервиса',
             'filter': filter_field('target_name', 'target_name__icontains'),
             'sortable': True,
             'sort_fields': ('target_name',),
         },
         {
             'data_index': 'method_name',
-            'header': u'Код метода',
+            'header': 'Код метода',
             'filter': filter_field('method_name', 'method_name__icontains'),
             'sortable': True,
             'sort_fields': ('method_name',),
         },
         {
             'data_index': 'method_verbose_name',
-            'header': u'Наименование метода',
+            'header': 'Наименование метода',
             'filter': filter_field(
                 'method_verbose_name', 'method_verbose_name__icontains'),
             'sortable': True,
             'sort_fields': ('method_verbose_name',),
         },
         {
             'data_index': 'result_with_default',
-            'header': u'Результат',
+            'header': 'Результат',
             'filter': text_field_filter(
                 'result', 'result_with_default__icontains'),
             'sortable': True,
             'sort_fields': ('result_with_default',),
         },
         {
             'data_index': 'interaction_type_verbose',
-            'header': u'Вид взаимодействия',
+            'header': 'Вид взаимодействия',
             'filter': ChoicesFilter(
                 choices=models.SmevLog.INTERACTION_TYPES + (
-                    (ALL_TYPES, u'Все'),),
+                    (ALL_TYPES, 'Все'),),
                 parser=int,
                 lookup=lambda index: Q(
                     interaction_type=index) if index != ALL_TYPES else Q(),
-                tooltip=u'Вид взаимодействия'
+                tooltip='Вид взаимодействия'
             ),
             'sortable': True,
             'sort_fields': ('interaction_type',),
         }
     ]
 
     # Название фильтра для столбца "Дата время" в ajax-запросе
     date_time_filter_param_name = 'filter_1'
 
     def get_rows_query(self, request, context):
-        u"""Получение данных."""
+        """Получение данных."""
         query = self.model.extended_manager.all()
         return query
 
     def configure_grid(self, grid):
-        u"""Настройка грида."""
+        """Настройка грида."""
         super(SmevLogPack, self).configure_grid(grid)
-        grid.top_bar.button_edit.text = u'Просмотр'
+        grid.top_bar.button_edit.text = 'Просмотр'
 
         grid.store.base_params = {
             self.date_time_filter_param_name: str(datetime.date.today())
         }
 
     def prepare_row(self, obj, request, context):
-        u"""Настройка строки грида, вызывается посточно для каждой строки."""
+        """Настройка строки грида, вызывается посточно для каждой строки."""
         obj.interaction_type_verbose = (
             dict(self.model.INTERACTION_TYPES)[obj.interaction_type])
 
         obj.consumer_type_verbose = (
-            dict(self.model.CONSUMER_TYPES).get(obj.consumer_type, u''))
+            dict(self.model.CONSUMER_TYPES).get(obj.consumer_type, ''))
 
         obj.source_verbose = (
-            dict(self.model.SOURCE_TYPES).get(obj.source, u''))
+            dict(self.model.SOURCE_TYPES).get(obj.source, ''))
 
         return obj
 
     def get_edit_window_params(self, params, request, context):
-        u"""Дополняет параметры для окна редактирования."""
+        """Дополняет параметры для окна редактирования."""
         log = params['object']
         method_name = log.method_name or log.method_verbose_name
 
-        params['title'] = u'Лог по методу: {}'.format(method_name)
+        params['title'] = 'Лог по методу: {}'.format(method_name)
 
         return params
 
     def extend_menu(self, menu):
-        u"""Размещение в меню."""
+        """Размещение в меню."""
         return menu.SubMenu(
-            u'Администрирование',
+            'Администрирование',
             menu.SubMenu(
-                u'Взаимодействие со СМЭВ',
+                'Взаимодействие со СМЭВ',
                 menu.Item(
-                    u'Логи СМЭВ',
+                    'Логи СМЭВ',
                     pack=self.get_default_action()
                 )
             )
         )
 
 
 class SmevProviderPack(PackValidationMixin, ObjectPack):
-
-    u"""Пак поставщики СМЭВ."""
+    """Пак поставщики СМЭВ."""
 
     model = models.SmevProvider
     add_window = edit_window = ui.SmevProviderEditWindow
     list_window = ui.SmevProviderListWindow
 
     columns = [
         {
             'data_index': 'mnemonics',
-            'header': u'Мнемоника',
+            'header': 'Мнемоника',
             'sortable': True,
             'searchable': True,
             'width': 1
         },
         {
             'data_index': 'address',
-            'header': u'Адрес СМЭВ',
+            'header': 'Адрес СМЭВ',
             'sortable': True,
             'searchable': True,
             'width': 1
         },
         {
             'data_index': 'service_name',
-            'header': u'Наименование электронного сервиса',
+            'header': 'Наименование электронного сервиса',
             'sortable': True,
             'searchable': True,
             'width': 3
         },
         {
             'data_index': 'source',
-            'header': u'Источник взаимодействия',
+            'header': 'Источник взаимодействия',
             'sortable': True,
             'searchable': True,
             'width': 2
         },
         {
             'data_index': 'entity',
-            'header': u'Наименование юр. лица',
+            'header': 'Наименование юр. лица',
             'sortable': True,
             'searchable': True,
             'width': 2
         },
         {
             'data_index': 'service_address_status_changes',
-            'header': u'Адрес сервиса изменения статуса',
+            'header': 'Адрес сервиса изменения статуса',
             'sortable': True,
             'searchable': True,
             'width': 3
         }
     ]
 
     def extend_menu(self, menu):
-        u"""Размещение в меню."""
+        """Размещение в меню."""
         return menu.SubMenu(
-            u'Администрирование',
+            'Администрирование',
             menu.SubMenu(
-                u'Взаимодействие со СМЭВ',
+                'Взаимодействие со СМЭВ',
                 menu.Item(
-                    u'Поставщики СМЭВ',
+                    'Поставщики СМЭВ',
                     pack=self.get_default_action()
                 )
             )
         )
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/base.py` & `educommon-3.0.0/src/educommon/ws_log/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-import abc
 import traceback
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
+from io import (
+    BytesIO,
+)
 
-from django.apps import apps
-import six
-
-
-if six.PY3:
-    from io import BytesIO
-
-    def read_request_body(request_body):
-        return BytesIO(request_body)
-else:
-    from six.moves import cStringIO as StringIO
+from django.apps import (
+    apps,
+)
 
-    def read_request_body(request_body):
-        return StringIO(request_body)
 
+def read_request_body(request_body):
+    return BytesIO(request_body)
 
-class BaseWsApplicationLogger(six.with_metaclass(abc.ABCMeta, object)):
 
+class BaseWsApplicationLogger(metaclass=ABCMeta):
     """Базовый класс логгера для приложения веб-сервиса.
 
     Ожидает что будут определены аттрибуты app_name и log_model в потомках.
     В качестве значения для log_model ожидается кортеж вида
     ('app_name', 'model_name').
     """
 
-    @abc.abstractproperty
+    @property
+    @abstractmethod
     def log_model(self):
         """Модель для логирования запросов."""
 
     def get_prepared_environ(self, request):
         """Возвращает подготовленное для логирования окружение запроса.
 
         :param request: Запрос.
@@ -51,15 +46,15 @@
     def collect_error(log_record, traceback_data):
         """Сохраняет ошибку при обращении к веб-сервису.
 
         :param log_record: Запись лога веб-сервиса
         :param traceback_data: Данные возникшей ошибки.
         """
         etype, value, tb = traceback_data
-        traceback_text = six.text_type(
+        traceback_text = str(
             ''.join(
                 traceback.format_exception(etype, value, tb, None)
             )
         )
         log_record.result = traceback_text
 
     def save_log_record(self, wsgi_app, uri, retval, traceback_data, environ):
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/migrations/0001_initial.py` & `educommon-3.0.0/src/educommon/ws_log/migrations/0001_initial.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
 import datetime
 
-from django.db import migrations
-from django.db import models
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py` & `educommon-3.0.0/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('ws_log', '0001_initial'),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py` & `educommon-3.0.0/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('ws_log', '0002_auto_20160628_1334'),
     ]
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py` & `educommon-3.0.0/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# coding: utf-8
-from __future__ import unicode_literals
-
-from django.db import migrations
-from django.db import models
+from django.db import (
+    migrations,
+    models,
+)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [('ws_log', '0007_auto_20180607_1040'), ]
 
     operations = [
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/models.py` & `educommon-3.0.0/src/educommon/ws_log/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,51 @@
-# coding: utf-8
-u"""Модели приложения логирования СМЭВ."""
-from __future__ import absolute_import
-
+"""Модели приложения логирования СМЭВ."""
 import datetime
 
-from django.db import models
-from django.db.models import Q
-from django.db.models.expressions import Case
-from django.db.models.expressions import Value
-from django.db.models.expressions import When
-from m3.db import BaseEnumerate
-from m3.db import BaseObjectModel
+from django.db import (
+    models,
+)
+from django.db.models import (
+    Q,
+)
+from django.db.models.expressions import (
+    Case,
+    Value,
+    When,
+)
+from m3.db import (
+    BaseEnumerate,
+    BaseObjectModel,
+)
 
 
 class SmevSourceEnum(BaseEnumerate):
-    u"""Источники взаимодействия."""
+    """Источники взаимодействия."""
 
     EPGU = 0
     RPGU = 1
     INTER = 2
     BARS_OBR = 3
     CONCENTRATOR = 4
     MFC = 5
 
     SOURCE_TYPES = (
-        (EPGU, u'ЕПГУ'),
-        (RPGU, u'РПГУ'),
-        (INTER, u'Межведомственное взаимодействие'),
-        (BARS_OBR, u'Барс-Образование'),
-        (CONCENTRATOR, u'Концентратор'),
-        (MFC, u'МФЦ'),
+        (EPGU, 'ЕПГУ'),
+        (RPGU, 'РПГУ'),
+        (INTER, 'Межведомственное взаимодействие'),
+        (BARS_OBR, 'Барс-Образование'),
+        (CONCENTRATOR, 'Концентратор'),
+        (MFC, 'МФЦ'),
     )
 
     values = dict(SOURCE_TYPES)
 
 
 class ExtendedSmevLogManager(models.Manager):
-
-    u"""Расширенный менеджер логов СМЭВ.
+    """Расширенный менеджер логов СМЭВ.
 
     Аннотирует дополнительные поля.
     """
 
     def get_queryset(self):
         query = super(ExtendedSmevLogManager, self).get_queryset()
         return query.annotate(
@@ -54,115 +58,115 @@
                 ),
                 default='result'
             ),
         )
 
 
 class SmevLog(BaseObjectModel):
-    u"""Логи СМЭВ web-сервисов."""
+    """Логи СМЭВ web-сервисов."""
 
     # Виды взаимодействия
     IS_SMEV = 0
     IS_NOT_SMEV = 1
     INTERACTION_TYPES = (
-        (IS_SMEV, u'СМЭВ'),
-        (IS_NOT_SMEV, u'Не СМЭВ'),
+        (IS_SMEV, 'СМЭВ'),
+        (IS_NOT_SMEV, 'Не СМЭВ'),
     )
 
     # Направление запроса
     INCOMING = 1
     OUTGOING = 0
     DIRECTION = (
-        (INCOMING, u'Входящие запросы'),
-        (OUTGOING, u'Исходящие запросы'),
+        (INCOMING, 'Входящие запросы'),
+        (OUTGOING, 'Исходящие запросы'),
     )
 
     # Потребители сервиса
     ENTITY = 0
     INDIVIDUAL = 1
     CONSUMER_TYPES = (
-        (ENTITY, u'Юридическое лицо'),
-        (INDIVIDUAL, u'Физическое лицо'),
+        (ENTITY, 'Юридическое лицо'),
+        (INDIVIDUAL, 'Физическое лицо'),
     )
 
     # Источник взаимодействия
     EPGU = SmevSourceEnum.EPGU
     RPGU = SmevSourceEnum.RPGU
     INTER = SmevSourceEnum.INTER
     BARS_OBR = SmevSourceEnum.BARS_OBR
     SOURCE_TYPES = SmevSourceEnum.SOURCE_TYPES
 
-    RESULT_DEFAULT_VALUE = u'Успешно'
+    RESULT_DEFAULT_VALUE = 'Успешно'
 
     service_address = models.CharField(
-        u'Адрес сервиса', max_length=250, null=True, blank=True)
+        'Адрес сервиса', max_length=250, null=True, blank=True)
 
     method_name = models.CharField(
-        u'Код метода', max_length=250, null=True, blank=True, db_index=True)
+        'Код метода', max_length=250, null=True, blank=True, db_index=True)
 
     method_verbose_name = models.CharField(
-        u'Наименование метода', max_length=250, null=True, blank=True)
+        'Наименование метода', max_length=250, null=True, blank=True)
 
-    request = models.TextField(u'SOAP запрос', null=True, blank=True)
-    response = models.TextField(u'SOAP ответ', null=True, blank=True)
-    result = models.TextField(u'Результат', null=True, blank=True)
+    request = models.TextField('SOAP запрос', null=True, blank=True)
+    response = models.TextField('SOAP ответ', null=True, blank=True)
+    result = models.TextField('Результат', null=True, blank=True)
 
     time = models.DateTimeField(
-        u'Время СМЭВ запроса', default=datetime.datetime.now, db_index=True)
+        'Время СМЭВ запроса', default=datetime.datetime.now, db_index=True)
 
     interaction_type = models.PositiveSmallIntegerField(
-        u'Вид взаимодействия', choices=INTERACTION_TYPES, default=IS_SMEV)
+        'Вид взаимодействия', choices=INTERACTION_TYPES, default=IS_SMEV)
 
     direction = models.SmallIntegerField(
         choices=DIRECTION,
-        verbose_name=u'Направление запроса'
+        verbose_name='Направление запроса'
     )
 
     consumer_type = models.PositiveSmallIntegerField(
-        u'Потребитель сервиса', choices=CONSUMER_TYPES, default=INDIVIDUAL,
+        'Потребитель сервиса', choices=CONSUMER_TYPES, default=INDIVIDUAL,
         null=True, blank=True)
 
     consumer_name = models.CharField(
-        u'Наименование потребителя', max_length=100, null=True, blank=True)
+        'Наименование потребителя', max_length=100, null=True, blank=True)
 
     source = models.PositiveSmallIntegerField(
-        u'Источник взаимодействия', choices=SOURCE_TYPES,
+        'Источник взаимодействия', choices=SOURCE_TYPES,
         default=None, null=True, blank=True)
 
     target_name = models.CharField(
-        u'Наименование электронного сервиса', max_length=100, null=True,
+        'Наименование электронного сервиса', max_length=100, null=True,
         blank=True)
 
     objects = models.Manager()
     extended_manager = ExtendedSmevLogManager()
 
     class Meta:
-        verbose_name = u'Лог запросов СМЭВ'
-        verbose_name_plural = u'Логи запросов СМЭВ'
+        verbose_name = 'Лог запросов СМЭВ'
+        verbose_name_plural = 'Логи запросов СМЭВ'
 
 
 class SmevProvider(BaseObjectModel):
-    u"""Поставщики СМЭВ."""
+    """Поставщики СМЭВ."""
 
     # Источник взаимодействия
     EPGU = SmevSourceEnum.EPGU
     RPGU = SmevSourceEnum.RPGU
     INTER = SmevSourceEnum.INTER
     CONCENTRATOR = SmevSourceEnum.CONCENTRATOR
     SOURCE_TYPES = SmevSourceEnum.SOURCE_TYPES
 
-    mnemonics = models.CharField(u'Мнемоника', max_length=100)
-    address = models.CharField(u'Адрес СМЭВ', max_length=100)
+    mnemonics = models.CharField('Мнемоника', max_length=100)
+    address = models.CharField('Адрес СМЭВ', max_length=100)
     source = models.PositiveSmallIntegerField(
-        u'Источник взаимодействия', choices=SOURCE_TYPES)
+        'Источник взаимодействия', choices=SOURCE_TYPES)
     service_name = models.CharField(
-        u'Наименование эл. сервиса', max_length=100)
+        'Наименование эл. сервиса', max_length=100)
     service_address_status_changes = models.CharField(
-        u'Адрес сервиса изменения статуса', max_length=100,
+        'Адрес сервиса изменения статуса', max_length=100,
         null=True, blank=True)
     entity = models.CharField(
-        u'Наименование юр.лица', max_length=255, null=True, blank=True)
+        'Наименование юр.лица', max_length=255, null=True, blank=True)
 
     class Meta:
-        verbose_name = u'Поставщик СМЭВ'
-        verbose_name_plural = u'Поставщики СМЭВ'
+        verbose_name = 'Поставщик СМЭВ'
+        verbose_name_plural = 'Поставщики СМЭВ'
         unique_together = ('mnemonics', 'address')
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/provider.py` & `educommon-3.0.0/src/educommon/ws_log/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# coding: utf-8
-from __future__ import absolute_import
-
 import datetime
 
-from educommon.report import AbstractDataProvider
-from educommon.ws_log.models import SmevLog
+from educommon.report import (
+    AbstractDataProvider,
+)
+from educommon.ws_log.models import (
+    SmevLog,
+)
 
 
 class SmevLogDataProvider(AbstractDataProvider):
-    u"""Провайдер данных отчета "Логи СМЭВ"."""
+    """Провайдер данных отчета "Логи СМЭВ"."""
 
     def init(self, **params):
         super(SmevLogDataProvider, self).init(**params)
         self.date_begin = params['date_begin']
         self.date_end = params['date_end']
 
     def get_smev_logs_data(self):
-        u"""Возвращает логи СМЭВ на отрезок времени."""
+        """Возвращает логи СМЭВ на отрезок времени."""
         return SmevLog.objects.filter(
             time__range=(
                 datetime.datetime.combine(self.date_begin, datetime.time.min),
                 datetime.datetime.combine(self.date_end, datetime.time.max),
             ),
         )
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/report.py` & `educommon-3.0.0/src/educommon/ws_log/report.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,43 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from m3 import ApplicationLogicException
-
-from educommon.report import AbstractReportBuilder
-from educommon.report.actions import CommonReportPack
-from educommon.report.reporter import SimpleReporter
-
-from .models import SmevLog
-from .provider import SmevLogDataProvider
-from .ui import SmevLogReportWindow
+from m3 import (
+    ApplicationLogicException,
+)
+
+from educommon.report import (
+    AbstractReportBuilder,
+)
+from educommon.report.actions import (
+    CommonReportPack,
+)
+from educommon.report.reporter import (
+    SimpleReporter,
+)
+from educommon.ws_log.models import (
+    SmevLog,
+)
+from educommon.ws_log.provider import (
+    SmevLogDataProvider,
+)
+from educommon.ws_log.ui import (
+    SmevLogReportWindow,
+)
 
 
 class SmevLogReportBuilder(AbstractReportBuilder):
-    u"""Билдер отчёта "Логи СМЭВ"."""
+    """Билдер отчёта "Логи СМЭВ"."""
 
     def __init__(self, provider, adapter, report, *args, **kwargs):
         super(SmevLogReportBuilder, self).__init__(*args, **kwargs)
         self.provider = provider
         self.adapter = adapter
         self.report = report
         self.params = kwargs.get('params', {})
 
     def build(self):
-        u"""Строит отчет, заполняя секции шаблона из данных провайдера."""
+        """Строит отчет, заполняя секции шаблона из данных провайдера."""
         self.header_section = self.report.get_section('header')
         self.row_section = self.report.get_section('row')
 
         self.header_section.flush(
             {'institute_name': self.params['institute_name']})
 
         smev_logs = self.provider.smev_logs_data.extra(
@@ -43,45 +52,45 @@
         for index,  smev_log in enumerate(smev_logs, 1):
             smev_log['index'] = index
             smev_log['source'] = sources.get(smev_log['source'], '')
             smev_log['consumer_type'] = consumers.get(
                 smev_log['consumer_type'], '')
 
             if not smev_log['result']:
-                smev_log['result'] = u'Успешно'
+                smev_log['result'] = 'Успешно'
 
             self.row_section.flush(smev_log)
 
 
 class SmevLogReporter(SimpleReporter):
-    u"""Строитель отчёта "Логи СМЭВ"."""
+    """Строитель отчёта "Логи СМЭВ"."""
 
     extension = '.xlsx'
     template_file_path = './templates/report/smev_logs.xlsx'
     data_provider_class = SmevLogDataProvider
     builder_class = SmevLogReportBuilder
 
 
 class SmevLogPrintReportPack(CommonReportPack):
-    u"""Пак печати отчета "Логи СМЭВ"."""
+    """Пак печати отчета "Логи СМЭВ"."""
 
-    title = u'Логи СМЭВ'
+    title = 'Логи СМЭВ'
     report_window = SmevLogReportWindow
     reporter_class = SmevLogReporter
 
     is_async = True
 
     extend_menu = extend_desktop = None
 
     def declare_context(self, action):
         context = super(SmevLogPrintReportPack, self).declare_context(action)
 
         if action is self.report_action:
             context.update(
-                institute_name={'type': 'unicode'},
+                institute_name={'type': 'str'},
                 date_begin={'type': 'date'},
                 date_end={'type': 'date'},
             )
 
         return context
 
     def get_provider_params(self, request, context):
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/smev/applications.py` & `educommon-3.0.0/src/educommon/ws_log/smev/applications.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,63 @@
-# coding: utf-8
-u"""Приложение для логирования запросов СМЭВ."""
-from __future__ import absolute_import
-
+"""Приложение для логирования запросов СМЭВ."""
 import sys
 import traceback
 
-from spyne.decorator import rpc
-from spyne.model import Fault
-from spyne.model.primitive import Unicode
-from spyne.protocol import ProtocolBase
-from spyne.server.wsgi import WsgiApplication
-from spyne.service import ServiceBase
-from spyne_smev.fault import ApiError
-from spyne_smev.server.django import DjangoApplication
-import six
-
-from educommon.ws_log.smev.exceptions import SpyneException
-from educommon.ws_log.utils import logger_manager
+from spyne.decorator import (
+    rpc,
+)
+from spyne.model import (
+    Fault,
+)
+from spyne.model.primitive import (
+    Unicode,
+)
+from spyne.protocol import (
+    ProtocolBase,
+)
+from spyne.server.wsgi import (
+    WsgiApplication,
+)
+from spyne.service import (
+    ServiceBase,
+)
+from spyne_smev.fault import (
+    ApiError,
+)
+from spyne_smev.server.django import (
+    DjangoApplication,
+)
+
+from educommon.ws_log.smev.exceptions import (
+    SpyneException,
+)
+from educommon.ws_log.utils import (
+    logger_manager,
+)
 
 
 class LoggingDjangoApplication(DjangoApplication):
-    u"""Переопределенный класс для логирования запросов СМЭВ."""
+    """Переопределенный класс для логирования запросов СМЭВ."""
 
     def __init__(self, app, chunked=True, max_content_length=10 * 1024 * 1024,
                  block_length=8 * 1024):
-        u"""Метод инициализации приложения для логирования запросов СМЭВ."""
+        """Метод инициализации приложения для логирования запросов СМЭВ."""
         super(LoggingDjangoApplication, self).__init__(
             app, chunked, max_content_length, block_length)
         self.application_logger = logger_manager.get_application_logger(
             self.app.name
         )
         self.app.event_manager.add_listener(
             'method_call',
             self.application_logger.collect_log_data
         )
         self.event_manager.add_listener('wsgi_exception', wsgi_exception)
 
     def generate_contexts(self, ctx, in_string_charset=None):
-        u"""Call create_in_document and decompose_incoming_envelope.
+        """Call create_in_document and decompose_incoming_envelope.
 
         To get method_request string in order to generate contexts.
         """
         try:
             # sets ctx.in_document
             self.app.in_protocol.create_in_document(ctx, in_string_charset)
 
@@ -62,15 +78,15 @@
             ctx.in_error = e
             ctx.out_error = e
             retval = (ctx,)
 
         return retval
 
     def __call__(self, request):
-        u"""Логируем запрос, при вызове объекта приложения как функции."""
+        """Логируем запрос, при вызове объекта приложения как функции."""
 
         def start_response(status, headers):
             # Status is one of spyne.const.http
             status, reason = status.split(' ', 1)
 
             retval.status_code = int(status)
             for header, value in headers:
@@ -99,19 +115,19 @@
             environ=environ
         )
 
         return retval
 
 
 class LoggingService(ServiceBase):
-    u"""Перекрытый класс базового класса web-сервисов spyne."""
+    """Перекрытый класс базового класса web-сервисов spyne."""
 
     @classmethod
     def call_wrapper(cls, ctx):
-        u"""Перекрыли, чтобы отдавать валидную для СМЭВ ошибку."""
+        """Перекрыли, чтобы отдавать валидную для СМЭВ ошибку."""
         try:
             if ctx.function is not None:
                 if ctx.descriptor.no_ctx:
                     result = ctx.function(*ctx.in_object)
                 else:
                     result = ctx.function(ctx, *ctx.in_object)
 
@@ -125,35 +141,35 @@
         except SpyneException as exc:
             raise ApiError(
                 exc.faultcode, exc.faultstring,
                 ctx.function.__name__.replace('Request', 'Response'))
 
         except Exception as exc:
             log = ctx.transport.req['log_record']
-            log.result = six.text_type(traceback.format_exc(), errors="ignore")
+            log.result = str(traceback.format_exc(), errors="ignore")
             raise ApiError(
                 'Server', exc.message,
                 ctx.function.__name__.replace('Request', 'Response')
             )
 
     @rpc(Unicode, _returns=Unicode)
     def upper(self, s):
         return s.upper()
 
 
 def wsgi_exception(ctx):
-    u"""Обработчик события 'wsgi_exception'.
+    """Обработчик события 'wsgi_exception'.
 
     Логирует обращения к web-сервисам, когда происходят ошибки десериализации
     входящего документа или ошибки функции web-сервиса.
     """
     log = ctx.transport.req['log_record']
     error = ctx.in_error or ctx.out_error
 
     log.method_name = ctx.method_name
     if isinstance(error, ApiError):
         log.result = error.errorMessage
     else:
-        log.result = six.text_type(error)
+        log.result = str(error)
 
     app_logger = logger_manager.get_application_logger(ctx.app.name)
     app_logger.collect_log_data(ctx)
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/smev/exceptions.py` & `educommon-3.0.0/src/educommon/ws_log/smev/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from spyne.error import Fault
-import six
+from spyne.error import (
+    Fault,
+)
 
 
 class SpyneException(Fault):
-    u"""Переопределенный Exception базового exception`а spyne.
+    """Переопределенный Exception базового exception`а spyne.
 
     По спецификации спайна faultcode
     It's a dot-delimited string whose first fragment is
             either 'Client' or 'Server'.
     """
     def __init__(self, code=0, message=''):
-        if isinstance(code, six.string_types):
+        if isinstance(code, str):
             Fault.__init__(self, faultstring=code)
         else:
             Fault.__init__(self,
                            faultcode='Server;%d' % code,
                            faultstring=message)
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/templates/report/smev_logs.xlsx` & `educommon-3.0.0/src/educommon/ws_log/templates/report/smev_logs.xlsx`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js` & `educommon-3.0.0/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js` & `educommon-3.0.0/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.20.0/src/educommon/ws_log/ui.py` & `educommon-3.0.0/src/educommon/ws_log/ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,119 +1,124 @@
-# coding: utf-8
-u"""Описания пользовательского интерфейса приложения логирования СМЭВ."""
-from __future__ import absolute_import
-
-from m3_ext.ui import all_components as ext
-from m3_ext.ui.icons import Icons
-from objectpack.ui import BaseEditWindow
-from objectpack.ui import BaseListWindow
-from objectpack.ui import ModelEditWindow
-
-from educommon.ws_log.models import SmevLog
-from educommon.ws_log.models import SmevProvider
+"""Описания пользовательского интерфейса приложения логирования СМЭВ."""
+from m3_ext.ui import (
+    all_components as ext,
+)
+from m3_ext.ui.icons import (
+    Icons,
+)
+
+from objectpack.ui import (
+    BaseEditWindow,
+    BaseListWindow,
+    ModelEditWindow,
+)
+
+from educommon.ws_log.models import (
+    SmevLog,
+    SmevProvider,
+)
 
 
 class SmevLogEditWindow(
     ModelEditWindow.fabricate(
         SmevLog, field_list=['request', 'response', 'result'])
 ):
-    u"""Окно редактирования логов СМЭВ."""
+    """Окно редактирования логов СМЭВ."""
 
     def set_params(self, params):
-        u"""Настройка окна."""
+        """Настройка окна."""
         super(SmevLogEditWindow, self).set_params(params)
         self.height, self.width = 800, 800
 
         self.make_read_only()
 
         for field in self.form.items:
             if isinstance(field, ext.ExtTextArea):
                 field.height = 240
 
 
 class SmevLogListWindow(BaseListWindow):
-    u"""Окно списка логов СМЭВ."""
+    """Окно списка логов СМЭВ."""
 
     def _init_components(self):
-        u"""Создание компонентов окна."""
+        """Создание компонентов окна."""
         super(SmevLogListWindow, self)._init_components()
         self.print_button = ext.ExtButton(
-            text=u'Печать', handler='printSmevLogsReport', icon_cls='printer')
+            text='Печать', handler='printSmevLogsReport', icon_cls='printer')
 
     def _do_layout(self):
-        u"""Расположение компонентов окна."""
+        """Расположение компонентов окна."""
         super(SmevLogListWindow, self)._do_layout()
         self.grid.top_bar.items.append(self.print_button)
         self.grid.top_bar.button_edit.icon_cls = Icons.APPLICATION_VIEW_DETAIL
 
     def set_params(self, params):
-        u"""Настройка окна."""
+        """Настройка окна."""
         super(SmevLogListWindow, self).set_params(params)
         self.maximized = True
         self.settings_report_window_url = params['settings_report_window_url']
         self.template_globals = 'ui-js/smev-logs-list-window.js'
 
-class SmevProviderListWindow(BaseListWindow):
 
-    u"""Окно списка поставщиков СМЭВ."""
+class SmevProviderListWindow(BaseListWindow):
+    """Окно списка поставщиков СМЭВ."""
 
     def set_params(self, params):
         super(SmevProviderListWindow, self).set_params(params)
         self.width = 1000
 
 
 class SmevProviderEditWindow(ModelEditWindow):
-
-    u"""Окно добавления/редактирования поставщиков СМЭВ."""
+    """Окно добавления/редактирования поставщиков СМЭВ."""
 
     model = SmevProvider
 
     def set_params(self, params):
         super(SmevProviderEditWindow, self).set_params(params)
         self.form.label_width = 200
         self.width = 500
 
 
 class SmevLogReportWindow(BaseEditWindow):
 
     def _init_components(self):
-        u"""Создание компонентов окна."""
+        """Создание компонентов окна."""
         super(SmevLogReportWindow, self)._init_components()
         self.field_date_begin = ext.ExtDateField(
             name='date_begin',
-            label=u'Дата с',
+            label='Дата с',
             allow_blank=False,
             anchor='100%')
 
         self.field_date_end = ext.ExtDateField(
             name='date_end',
-            label=u'Дата по',
+            label='Дата по',
             allow_blank=False,
             anchor='100%')
 
         self.field_institute = ext.ExtDictSelectField(
-            label=u'Организация',
+            label='Организация',
             name='institute_id',
             display_field='code',
             anchor='100%',
             hide_trigger=False,
             hide_edit_trigger=True,
             allow_blank=False)
 
     def _do_layout(self):
-        u"""Расположение компонентов окна."""
+        """Расположение компонентов окна."""
         super(SmevLogReportWindow, self)._do_layout()
         self.form.items.extend([
             self.field_institute,
             self.field_date_begin,
             self.field_date_end,
         ])
 
     def set_params(self, params):
-        u"""Настройка окна."""
+        """Настройка окна."""
         super(SmevLogReportWindow, self).set_params(params)
         self.height, self.width = 200, 400
 
         self.field_institute.pack = params['institute_pack']
 
         if params.get('institute'):
             self.field_institute.set_value_from_model(params['institute'])
```

### Comparing `educommon-2.20.0/src/educommon/ws_log/utils.py` & `educommon-3.0.0/src/educommon/ws_log/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
+from django.utils.module_loading import (
+    import_string,
+)
+
+from educommon.ws_log import (
+    config as manager_config,
+)
+from educommon.ws_log.base import (
+    DefaultWsApplicationLogger,
+)
 
-from django.utils.module_loading import import_string
-
-from . import config as manager_config
-from .base import DefaultWsApplicationLogger
-
-
-class LoggerManager(object):
 
+class LoggerManager:
     """Класс для работы с логгерами приложений веб-сервисов."""
 
     def __init__(self):
         self._ws_loggers = dict(
             default=DefaultWsApplicationLogger()
         )
```

### Comparing `educommon-2.20.0/src/educommon.egg-info/PKG-INFO` & `educommon-3.0.0/src/educommon.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: educommon
-Version: 2.20.0
+Version: 3.0.0
 Summary: Общая кодовая база для проектов БЦ Образование
 Home-page: https://stash.bars-open.ru/projects/EDUBASE/repos/educommon
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Django :: 1.7
 Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
```

### Comparing `educommon-2.20.0/src/educommon.egg-info/SOURCES.txt` & `educommon-3.0.0/src/educommon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-CHANGELOG.rst
 MANIFEST.in
 README.rst
 UPGRADE.rst
 setup.py
 src/educommon/__init__.py
 src/educommon/thread_data.py
 src/educommon/version.conf
@@ -186,14 +185,22 @@
 src/educommon/integration_entities/__init__.py
 src/educommon/integration_entities/consts.py
 src/educommon/integration_entities/entities.py
 src/educommon/integration_entities/enums.py
 src/educommon/integration_entities/helpers.py
 src/educommon/integration_entities/mixins.py
 src/educommon/ioc/__init__.py
+src/educommon/logger/__init__.py
+src/educommon/logger/app_settings.py
+src/educommon/logger/apps.py
+src/educommon/logger/consts.py
+src/educommon/logger/formatters.py
+src/educommon/logger/helpers.py
+src/educommon/logger/loggers.py
+src/educommon/logger/records.py
 src/educommon/m3/__init__.py
 src/educommon/m3/transaction_context.py
 src/educommon/m3/extensions/__init__.py
 src/educommon/m3/extensions/ui.py
 src/educommon/m3/extensions/listeners/__init__.py
 src/educommon/m3/extensions/listeners/delete_check/__init__.py
 src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js
```

### Comparing `educommon-2.20.0/tests/test_contingent_plugin_utils.py` & `educommon-3.0.0/tests/test_contingent_plugin_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,31 @@
-# coding: utf-8
-from django.contrib.contenttypes.models import ContentType
-from django.db.models import QuerySet
-from django.test import TestCase
-from educommon.contingent.contingent_plugin.utils import convert_to_json
-from educommon.contingent.contingent_plugin.utils import get_new_param_tuples
-from educommon.contingent.contingent_plugin.utils import (
-    get_original_and_deleted_instances_info)
-from educommon.contingent.contingent_plugin.utils import (
-    get_param_value_from_deleted_model)
+
+from django.contrib.contenttypes.models import (
+    ContentType,
+)
+from django.db.models import (
+    QuerySet,
+)
+from django.test import (
+    TestCase,
+)
+from m3 import (
+    ApplicationLogicException,
+)
+from m3_django_compat import (
+    get_model,
+)
+
 from educommon.contingent.contingent_plugin.utils import (
-    get_params_from_deleted_model)
-from m3_django_compat import get_model
-from m3 import ApplicationLogicException
+    convert_to_json,
+    get_new_param_tuples,
+    get_original_and_deleted_instances_info,
+    get_param_value_from_deleted_model,
+    get_params_from_deleted_model,
+)
 
 
 ContingentModelDeleted = get_model(
     'contingent_plugin', 'ContingentModelDeleted')
 
 
 class TestContingentPluginUtils(TestCase):
@@ -61,15 +71,15 @@
         return get_params_from_deleted_model(self.model, object_id)
 
     def test_get_params_from_deleted_model(self):
         """Тест функции get_params_from_deleted_model."""
 
         data_list = [
             'string', '', '{}',
-            {u'param1': u'param1_value', u'параметр1': u'параметр1_value'}
+            {'param1': 'param1_value', 'параметр1': 'параметр1_value'}
         ]
         for obj_id, data in enumerate(data_list, self.get_next_id()):
             json_data = convert_to_json(data)
             params = self.get_params_from_deleted_model(
                 json_data, object_id=obj_id)
             if isinstance(data, dict):
                 self.assertDictEqual(data, params)
```

### Comparing `educommon-2.20.0/tests/test_delete_objects.py` & `educommon-3.0.0/tests/test_delete_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-# coding:utf-8
-from __future__ import absolute_import
-
 import os
-
-from django.test import TestCase
-from six.moves import cStringIO as StringIO
-from tests.testapp import models
-
-from educommon.utils.system_app.management.commands.delete_objects import \
-    call_custom_command
+from io import (
+    StringIO,
+)
+
+from django.test import (
+    TestCase,
+)
+
+from tests.testapp import (
+    models,
+)
+
+from educommon.utils.system_app.management.commands.delete_objects import (
+    call_custom_command,
+)
 
 
 APP_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 
 
 class DeleteObjectsCommandTestCase(TestCase):
-
-    u"""Тесты для команды educommon.utils.system_app.delete_objects."""
+    """Тесты для команды educommon.utils.system_app.delete_objects."""
 
     count_const = 'ModelA Модель A 4\nModelB Модель B 4\n'
     some_count_const = 'ModelA Модель A 2\nModelB Модель B 2\n'
 
     def add_test_records(self):
-        u"""Заполняет бд тестовыми данными."""
+        """Заполняет бд тестовыми данными."""
         chars = ('test1', 'test2', 'test3', 'test4')
         for index, name in enumerate(chars, 1):
             record = models.ModelA(
                 pk=index,
                 field_a=name,
             )
             record.full_clean()
@@ -38,15 +42,15 @@
                 field_b=name,
                 field_fk=models.ModelA.objects.get(field_a=name)
             )
             record.full_clean()
             record.save()
 
     def test_data_option(self):
-        u"""Тест работы опции --data."""
+        """Тест работы опции --data."""
         # pylint: disable=protected-access
         self.add_test_records()
         out = StringIO()
         call_custom_command(
             'delete_objects', '--model=modela', '--data',
             stdout=out
         )
@@ -54,41 +58,41 @@
             APP_DIR, 'tests', 'fixtures', 'delete_data.json'
         )
         with open(json_path) as json_data:
             reference_data = json_data.read()
         self.assertMultiLineEqual(reference_data, out.getvalue())
 
     def test_count_option(self):
-        u"""Тест работы опции --count."""
+        """Тест работы опции --count."""
         # pylint: disable=protected-access
         self.add_test_records()
         out = StringIO()
         call_custom_command(
             'delete_objects', '--model=modela', '--count',
             stdout=out
         )
         self.assertMultiLineEqual(self.count_const, out.getvalue())
         records = models.ModelA.objects.all().count()
         records += models.ModelB.objects.all().count()
         self.assertEqual(8, records)
 
     def test_some_objects(self):
-        u"""Тест удаления части обьектов."""
+        """Тест удаления части обьектов."""
         # pylint: disable=protected-access
         self.add_test_records()
         out = StringIO()
         call_custom_command('delete_objects', '--model=modela',
                             '--count', '--id__gt=2', stdout=out)
         self.assertMultiLineEqual(self.some_count_const, out.getvalue())
         records = models.ModelA.objects.all().count()
         records += models.ModelB.objects.all().count()
         self.assertEqual(8, records)
 
     def test_delete_objects(self):
-        u"""Тест удаления зависимых обьектов."""
+        """Тест удаления зависимых обьектов."""
         # pylint: disable=protected-access
         self.add_test_records()
         out = StringIO()
         call_custom_command(
             'delete_objects', '--model=modela',
             '--id__gt=2', stdout=out
         )
@@ -98,17 +102,17 @@
         self.assertEqual(2, records)
         records += models.ModelB.objects.all().count()
         self.assertQuerysetEqual([], reference_queryset)
         self.assertQuerysetEqual([], reference_queryset_rel)
         self.assertEqual(4, records)
 
     def test_literal_filter(self):
-        u"""Тест удаления зависимых обьектов с символами кириллицы."""
+        """Тест удаления зависимых обьектов с символами кириллицы."""
         # pylint: disable=protected-access
-        chars = (u'тест1', u'тест2', u'тест3', u'тест4')
+        chars = ('тест1', 'тест2', 'тест3', 'тест4')
         for index, name in enumerate(chars, 1):
             record = models.ModelA(
                 pk=index,
                 field_a=name,
             )
             record.full_clean()
             record.save()
```

### Comparing `educommon-2.20.0/tests/test_django_db_utils.py` & `educommon-3.0.0/tests/test_django_db_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from django.apps import apps
-from django.core.exceptions import ValidationError
-from django.test import TestCase
-
-from educommon.django.db.utils import LazyModel
+from django.apps import (
+    apps,
+)
+from django.core.exceptions import (
+    ValidationError,
+)
+from django.test import (
+    TestCase,
+)
+
+from educommon.django.db.utils import (
+    LazyModel,
+)
 
 
 class LazyModelTestCase(TestCase):
-
-    u"""Тесты для класса educommon.django.db.utils.LazyModel."""
+    """Тесты для класса educommon.django.db.utils.LazyModel."""
 
     def test(self):
         model = apps.get_model('testapp', 'ModelA')
 
         for arg in (
             'testapp.ModelA',
             ('testapp', 'ModelA'),
             model
         ):
             lazy_model = LazyModel(arg)
             self.assertIs(lazy_model.get_model(), model)
 
 
 class ModelModifierWIthMetaClassTestCase(TestCase):
-
     """
     Тесты для утилиты educommon.django.db.utils.model_modifier_metaclass.
     """
 
     def test_max_length_validator(self):
         """Проверяет валидатор максимальной длины.
```

### Comparing `educommon-2.20.0/tests/test_interval_mixins.py` & `educommon-3.0.0/tests/test_interval_mixins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,44 @@
-# coding: utf-8
-from __future__ import absolute_import
-
-from datetime import date
-from datetime import datetime
-from itertools import permutations
-
-from django.core.exceptions import FieldDoesNotExist
-from django.core.exceptions import ValidationError
-from django.test import SimpleTestCase
-from django.test import TestCase
-from tests.testapp.models import DateIntervalModel_1_1
-from tests.testapp.models import DateIntervalModel_1_2
-from tests.testapp.models import DateIntervalModel_1_3
-from tests.testapp.models import DateIntervalModel_2_1
-from tests.testapp.models import DateIntervalModel_2_2
-from tests.testapp.models import DateTimeIntervalModel_1_1
-from tests.testapp.models import DateTimeIntervalModel_1_2
-from tests.testapp.models import DateTimeIntervalModel_1_3
-from tests.testapp.models import DateTimeIntervalModel_2_1
-from tests.testapp.models import DateTimeIntervalModel_2_2
-from tests.testapp.models import ExtraIntervalModel
+from datetime import (
+    date,
+    datetime,
+)
+from itertools import (
+    permutations,
+)
+
+from django.core.exceptions import (
+    FieldDoesNotExist,
+    ValidationError,
+)
+from django.test import (
+    SimpleTestCase,
+    TestCase,
+)
+
+from tests.testapp.models import (
+    DateIntervalModel_1_1,
+    DateIntervalModel_1_2,
+    DateIntervalModel_1_3,
+    DateIntervalModel_2_1,
+    DateIntervalModel_2_2,
+    DateTimeIntervalModel_1_1,
+    DateTimeIntervalModel_1_2,
+    DateTimeIntervalModel_1_3,
+    DateTimeIntervalModel_2_1,
+    DateTimeIntervalModel_2_2,
+    ExtraIntervalModel,
+)
 
 
 class DateIntervalMixinTestCase(TestCase):
-
-    u"""Тесты для примеси DateIntervalMixin."""
+    """Тесты для примеси DateIntervalMixin."""
 
     def test_interval_model_meta(self):
-        u"""Тесты правильности работы метакласса DateIntervalMeta."""
+        """Тесты правильности работы метакласса DateIntervalMeta."""
         # pylint: disable=protected-access
         data = (
             (DateIntervalModel_1_1, 'date_from', 'date_to'),
             (DateIntervalModel_1_2, 'qwe', 'rty'),
             (DateIntervalModel_1_3, 'asd', 'fgh'),
         )
         for model, field_from, field_to in data:
@@ -53,15 +60,15 @@
         finally:
             if 'object1' in locals() and object1.pk is not None:
                 object1.delete()
             if 'object2' in locals() and object2.pk is not None:
                 object2.delete()
 
     def test_intersections(self):
-        u"""Тесты правильности проверки пересечений интервалов."""
+        """Тесты правильности проверки пересечений интервалов."""
         dates = (
             None,
             date(2000, 1, 1),
             date(2000, 2, 1),
             date(2000, 3, 1),
             date(2000, 4, 1),
             None
@@ -91,15 +98,15 @@
                     model,
                     from1, to1, from2, to2,
                     params,
                     invalid=invalid
                 )
 
     def test_date_in_intervals_filter(self):
-        u"""Тестирование метода get_date_in_intervals_filter()."""
+        """Тестирование метода get_date_in_intervals_filter()."""
         model = DateIntervalModel_1_1
 
         # Данные для моделей
         models_data = (
             (1, date(2015, 1, 1), date(2015, 1, 31)),
             (2, date(2015, 2, 1), date(2015, 2, 28)),
             (3, date(2015, 3, 1), date(2015, 3, 31)),
@@ -155,15 +162,15 @@
                     )
                     self.assertEqual(
                         len(result_ids), 1 if include_bounds else 0
                     )
                     self.assertEqual(pk in result_ids, include_bounds)
 
     def test_intersection_daterange_filter(self):
-        u"""Тестирование метода get_intersection_daterange_filter()."""
+        """Тестирование метода get_intersection_daterange_filter()."""
         model = DateIntervalModel_1_1
 
         # Данные для моделей
         models_data = (
             (1, date(2020, 1, 1), date(2020, 1, 31)),
         )
 
@@ -201,15 +208,15 @@
 
             if not exclude:
                 self.assertIn(result.pk, test_ids)
             else:
                 self.assertIsNone(result)
 
     def test_intersection_daterange_filter_with_null_field(self):
-        u"""Тестирование метода get_intersection_daterange_filter() с null."""
+        """Тестирование метода get_intersection_daterange_filter() с null."""
         model = DateIntervalModel_1_1
 
         # Данные для моделей
         models_data = (
             (1, None, date(2020, 1, 31)),
             (2, date(2020, 1, 1), None),
         )
@@ -253,19 +260,18 @@
 
             if result_2:
                 self.assertIn(result_2.pk, test_ids)
 
 
 
 class DateTimeIntervalMixinTestCase(TestCase):
-
-    u"""Тесты для примеси DateTimeIntervalMixin."""
+    """Тесты для примеси DateTimeIntervalMixin."""
 
     def test_interval_model_meta(self):
-        u"""Тесты правильности работы метакласса DateTimeIntervalMeta."""
+        """Тесты правильности работы метакласса DateTimeIntervalMeta."""
         # pylint: disable=protected-access
         data = (
             (DateTimeIntervalModel_1_1, 'datetime_from', 'datetime_to'),
             (DateTimeIntervalModel_1_2, 'qwe', 'rty'),
             (DateTimeIntervalModel_1_3, 'asd', 'fgh'),
         )
         for model, field_from, field_to in data:
@@ -287,15 +293,15 @@
         finally:
             if 'object1' in locals() and object1.pk is not None:
                 object1.delete()
             if 'object2' in locals() and object2.pk is not None:
                 object2.delete()
 
     def test_intersections(self):
-        u"""Тесты правильности проверки пересечений интервалов."""
+        """Тесты правильности проверки пересечений интервалов."""
         dates = (
             None,
             datetime(2000, 1, 1, 10, 9, 15),
             datetime(2000, 2, 1, 10, 9, 15),
             datetime(2000, 3, 1, 10, 9, 15),
             datetime(2000, 4, 1, 10, 9, 15),
             datetime(2000, 4, 1, 10, 9, 15),
@@ -327,15 +333,15 @@
                     model,
                     from1, to1, from2, to2,
                     params,
                     invalid=invalid
                 )
 
     def test_date_in_intervals_filter(self):
-        u"""Тестирование метода get_date_in_intervals_filter()."""
+        """Тестирование метода get_date_in_intervals_filter()."""
         model = DateTimeIntervalModel_1_1
 
         # Данные для моделей
         models_data = (
             (1, datetime(2015, 1, 1), datetime(2015, 1, 31)),
             (2, datetime(2015, 2, 1), datetime(2015, 2, 28)),
             (3, datetime(2015, 3, 1), datetime(2015, 3, 31)),
@@ -395,15 +401,15 @@
                     )
                     self.assertEqual(
                         len(result_ids), 1 if include_bounds else 0
                     )
                     self.assertEqual(pk in result_ids, include_bounds)
 
     def test_intersection_daterange_filter(self):
-        u"""Тестирование метода get_intersection_daterange_filter()."""
+        """Тестирование метода get_intersection_daterange_filter()."""
         model = DateTimeIntervalModel_1_1
 
         # Данные для моделей
         models_data = (
             (1, datetime(2020, 1, 1, 15, 48, 21), datetime(2020, 1, 31, 16)),
         )
 
@@ -474,15 +480,15 @@
 
             if not exclude:
                 self.assertIn(result.pk, test_ids)
             else:
                 self.assertIsNone(result)
 
     def test_intersection_daterange_filter_with_null_field(self):
-        u"""Тестирование метода get_intersection_daterange_filter() с null."""
+        """Тестирование метода get_intersection_daterange_filter() с null."""
         model = DateTimeIntervalModel_1_1
 
         # Данные для моделей
         models_data = (
             (1, None, datetime(2020, 1, 31, 16)),
             (2, datetime(2020, 1, 1, 15, 48, 21), None),
         )
```

### Comparing `educommon-2.20.0/tests/test_patches.py` & `educommon-3.0.0/tests/test_patches.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# coding: utf-8
 """Тесты для патчей."""
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from unittest import TestCase
-from unittest.case import skipUnless
 import sys
-
-from six import binary_type
-
-from educommon.utils.patches import patch_utf8_assertion_error
+from unittest import (
+    TestCase,
+)
+from unittest.case import (
+    skipUnless,
+)
+
+from educommon.utils.patches import (
+    patch_utf8_assertion_error,
+)
 
 
 @skipUnless(sys.version_info.major == 2, 'Python 2 only')
 class AssertionErrorUtf8PatchTestCase(TestCase):
-
     """Проверка патча AssertionError, позволяющего использовать кириллицу."""
 
     @classmethod
     def setUpClass(cls):
         """Патчит AssertionError."""
         cls._old_assertion_error = __builtins__['AssertionError']
         patch_utf8_assertion_error()
```

### Comparing `educommon-2.20.0/tests/test_report.py` & `educommon-3.0.0/tests/test_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# coding: utf-8
-# Unit-тесты для базовых классов отчётной системы
-from __future__ import absolute_import
-
-from django.test import TestCase
-import six
-
-from educommon.report import AbstractDataProvider
-from educommon.report import CompositeDataProvider
-from educommon.report import DependentCompositeProvider
-from educommon.report import FlatDataProviderAdapter
-from educommon.report import NestedDataProviderAdapter
+from django.test import (
+    TestCase,
+)
+
+from educommon.report import (
+    AbstractDataProvider,
+    CompositeDataProvider,
+    DependentCompositeProvider,
+    FlatDataProviderAdapter,
+    NestedDataProviderAdapter,
+)
 
 
 class Provider01(AbstractDataProvider):
-
-    u"""Тестовый провайдер #1."""
+    """Тестовый провайдер #1."""
 
     def init(self, a, b, c):
         self._a = a
         self._b = b
         self._c = c
 
     @property
@@ -31,16 +29,15 @@
 
     @property
     def param03(self):
         return self._c
 
 
 class Provider02(AbstractDataProvider):
-
-    u"""Тестовый провайдер #2."""
+    """Тестовый провайдер #2."""
 
     def init(self, a, b, c):
         self._a = a
         self._b = b
         self._c = c
 
     @property
@@ -57,16 +54,15 @@
 
     @property
     def param04(self):
         return self._a + self._b + self._c
 
 
 class Provider03(AbstractDataProvider):
-
-    u"""Тестовый провайдер #3."""
+    """Тестовый провайдер #3."""
 
     def init(self, a, b, c):
         self._a = a
         self._b = b
         self._c = c
 
     @property
@@ -79,16 +75,15 @@
 
     @property
     def param03(self):
         return self._c
 
 
 class Provider04(AbstractDataProvider):
-
-    u"""Тестовый провайдер #4."""
+    """Тестовый провайдер #4."""
 
     def init(self, a, b, c):
         self._a = a
         self._b = b
         self._c = c
 
     @property
@@ -110,27 +105,25 @@
 BAR, FOO = 42, 2128506
 
 # число параметров во всём дереве провайдеров
 PARAMS_COUNT = 15
 
 
 class MainDataProvider(CompositeDataProvider):
-
-    u"""Композитный тестовый провайдер #1."""
+    """Композитный тестовый провайдер #1."""
 
     provider_name = 'Main'
 
     @property
     def bar(self):
         return BAR
 
 
 class SuperDataProvider(CompositeDataProvider):
-
-    u"""Композитный тестовый провайдер #2."""
+    """Композитный тестовый провайдер #2."""
 
     @property
     def foo(self):
         return FOO
 
 
 def setup_provider():
@@ -149,16 +142,15 @@
     provider.init(a=A, b=B, c=C)
     provider.load_data()
 
     return provider
 
 
 class FlatAdapterTestCase(TestCase):
-
-    u"""Тестирование "плоского" адаптера."""
+    """Тестирование "плоского" адаптера."""
 
     def setUp(self):
         provider = setup_provider()
         self.adapter = FlatDataProviderAdapter(provider, splitter='__')
 
     def test_common(self):
         adapter = self.adapter
@@ -200,36 +192,35 @@
         self.assertEquals(adapter['Main__bar'], BAR)
         self.assertEquals(adapter['foo'], FOO)
 
     def test_iter(self):
         adapter = self.adapter
 
         keys = list(adapter.keys())
-        iter_keys = [k for k in six.iterkeys(adapter)]
+        iter_keys = [k for k in adapter]
         self.assertEqual(keys, iter_keys)
         self.assertEqual(len(keys), PARAMS_COUNT)
 
-        iteritems = [x for x in six.iteritems(adapter)]
+        iteritems = [x for x in adapter.items()]
         self.assertEqual(len(iteritems), PARAMS_COUNT)
         for key, value in iteritems:
             self.assertEqual(value, adapter[key])
 
         items = list(adapter.items())
         for (key, value) in items:
             self.assertEqual(value, adapter[key])
 
         values = list(adapter.values())
-        iter_values = [v for v in six.itervalues(adapter)]
+        iter_values = [v for v in adapter.values()]
         self.assertEqual(values, iter_values)
         self.assertEqual(len(values), PARAMS_COUNT)
 
 
 class NestedAdapterTestCase(TestCase):
-
-    u"""Тестирование иерархического адаптера."""
+    """Тестирование иерархического адаптера."""
 
     def setUp(self):
         provider = setup_provider()
         self.adapter = NestedDataProviderAdapter(provider)
 
     def test_common(self):
         adapter = self.adapter
@@ -268,143 +259,140 @@
         self.assertEquals(adapter['Main']['bar'], BAR)
         self.assertEquals(adapter['foo'], FOO)
 
     def test_iter(self):
         adapter = self.adapter
 
         keys = list(adapter.keys())
-        iter_keys = [k for k in six.iterkeys(adapter)]
+        iter_keys = [k for k in adapter]
         self.assertEqual(keys, iter_keys)
         self.assertEqual(len(keys), 4)
 
         main_keys = list(adapter['Main'].keys())
-        main_iter_keys = [k for k in six.iterkeys(adapter['Main'])]
+        main_iter_keys = [k for k in adapter['Main']]
         self.assertEqual(main_keys, main_iter_keys)
         self.assertEqual(len(main_keys), 3)
 
         p3_keys = list(adapter['Provider03'].keys())
-        p3_iter_keys = [k for k in six.iterkeys(adapter['Provider03'])]
+        p3_iter_keys = [k for k in adapter['Provider03']]
         self.assertEqual(p3_keys, p3_iter_keys)
         self.assertEqual(len(p3_keys), 3)
 
         p4_keys = list(adapter['Provider04'].keys())
-        p4_iter_keys = [k for k in six.iterkeys(adapter['Provider04'])]
+        p4_iter_keys = [k for k in adapter['Provider04']]
         self.assertEqual(p4_keys, p4_iter_keys)
         self.assertEqual(len(p4_keys), 3)
 
-        iteritems = [x for x in six.iteritems(adapter)]
+        iteritems = [x for x in adapter.items()]
         self.assertEqual(len(iteritems), 4)
         for key, value in iteritems:
             self.assertEqual(value, adapter[key])
 
         items = list(adapter.items())
         self.assertEqual(len(items), 4)
         for key, value in items:
             self.assertEqual(value, adapter[key])
 
-        main_iteritems = [x for x in six.iteritems(adapter['Main'])]
+        main_iteritems = [x for x in adapter['Main'].items()]
         self.assertEqual(len(main_iteritems), 3)
         for key, value in main_iteritems:
             self.assertEqual(value, adapter['Main'][key])
 
         main_items = list(adapter['Main'].items())
         self.assertEqual(len(main_items), 3)
         for key, value in main_items:
             self.assertEqual(value, adapter['Main'][key])
 
-        p3_iteritems = [x for x in six.iteritems(adapter['Provider03'])]
+        p3_iteritems = [x for x in adapter['Provider03'].items()]
         self.assertEqual(len(p3_iteritems), 3)
         for key, value in p3_iteritems:
             self.assertEqual(value, adapter['Provider03'][key])
 
         p3_items = [x for x in adapter['Provider03'].items()]
         self.assertEqual(len(p3_items), 3)
         for key, value in p3_items:
             self.assertEqual(value, adapter['Provider03'][key])
 
-        p4_iteritems = [x for x in six.iteritems(adapter['Provider04'])]
+        p4_iteritems = [x for x in adapter['Provider04'].items()]
         self.assertEqual(len(p4_iteritems), 3)
         for key, value in p4_iteritems:
             self.assertEqual(value, adapter['Provider04'][key])
 
         p4_items = [x for x in adapter['Provider04'].items()]
         self.assertEqual(len(p4_items), 3)
         for key, value in p4_items:
             self.assertEqual(value, adapter['Provider04'][key])
 
         values = list(adapter.values())
-        iter_values = [v for v in six.itervalues(adapter)]
+        iter_values = [v for v in adapter.values()]
         self.assertEqual(values, iter_values)
         self.assertEqual(len(values), 4)
 
         main_values = list(adapter['Main'].values())
-        main_iter_values = [k for k in six.itervalues(adapter['Main'])]
+        main_iter_values = [k for k in adapter['Main'].values()]
         self.assertEqual(main_values, main_iter_values)
         self.assertEqual(len(main_values), 3)
 
         p1_values = list(adapter['Main']['Provider01'].values())
         p1_iter_values = [
-            k for k in six.itervalues(adapter['Main']['Provider01'])
+            k for k in adapter['Main']['Provider01'].values()
         ]
         self.assertEqual(p1_values, p1_iter_values)
         self.assertEqual(len(p1_values), 3)
 
         p2_values = list(adapter['Main']['Provider02'].values())
         p2_iter_values = [
-            k for k in six.itervalues(adapter['Main']['Provider02'])
+            k for k in adapter['Main']['Provider02'].values()
         ]
         self.assertEqual(p2_values, p2_iter_values)
         self.assertEqual(len(p2_values), 4)
 
         p3_values = list(adapter['Provider03'].values())
-        p3_iter_values = [k for k in six.itervalues(adapter['Provider03'])]
+        p3_iter_values = [k for k in adapter['Provider03'].values()]
         self.assertEqual(p3_values, p3_iter_values)
         self.assertEqual(len(p3_values), 3)
 
         p4_values = list(adapter['Provider04'].values())
-        p4_iter_values = [k for k in six.itervalues(adapter['Provider04'])]
+        p4_iter_values = [k for k in adapter['Provider04'].values()]
         self.assertEqual(p4_values, p4_iter_values)
         self.assertEqual(len(p4_values), 3)
 
 
 # -----------------------------------------------------------------------------
 # Тест зависимого провайдера
 
 class LowLevel01(AbstractDataProvider):
-
-    u"""Простой подпродвайдер."""
+    """Простой подпродвайдер."""
 
     data = None  # данные будут здесь
 
     def init(self, a, b, c, **params):
         self._a = a
         self._b = b
         self._c = c
 
     def load_data(self):
         self.data = self._a + self._b + self._c
 
 
 class LowLevel02(AbstractDataProvider):
-
-    u"""Простой подпродвайдер."""
+    """Простой подпродвайдер."""
 
     data = None  # данные будут здесь
 
     def init(self, d, e, **params):
         self._d = d
         self._e = e
 
     def load_data(self):
         self.data = self._d + self._e
 
 
 class LowLevelDependent03(AbstractDataProvider):
-
-    u"""
+    """
     Простой подпродвайдер.
 
     Зависит от данных LowLevel01.data и LowLevel02.data
     """
 
     def init(self, f, **params):
         self._f = f
@@ -413,16 +401,15 @@
         self.d_e = None
 
     def load_data(self):
         self.data = self.a_b_c + self.d_e + self._f
 
 
 class HighLevelProvider(DependentCompositeProvider):
-
-    u"""Композитный провайдер с описанием подпровайдеров."""
+    """Композитный провайдер с описанием подпровайдеров."""
 
     providers_order = (
         ('_low_level_01', LowLevel01),
         ('_low_level_02', LowLevel02),
         ('_low_level_03', LowLevelDependent03)
     )
 
@@ -439,16 +426,15 @@
 
     def load_data(self):
         super(HighLevelProvider, self).load_data()
         self.data = self._g + self._low_level_03.data
 
 
 class DependentProviderTestCase(TestCase):
-
-    u"""Тестирование композитного провайдера с описанием подпровайдеров."""
+    """Тестирование композитного провайдера с описанием подпровайдеров."""
 
     def setUp(self):
         self._initial_data = {
             'a': 1,
             'b': 2,
             'c': 3,
             'd': 4,
@@ -456,15 +442,15 @@
             'f': 6,
             'g': 7,
         }
         self.provider = HighLevelProvider()
         self.provider.init(**self._initial_data)
 
     def test_sum(self):
-        u"""
+        """
         Сверка суммы.
 
         Подпровайдеры занимались суммой переданных им значений.
         Один из подпровайдеров (LowLevelDependent03) - зависим от данных
         LowLevel01 и LowLevel02
         """
         self.provider.load_data()
```

### Comparing `educommon-2.20.0/tests/test_service_db_router.py` & `educommon-3.0.0/tests/test_service_db_router.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-# coding: utf-8
-u"""Unit-тесты для роутера моделей приложения, использующего сервисную БД."""
-from __future__ import absolute_import
-
-from django.apps.registry import apps
-from django.test import TestCase
-
-from educommon.django.db.routers import ServiceDbRouterBase
-
-from .settings import DEFAULT_DB_ALIAS
-from .settings import SERVICE_DB_ALIAS
+"""Unit-тесты для роутера моделей приложения, использующего сервисную БД."""
+from django.apps.registry import (
+    apps,
+)
+from django.test import (
+    TestCase,
+)
+
+from educommon.django.db.routers import (
+    ServiceDbRouterBase,
+)
+
+from .settings import (
+    DEFAULT_DB_ALIAS,
+    SERVICE_DB_ALIAS,
+)
 
 
 class ServiceDbRouterTestCase(TestCase):
-
     """Тесты для роутера моделей приложения, использующего сервисную БД."""
 
     def test(self):
         """Проверка правильности выбора роутером базы данных."""
         model1 = apps.get_model('testapp', 'ModelA')
         model2 = apps.get_model('testapp', 'ModelB')
         model3 = apps.get_model('testapp', 'ModelC')
```

### Comparing `educommon-2.20.0/tests/test_utils_plugins.py` & `educommon-3.0.0/tests/test_utils_plugins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# coding: utf-8
-from django.test.testcases import SimpleTestCase
-from six import iteritems
+from django.test.testcases import (
+    SimpleTestCase,
+)
 
-from educommon.utils.plugins import extender_for
+from educommon.utils.plugins import (
+    extender_for,
+)
 
 
-class Window(object):
+class Window:
 
     def __init__(self):
         self._init_components()
         self._do_layout()
 
     def _init_components(self):
         self.items = []
@@ -19,15 +21,15 @@
         self.items.append(self.field1)
 
     def set_params(self, params):
         self.field1.width = 100
 
 
 @extender_for(Window)
-class WindowExtender1(object):
+class WindowExtender1:
 
     extends_methods = ('_init_components', '_do_layout', 'set_params')
 
     @staticmethod
     def _init_components(window, result):
         window.field2 = type('', (), {})()
 
@@ -44,42 +46,41 @@
         window.field1.width = 200
         window.field2.width = 200
 
         return result
 
 
 @extender_for(Window)
-class WindowExtender2(object):
+class WindowExtender2:
 
     extends_methods = ('set_params',)
 
     @staticmethod
     def set_params(window, result, params):
         for item in window.items:
-            for name, value in iteritems(params):
+            for name, value in params.items():
                 setattr(item, name, value)
 
         return result
 
 
 @extender_for(Window)
-class WindowExtender3(object):
+class WindowExtender3:
 
     priority = -1
     extends_methods = ('set_params',)
 
     @staticmethod
     def set_params(window, result, params):
         window.field2.width = 300
         return result
 
 
 class TestCase(SimpleTestCase):
-
-    u"""Проверка работы инструментария для ширения классов."""
+    """Проверка работы инструментария для ширения классов."""
 
     def test(self):
         win = Window()
         win.set_params({'anchor': '100%'})
 
         self.assertIsInstance(win.items, list)
         self.assertEquals(len(win.items), 2)
```

### Comparing `educommon-2.20.0/tests/test_validators.py` & `educommon-3.0.0/tests/test_validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,58 @@
-# coding: utf-8
-u"""Unit-тесты для валидаторов простых полей модели Django."""
-from __future__ import absolute_import
-
-from unittest import TestCase
-
-from django.core.exceptions import ValidationError
-
-from educommon.django.db.validators.simple import doc_type_validator
-from educommon.django.db.validators.simple import inn10_validator
-from educommon.django.db.validators.simple import inn12_validator
-from educommon.django.db.validators.simple import inn_validator
-from educommon.django.db.validators.simple import is_doc_type_valid
-from educommon.django.db.validators.simple import is_inn10_valid
-from educommon.django.db.validators.simple import is_inn12_valid
-from educommon.django.db.validators.simple import is_inn_valid
-from educommon.django.db.validators.simple import is_snils_valid
-from educommon.django.db.validators.simple import snils_validator
+"""Unit-тесты для валидаторов простых полей модели Django."""
+from unittest import (
+    TestCase,
+)
+
+from django.core.exceptions import (
+    ValidationError,
+)
+
+from educommon.django.db.validators.simple import (
+    doc_type_validator,
+    inn10_validator,
+    inn12_validator,
+    inn_validator,
+    is_doc_type_valid,
+    is_inn10_valid,
+    is_inn12_valid,
+    is_inn_valid,
+    is_snils_valid,
+    snils_validator,
+)
 
 
 class SnilsValidatorTestCase(TestCase):
-
     """Тесты для валидатора СНИЛС."""
 
     def test_valid_snils(self):
         """Проверка правильности обработки корректных СНИЛС."""
         valid_snils_list = (
-            u'000-000-111 00',  # < 001-001-998
-            u'111-223-555 88',  # sum < 100
-            u'211-223-655 00',  # sum == 100
-            u'211-223-656 00',  # sum == 101
-            u'231-223-655 15',  # sum > 101, mod < 100
-            u'871-223-654 00',  # sum > 101, mod == 100
+            '000-000-111 00',  # < 001-001-998
+            '111-223-555 88',  # sum < 100
+            '211-223-655 00',  # sum == 100
+            '211-223-656 00',  # sum == 101
+            '231-223-655 15',  # sum > 101, mod < 100
+            '871-223-654 00',  # sum > 101, mod == 100
         )
 
         for snils in valid_snils_list:
             snils_validator(snils)
             self.assertTrue(is_snils_valid(snils), snils)
 
     def test_invalid_snils(self):
         """Проверка правильности обработки некорректных СНИЛС."""
         valid_snils_list = (
-            u'00000011100',
-            u'daskjbn',
-            u'111-223-555 81',
-            u'211-223-655 01',
-            u'211-223-656 01',
-            u'231-223-655 11',
-            u'871-223-654 01',
+            '00000011100',
+            'daskjbn',
+            '111-223-555 81',
+            '211-223-655 01',
+            '211-223-656 01',
+            '231-223-655 11',
+            '871-223-654 01',
         )
 
         for snils in valid_snils_list:
             self.assertRaises(ValidationError, snils_validator, snils)
             self.assertFalse(is_snils_valid(snils), snils)
 
 
@@ -99,72 +101,72 @@
 
 class DocumentTypeValidatorTestCase(TestCase):
     """Тесты для валидатора тип документа."""
 
     def test_valid_snils(self):
         """Проверка правильности обработки корректных типов документа."""
         valid_doc_type_list = (
-            u'Свидетельство о рождении',
-            u'Паспорт гражданина РФ',
-            u'Другой документ, удостоверяющий личность',
-            u'Временное удостоверение личности гражданина РФ',
-            u'Паспорт иностранного гражданина',
-            u'Загранпаспорт гражданина РФ',
-            u'Военный билет',
-            u'Дипломатический паспорт гражданина Российской Федерации',
-            u'Паспорт гражданина СССР',
-            u'Паспорт Минморфлота',
-            u'Паспорт моряка',
-            u'Разрешение на временное проживание в Российской Федерации',
-            u'Свидетельство о рассмотрении ходатайства о признании беженцем '
-            u'на территории Российской Федерации',
-            u'Свидетельство о рождении, выданное уполномоченным органом '
-            u'иностранного государства',
-            u'Справка об освобождении из места лишения свободы',
-            u'Удостоверение личности лица, признанного беженцем',
-            u'Удостоверение личности офицера',
-            u'Удостоверение личности военнослужащего РФ',
-            u'Временное удостоверение, выданное взамен военного билета',
-            u'Удостоверение личности лица без гражданства в РФ',
-            u'Удостоверение личности отдельных категорий лиц, находящихся '
-            u'на территории РФ, подавших заявление о признании гражданами '
-            u'РФ или о приеме в гражданство РФ',
-            u'Удостоверение личности лица, ходатайствующего о признании '
-            u'беженцем на территории РФ',
-            u'Удостоверение личности лица, получившего временное убежище '
-            u'на территории РФ',
-            u'Вид на жительство в Российской Федерации',
-            u'Свидетельство о предоставлении временного убежища на '
-            u'территории Российской Федерации',
-            u'а',
-            u'абв',  # одно слово
-            u'абв абв',  # один пробел
-            u'абв, абв',  # запятая
-            u'абв абв абв',  # три слова
-            u'абв, абв, абв',  # три слова через запятую
-            u'АБВ',
-            u'АБВ АБВ',
-            u'АБВ, АБВ',
-            u'АБВ АБВ АБВ',
-            u'АБВ, АБВ, АБВ',
+            'Свидетельство о рождении',
+            'Паспорт гражданина РФ',
+            'Другой документ, удостоверяющий личность',
+            'Временное удостоверение личности гражданина РФ',
+            'Паспорт иностранного гражданина',
+            'Загранпаспорт гражданина РФ',
+            'Военный билет',
+            'Дипломатический паспорт гражданина Российской Федерации',
+            'Паспорт гражданина СССР',
+            'Паспорт Минморфлота',
+            'Паспорт моряка',
+            'Разрешение на временное проживание в Российской Федерации',
+            'Свидетельство о рассмотрении ходатайства о признании беженцем '
+            'на территории Российской Федерации',
+            'Свидетельство о рождении, выданное уполномоченным органом '
+            'иностранного государства',
+            'Справка об освобождении из места лишения свободы',
+            'Удостоверение личности лица, признанного беженцем',
+            'Удостоверение личности офицера',
+            'Удостоверение личности военнослужащего РФ',
+            'Временное удостоверение, выданное взамен военного билета',
+            'Удостоверение личности лица без гражданства в РФ',
+            'Удостоверение личности отдельных категорий лиц, находящихся '
+            'на территории РФ, подавших заявление о признании гражданами '
+            'РФ или о приеме в гражданство РФ',
+            'Удостоверение личности лица, ходатайствующего о признании '
+            'беженцем на территории РФ',
+            'Удостоверение личности лица, получившего временное убежище '
+            'на территории РФ',
+            'Вид на жительство в Российской Федерации',
+            'Свидетельство о предоставлении временного убежища на '
+            'территории Российской Федерации',
+            'а',
+            'абв',  # одно слово
+            'абв абв',  # один пробел
+            'абв, абв',  # запятая
+            'абв абв абв',  # три слова
+            'абв, абв, абв',  # три слова через запятую
+            'АБВ',
+            'АБВ АБВ',
+            'АБВ, АБВ',
+            'АБВ АБВ АБВ',
+            'АБВ, АБВ, АБВ',
         )
 
         for doc_type in valid_doc_type_list:
             doc_type_validator(doc_type)
             self.assertTrue(is_doc_type_valid(doc_type), doc_type)
 
     def test_invalid_doc_type(self):
         """Проверка правильности обработки некорректных типов документа."""
         invalid_doc_type_list = (
-            u'00000011100',  # цифры
-            u'daskjbn',  # латиница нижний регистр
-            u'DASKJBN',  # латиница верхний регистр
-            u'!*%',  # недопустимые символы
-            u'абв  абв',  # два пробела
-            u' абв абв',  # пробел в начале
-            u'абв абв абв ',  # пробел в конце
-            u'абв , абв',  # пробел до запятой
+            '00000011100',  # цифры
+            'daskjbn',  # латиница нижний регистр
+            'DASKJBN',  # латиница верхний регистр
+            '!*%',  # недопустимые символы
+            'абв  абв',  # два пробела
+            ' абв абв',  # пробел в начале
+            'абв абв абв ',  # пробел в конце
+            'абв , абв',  # пробел до запятой
         )
 
         for doc_type in invalid_doc_type_list:
             self.assertRaises(ValidationError, doc_type_validator, doc_type)
             self.assertFalse(is_doc_type_valid(doc_type), doc_type)
```

### Comparing `educommon-2.20.0/tests/tests_rbac.py` & `educommon-3.0.0/tests/tests_rbac.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-# coding: utf-8
-u"""Тесты для моделей приложения."""
-from __future__ import absolute_import
-
-from abc import ABCMeta
-from abc import abstractproperty
-
-from django.core.exceptions import ValidationError
-from django.test import TestCase
-from six.moves import range
-import six
-
-from educommon.auth.rbac.manager import RBACManager
-from educommon.auth.rbac.models import Permission
-from educommon.auth.rbac.models import Role
-from educommon.auth.rbac.models import RoleParent
-from educommon.auth.rbac.models import RolePermission
+"""Тесты для моделей приложения."""
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
+
+from django.core.exceptions import (
+    ValidationError,
+)
+from django.test import (
+    TestCase,
+)
+
+from educommon.auth.rbac.manager import (
+    RBACManager,
+)
+from educommon.auth.rbac.models import (
+    Permission,
+    Role,
+    RoleParent,
+    RolePermission,
+)
 
 
 class RoleTestCase(TestCase):
-
-    u"""Тесты для модели "Роль"."""
+    """Тесты для модели "Роль"."""
 
     @classmethod
     def setUp(cls):
         cls.roles = {}
         for i in range(1, 9):
             r = Role(name='role{}'.format(i))
             r.full_clean()
@@ -45,31 +49,31 @@
         for child, parent in links:
             child, parent = cls.roles[child], cls.roles[parent]
             rp = RoleParent(role=child, parent=parent)
             rp.full_clean()
             rp.save()
 
         cls.permissions = {
-            1: u'p1',
-            2: u'p2',
-            3: u'p3',
-            4: u'p4',
+            1: 'p1',
+            2: 'p2',
+            3: 'p3',
+            4: 'p4',
         }
-        for i, name in six.iteritems(cls.permissions):
+        for i, name in cls.permissions.items():
             permission = Permission(name=name)
             permission.full_clean()
             permission.save()
             cls.permissions[i] = permission
 
         role_permissions = {
             2: (1, 2),
             6: (3,),
             8: (4,),
         }
-        for role, permissions in six.iteritems(role_permissions):
+        for role, permissions in role_permissions.items():
             role = cls.roles[role]
             for permission in permissions:
                 permission = cls.permissions[permission]
                 RolePermission.objects.create(
                     role=role,
                     permission=permission,
                 )
@@ -78,86 +82,88 @@
     def tearDown(cls):
         RoleParent.objects.all().delete()
         RolePermission.objects.all().delete()
         Role.objects.all().delete()
         cls.roles = {}
 
     def test_cycle(self):
-        u"""Проверка на невозможность создания циклов в иерархии."""
+        """Проверка на невозможность создания циклов в иерархии."""
         links = (
             # role, parent
             (1, 6),
             (1, 4),
         )
 
         for role, parent in links:
             rp = RoleParent(role=self.roles[role], parent=self.roles[parent])
             self.assertRaises(ValidationError, rp.full_clean)
 
     def test_subroles(self):
-        u"""Проверка свойства Role.subroles."""
+        """Проверка свойства Role.subroles."""
         test_data = {
             1: (2, 3, 4, 5, 6, 7, 8),
             2: (4, 5, 6),
             3: (5, 6, 7, 8),
             4: (),
             5: (),
             6: (),
             7: (),
             8: (),
         }
-        for role, subroles in six.iteritems(test_data):
+        for role, subroles in test_data.items():
             role = self.roles[role]
             self.assertEquals(
-                set(u'role{}'.format(i) for i in subroles),
+                set('role{}'.format(i) for i in subroles),
                 set(r.name for r in role.subroles)
             )
 
     def test_permissions(self):
-        u"""Проверка правильности формирования списков разрешений для роли."""
+        """Проверка правильности формирования списков разрешений для роли."""
         test_data = {
             1: (1, 2, 3, 4),
             2: (1, 2, 3),
             3: (3, 4),
             4: (),
             5: (),
             6: (3,),
             7: (),
             8: (4,),
         }
-        for role, permissions in six.iteritems(test_data):
+        for role, permissions in test_data.items():
             role = self.roles[role]
             for i in permissions:
                 self.assertIn(self.permissions[i], role.get_permissions())
 
 
-class ManagerTestCaseBase(six.with_metaclass(ABCMeta, object)):
-
-    u"""Тесты для менеджера RBAC."""
+class ManagerTestCaseBase(metaclass=ABCMeta):
+    """Тесты для менеджера RBAC."""
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def _rbac_backend_class_name(self):
         pass
 
     def setUp(self):
         if not hasattr(self, 'rbac'):
             with self.settings(RBAC_BACKEND=self._rbac_backend_class_name):
                 self.rbac = RBACManager()
                 self.rbac.init()
 
         return super(ManagerTestCaseBase, self).setUp()
 
     def test_permission_dependencies(self):
-        u"""Проверка правильности обработки зависимостей."""
-        from tests.rbac_test.permissions import PERM__PACK1__EDIT
-        from tests.rbac_test.permissions import PERM__PACK1__VIEW
-        from tests.rbac_test.permissions import PERM__PACK2__EDIT
-        from tests.rbac_test.permissions import PERM__PACK2__VIEW
-        from tests.rbac_test.permissions import PERM__PACK3__EDIT
-        from tests.rbac_test.permissions import PERM__PACK3__VIEW
+        """Проверка правильности обработки зависимостей."""
+        from tests.rbac_test.permissions import (
+            PERM__PACK1__EDIT,
+            PERM__PACK1__VIEW,
+            PERM__PACK2__EDIT,
+            PERM__PACK2__VIEW,
+            PERM__PACK3__EDIT,
+            PERM__PACK3__VIEW,
+        )
 
         permissions_map = {
             PERM__PACK1__EDIT: {
                 PERM__PACK1__VIEW,
                 PERM__PACK2__VIEW,
                 PERM__PACK3__EDIT,
                 PERM__PACK3__VIEW,
@@ -171,38 +177,30 @@
             },
             PERM__PACK3__VIEW: {
                 PERM__PACK1__EDIT,
                 PERM__PACK1__VIEW,
                 PERM__PACK2__VIEW,
                 PERM__PACK3__EDIT,
             },
-            PERM__PACK3__VIEW: {
-                PERM__PACK1__EDIT,
-                PERM__PACK1__VIEW,
-                PERM__PACK2__VIEW,
-                PERM__PACK3__EDIT,
-            },
         }
 
-        for permission, dependencies in six.iteritems(permissions_map):
+        for permission, dependencies in permissions_map.items():
             self.assertEquals(
                 self.rbac.get_dependent_permissions(permission),
                 dependencies
             )
 
 
 class ManagerWithSimpleBackendTestCase(ManagerTestCaseBase, TestCase):
-
-    u"""Проверка менеджера RBAC с НЕкеширующим бэкендом ."""
+    """Проверка менеджера RBAC с НЕкеширующим бэкендом ."""
 
     _rbac_backend_class_name = (
         'educommon.auth.rbac.backends.simple.SimpleBackend'
     )
 
 
 class ManagerWithCachingBackendTestCase(ManagerTestCaseBase, TestCase):
-
-    u"""Проверка менеджера RBAC с кеширующим бэкендом ."""
+    """Проверка менеджера RBAC с кеширующим бэкендом ."""
 
     _rbac_backend_class_name = (
         'educommon.auth.rbac.backends.caching.CachingBackend'
     )
```

