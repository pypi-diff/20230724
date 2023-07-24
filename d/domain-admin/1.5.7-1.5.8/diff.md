# Comparing `tmp/domain-admin-1.5.7.tar.gz` & `tmp/domain-admin-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domain-admin-1.5.7.tar", last modified: Mon Jul 24 05:27:45 2023, max compression
+gzip compressed data, was "domain-admin-1.5.8.tar", last modified: Mon Jul 24 15:15:14 2023, max compression
```

## Comparing `domain-admin-1.5.7.tar` & `domain-admin-1.5.8.tar`

### file list

```diff
@@ -1,457 +1,458 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 05:27:30.000000 domain-admin-1.5.7/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-24 05:27:30.000000 domain-admin-1.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-24 05:27:45.933064 domain-admin-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-07-24 05:27:30.000000 domain-admin-1.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.897063 domain-admin-1.5.7/domain_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.901063 domain-admin-1.5.7/domain_admin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/address_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/cert_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/domain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16941 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/domain_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/group_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/ip_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/issue_certificate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/log_async_task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/log_operation_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/log_scheduler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/notify_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/prometheus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/whois_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.901063 domain-admin-1.5.7/domain_admin/config/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/config/default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/config/env_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/config/runtime_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.901063 domain-admin-1.5.7/domain_admin/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/config_key_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/event_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/notify_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/operation_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/role_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/status_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/version_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.901063 domain-admin-1.5.7/domain_admin/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_102_to_103.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_106_to_110.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_110_to_1212.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_1212_to_1213.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_1213_to_131.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_136_to_140_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_140_alpha_to_140.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_1413_to_1414.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_1422_to_1423.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_143_to_144.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_145_to_146.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_151_to_152.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_154_to_155.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/model/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/address_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/domain_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/group_user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/issue_certificate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/log_async_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/log_operation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/log_scheduler_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/notify_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/system_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/version_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.889063 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.889063 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.893063 domain-admin-1.5.7/domain_admin/public/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/objects/01/
--r--r--r--   0 runner    (1001) docker     (123)     1738 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/01/9bb44cfca57b7aa35ea7f5b6f99c3ef48e8d8f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/objects/19/
--r--r--r--   0 runner    (1001) docker     (123)    64350 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/objects/1e/
--r--r--r--   0 runner    (1001) docker     (123)      984 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/1e/270d8f3cc5167242582434675642b5858ba482
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/objects/21/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/objects/30/
--r--r--r--   0 runner    (1001) docker     (123)     7634 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/30/0478ea1f19f5a14d6a7167e9f71f5848707d76
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/3c/
--r--r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
--r--r--r--   0 runner    (1001) docker     (123)   148706 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/40/
--r--r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/40/03c2e07280d146ee3443587c38ea2d264c07ca
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/50/
--r--r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/50/c771a9bca6f87a2fb3381719fe0622eeae23bf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/52/
--r--r--r--   0 runner    (1001) docker     (123)    62564 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/53/
--r--r--r--   0 runner    (1001) docker     (123)      221 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/53/0864cbe282ec11e8564a8a3ce33756977d59ee
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/55/
--r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/58/
--r--r--r--   0 runner    (1001) docker     (123)    11674 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/58/1d5e80145e76e2ba0d08b038e1a2fefebef3bb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/5f/
--r--r--r--   0 runner    (1001) docker     (123)      530 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/69/
--r--r--r--   0 runner    (1001) docker     (123)   279936 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/6c/
--r--r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/6d/
--r--r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/77/
--r--r--r--   0 runner    (1001) docker     (123)     1436 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/77/bb86f804268cc8045d2cd2547ec17c22a0d166
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/79/
--r--r--r--   0 runner    (1001) docker     (123)   105817 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/7f/
--r--r--r--   0 runner    (1001) docker     (123)      368 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/89/
--r--r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/8c/
--r--r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/90/
--r--r--r--   0 runner    (1001) docker     (123)     2691 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/90/4a4570929957b2678d3c499a9cd83658a6675e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/91/
--r--r--r--   0 runner    (1001) docker     (123)      310 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/91/dcfad5270425be228e01a34e9c9b11ef3a0c4e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/92/
--r--r--r--   0 runner    (1001) docker     (123)      200 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/92/cfface0a460c51331fb8f25083a09948e00cbf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/93/
--r--r--r--   0 runner    (1001) docker     (123)     8844 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/93/522d98a7fe61eb676e55f33d92d8d090b967e4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/95/
--r--r--r--   0 runner    (1001) docker     (123)      118 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/95/f07af46d709638b20c0b2c66cdf6de8e89a7e4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/a0/
--r--r--r--   0 runner    (1001) docker     (123)     1814 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/a0/e9b4ee6e91d304066df26b1bc6218de181c2c2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/a2/
--r--r--r--   0 runner    (1001) docker     (123)    17343 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/a2/86b0b36b3538d177580f0c25e8e3a3a9f007b7
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/ab/
--r--r--r--   0 runner    (1001) docker     (123)     1701 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/ab/2ba13bd2bd0cbf3e5b764ff0a29fd5872380c5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/b1/
--r--r--r--   0 runner    (1001) docker     (123)     6011 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/b1/115cb42fa8938fe1dbebccc9584aa03a895df0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/b3/
--r--r--r--   0 runner    (1001) docker     (123)    41902 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/bb/
--r--r--r--   0 runner    (1001) docker     (123)      474 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/bb/ecd10fc84228b6f4a1c2e0c90e2b68d4aa6bf2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/c0/
--r--r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/c0/76a86e24db79ccf75f79903b19cf145419d4bf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/c1/
--r--r--r--   0 runner    (1001) docker     (123)      694 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/c1/ff198374b288725eab95bc1294e1f04fe5c561
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/c4/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/cc/
--r--r--r--   0 runner    (1001) docker     (123)   361458 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/ce/
--r--r--r--   0 runner    (1001) docker     (123)     4311 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/ce/dcd8ba4511fabecdc11df81e55d82ca8b96ca3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/cf/
--r--r--r--   0 runner    (1001) docker     (123)     5817 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/cf/1eea719ca3a291ef7edaa6c60eaa808ca6e4ae
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/d4/
--r--r--r--   0 runner    (1001) docker     (123)     1026 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/d4/9eb5d776f5b92a02189cebbe590f76db9575bd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/d8/
--r--r--r--   0 runner    (1001) docker     (123)      464 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/d8/1e4838c9ac36863e037e68a2f3552f736c5c8f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/e1/
--r--r--r--   0 runner    (1001) docker     (123)    23927 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/e4/
--r--r--r--   0 runner    (1001) docker     (123)     3441 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/e4/c5465d396f947d57739ed8266597d6a47ef51b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/e6/
--r--r--r--   0 runner    (1001) docker     (123)     4593 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/e6/72b6afc2744b043e6fbdf3031eb086a109ec3c
--r--r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/e6/e5ddee110d6ed47cbb0a4f30db3d055efd21da
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/fd/
--r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/ff/
--r--r--r--   0 runner    (1001) docker     (123)    13943 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.893063 domain-admin-1.5.7/domain_admin/public/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.893063 domain-admin-1.5.7/domain_admin/public/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.302e10d7.css
--rw-r--r--   0 runner    (1001) docker     (123)   331526 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.69a97337.css
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.75ef7015.css
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.a676cc2e.css
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.b285e10a.css
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.cf805e1c.css
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.d028ae37.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/gif/
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/gif/user-avatar.ea67286d.gif
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/jpg/
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/jpg/chatpet.fce5580e.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/js/
--rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/ConditionFilterGroup.340936f7.js
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/ConnectStatus.89654d5c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/SearchUser.983b7494.js
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/SelectGroup.d7e6e540.js
--rw-r--r--   0 runner    (1001) docker     (123)   390997 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/codemirror-lib.a3a39aa0.js
--rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/element-icon.1ce1c350.js
--rw-r--r--   0 runner    (1001) docker     (123)   749914 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/element-plus.30eb1cab.js
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/event-enums.6c6f25e7.js
--rw-r--r--   0 runner    (1001) docker     (123)  1058329 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/highlight-lib.3654f6d3.js
--rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.075c6a16.js
--rw-r--r--   0 runner    (1001) docker     (123)    64823 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.12198a8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.127485d4.js
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.16184f42.js
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.2e3ad8c8.js
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.34096d0f.js
--rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.4704b0d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.51aeadc3.js
--rw-r--r--   0 runner    (1001) docker     (123)    28081 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.58059e0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.86cef4dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.a3947126.js
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.ab38e8b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.b84878f9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.c05aa8e8.js
--rw-r--r--   0 runner    (1001) docker     (123)    28958 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.c512b8f1.js
--rw-r--r--   0 runner    (1001) docker     (123)   312580 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/vendor-lib.76301fc3.js
--rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/vendor-vue.9e61e0af.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.893063 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.893063 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.897063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/2d/
--r--r--r--   0 runner    (1001) docker     (123)      814 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/43/
--r--r--r--   0 runner    (1001) docker     (123)     1262 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/4b/
--r--r--r--   0 runner    (1001) docker     (123)     5351 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/5c/
--r--r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/5c/98d16331bcc99b0cbbe89a3ffb23e3f5918ff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/61/
--r--r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/61/05f9fd4f4b11812fcca0d2e0704e4c8dd6e7a3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/62/
--r--r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/62/59838c4de171bc95a934ee2384d626eeb3040a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/67/
--r--r--r--   0 runner    (1001) docker     (123)      478 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/67/d2a69f1213016d777c02e0c99a38871d07da5b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/6f/
--r--r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/71/
--r--r--r--   0 runner    (1001) docker     (123)     2231 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/7a/
--r--r--r--   0 runner    (1001) docker     (123)     2494 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329
--r--r--r--   0 runner    (1001) docker     (123)      968 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/8e/
--r--r--r--   0 runner    (1001) docker     (123)     2655 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/93/
--r--r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6
--r--r--r--   0 runner    (1001) docker     (123)     4673 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/98/
--r--r--r--   0 runner    (1001) docker     (123)     5141 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/a9/
--r--r--r--   0 runner    (1001) docker     (123)     1110 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/b0/
--r--r--r--   0 runner    (1001) docker     (123)     1821 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c2/
--r--r--r--   0 runner    (1001) docker     (123)      505 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c2/c748e84bc4d5118b0e33d6e0073e315a36d034
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c7/
--r--r--r--   0 runner    (1001) docker     (123)    31300 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c8/
--r--r--r--   0 runner    (1001) docker     (123)   143922 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/d9/
--r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/d9/d9ca2809d6994fef91c1ee2d22bc7a54b8b4a5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/ed/
--r--r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/f0/
--r--r--r--   0 runner    (1001) docker     (123)      755 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/f8/
--r--r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/fd/
--r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.897063 domain-admin-1.5.7/domain_admin/public/m/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.897063 domain-admin-1.5.7/domain_admin/public/m/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/common-c7dd5d89.css
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/common.6194c42f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-5eda257b.css
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-958ae3a0.css
--rw-r--r--   0 runner    (1001) docker     (123)   379599 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-9c365a03.js
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-ad047368.css
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-e8224928.css
--rw-r--r--   0 runner    (1001) docker     (123)    53115 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-f79acb3d.css
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index.1a0d1182.js
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index.1d067866.js
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index.daaf9893.js
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index.feef7c0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/login-cb9f43ad.css
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/pages-login-login.09426b90.js
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/uni.06dd3c8e.css
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/user-index-be7005ab.css
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6334 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/static/user-avatar.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/svg/logo.184a2d7d.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.929063 domain-admin-1.5.7/domain_admin/router/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/router/api_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/router/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.929063 domain-admin-1.5.7/domain_admin/service/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/async_task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/common_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/domain_info_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/group_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/group_user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/issue_certificate_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/notify_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/operation_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/render_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/scheduler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/system_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/version_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.929063 domain-admin-1.5.7/domain_admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/templates/cert-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/templates/cert-export.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/templates/domain-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/templates/domain-export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.929063 domain-admin-1.5.7/domain_admin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.929063 domain-admin-1.5.7/domain_admin/utils/acme_util/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/acme_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/acme_util/acme_v2_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/bcrypt_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/cert_util/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_openssl_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_socket_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/datetime_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/domain_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/flask_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/api_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/app_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/flask_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/http_code_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/flask_ext/json/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/json/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/json/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/json/json_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/icp_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/md5_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/open_api/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/open_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/open_api/crtsh_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/open_api/ding_talk_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/open_api/feishu_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/open_api/work_weixin_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/peewee_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/peewee_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/peewee_ext/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/secret_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/text_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/whois_util/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/whois_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/whois_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/whois_util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/whois_util/whois-servers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/whois_util/whois_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.897063 domain-admin-1.5.7/domain_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16145 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-24 05:27:30.000000 domain-admin-1.5.7/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 05:27:45.933064 domain-admin-1.5.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3190 2023-07-24 05:27:30.000000 domain-admin-1.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.793414 domain-admin-1.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 15:14:59.000000 domain-admin-1.5.8/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-24 15:14:59.000000 domain-admin-1.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-24 15:15:14.793414 domain-admin-1.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-07-24 15:14:59.000000 domain-admin-1.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.737414 domain-admin-1.5.8/domain_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.741413 domain-admin-1.5.8/domain_admin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/address_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/cert_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/domain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16941 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/domain_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/group_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/ip_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/issue_certificate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/log_async_task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/log_operation_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/log_scheduler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/notify_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/prometheus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/whois_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.741413 domain-admin-1.5.8/domain_admin/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/config/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/config/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/config/runtime_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.741413 domain-admin-1.5.8/domain_admin/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/config_key_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/event_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/notify_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/operation_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/version_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.745413 domain-admin-1.5.8/domain_admin/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_102_to_103.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_106_to_110.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_110_to_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_1212_to_1213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_1213_to_131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_136_to_140_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_140_alpha_to_140.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_1413_to_1414.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_1422_to_1423.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_143_to_144.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_145_to_146.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_151_to_152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_154_to_155.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.745413 domain-admin-1.5.8/domain_admin/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/address_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/domain_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/group_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/issue_certificate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/log_async_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/log_operation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/log_scheduler_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/notify_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/system_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/version_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.745413 domain-admin-1.5.8/domain_admin/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.725413 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.725413 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.729413 domain-admin-1.5.8/domain_admin/public/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/objects/19/
+-r--r--r--   0 runner    (1001) docker     (123)    64350 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/objects/21/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/objects/2b/
+-r--r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/2b/3195083ee5802a2c60fdb9919fbf35e18e6478
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/objects/32/
+-r--r--r--   0 runner    (1001) docker     (123)     1435 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/32/dd3b54be707f423bd7375381bbc2baede37f8c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/objects/37/
+-r--r--r--   0 runner    (1001) docker     (123)     1700 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/37/11576f2b615224b9477da0a0a9a43c17539d12
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/3c/
+-r--r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
+-r--r--r--   0 runner    (1001) docker     (123)   148706 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/3e/
+-r--r--r--   0 runner    (1001) docker     (123)     1736 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/3e/24054f5e3a680f56b9276efe009e73b7133a99
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/4b/
+-r--r--r--   0 runner    (1001) docker     (123)     8843 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/4b/f6af202944cd3e22f8a375977737ce52b17763
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/52/
+-r--r--r--   0 runner    (1001) docker     (123)    62564 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/55/
+-r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/57/
+-r--r--r--   0 runner    (1001) docker     (123)     5129 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/57/bd1a9bfce972b50e5efecf11f71a3f5b2ec3d3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/5f/
+-r--r--r--   0 runner    (1001) docker     (123)      530 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/60/
+-r--r--r--   0 runner    (1001) docker     (123)      464 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/60/727d43f26f701780e7c55e90cb084973a1be9e
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/69/
+-r--r--r--   0 runner    (1001) docker     (123)   279936 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/6c/
+-r--r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
+-r--r--r--   0 runner    (1001) docker     (123)     6011 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/6c/f21ee6e3a69b2e234f6012f1636e3621d25db8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/6d/
+-r--r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/71/
+-r--r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/71/6b5718c659ed5a85d4f93a2cf25fc5ff5031cb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/79/
+-r--r--r--   0 runner    (1001) docker     (123)   105817 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/7c/
+-r--r--r--   0 runner    (1001) docker     (123)    17315 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/7c/7a565bed760068496030f030f2b05ede1bec4b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/7f/
+-r--r--r--   0 runner    (1001) docker     (123)      368 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/88/
+-r--r--r--   0 runner    (1001) docker     (123)     5817 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/88/eed16a647060a310c6f8fd8cbf109ad11d1211
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/89/
+-r--r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/8c/
+-r--r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/8f/
+-r--r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/8f/3fc862ebdfdd80953e51ae5e44e7862b79ad63
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/92/
+-r--r--r--   0 runner    (1001) docker     (123)      200 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/92/cfface0a460c51331fb8f25083a09948e00cbf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/95/
+-r--r--r--   0 runner    (1001) docker     (123)      118 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/95/f07af46d709638b20c0b2c66cdf6de8e89a7e4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/9a/
+-r--r--r--   0 runner    (1001) docker     (123)     3440 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/9a/44f010e55bd5cd3a7d60bcd86ee9b8e7ef2cef
+-r--r--r--   0 runner    (1001) docker     (123)      177 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/9a/4e8fcc1912f0c1af9a1836ebd9847d8b0e3118
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/a5/
+-r--r--r--   0 runner    (1001) docker     (123)    11673 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/a5/6b22c2eacca280122dde700a98068ebdd8c5af
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/a7/
+-r--r--r--   0 runner    (1001) docker     (123)     4249 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/a7/49320e6e50d7593d7d1d30ee0159023cd4e422
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/ae/
+-r--r--r--   0 runner    (1001) docker     (123)     1815 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/ae/1c9a7def175d7a6389679bf822a6a9219c3ca3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/b2/
+-r--r--r--   0 runner    (1001) docker     (123)     1021 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/b2/9b2820070fd0808f478afc2a5995aaee9cd79f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/b3/
+-r--r--r--   0 runner    (1001) docker     (123)    41902 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/c4/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/c9/
+-r--r--r--   0 runner    (1001) docker     (123)     2690 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/c9/3d3f53fd06fdbc8587e3a8f37876356c5cdb56
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/cc/
+-r--r--r--   0 runner    (1001) docker     (123)   361458 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/d2/
+-r--r--r--   0 runner    (1001) docker     (123)     1024 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/d2/5bbe60e329a2e662af042df10825c9dcdc3887
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/e0/
+-r--r--r--   0 runner    (1001) docker     (123)      312 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/e0/6f4cc670d4bb8f606c4edfb9d7aa51becaaf2a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/e1/
+-r--r--r--   0 runner    (1001) docker     (123)    23927 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/e6/
+-r--r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/e6/8884f9d8cc37153041b8b82943d995c95ba1aa
+-r--r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/e6/e9c9b85a9477efa2c8f05874bd09fa93a6b34c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/e9/
+-r--r--r--   0 runner    (1001) docker     (123)      474 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/e9/8d4dd298d6c05d0bfa2fbe9182ec7cddde7926
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/f9/
+-r--r--r--   0 runner    (1001) docker     (123)      694 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/f9/78f4b33c1fdc0cb74f1df45d0fc049f5da1c89
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/fb/
+-r--r--r--   0 runner    (1001) docker     (123)     7633 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/fb/ac0b57e4138b4fca9c9f5babf558611a38e6d0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/fd/
+-r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/ff/
+-r--r--r--   0 runner    (1001) docker     (123)    13943 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.761413 domain-admin-1.5.8/domain_admin/public/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.761413 domain-admin-1.5.8/domain_admin/public/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.761413 domain-admin-1.5.8/domain_admin/public/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.302e10d7.css
+-rw-r--r--   0 runner    (1001) docker     (123)   331526 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.69a97337.css
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.93c714bb.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.a676cc2e.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.b285e10a.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.cf805e1c.css
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.d028ae37.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.761413 domain-admin-1.5.8/domain_admin/public/gif/
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/gif/user-avatar.ea67286d.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.761413 domain-admin-1.5.8/domain_admin/public/jpg/
+-rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/jpg/chatpet.fce5580e.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.769414 domain-admin-1.5.8/domain_admin/public/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/ConditionFilterGroup.3c6ac067.js
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/ConnectStatus.a429b01b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/SearchUser.f8e52158.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/SelectGroup.53d83114.js
+-rw-r--r--   0 runner    (1001) docker     (123)   390997 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/codemirror-lib.a3a39aa0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/element-icon.1ce1c350.js
+-rw-r--r--   0 runner    (1001) docker     (123)   749914 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/element-plus.30eb1cab.js
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/event-enums.6c6f25e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1058329 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/highlight-lib.3654f6d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/highlight-util.a4f1867f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.0963ab53.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.0d4c27ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64712 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.165f9ce1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28081 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.24e255af.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.2ab02c40.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.3b5a616c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.5b4cd516.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.5f8ece3f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.654f7830.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.8c31b31b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.a8bb8abf.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28958 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.af06b2dc.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.c22f6489.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.deff2c63.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.ef82c865.js
+-rw-r--r--   0 runner    (1001) docker     (123)   312580 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/vendor-lib.76301fc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/vendor-vue.9e61e0af.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.769414 domain-admin-1.5.8/domain_admin/public/m/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/2d/
+-r--r--r--   0 runner    (1001) docker     (123)      814 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/43/
+-r--r--r--   0 runner    (1001) docker     (123)     1262 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/4b/
+-r--r--r--   0 runner    (1001) docker     (123)     5351 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/5c/
+-r--r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/5c/98d16331bcc99b0cbbe89a3ffb23e3f5918ff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/61/
+-r--r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/61/05f9fd4f4b11812fcca0d2e0704e4c8dd6e7a3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/62/
+-r--r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/62/59838c4de171bc95a934ee2384d626eeb3040a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/67/
+-r--r--r--   0 runner    (1001) docker     (123)      478 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/67/d2a69f1213016d777c02e0c99a38871d07da5b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/6f/
+-r--r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/71/
+-r--r--r--   0 runner    (1001) docker     (123)     2231 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/7a/
+-r--r--r--   0 runner    (1001) docker     (123)     2494 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329
+-r--r--r--   0 runner    (1001) docker     (123)      968 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/8e/
+-r--r--r--   0 runner    (1001) docker     (123)     2655 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/93/
+-r--r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6
+-r--r--r--   0 runner    (1001) docker     (123)     4673 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/98/
+-r--r--r--   0 runner    (1001) docker     (123)     5141 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/a9/
+-r--r--r--   0 runner    (1001) docker     (123)     1110 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/b0/
+-r--r--r--   0 runner    (1001) docker     (123)     1821 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c2/
+-r--r--r--   0 runner    (1001) docker     (123)      505 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c2/c748e84bc4d5118b0e33d6e0073e315a36d034
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c7/
+-r--r--r--   0 runner    (1001) docker     (123)    31300 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c8/
+-r--r--r--   0 runner    (1001) docker     (123)   143922 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/d9/
+-r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/d9/d9ca2809d6994fef91c1ee2d22bc7a54b8b4a5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/ed/
+-r--r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/f0/
+-r--r--r--   0 runner    (1001) docker     (123)      755 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/f8/
+-r--r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/fd/
+-r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/m/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/m/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.781414 domain-admin-1.5.8/domain_admin/public/m/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/common-c7dd5d89.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/common.6194c42f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-5eda257b.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-958ae3a0.css
+-rw-r--r--   0 runner    (1001) docker     (123)   379599 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-9c365a03.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-ad047368.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-e8224928.css
+-rw-r--r--   0 runner    (1001) docker     (123)    53115 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-f79acb3d.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index.1a0d1182.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index.1d067866.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index.daaf9893.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index.feef7c0f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/login-cb9f43ad.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/pages-login-login.09426b90.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/uni.06dd3c8e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/user-index-be7005ab.css
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.781414 domain-admin-1.5.8/domain_admin/public/m/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6334 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/static/user-avatar.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.781414 domain-admin-1.5.8/domain_admin/public/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/svg/logo.184a2d7d.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.781414 domain-admin-1.5.8/domain_admin/router/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/router/api_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/router/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.785414 domain-admin-1.5.8/domain_admin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/async_task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/common_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/domain_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/group_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/group_user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/issue_certificate_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/notify_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/operation_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/render_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/scheduler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/system_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/version_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.785414 domain-admin-1.5.8/domain_admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/templates/cert-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/templates/cert-export.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/templates/domain-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/templates/domain-export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.785414 domain-admin-1.5.8/domain_admin/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.785414 domain-admin-1.5.8/domain_admin/utils/acme_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/acme_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/acme_util/acme_v2_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/bcrypt_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/cert_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_openssl_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_socket_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/datetime_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/domain_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/flask_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/api_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/app_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/http_code_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/flask_ext/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/json/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/json/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/json/json_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/icp_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/md5_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/open_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/open_api/crtsh_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/open_api/ding_talk_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/open_api/feishu_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/open_api/work_weixin_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/peewee_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/peewee_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/peewee_ext/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/secret_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/text_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/whois_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/whois_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/whois_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/whois_util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/whois_util/whois-servers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/whois_util/whois_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.737414 domain-admin-1.5.8/domain_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-24 15:14:59.000000 domain-admin-1.5.8/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:15:14.793414 domain-admin-1.5.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3190 2023-07-24 15:14:59.000000 domain-admin-1.5.8/setup.py
```

### Comparing `domain-admin-1.5.7/LICENSE` & `domain-admin-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/PKG-INFO` & `domain-admin-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.5.7
+Version: 1.5.8
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain,ssl,cert,web,monitor
 Platform: any
```

### Comparing `domain-admin-1.5.7/README.md` & `domain-admin-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/address_api.py` & `domain-admin-1.5.8/domain_admin/api/address_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/auth_api.py` & `domain-admin-1.5.8/domain_admin/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/cert_api.py` & `domain-admin-1.5.8/domain_admin/api/cert_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/domain_api.py` & `domain-admin-1.5.8/domain_admin/api/domain_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/domain_info_api.py` & `domain-admin-1.5.8/domain_admin/api/domain_info_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/group_api.py` & `domain-admin-1.5.8/domain_admin/api/group_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/group_user_api.py` & `domain-admin-1.5.8/domain_admin/api/group_user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/issue_certificate_api.py` & `domain-admin-1.5.8/domain_admin/api/issue_certificate_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/log_async_task_api.py` & `domain-admin-1.5.8/domain_admin/api/log_async_task_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/log_operation_api.py` & `domain-admin-1.5.8/domain_admin/api/log_operation_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/log_scheduler_api.py` & `domain-admin-1.5.8/domain_admin/api/log_scheduler_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/notify_api.py` & `domain-admin-1.5.8/domain_admin/api/notify_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/prometheus_api.py` & `domain-admin-1.5.8/domain_admin/api/prometheus_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/system_api.py` & `domain-admin-1.5.8/domain_admin/api/system_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/user_api.py` & `domain-admin-1.5.8/domain_admin/api/user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/api/whois_api.py` & `domain-admin-1.5.8/domain_admin/api/whois_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/compat.py` & `domain-admin-1.5.8/domain_admin/compat.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/config/default_config.py` & `domain-admin-1.5.8/domain_admin/config/default_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/config/env_config.py` & `domain-admin-1.5.8/domain_admin/config/env_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/config/runtime_config.py` & `domain-admin-1.5.8/domain_admin/config/runtime_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/enums/config_key_enum.py` & `domain-admin-1.5.8/domain_admin/enums/config_key_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/enums/operation_enum.py` & `domain-admin-1.5.8/domain_admin/enums/operation_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/enums/version_enum.py` & `domain-admin-1.5.8/domain_admin/enums/version_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/log.py` & `domain-admin-1.5.8/domain_admin/log.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/main.py` & `domain-admin-1.5.8/domain_admin/main.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_102_to_103.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_102_to_103.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_106_to_110.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_106_to_110.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_110_to_1212.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_110_to_1212.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_1212_to_1213.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_1212_to_1213.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_1213_to_131.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_1213_to_131.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_136_to_140_alpha.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_136_to_140_alpha.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_140_alpha_to_140.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_140_alpha_to_140.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_1413_to_1414.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_1413_to_1414.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_1422_to_1423.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_1422_to_1423.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_143_to_144.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_143_to_144.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_145_to_146.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_145_to_146.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_151_to_152.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_151_to_152.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_154_to_155.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_154_to_155.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/migrate/migrate_common.py` & `domain-admin-1.5.8/domain_admin/migrate/migrate_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/address_model.py` & `domain-admin-1.5.8/domain_admin/model/address_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/base_model.py` & `domain-admin-1.5.8/domain_admin/model/base_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/database.py` & `domain-admin-1.5.8/domain_admin/model/database.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/domain_info_model.py` & `domain-admin-1.5.8/domain_admin/model/domain_info_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/domain_model.py` & `domain-admin-1.5.8/domain_admin/model/domain_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/group_model.py` & `domain-admin-1.5.8/domain_admin/model/group_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/group_user_model.py` & `domain-admin-1.5.8/domain_admin/model/group_user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/issue_certificate_model.py` & `domain-admin-1.5.8/domain_admin/model/issue_certificate_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/log_async_task_model.py` & `domain-admin-1.5.8/domain_admin/model/log_async_task_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/log_operation_model.py` & `domain-admin-1.5.8/domain_admin/model/log_operation_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/log_scheduler_model.py` & `domain-admin-1.5.8/domain_admin/model/log_scheduler_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/notify_model.py` & `domain-admin-1.5.8/domain_admin/model/notify_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/system_model.py` & `domain-admin-1.5.8/domain_admin/model/system_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/user_model.py` & `domain-admin-1.5.8/domain_admin/model/user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/model/version_model.py` & `domain-admin-1.5.8/domain_admin/model/version_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/hooks/commit-msg.sample` & `domain-admin-1.5.8/domain_admin/public/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.5.8/domain_admin/public/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-commit.sample` & `domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-push.sample` & `domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-rebase.sample` & `domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-receive.sample` & `domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.5.8/domain_admin/public/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/hooks/push-to-checkout.sample` & `domain-admin-1.5.8/domain_admin/public/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/hooks/sendemail-validate.sample` & `domain-admin-1.5.8/domain_admin/public/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/hooks/update.sample` & `domain-admin-1.5.8/domain_admin/public/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63` & `domain-admin-1.5.8/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949` & `domain-admin-1.5.8/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1` & `domain-admin-1.5.8/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462` & `domain-admin-1.5.8/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34` & `domain-admin-1.5.8/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a` & `domain-admin-1.5.8/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc` & `domain-admin-1.5.8/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b` & `domain-admin-1.5.8/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad` & `domain-admin-1.5.8/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9` & `domain-admin-1.5.8/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b` & `domain-admin-1.5.8/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3` & `domain-admin-1.5.8/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd` & `domain-admin-1.5.8/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/css/ConditionFilterGroup.a91875e6.css` & `domain-admin-1.5.8/domain_admin/public/css/ConditionFilterGroup.a91875e6.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/css/index.69a97337.css` & `domain-admin-1.5.8/domain_admin/public/css/index.69a97337.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/favicon.ico` & `domain-admin-1.5.8/domain_admin/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/gif/user-avatar.ea67286d.gif` & `domain-admin-1.5.8/domain_admin/public/gif/user-avatar.ea67286d.gif`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/index.html` & `domain-admin-1.5.8/domain_admin/public/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       content="width=device-width, initial-scale=1.0"
     />
     <meta
       name="referrer"
       content="no-referrer"
     />
     <title>Domain Admin-域名和SSL证书监测系统</title>
-    <script type="module" crossorigin src="./js/index.12198a8e.js"></script>
+    <script type="module" crossorigin src="./js/index.165f9ce1.js"></script>
     <link rel="modulepreload" crossorigin href="./js/vendor-vue.9e61e0af.js">
     <link rel="modulepreload" crossorigin href="./js/element-icon.1ce1c350.js">
     <link rel="modulepreload" crossorigin href="./js/element-plus.30eb1cab.js">
     <link rel="modulepreload" crossorigin href="./js/vendor-lib.76301fc3.js">
     <link rel="stylesheet" href="./css/index.69a97337.css">
   </head>
   <body>
```

### Comparing `domain-admin-1.5.7/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg` & `domain-admin-1.5.8/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/jpg/chatpet.fce5580e.jpg` & `domain-admin-1.5.8/domain_admin/public/jpg/chatpet.fce5580e.jpg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/js/ConditionFilterGroup.340936f7.js` & `domain-admin-1.5.8/domain_admin/public/js/ConditionFilterGroup.3c6ac067.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     d as O
 } from "./element-plus.30eb1cab.js";
 import {
     _ as D,
     R as E
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     o as d,
     c as u,
     J as I,
     U as w,
     ah as l,
     V as n,
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/ConnectStatus.89654d5c.js` & `domain-admin-1.5.8/domain_admin/public/js/ConnectStatus.a429b01b.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ah as n,
     o as a,
     O as s,
     P as e,
     V as l
 } from "./vendor-vue.9e61e0af.js";
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/SearchUser.983b7494.js` & `domain-admin-1.5.8/domain_admin/public/js/SearchUser.f8e52158.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as l
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ah as c,
     o as d,
     O as i
 } from "./vendor-vue.9e61e0af.js";
 const u = {
     name: "SearchUser",
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/SelectGroup.d7e6e540.js` & `domain-admin-1.5.8/domain_admin/public/js/SelectGroup.53d83114.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     F as h,
     L as g,
     al as _
 } from "./vendor-vue.9e61e0af.js";
 import {
     H as f,
     _ as O
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 const S = u({
         id: "group-store",
         state: () => ({
             groupOptions: []
         }),
         getters: {
             getGroupOptions: e => e.groupOptions
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/codemirror-lib.a3a39aa0.js` & `domain-admin-1.5.8/domain_admin/public/js/codemirror-lib.a3a39aa0.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/js/element-icon.1ce1c350.js` & `domain-admin-1.5.8/domain_admin/public/js/element-icon.1ce1c350.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/js/element-plus.30eb1cab.js` & `domain-admin-1.5.8/domain_admin/public/js/element-plus.30eb1cab.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/js/event-enums.6c6f25e7.js` & `domain-admin-1.5.8/domain_admin/public/js/event-enums.6c6f25e7.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/js/highlight-lib.3654f6d3.js` & `domain-admin-1.5.8/domain_admin/public/js/highlight-lib.3654f6d3.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.075c6a16.js` & `domain-admin-1.5.8/domain_admin/public/js/index.c22f6489.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 import {
     _ as C,
     R as O
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ah as a,
     o as p,
     c as y,
     V as s,
     P as i,
     a as _,
@@ -21,18 +21,18 @@
     Q as T,
     F as A,
     ay as N
 } from "./vendor-vue.9e61e0af.js";
 import {
     S as j,
     u as B
-} from "./SelectGroup.d7e6e540.js";
+} from "./SelectGroup.53d83114.js";
 import {
     S as F
-} from "./SearchUser.983b7494.js";
+} from "./SearchUser.f8e52158.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.76301fc3.js";
 import "./element-plus.30eb1cab.js";
 const P = {
         name: [{
             message: "\u540D\u79F0\u4E0D\u80FD\u4E3A\u7A7A",
             required: !0,
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.12198a8e.js` & `domain-admin-1.5.8/domain_admin/public/js/index.165f9ce1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1259,14 +1259,18 @@
             }, {
                 value: "theme--dark",
                 label: "\u6781\u5BA2"
             }];
             return {
                 toolList: [{
                     type: "router",
+                    label: "SSL\u8BC1\u4E66\u7533\u8BF7",
+                    value: "issue-certificate-list"
+                }, {
+                    type: "router",
                     label: "WHOIS\u67E5\u8BE2",
                     value: "lab"
                 }, {
                     type: "router",
                     label: "\u5B50\u57DF\u540D\u8BC1\u4E66\u67E5\u8BE2",
                     value: "domain-cert-list"
                 }, {
@@ -1274,31 +1278,19 @@
                     label: "\u8BC1\u4E66\u4FE1\u606F\u67E5\u8BE2",
                     value: "cert-info"
                 }, {
                     type: "router",
                     label: "ICP\u5907\u6848\u67E5\u8BE2",
                     value: "icp-info"
                 }, {
-                    type: "router",
-                    label: "SSL\u8BC1\u4E66\u7533\u8BF7",
-                    value: "issue-certificate-list"
-                }, {
                     type: "url",
                     label: "SSL\u914D\u7F6E\u751F\u6210",
                     value: "https://ssl-config.mozilla.org/"
                 }, {
                     type: "url",
-                    label: "\u514D\u8D39SSL\u8BC1\u4E66",
-                    value: "https://yundun.console.aliyun.com/?p=cas#/certExtend/free"
-                }, {
-                    type: "url",
-                    label: "\u57DF\u540D\u6CE8\u518C",
-                    value: "https://wanwang.aliyun.com/"
-                }, {
-                    type: "url",
                     label: "HTTPS\u7F51\u7AD9\u68C0\u6D4B",
                     value: "https://myssl.com/"
                 }],
                 dialogVisible: !1,
                 aboutDialogVisible: !1,
                 userDialogVisible: !1,
                 themeList: e,
@@ -1751,15 +1743,15 @@
         },
         redirect: {
             name: "cert-list"
         },
         children: [{
             path: "list",
             name: "cert-list",
-            component: () => h(() => import("./index.c512b8f1.js"), ["index.c512b8f1.js", "event-enums.6c6f25e7.js", "SelectGroup.d7e6e540.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.340936f7.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "ConnectStatus.89654d5c.js", "vendor-lib.76301fc3.js"], import.meta.url),
+            component: () => h(() => import("./index.af06b2dc.js"), ["index.af06b2dc.js", "event-enums.6c6f25e7.js", "SelectGroup.53d83114.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.3c6ac067.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "ConnectStatus.a429b01b.js", "vendor-lib.76301fc3.js"], import.meta.url),
             meta: {
                 title: "\u8BC1\u4E66\u5217\u8868",
                 icon: "Tickets"
             }
         }]
     }, {
         path: "/domain",
@@ -1771,15 +1763,15 @@
         },
         redirect: {
             name: "domain-list"
         },
         children: [{
             path: "list",
             name: "domain-list",
-            component: () => h(() => import("./index.4704b0d3.js"), ["index.4704b0d3.js", "../css/index.302e10d7.css", "event-enums.6c6f25e7.js", "SelectGroup.d7e6e540.js", "vendor-vue.9e61e0af.js", "SearchUser.983b7494.js", "ConditionFilterGroup.340936f7.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
+            component: () => h(() => import("./index.a8bb8abf.js"), ["index.a8bb8abf.js", "../css/index.302e10d7.css", "event-enums.6c6f25e7.js", "SelectGroup.53d83114.js", "vendor-vue.9e61e0af.js", "SearchUser.f8e52158.js", "ConditionFilterGroup.3c6ac067.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
             meta: {
                 title: "\u57DF\u540D\u5217\u8868",
                 icon: "Coin"
             }
         }]
     }, {
         path: "/group",
@@ -1791,15 +1783,15 @@
         },
         redirect: {
             name: "group-list"
         },
         children: [{
             path: "list",
             name: "group-list",
-            component: () => h(() => import("./index.075c6a16.js"), ["index.075c6a16.js", "vendor-vue.9e61e0af.js", "SelectGroup.d7e6e540.js", "SearchUser.983b7494.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.c22f6489.js"), ["index.c22f6489.js", "vendor-vue.9e61e0af.js", "SelectGroup.53d83114.js", "SearchUser.f8e52158.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u5206\u7EC4\u7BA1\u7406",
                 icon: "Files"
             }
         }]
     }, {
         path: "/notify",
@@ -1811,15 +1803,15 @@
         },
         redirect: {
             name: "notify-list"
         },
         children: [{
             path: "edit",
             name: "notify-list",
-            component: () => h(() => import("./index.58059e0f.js"), ["index.58059e0f.js", "event-enums.6c6f25e7.js", "codemirror-lib.a3a39aa0.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.24e255af.js"), ["index.24e255af.js", "event-enums.6c6f25e7.js", "codemirror-lib.a3a39aa0.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u901A\u77E5\u5217\u8868",
                 icon: "Message"
             }
         }]
     }, {
         path: "/data",
@@ -1832,37 +1824,37 @@
             title: "\u6570\u636E\u7BA1\u7406",
             icon: "Box",
             roles: [D.Admin]
         },
         children: [{
             path: "cert-list",
             name: "data-cert-list",
-            component: () => h(() => import("./index.c512b8f1.js"), ["index.c512b8f1.js", "event-enums.6c6f25e7.js", "SelectGroup.d7e6e540.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.340936f7.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "ConnectStatus.89654d5c.js", "vendor-lib.76301fc3.js"], import.meta.url),
+            component: () => h(() => import("./index.af06b2dc.js"), ["index.af06b2dc.js", "event-enums.6c6f25e7.js", "SelectGroup.53d83114.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.3c6ac067.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "ConnectStatus.a429b01b.js", "vendor-lib.76301fc3.js"], import.meta.url),
             meta: {
                 title: "\u5168\u90E8\u8BC1\u4E66",
                 icon: "Tickets"
             },
             props: {
                 role: D.Admin
             }
         }, {
             path: "domain-list",
             name: "data-domain-list",
-            component: () => h(() => import("./index.4704b0d3.js"), ["index.4704b0d3.js", "../css/index.302e10d7.css", "event-enums.6c6f25e7.js", "SelectGroup.d7e6e540.js", "vendor-vue.9e61e0af.js", "SearchUser.983b7494.js", "ConditionFilterGroup.340936f7.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
+            component: () => h(() => import("./index.a8bb8abf.js"), ["index.a8bb8abf.js", "../css/index.302e10d7.css", "event-enums.6c6f25e7.js", "SelectGroup.53d83114.js", "vendor-vue.9e61e0af.js", "SearchUser.f8e52158.js", "ConditionFilterGroup.3c6ac067.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
             meta: {
                 title: "\u5168\u90E8\u57DF\u540D",
                 icon: "Coin"
             },
             props: {
                 role: D.Admin
             }
         }, {
             path: "group-list",
             name: "data-group-list",
-            component: () => h(() => import("./index.075c6a16.js"), ["index.075c6a16.js", "vendor-vue.9e61e0af.js", "SelectGroup.d7e6e540.js", "SearchUser.983b7494.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.c22f6489.js"), ["index.c22f6489.js", "vendor-vue.9e61e0af.js", "SelectGroup.53d83114.js", "SearchUser.f8e52158.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u5168\u90E8\u5206\u7EC4",
                 icon: "Files"
             },
             props: {
                 role: D.Admin
             }
@@ -1878,24 +1870,24 @@
             title: "\u7CFB\u7EDF\u7BA1\u7406",
             icon: "Setting",
             roles: [D.Admin]
         },
         children: [{
             path: "user-list",
             name: "admin-user-list",
-            component: () => h(() => import("./index.2e3ad8c8.js"), ["index.2e3ad8c8.js", "vendor-vue.9e61e0af.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js"], import.meta.url),
+            component: () => h(() => import("./index.deff2c63.js"), ["index.deff2c63.js", "vendor-vue.9e61e0af.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js"], import.meta.url),
             meta: {
                 title: "\u7528\u6237\u7BA1\u7406",
                 icon: "User",
                 roles: [D.Admin]
             }
         }, {
             path: "system-setup",
             name: "system-setup",
-            component: () => h(() => import("./index.86cef4dd.js"), ["index.86cef4dd.js", "../css/index.d028ae37.css", "vendor-vue.9e61e0af.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
+            component: () => h(() => import("./index.5b4cd516.js"), ["index.5b4cd516.js", "../css/index.d028ae37.css", "vendor-vue.9e61e0af.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
             meta: {
                 title: "\u7CFB\u7EDF\u8BBE\u7F6E",
                 icon: "Setting",
                 roles: [D.Admin]
             }
         }]
     }, {
@@ -1909,33 +1901,33 @@
             title: "\u7CFB\u7EDF\u65E5\u5FD7",
             icon: "Clock",
             roles: [D.Admin]
         },
         children: [{
             path: "log-scheduler-list",
             name: "log-scheduler-list",
-            component: () => h(() => import("./index.b84878f9.js"), ["index.b84878f9.js", "ConnectStatus.89654d5c.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.5f8ece3f.js"), ["index.5f8ece3f.js", "ConnectStatus.a429b01b.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u76D1\u6D4B\u65E5\u5FD7",
                 icon: "Calendar",
                 roles: [D.Admin]
             }
         }, {
             path: "log-operation-list",
             name: "log-operation-list",
-            component: () => h(() => import("./index.16184f42.js"), ["index.16184f42.js", "../css/index.b285e10a.css", "highlight-lib.3654f6d3.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.8c31b31b.js"), ["index.8c31b31b.js", "../css/index.b285e10a.css", "highlight-lib.3654f6d3.js", "vendor-vue.9e61e0af.js", "highlight-util.a4f1867f.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u64CD\u4F5C\u65E5\u5FD7",
                 icon: "Compass",
                 roles: [D.Admin]
             }
         }, {
             path: "log-async-task-list",
             name: "log-async-task-list",
-            component: () => h(() => import("./index.ab38e8b8.js"), ["index.ab38e8b8.js", "ConnectStatus.89654d5c.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.0963ab53.js"), ["index.0963ab53.js", "ConnectStatus.a429b01b.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u5F02\u6B65\u4EFB\u52A1",
                 icon: "Compass",
                 roles: [D.Admin]
             }
         }]
     }, {
@@ -1948,51 +1940,51 @@
         meta: {
             hidden: !0,
             title: "\u5DE5\u5177\u7BB1"
         },
         children: [{
             path: "lab",
             name: "lab",
-            component: () => h(() => import("./index.127485d4.js"), ["index.127485d4.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.3b5a616c.js"), ["index.3b5a616c.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "WHOIS\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }, {
             path: "domain-cert-list",
             name: "domain-cert-list",
-            component: () => h(() => import("./index.51aeadc3.js"), ["index.51aeadc3.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.654f7830.js"), ["index.654f7830.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u5B50\u57DF\u540D\u8BC1\u4E66\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }, {
             path: "cert-info",
             name: "cert-info",
-            component: () => h(() => import("./index.34096d0f.js"), ["index.34096d0f.js", "../css/index.a676cc2e.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.ef82c865.js"), ["index.ef82c865.js", "../css/index.a676cc2e.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u8BC1\u4E66\u4FE1\u606F\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }, {
             path: "icp-info",
             name: "icp-info",
-            component: () => h(() => import("./index.c05aa8e8.js"), ["index.c05aa8e8.js", "../css/index.cf805e1c.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.2ab02c40.js"), ["index.2ab02c40.js", "../css/index.cf805e1c.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "ICP\u5907\u6848\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }, {
             path: "issue-certificate-list",
             name: "issue-certificate-list",
-            component: () => h(() => import("./index.a3947126.js"), ["index.a3947126.js", "../css/index.75ef7015.css", "vendor-vue.9e61e0af.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "ConnectStatus.89654d5c.js"], import.meta.url),
+            component: () => h(() => import("./index.0d4c27ce.js"), ["index.0d4c27ce.js", "../css/index.93c714bb.css", "vendor-vue.9e61e0af.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "highlight-lib.3654f6d3.js", "highlight-util.a4f1867f.js", "ConnectStatus.a429b01b.js"], import.meta.url),
             meta: {
                 title: "SSL\u8BC1\u4E66\u7533\u8BF7",
                 icon: "Box",
                 hidden: !0
             }
         }]
     }];
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.127485d4.js` & `domain-admin-1.5.8/domain_admin/public/js/index.3b5a616c.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
     a as i,
     U as w,
     a9 as S,
     T as b
 } from "./vendor-vue.9e61e0af.js";
 import {
     _ as V
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.76301fc3.js";
 import "./element-plus.30eb1cab.js";
 const k = {
         name: "index",
         props: {},
         components: {},
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.16184f42.js` & `domain-admin-1.5.8/domain_admin/public/js/index.8c31b31b.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,32 @@
 import {
-    H as U,
-    a as J
+    H as U
 } from "./highlight-lib.3654f6d3.js";
 import {
-    _ as R
-} from "./index.12198a8e.js";
+    _ as H
+} from "./index.165f9ce1.js";
 import {
     ah as m,
-    o as x,
+    o as b,
     c as O,
     V as f,
-    P as d,
+    P as h,
     a as w,
     U as T,
-    T as q,
-    ar as M,
-    Q as F
+    T as J,
+    ar as B,
+    Q as M
 } from "./vendor-vue.9e61e0af.js";
+import {
+    h as $
+} from "./highlight-util.a4f1867f.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.76301fc3.js";
 import "./element-plus.30eb1cab.js";
-const W = {
+const F = {
         name: "",
         components: {},
         props: {
             list: {
                 type: Array
             }
         },
@@ -58,158 +60,158 @@
             }
         },
         mounted() {
             U.highlightAll()
         },
         created() {}
     },
-    Q = {
+    W = {
         key: 0
     },
-    Z = ["innerHTML"],
-    G = {
+    Q = ["innerHTML"],
+    Z = {
         key: 1
     },
-    P = ["innerHTML"];
+    G = ["innerHTML"];
 
 function X(n, e, t, s, r, o) {
-    const l = m("el-table-column"),
+    const a = m("el-table-column"),
         u = m("el-tag"),
-        a = m("el-table");
-    return x(), O("div", null, [f(a, {
+        l = m("el-table");
+    return b(), O("div", null, [f(l, {
         data: t.list,
         stripe: "",
         border: ""
     }, {
-        default: d(() => [f(l, {
+        default: h(() => [f(a, {
             label: "\u64CD\u4F5C\u4EBA",
             "header-align": "center",
             align: "center",
             width: "100",
             prop: "user_name",
             "show-overflow-tooltip": ""
         }, {
-            default: d(i => [w("span", null, T(i.row.user_name || "-"), 1)]),
+            default: h(i => [w("span", null, T(i.row.user_name || "-"), 1)]),
             _: 1
-        }), f(l, {
+        }), f(a, {
             label: "\u64CD\u4F5C\u8868",
             width: "120",
             "header-align": "center",
             align: "center",
             prop: "table",
             "show-overflow-tooltip": ""
         }, {
-            default: d(i => [w("span", null, T(i.row.table || "-"), 1)]),
+            default: h(i => [w("span", null, T(i.row.table || "-"), 1)]),
             _: 1
-        }), f(l, {
+        }), f(a, {
             label: "\u64CD\u4F5C\u7C7B\u578B",
             "header-align": "center",
             align: "center",
             prop: "type_id",
             width: "100"
         }, {
-            default: d(i => [f(u, {
+            default: h(i => [f(u, {
                 type: i.row.type_style
             }, {
-                default: d(() => [q(T(i.row.type_label), 1)]),
+                default: h(() => [J(T(i.row.type_label), 1)]),
                 _: 2
             }, 1032, ["type"])]),
             _: 1
-        }), f(l, {
+        }), f(a, {
             label: "\u6570\u636E\u53D8\u5316",
             "header-align": "center",
             align: "left",
             prop: "type_id"
         }, {
-            default: d(i => [i.row.type_style == "" ? (x(), O("pre", Q, [w("code", {
+            default: h(i => [i.row.type_style == "" ? (b(), O("pre", W, [w("code", {
                 class: "language-diff",
                 innerHTML: i.row.data
-            }, null, 8, Z)])) : (x(), O("pre", G, [w("code", {
+            }, null, 8, Q)])) : (b(), O("pre", Z, [w("code", {
                 class: "language-json",
                 innerHTML: i.row.data
-            }, null, 8, P)]))]),
+            }, null, 8, G)]))]),
             _: 1
-        }), f(l, {
+        }), f(a, {
             label: "\u64CD\u4F5C\u65F6\u95F4",
             "header-align": "center",
             align: "center",
             prop: "create_time",
             width: "100"
         }, {
-            default: d(i => [w("span", null, T(i.row.create_time_label || "-"), 1)]),
+            default: h(i => [w("span", null, T(i.row.create_time_label || "-"), 1)]),
             _: 1
         })]),
         _: 1
     }, 8, ["data"])])
 }
-const Y = R(W, [
+const Y = H(F, [
         ["render", X]
     ]),
-    $ = {
+    x = {
         CREATE: 1,
         UPDATE: 2,
         DELETE: 3,
         BATCH_DELETE: 4
     };
 
 function v() {}
 v.prototype = {
     diff: function(e, t) {
         var s = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {},
             r = s.callback;
         typeof s == "function" && (r = s, s = {}), this.options = s;
         var o = this;
 
-        function l(c) {
+        function a(c) {
             return r ? (setTimeout(function() {
                 r(void 0, c)
             }, 0), !0) : c
         }
         e = this.castInput(e), t = this.castInput(t), e = this.removeEmpty(this.tokenize(e)), t = this.removeEmpty(this.tokenize(t));
         var u = t.length,
-            a = e.length,
+            l = e.length,
             i = 1,
-            h = u + a;
-        s.maxEditLength && (h = Math.min(h, s.maxEditLength));
+            d = u + l;
+        s.maxEditLength && (d = Math.min(d, s.maxEditLength));
         var p = [{
                 newPos: -1,
                 components: []
             }],
             g = this.extractCommon(p[0], t, e, 0);
-        if (p[0].newPos + 1 >= u && g + 1 >= a) return l([{
+        if (p[0].newPos + 1 >= u && g + 1 >= l) return a([{
             value: this.join(t),
             count: t.length
         }]);
 
         function _() {
             for (var c = -1 * i; c <= i; c += 2) {
                 var y = void 0,
                     C = p[c - 1],
                     z = p[c + 1],
                     L = (z ? z.newPos : 0) - c;
                 C && (p[c - 1] = void 0);
-                var N = C && C.newPos + 1 < u,
-                    V = z && 0 <= L && L < a;
-                if (!N && !V) {
+                var k = C && C.newPos + 1 < u,
+                    V = z && 0 <= L && L < l;
+                if (!k && !V) {
                     p[c] = void 0;
                     continue
                 }
-                if (!N || V && C.newPos < z.newPos ? (y = ee(z), o.pushComponent(y.components, void 0, !0)) : (y = C, y.newPos++, o.pushComponent(y.components, !0, void 0)), L = o.extractCommon(y, t, e, c), y.newPos + 1 >= u && L + 1 >= a) return l(K(o, y.components, t, e, o.useLongestToken));
+                if (!k || V && C.newPos < z.newPos ? (y = K(z), o.pushComponent(y.components, void 0, !0)) : (y = C, y.newPos++, o.pushComponent(y.components, !0, void 0)), L = o.extractCommon(y, t, e, c), y.newPos + 1 >= u && L + 1 >= l) return a(P(o, y.components, t, e, o.useLongestToken));
                 p[c] = y
             }
             i++
         }
         if (r)(function c() {
             setTimeout(function() {
-                if (i > h) return r();
+                if (i > d) return r();
                 _() || c()
             }, 0)
         })();
         else
-            for (; i <= h;) {
+            for (; i <= d;) {
                 var E = _();
                 if (E) return E
             }
     },
     pushComponent: function(e, t, s) {
         var r = e[e.length - 1];
         r && r.added === t && r.removed === s ? e[e.length - 1] = {
@@ -219,18 +221,18 @@
         } : e.push({
             count: 1,
             added: t,
             removed: s
         })
     },
     extractCommon: function(e, t, s, r) {
-        for (var o = t.length, l = s.length, u = e.newPos, a = u - r, i = 0; u + 1 < o && a + 1 < l && this.equals(t[u + 1], s[a + 1]);) u++, a++, i++;
+        for (var o = t.length, a = s.length, u = e.newPos, l = u - r, i = 0; u + 1 < o && l + 1 < a && this.equals(t[u + 1], s[l + 1]);) u++, l++, i++;
         return i && e.components.push({
             count: i
-        }), e.newPos = u, a
+        }), e.newPos = u, l
     },
     equals: function(e, t) {
         return this.options.comparator ? this.options.comparator(e, t) : e === t || this.options.ignoreCase && e.toLowerCase() === t.toLowerCase()
     },
     removeEmpty: function(e) {
         for (var t = [], s = 0; s < e.length; s++) e[s] && t.push(e[s]);
         return t
@@ -242,145 +244,129 @@
         return e.split("")
     },
     join: function(e) {
         return e.join("")
     }
 };
 
-function K(n, e, t, s, r) {
-    for (var o = 0, l = e.length, u = 0, a = 0; o < l; o++) {
+function P(n, e, t, s, r) {
+    for (var o = 0, a = e.length, u = 0, l = 0; o < a; o++) {
         var i = e[o];
         if (i.removed) {
-            if (i.value = n.join(s.slice(a, a + i.count)), a += i.count, o && e[o - 1].added) {
+            if (i.value = n.join(s.slice(l, l + i.count)), l += i.count, o && e[o - 1].added) {
                 var p = e[o - 1];
                 e[o - 1] = e[o], e[o] = p
             }
         } else {
             if (!i.added && r) {
-                var h = t.slice(u, u + i.count);
-                h = h.map(function(_, E) {
-                    var c = s[a + E];
+                var d = t.slice(u, u + i.count);
+                d = d.map(function(_, E) {
+                    var c = s[l + E];
                     return c.length > _.length ? c : _
-                }), i.value = n.join(h)
+                }), i.value = n.join(d)
             } else i.value = n.join(t.slice(u, u + i.count));
-            u += i.count, i.added || (a += i.count)
+            u += i.count, i.added || (l += i.count)
         }
     }
-    var g = e[l - 1];
-    return l > 1 && typeof g.value == "string" && (g.added || g.removed) && n.equals("", g.value) && (e[l - 2].value += g.value, e.pop()), e
+    var g = e[a - 1];
+    return a > 1 && typeof g.value == "string" && (g.added || g.removed) && n.equals("", g.value) && (e[a - 2].value += g.value, e.pop()), e
 }
 
-function ee(n) {
+function K(n) {
     return {
         newPos: n.newPos,
         components: n.components.slice(0)
     }
 }
-var H = /^[A-Za-z\xC0-\u02C6\u02C8-\u02D7\u02DE-\u02FF\u1E00-\u1EFF]+$/,
-    I = /\S/,
-    B = new v;
-B.equals = function(n, e) {
-    return this.options.ignoreCase && (n = n.toLowerCase(), e = e.toLowerCase()), n === e || this.options.ignoreWhitespace && !I.test(n) && !I.test(e)
+var I = /^[A-Za-z\xC0-\u02C6\u02C8-\u02D7\u02DE-\u02FF\u1E00-\u1EFF]+$/,
+    R = /\S/,
+    q = new v;
+q.equals = function(n, e) {
+    return this.options.ignoreCase && (n = n.toLowerCase(), e = e.toLowerCase()), n === e || this.options.ignoreWhitespace && !R.test(n) && !R.test(e)
 };
-B.tokenize = function(n) {
-    for (var e = n.split(/([^\S\r\n]+|[()[\]{}'"\r\n]|\b)/), t = 0; t < e.length - 1; t++) !e[t + 1] && e[t + 2] && H.test(e[t]) && H.test(e[t + 2]) && (e[t] += e[t + 2], e.splice(t + 1, 2), t--);
+q.tokenize = function(n) {
+    for (var e = n.split(/([^\S\r\n]+|[()[\]{}'"\r\n]|\b)/), t = 0; t < e.length - 1; t++) !e[t + 1] && e[t + 2] && I.test(e[t]) && I.test(e[t + 2]) && (e[t] += e[t + 2], e.splice(t + 1, 2), t--);
     return e
 };
 var j = new v;
 j.tokenize = function(n) {
     var e = [],
         t = n.split(/(\n|\r\n)/);
     t[t.length - 1] || t.pop();
     for (var s = 0; s < t.length; s++) {
         var r = t[s];
         s % 2 && !this.options.newlineIsToken ? e[e.length - 1] += r : (this.options.ignoreWhitespace && (r = r.trim()), e.push(r))
     }
     return e
 };
-var te = new v;
-te.tokenize = function(n) {
+var ee = new v;
+ee.tokenize = function(n) {
     return n.split(/(\S.+?[.!?])(?=\s+|$)/)
 };
-var ne = new v;
-ne.tokenize = function(n) {
+var te = new v;
+te.tokenize = function(n) {
     return n.split(/([{}:;,]|\s+)/)
 };
 
 function A(n) {
     return typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? A = function(e) {
         return typeof e
     } : A = function(e) {
         return e && typeof Symbol == "function" && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
     }, A(n)
 }
-var oe = Object.prototype.toString,
+var ne = Object.prototype.toString,
     D = new v;
 D.useLongestToken = !0;
 D.tokenize = j.tokenize;
 D.castInput = function(n) {
     var e = this.options,
         t = e.undefinedReplacement,
         s = e.stringifyReplacer,
-        r = s === void 0 ? function(o, l) {
-            return typeof l > "u" ? t : l
+        r = s === void 0 ? function(o, a) {
+            return typeof a > "u" ? t : a
         } : s;
     return typeof n == "string" ? n : JSON.stringify(S(n, null, null, r), r, "  ")
 };
 D.equals = function(n, e) {
     return v.prototype.equals.call(D, n.replace(/,([\r\n])/g, "$1"), e.replace(/,([\r\n])/g, "$1"))
 };
 
 function S(n, e, t, s, r) {
     e = e || [], t = t || [], s && (n = s(r, n));
     var o;
     for (o = 0; o < e.length; o += 1)
         if (e[o] === n) return t[o];
-    var l;
-    if (oe.call(n) === "[object Array]") {
-        for (e.push(n), l = new Array(n.length), t.push(l), o = 0; o < n.length; o += 1) l[o] = S(n[o], e, t, s, r);
-        return e.pop(), t.pop(), l
+    var a;
+    if (ne.call(n) === "[object Array]") {
+        for (e.push(n), a = new Array(n.length), t.push(a), o = 0; o < n.length; o += 1) a[o] = S(n[o], e, t, s, r);
+        return e.pop(), t.pop(), a
     }
     if (n && n.toJSON && (n = n.toJSON()), A(n) === "object" && n !== null) {
-        e.push(n), l = {}, t.push(l);
+        e.push(n), a = {}, t.push(a);
         var u = [],
-            a;
-        for (a in n) n.hasOwnProperty(a) && u.push(a);
-        for (u.sort(), o = 0; o < u.length; o += 1) a = u[o], l[a] = S(n[a], e, t, s, a);
+            l;
+        for (l in n) n.hasOwnProperty(l) && u.push(l);
+        for (u.sort(), o = 0; o < u.length; o += 1) l = u[o], a[l] = S(n[l], e, t, s, l);
         e.pop(), t.pop()
-    } else l = n;
-    return l
+    } else a = n;
+    return a
 }
-var k = new v;
-k.tokenize = function(n) {
+var N = new v;
+N.tokenize = function(n) {
     return n.slice()
 };
-k.join = k.removeEmpty = function(n) {
+N.join = N.removeEmpty = function(n) {
     return n
 };
 
-function se(n, e, t) {
-    return k.diff(n, e, t)
+function oe(n, e, t) {
+    return N.diff(n, e, t)
 }
-J.addPlugin({
-    "before:highlightBlock": ({
-        el: n,
-        result: e
-    }) => {
-        console.log("before:highlightBlock")
-    },
-    "after:highlightElement": ({
-        el: n,
-        result: e
-    }) => {
-        console.log("after:highlightElement")
-    },
-    "after:highlight": n => {}
-});
-const b = J.highlight,
-    ie = {
+const se = {
         name: "log_operation-list",
         props: {},
         components: {
             DataTable: Y
         },
         data() {
             return {
@@ -411,30 +397,30 @@
                     e.code == 0 && (this.list = e.data.list.map(t => {
                         try {
                             t.before = JSON.stringify(JSON.parse(t.before), null, 2)
                         } catch {}
                         try {
                             t.after = JSON.stringify(JSON.parse(t.after), null, 2)
                         } catch {}
-                        if (t.type_id == $.UPDATE) {
-                            let r = se(t.before.split(`
+                        if (t.type_id == x.UPDATE) {
+                            let r = oe(t.before.split(`
 `), t.after.split(`
-`)).map(o => o.added ? o.value.map(l => "+" + l).join(`
-`) : o.removed ? o.value.map(l => "-" + l).join(`
-`) : o.value.map(l => l).join(`
+`)).map(o => o.added ? o.value.map(a => "+" + a).join(`
+`) : o.removed ? o.value.map(a => "-" + a).join(`
+`) : o.value.map(a => a).join(`
 `));
-                            t.data = b(r.join(`
+                            t.data = $(r.join(`
 `), {
                                 language: "diff"
                             }).value, t.type_style = ""
-                        } else t.type_id == $.CREATE ? (t.data = b(t.after, {
+                        } else t.type_id == x.CREATE ? (t.data = $(t.after, {
                             language: "json"
-                        }).value, t.type_style = "success") : t.type_id == $.DELETE ? (t.data = b(t.before, {
+                        }).value, t.type_style = "success") : t.type_id == x.DELETE ? (t.data = $(t.before, {
                             language: "json"
-                        }).value, t.type_style = "danger") : t.type_id == $.BATCH_DELETE && (t.data = b(t.before, {
+                        }).value, t.type_style = "danger") : t.type_id == x.BATCH_DELETE && (t.data = $(t.before, {
                             language: "json"
                         }).value, t.type_style = "danger");
                         return t
                     }), this.total = e.data.total)
                 } catch (e) {
                     console.log(e)
                 } finally {
@@ -479,47 +465,47 @@
                 }
             }
         },
         created() {
             this.loadPageSize(), this.getData()
         }
     },
-    re = {
+    ie = {
         class: "app-container"
     },
-    le = {
+    re = {
         class: "flex justify-between mb-sm"
     },
     ae = w("div", null, null, -1);
 
-function ue(n, e, t, s, r, o) {
-    const l = m("Delete"),
+function le(n, e, t, s, r, o) {
+    const a = m("Delete"),
         u = m("el-icon"),
-        a = m("el-link"),
+        l = m("el-link"),
         i = m("el-popconfirm"),
-        h = m("DataTable"),
+        d = m("DataTable"),
         p = m("el-pagination"),
-        g = M("loading");
-    return x(), O("div", re, [w("div", le, [ae, f(i, {
+        g = B("loading");
+    return b(), O("div", ie, [w("div", re, [ae, f(i, {
         title: "\u786E\u5B9A\u6E05\u7A7A\u65E5\u5FD7\uFF1F",
         onConfirm: o.clearLogOperationList
     }, {
-        reference: d(() => [f(a, {
+        reference: h(() => [f(l, {
             underline: !1,
             type: "danger",
             class: "mr-sm"
         }, {
-            default: d(() => [f(u, null, {
-                default: d(() => [f(l)]),
+            default: h(() => [f(u, null, {
+                default: h(() => [f(a)]),
                 _: 1
-            }), q("\u6E05\u7A7A\u65E5\u5FD7")]),
+            }), J("\u6E05\u7A7A\u65E5\u5FD7")]),
             _: 1
         })]),
         _: 1
-    }, 8, ["onConfirm"])]), F(f(h, {
+    }, 8, ["onConfirm"])]), M(f(d, {
         list: r.list,
         onOnSuccess: o.resetData
     }, null, 8, ["list", "onOnSuccess"]), [
         [g, r.loading]
     ]), f(p, {
         class: "mt-md justify-center",
         background: "",
@@ -529,14 +515,14 @@
         "onUpdate:pageSize": e[0] || (e[0] = _ => r.size = _),
         "current-page": r.page,
         "onUpdate:currentPage": e[1] || (e[1] = _ => r.page = _),
         onCurrentChange: o.getData,
         onSizeChange: o.handleSizeChange
     }, null, 8, ["total", "page-size", "current-page", "onCurrentChange", "onSizeChange"])])
 }
-const _e = R(ie, [
-    ["render", ue]
+const _e = H(se, [
+    ["render", le]
 ]);
 export {
     _e as
     default
 };
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.2e3ad8c8.js` & `domain-admin-1.5.8/domain_admin/public/js/index.deff2c63.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as C
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ah as i,
     o as b,
     c as k,
     V as t,
     P as l,
     a as h,
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.34096d0f.js` & `domain-admin-1.5.8/domain_admin/public/js/index.ef82c865.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
     F as k,
     a8 as N,
     az as w,
     aA as j
 } from "./vendor-vue.9e61e0af.js";
 import {
     _ as V
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.76301fc3.js";
 import "./element-plus.30eb1cab.js";
 const A = {
         name: "index",
         props: {},
         components: {},
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.4704b0d3.js` & `domain-admin-1.5.8/domain_admin/public/js/index.a8bb8abf.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 import {
     i as X,
     E as Z
 } from "./event-enums.6c6f25e7.js";
 import {
     S as q,
     u as $
-} from "./SelectGroup.d7e6e540.js";
+} from "./SelectGroup.53d83114.js";
 import {
     S as ee
-} from "./SearchUser.983b7494.js";
+} from "./SearchUser.f8e52158.js";
 import {
     R as V,
     _ as v,
     u as te,
     d as j,
     r as oe
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ax as G,
     ah as r,
     ar as P,
     Q as A,
     o as m,
     c as y,
@@ -40,15 +40,15 @@
 } from "./vendor-vue.9e61e0af.js";
 import {
     E as M,
     A as ae,
     a as re,
     b as de,
     C as ce
-} from "./ConditionFilterGroup.340936f7.js";
+} from "./ConditionFilterGroup.3c6ac067.js";
 import {
     F as me
 } from "./vendor-lib.76301fc3.js";
 import {
     b as ue
 } from "./element-plus.30eb1cab.js";
 import "./element-icon.1ce1c350.js";
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.51aeadc3.js` & `domain-admin-1.5.8/domain_admin/public/js/index.654f7830.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as u
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ah as n,
     o as _,
     c as g,
     V as a,
     P as l,
     a as c,
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.58059e0f.js` & `domain-admin-1.5.8/domain_admin/public/js/index.24e255af.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
     T as K,
     t as Q,
     o as B,
     j as X
 } from "./codemirror-lib.a3a39aa0.js";
 import {
     _ as V
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ah as i,
     o as b,
     O as x,
     K as Y,
     c as S,
     V as o,
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.86cef4dd.js` & `domain-admin-1.5.8/domain_admin/public/js/index.5b4cd516.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as g
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ah as a,
     o as u,
     c as d,
     V as r,
     P as l,
     a as f,
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.a3947126.js` & `domain-admin-1.5.8/domain_admin/public/js/index.0d4c27ce.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,42 @@
 import {
     _ as v
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
-    ah as a,
-    o as d,
+    ah as l,
+    o as m,
     c as h,
-    V as s,
+    V as t,
     P as n,
-    a as p,
-    T as y,
-    U as g,
+    a as d,
+    T as w,
+    U as S,
     F as $,
     a8 as V,
-    az as L,
-    aA as R,
     O as k,
     S as O,
-    ar as T,
-    a9 as U,
-    Q as z
+    ar as R,
+    a9 as F,
+    Q as E
 } from "./vendor-vue.9e61e0af.js";
 import {
-    F as x
+    F as D
 } from "./vendor-lib.76301fc3.js";
 import {
-    C as A
-} from "./ConnectStatus.89654d5c.js";
+    H as L
+} from "./highlight-lib.3654f6d3.js";
+import {
+    h as H
+} from "./highlight-util.a4f1867f.js";
+import {
+    C as I
+} from "./ConnectStatus.a429b01b.js";
 import "./element-icon.1ce1c350.js";
 import "./element-plus.30eb1cab.js";
-const B = {
+const U = {
         domains: [{
             message: "\u57DF\u540D\u5217\u8868\u4E0D\u80FD\u4E3A\u7A7A",
             required: !0,
             trigger: "blur"
         }],
         status: [{
             message: "\u9A8C\u8BC1\u72B6\u6001\u4E0D\u80FD\u4E3A\u7A7A",
@@ -51,26 +55,26 @@
         }],
         create_time_label: [{
             message: "\u521B\u5EFA\u65F6\u95F4\u4E0D\u80FD\u4E3A\u7A7A",
             required: !0,
             trigger: "blur"
         }]
     },
-    j = {
+    B = {
         name: "",
         props: {
             row: {
                 type: Object,
                 default: null
             }
         },
         components: {},
         data() {
             return {
-                rules: B,
+                rules: U,
                 form: {
                     domains: "",
                     status: "",
                     start_time: "",
                     expire_time: "",
                     create_time_label: ""
                 }
@@ -81,16 +85,16 @@
             async getData() {
                 if (this.row) {
                     let i = {
                         id: this.row.id
                     };
                     const e = await this.$http.function(i);
                     if (e.code != 0) return;
-                    let t = e.data;
-                    this.form.domains = t.domains, this.form.status = t.status, this.form.start_time = t.start_time, this.form.expire_time = t.expire_time, this.form.create_time_label = t.create_time_label
+                    let s = e.data;
+                    this.form.domains = s.domains, this.form.status = s.status, this.form.start_time = s.start_time, this.form.expire_time = s.expire_time, this.form.create_time_label = s.create_time_label
                 }
             },
             handleCancel() {
                 this.$emit("on-cancel")
             },
             handleSubmit() {
                 this.$refs.form.validate(i => {
@@ -103,309 +107,401 @@
                         fullscreen: !0
                     }),
                     e = {
                         domains: this.form.domains.split(`
 `)
                     };
                 this.row && (e.id = this.row.id);
-                const t = await this.$http.issueCertificate(e);
-                t.code == 0 ? (this.$msg.success("\u64CD\u4F5C\u6210\u529F"), this.$emit("on-success", t.data)) : this.$msg.error(t.msg), this.$nextTick(() => {
+                const s = await this.$http.issueCertificate(e);
+                s.code == 0 ? (this.$msg.success("\u64CD\u4F5C\u6210\u529F"), this.$emit("on-success", s.data)) : this.$msg.error(s.msg), this.$nextTick(() => {
                     i.close()
                 })
             }
         },
         created() {
             this.getData()
         }
     },
-    E = {
+    j = {
         class: "text-center"
     };
 
-function q(i, e, t, C, l, o) {
-    const r = a("el-input"),
-        u = a("el-form-item"),
-        m = a("el-form"),
-        _ = a("el-button");
-    return d(), h("div", null, [s(m, {
+function z(i, e, s, C, a, o) {
+    const r = l("el-input"),
+        _ = l("el-form-item"),
+        p = l("el-form"),
+        u = l("el-button");
+    return m(), h("div", null, [t(p, {
         ref: "form",
-        model: l.form,
-        rules: l.rules,
+        model: a.form,
+        rules: a.rules,
         "label-width": "100px"
     }, {
-        default: n(() => [s(u, {
+        default: n(() => [t(_, {
             label: "id",
             prop: "id",
             style: {
                 display: "none"
             }
         }, {
-            default: n(() => [s(r, {
+            default: n(() => [t(r, {
                 type: "text",
-                modelValue: l.form.id,
-                "onUpdate:modelValue": e[0] || (e[0] = f => l.form.id = f),
-                rows: 3,
+                modelValue: a.form.id,
+                "onUpdate:modelValue": e[0] || (e[0] = f => a.form.id = f),
                 placeholder: "id"
             }, null, 8, ["modelValue"])]),
             _: 1
-        }), s(u, {
+        }), t(_, {
             label: "\u57DF\u540D\u5217\u8868",
             prop: "domains"
         }, {
-            default: n(() => [s(r, {
+            default: n(() => [t(r, {
                 type: "textarea",
-                modelValue: l.form.domains,
-                "onUpdate:modelValue": e[1] || (e[1] = f => l.form.domains = f),
-                rows: 3,
+                modelValue: a.form.domains,
+                "onUpdate:modelValue": e[1] || (e[1] = f => a.form.domains = f),
+                rows: 5,
                 placeholder: "\u8BF7\u8F93\u5165\u57DF\u540D\u5217\u8868\uFF0C\u6BCF\u884C\u4E00\u4E2A"
             }, null, 8, ["modelValue"])]),
             _: 1
         })]),
         _: 1
-    }, 8, ["model", "rules"]), p("div", E, [s(_, {
+    }, 8, ["model", "rules"]), d("div", j, [t(u, {
         onClick: o.handleCancel
     }, {
-        default: n(() => [y("\u53D6 \u6D88")]),
+        default: n(() => [w("\u53D6 \u6D88")]),
         _: 1
-    }, 8, ["onClick"]), s(_, {
+    }, 8, ["onClick"]), t(u, {
         type: "primary",
         onClick: o.handleSubmit
     }, {
-        default: n(() => [y("\u786E \u5B9A")]),
+        default: n(() => [w("\u786E \u5B9A")]),
         _: 1
     }, 8, ["onClick"])])])
 }
-const F = v(j, [
-    ["render", q]
+const A = v(B, [
+    ["render", z]
 ]);
-const K = {
+const M = {
         name: "VerifyStep",
         props: {
             form: {
                 type: Object
             }
         },
         components: {},
         data() {
             return {}
         },
-        computed: {},
+        computed: {
+            domain_list() {
+                return this.form.domains.join(" ")
+            },
+            nginxConfig() {
+                return `server {
+  listen 80;
+  server_name ${this.domain_list};
+
+  location /.well-known/acme-challenge/ {
+      alias /var/www/challenges/;
+      try_files $uri =404;
+  }
+}`
+            }
+        },
         methods: {
             async getData() {},
             async handleSubmit() {
                 let i = this.$loading({
                         fullscreen: !0
                     }),
                     e = {
                         issue_certificate_id: this.form.id
                     };
-                const t = await this.$http.verifyCertificateById(e);
-                t.code == 0 ? (this.$msg.success("\u9A8C\u8BC1\u6210\u529F"), this.$emit("on-success", t.data)) : this.$msg.error(t.msg), this.$nextTick(() => {
+                const s = await this.$http.verifyCertificateById(e);
+                s.code == 0 ? (this.$msg.success("\u9A8C\u8BC1\u6210\u529F"), this.$emit("on-success", s.data)) : this.$msg.error(s.msg), this.$nextTick(() => {
                     i.close()
                 })
+            },
+            downloadVerifyFile() {
+                let i = new Blob([this.form.validation], {
+                    type: "application/octet-stream;charset=utf-8"
+                });
+                D.saveAs(i, this.form.token)
             }
         },
+        mounted() {
+            L.highlightAll()
+        },
         created() {
             this.getData()
         }
     },
-    N = i => (L("data-v-5e5bcfb1"), i = i(), R(), i),
-    P = {
+    N = {
         class: "mo-form-detail"
     },
-    H = N(() => p("span", null, "\u6587\u4EF6", -1)),
-    J = {
+    q = {
         class: "verify-step__value"
     },
-    Q = {
+    K = {
         class: "verify-step__value"
     },
-    G = ["href"],
-    M = {
+    P = ["href"],
+    G = {
+        style: {
+            padding: "10px 0",
+            "overflow-x": "auto",
+            width: "100%"
+        }
+    },
+    J = ["innerHTML"],
+    Q = {
         class: "text-center mt-md"
     };
 
-function W(i, e, t, C, l, o) {
-    const r = a("el-form-item"),
-        u = a("el-form"),
-        m = a("el-button");
-    return d(), h("div", P, [s(u, {
+function W(i, e, s, C, a, o) {
+    const r = l("Download"),
+        _ = l("el-icon"),
+        p = l("el-link"),
+        u = l("el-form-item"),
+        f = l("el-form"),
+        b = l("el-button");
+    return m(), h("div", N, [t(f, {
         "label-width": "130px"
     }, {
-        default: n(() => [s(r, {
-            label: "\u57DF\u540D\u6388\u6743\u9A8C\u8BC1\u7C7B\u578B",
+        default: n(() => [t(u, {
+            label: "\u9A8C\u8BC1\u6587\u4EF6",
             prop: "domain"
         }, {
-            default: n(() => [H]),
+            default: n(() => [t(p, {
+                underline: !1,
+                type: "primary",
+                class: "mr-sm",
+                onClick: o.downloadVerifyFile
+            }, {
+                default: n(() => [t(_, null, {
+                    default: n(() => [t(r)]),
+                    _: 1
+                }), w("\u70B9\u51FB\u4E0B\u8F7D")]),
+                _: 1
+            }, 8, ["onClick"])]),
             _: 1
-        }), s(r, {
+        }), t(u, {
             label: "\u6587\u4EF6\u5185\u5BB9",
             prop: "create_time"
         }, {
-            default: n(() => [p("span", J, g(t.form.validation), 1)]),
+            default: n(() => [d("span", q, S(s.form.validation), 1)]),
             _: 1
-        }), s(r, {
+        }), t(u, {
             label: "\u670D\u52A1\u5668\u76EE\u5F55",
             prop: "create_time"
         }, {
-            default: n(() => [p("span", Q, "/.well-known/acme-challenge/" + g(t.form.token), 1)]),
+            default: n(() => [d("span", K, "/.well-known/acme-challenge/" + S(s.form.token), 1)]),
             _: 1
-        }), s(r, {
+        }), t(u, {
             label: "HTTP\u5730\u5740",
             prop: "isp"
         }, {
-            default: n(() => [(d(!0), h($, null, V(t.form.domain_validation_urls, _ => (d(), h("div", null, [p("a", {
-                href: _,
+            default: n(() => [(m(!0), h($, null, V(s.form.domain_validation_urls, g => (m(), h("div", null, [d("a", {
+                href: g,
                 class: "verify-step__value mo-link",
                 target: "_blank"
-            }, g(_), 9, G)]))), 256))]),
+            }, S(g), 9, P)]))), 256))]),
+            _: 1
+        }), t(u, {
+            label: "Nginx\u914D\u7F6E",
+            prop: "isp"
+        }, {
+            default: n(() => [d("div", G, [d("pre", null, [d("code", {
+                innerHTML: o.nginxConfig
+            }, null, 8, J)])])]),
             _: 1
         })]),
         _: 1
-    }), p("div", M, [s(m, {
+    }), d("div", Q, [t(b, {
         type: "primary",
         onClick: o.handleSubmit
     }, {
-        default: n(() => [y("\u9A8C \u8BC1")]),
+        default: n(() => [w("\u9A8C \u8BC1")]),
         _: 1
     }, 8, ["onClick"])])])
 }
-const X = v(K, [
+const X = v(M, [
     ["render", W],
-    ["__scopeId", "data-v-5e5bcfb1"]
+    ["__scopeId", "data-v-1fbf3592"]
 ]);
 const Y = {
         name: "VerifyStep",
         props: {
             form: {
                 type: Object
             }
         },
         components: {},
         data() {
-            return {}
+            return {
+                nginxConfigTemplate: `server {
+    listen 443 ssl;
+    server_name ${this.form.domain_list};
+
+    ssl_certificate /path/to/${this.form.domains[0]}.pem;
+    ssl_certificate_key /path/to/${this.form.domains[0]}.key;
+    ssl_session_timeout 5m;
+    ssl_protocols TLSv1.2;
+    ssl_ciphers ECDHE-RSA-AES256-GCM-SHA384:ECDHE-RSA-AES128-GCM-SHA256:DHE-RSA-AES256-GCM-SHA384;
+    ssl_session_cache shared:SSL:50m;
+    ssl_dhparam /path/to/server.dhparam;
+    ssl_prefer_server_ciphers on;
+}`
+            }
+        },
+        computed: {
+            domain_list() {
+                return this.form.domains.join(" ")
+            },
+            nginxConfig() {
+                return H(this.nginxConfigTemplate, {
+                    language: "nginx"
+                }).value
+            }
         },
-        computed: {},
         methods: {
             async getData() {},
             handleClose() {
                 this.$emit("on-close")
             },
             async handleSubmit() {
                 let i = this.$loading({
                         fullscreen: !0
                     }),
                     e = {
                         issue_certificate_id: this.form.id
                     };
-                const t = await this.$http.renewCertificate(e);
-                return t.code == 0 ? (this.$msg.success("\u64CD\u4F5C\u6210\u529F"), this.$emit("on-success", t.data)) : this.$msg.error(t.msg), this.$nextTick(() => {
+                const s = await this.$http.renewCertificate(e);
+                return s.code == 0 ? (this.$msg.success("\u64CD\u4F5C\u6210\u529F"), this.$emit("on-success", s.data)) : this.$msg.error(s.msg), this.$nextTick(() => {
                     i.close()
-                }), t
+                }), s
             },
             downloadSSLKeyFile() {
                 console.log(JSON.stringify(this.form, null, 2));
                 let i = new Blob([this.form.ssl_certificate_key], {
                         type: "text/plain;charset=utf-8"
                     }),
                     e = this.form.domains[0];
-                x.saveAs(i, `${e}.key`)
+                D.saveAs(i, `${e}.key`)
             },
             async downloadSSLFile() {
                 if (!this.form.ssl_certificate) {
-                    const t = await this.handleSubmit();
-                    this.form.ssl_certificate = t.data.ssl_certificate
+                    const s = await this.handleSubmit();
+                    this.form.ssl_certificate = s.data.ssl_certificate
                 }
                 let i = new Blob([this.form.ssl_certificate], {
                         type: "text/plain;charset=utf-8"
                     }),
                     e = this.form.domains[0];
-                x.saveAs(i, `${e}.pem`)
+                D.saveAs(i, `${e}.pem`)
             }
         },
+        mounted() {
+            L.highlightAll()
+        },
         created() {
             this.getData()
         }
     },
     Z = {
         class: "mo-form-detail"
     },
     ee = {
+        style: {
+            padding: "10px 0",
+            "overflow-x": "auto"
+        }
+    },
+    te = ["innerHTML"],
+    se = {
         class: "text-center mt-md"
     };
 
-function te(i, e, t, C, l, o) {
-    const r = a("Download"),
-        u = a("el-icon"),
-        m = a("el-link"),
-        _ = a("el-form-item"),
-        f = a("el-form"),
-        b = a("el-button");
-    return d(), h("div", Z, [s(f, {
+function ie(i, e, s, C, a, o) {
+    const r = l("Download"),
+        _ = l("el-icon"),
+        p = l("el-link"),
+        u = l("el-form-item"),
+        f = l("el-form"),
+        b = l("el-button");
+    return m(), h("div", Z, [t(f, {
         "label-width": "130px"
     }, {
-        default: n(() => [s(_, {
+        default: n(() => [t(u, {
             label: "\u79C1\u94A5",
             prop: "domain"
         }, {
-            default: n(() => [s(m, {
+            default: n(() => [t(p, {
                 underline: !1,
                 type: "primary",
                 class: "mr-sm",
                 onClick: o.downloadSSLKeyFile
             }, {
-                default: n(() => [s(u, null, {
-                    default: n(() => [s(r)]),
+                default: n(() => [t(_, null, {
+                    default: n(() => [t(r)]),
                     _: 1
-                }), y("\u70B9\u51FB\u4E0B\u8F7D")]),
+                }), w("\u70B9\u51FB\u4E0B\u8F7D")]),
                 _: 1
             }, 8, ["onClick"])]),
             _: 1
-        }), s(_, {
+        }), t(u, {
             label: "\u516C\u94A5",
             prop: "domain"
         }, {
-            default: n(() => [s(m, {
+            default: n(() => [t(p, {
                 underline: !1,
                 type: "primary",
                 class: "mr-sm",
                 onClick: o.downloadSSLFile
             }, {
-                default: n(() => [s(u, null, {
-                    default: n(() => [s(r)]),
+                default: n(() => [t(_, null, {
+                    default: n(() => [t(r)]),
                     _: 1
-                }), y("\u70B9\u51FB\u4E0B\u8F7D")]),
+                }), w("\u70B9\u51FB\u4E0B\u8F7D")]),
                 _: 1
             }, 8, ["onClick"])]),
             _: 1
+        }), t(u, {
+            label: "Nginx\u914D\u7F6E",
+            prop: "domain"
+        }, {
+            default: n(() => [d("div", ee, [d("pre", null, [d("code", {
+                innerHTML: o.nginxConfig
+            }, null, 8, te)])])]),
+            _: 1
         })]),
         _: 1
-    }), p("div", ee, [s(b, {
+    }), d("div", se, [t(b, {
         type: "primary",
         onClick: o.handleClose
     }, {
-        default: n(() => [y("\u5173 \u95ED")]),
+        default: n(() => [w("\u5173 \u95ED")]),
         _: 1
     }, 8, ["onClick"])])])
 }
-const se = v(Y, [
-        ["render", te],
-        ["__scopeId", "data-v-bc5bd2e2"]
+const ne = v(Y, [
+        ["render", ie],
+        ["__scopeId", "data-v-047a985f"]
     ]),
-    ie = {
+    le = {
         name: "IssueCertificateStep",
         props: {
             row: {
                 type: Object
             }
         },
         components: {
-            DataForm: F,
+            DataForm: A,
             VerifyStep: X,
-            RenewStep: se
+            RenewStep: ne
         },
         data() {
             return {
                 activeStep: 0,
                 issue_certificate_id: null,
                 form: {
                     id: null,
@@ -431,85 +527,85 @@
             async getData() {
                 if (!this.issue_certificate_id) return;
                 let i = {
                     issue_certificate_id: this.issue_certificate_id
                 };
                 const e = await this.$http.getIssueCertificateById(i);
                 if (!!e.ok) {
-                    for (let t in this.form) this.form[t] = e.data[t];
+                    for (let s in this.form) this.form[s] = e.data[s];
                     e.data.ssl_certificate ? this.activeStep = 3 : e.data.status == "valid" ? this.activeStep = 2 : e.data.status == "pending" ? this.activeStep = 1 : this.activeStep = 0
                 }
             },
             handleIssueSuccess(i) {
                 this.issue_certificate_id = i.id, this.getData()
             },
             handleVerifySuccess() {
                 this.getData()
             }
         },
         created() {
             this.row && (this.issue_certificate_id = this.row.id), this.getData()
         }
     },
-    ne = {
+    ae = {
         class: ""
     },
-    ae = {
+    oe = {
         class: "mt-md"
     };
 
-function le(i, e, t, C, l, o) {
-    const r = a("el-step"),
-        u = a("el-steps"),
-        m = a("el-divider"),
-        _ = a("DataForm"),
-        f = a("VerifyStep"),
-        b = a("RenewStep");
-    return d(), h("div", ne, [s(u, {
-        active: l.activeStep,
+function re(i, e, s, C, a, o) {
+    const r = l("el-step"),
+        _ = l("el-steps"),
+        p = l("el-divider"),
+        u = l("DataForm"),
+        f = l("VerifyStep"),
+        b = l("RenewStep");
+    return m(), h("div", ae, [t(_, {
+        active: a.activeStep,
         "align-center": "",
         "finish-status": "success"
     }, {
-        default: n(() => [(d(!0), h($, null, V(l.setpList, S => (d(), k(r, {
-            title: S.title
+        default: n(() => [(m(!0), h($, null, V(a.setpList, g => (m(), k(r, {
+            title: g.title
         }, null, 8, ["title"]))), 256))]),
         _: 1
-    }, 8, ["active"]), s(m), p("div", ae, [l.activeStep == 0 ? (d(), k(_, {
+    }, 8, ["active"]), t(p), d("div", oe, [a.activeStep == 0 ? (m(), k(u, {
         key: 0,
         onOnSuccess: o.handleIssueSuccess,
-        onOnCancel: e[0] || (e[0] = S => i.$emit("on-cancel"))
-    }, null, 8, ["onOnSuccess"])) : l.activeStep == 1 ? (d(), k(f, {
+        onOnCancel: e[0] || (e[0] = g => i.$emit("on-cancel"))
+    }, null, 8, ["onOnSuccess"])) : a.activeStep == 1 ? (m(), k(f, {
         key: 1,
-        form: l.form,
+        form: a.form,
         onOnSuccess: o.handleVerifySuccess
-    }, null, 8, ["form", "onOnSuccess"])) : l.activeStep == 2 || l.activeStep == 3 ? (d(), k(b, {
+    }, null, 8, ["form", "onOnSuccess"])) : a.activeStep == 2 || a.activeStep == 3 ? (m(), k(b, {
         key: 2,
-        form: l.form,
-        onOnClose: e[1] || (e[1] = S => i.$emit("on-cancel"))
+        form: a.form,
+        onOnClose: e[1] || (e[1] = g => i.$emit("on-cancel"))
     }, null, 8, ["form"])) : O("", !0)])])
 }
-const oe = v(ie, [
-        ["render", le]
+const ce = v(le, [
+        ["render", re]
     ]),
-    re = {
+    de = {
         name: "",
         props: {
             row: {
                 type: Object,
                 default: null
             },
             visible: {
                 type: Boolean,
                 default: !1
             }
         },
         emits: ["update:visible"],
         components: {
-            DataForm: F,
-            IssueCertificateStep: oe
+            DataForm: A,
+            IssueCertificateStep: ce
         },
         data() {
             return {}
         },
         computed: {
             dialogTitle() {
                 return this.row ? "\u7F16\u8F91" : "\u7533\u8BF7SSL\u8BC1\u4E66"
@@ -533,42 +629,42 @@
             handleSuccess() {
                 this.handleClose(), this.$emit("on-success")
             }
         },
         created() {}
     };
 
-function ce(i, e, t, C, l, o) {
-    const r = a("IssueCertificateStep"),
-        u = a("el-dialog");
-    return d(), k(u, {
+function ue(i, e, s, C, a, o) {
+    const r = l("IssueCertificateStep"),
+        _ = l("el-dialog");
+    return m(), k(_, {
         title: "\u7533\u8BF7SSL\u8BC1\u4E66",
         modelValue: o.dialogVisible,
-        "onUpdate:modelValue": e[0] || (e[0] = m => o.dialogVisible = m),
+        "onUpdate:modelValue": e[0] || (e[0] = p => o.dialogVisible = p),
         width: "900px",
         center: "",
         "append-to-body": ""
     }, {
-        default: n(() => [o.dialogVisible ? (d(), k(r, {
+        default: n(() => [o.dialogVisible ? (m(), k(r, {
             key: 0,
-            row: t.row,
+            row: s.row,
             onOnCancel: o.handleClose,
             onOnSuccess: o.handleSuccess
         }, null, 8, ["row", "onOnCancel", "onOnSuccess"])) : O("", !0)]),
         _: 1
     }, 8, ["modelValue"])
 }
-const I = v(re, [
-        ["render", ce]
+const T = v(de, [
+        ["render", ue]
     ]),
-    de = {
+    me = {
         name: "",
         components: {
-            DataFormDialog: I,
-            ConnectStatus: A
+            DataFormDialog: T,
+            ConnectStatus: I
         },
         props: {
             list: {
                 type: Array
             }
         },
         computed: {},
@@ -582,139 +678,139 @@
             handleEditRow(i) {
                 this.currentRow = i, this.dialogVisible = !0
             },
             async handleDeleteClick(i) {
                 let e = {
                     id: i.id
                 };
-                const t = await this.$http.function(e);
-                t.code == 0 ? (this.$msg.success("\u64CD\u4F5C\u6210\u529F"), this.$emit("on-success")) : this.$msg.error(t.msg)
+                const s = await this.$http.function(e);
+                s.code == 0 ? (this.$msg.success("\u64CD\u4F5C\u6210\u529F"), this.$emit("on-success")) : this.$msg.error(s.msg)
             },
             async handleStatusChange(i) {
                 let e = {
                     id: i.id
                 };
-                const t = await this.$http.function(e);
-                t.code == 0 ? (this.$msg.success("\u64CD\u4F5C\u6210\u529F"), this.$emit("on-success")) : this.$msg.error(t.msg)
+                const s = await this.$http.function(e);
+                s.code == 0 ? (this.$msg.success("\u64CD\u4F5C\u6210\u529F"), this.$emit("on-success")) : this.$msg.error(s.msg)
             },
             handleUpdateSuccess() {
                 this.$emit("on-success")
             }
         },
         created() {}
     },
-    ue = {
+    _e = {
         style: {
             "margin-left": "4px"
         }
     };
 
-function me(i, e, t, C, l, o) {
-    const r = a("el-table-column"),
-        u = a("ConnectStatus"),
-        m = a("Tickets"),
-        _ = a("el-icon"),
-        f = a("el-link"),
-        b = a("el-table"),
-        S = a("DataFormDialog");
-    return d(), h("div", null, [s(b, {
-        data: t.list,
+function pe(i, e, s, C, a, o) {
+    const r = l("el-table-column"),
+        _ = l("ConnectStatus"),
+        p = l("Tickets"),
+        u = l("el-icon"),
+        f = l("el-link"),
+        b = l("el-table"),
+        g = l("DataFormDialog");
+    return m(), h("div", null, [t(b, {
+        data: s.list,
         stripe: "",
         border: ""
     }, {
-        default: n(() => [s(r, {
+        default: n(() => [t(r, {
             label: "ID",
             align: "center",
             prop: "id",
             width: "60"
         }, {
-            default: n(c => [p("span", null, g(c.row.id || "-"), 1)]),
+            default: n(c => [d("span", null, S(c.row.id || "-"), 1)]),
             _: 1
-        }), s(r, {
+        }), t(r, {
             label: "\u57DF\u540D",
             "header-align": "center",
             align: "center",
             prop: "domains"
         }, {
-            default: n(c => [(d(!0), h($, null, V(c.row.domains, D => (d(), h("div", null, g(D), 1))), 256))]),
+            default: n(c => [(m(!0), h($, null, V(c.row.domains, x => (m(), h("div", null, S(x), 1))), 256))]),
             _: 1
-        }), s(r, {
+        }), t(r, {
             label: "\u9A8C\u8BC1\u72B6\u6001",
             "header-align": "center",
             align: "center",
             prop: "status",
             width: "80"
         }, {
-            default: n(c => [s(u, {
+            default: n(c => [t(_, {
                 value: c.row.show_status,
-                onOnClick: D => i.handleShowAddressListgDialog(c.row)
-            }, null, 8, ["value", "onOnClick"]), p("span", ue, g(c.row.status_label || "-"), 1)]),
+                onOnClick: x => i.handleShowAddressListgDialog(c.row)
+            }, null, 8, ["value", "onOnClick"]), d("span", _e, S(c.row.status_label || "-"), 1)]),
             _: 1
-        }), s(r, {
+        }), t(r, {
             label: "SSL\u7B7E\u53D1\u65F6\u95F4",
             "header-align": "center",
             align: "center",
             prop: "start_time",
             width: "160"
         }, {
-            default: n(c => [p("span", null, g(c.row.start_time || "-"), 1)]),
+            default: n(c => [d("span", null, S(c.row.start_time || "-"), 1)]),
             _: 1
-        }), s(r, {
+        }), t(r, {
             label: "SSL\u8FC7\u671F\u65F6\u95F4",
             "header-align": "center",
             align: "center",
             prop: "expire_time",
             width: "160"
         }, {
-            default: n(c => [p("span", null, g(c.row.expire_time || "-"), 1)]),
+            default: n(c => [d("span", null, S(c.row.expire_time || "-"), 1)]),
             _: 1
-        }), s(r, {
+        }), t(r, {
             label: "\u521B\u5EFA\u65F6\u95F4",
             "header-align": "center",
             align: "center",
             prop: "create_time_label"
         }, {
-            default: n(c => [p("span", null, g(c.row.create_time_label || "-"), 1)]),
+            default: n(c => [d("span", null, S(c.row.create_time_label || "-"), 1)]),
             _: 1
-        }), s(r, {
+        }), t(r, {
             label: "\u67E5\u770B",
             width: "60",
             "header-align": "center",
             align: "center"
         }, {
-            default: n(c => [s(f, {
+            default: n(c => [t(f, {
                 underline: !1,
                 type: "primary",
-                onClick: D => o.handleEditRow(c.row)
+                onClick: x => o.handleEditRow(c.row)
             }, {
-                default: n(() => [s(_, null, {
-                    default: n(() => [s(m)]),
+                default: n(() => [t(u, null, {
+                    default: n(() => [t(p)]),
                     _: 1
                 })]),
                 _: 2
             }, 1032, ["onClick"])]),
             _: 1
         })]),
         _: 1
-    }, 8, ["data"]), s(S, {
-        visible: l.dialogVisible,
-        "onUpdate:visible": e[0] || (e[0] = c => l.dialogVisible = c),
-        row: l.currentRow,
+    }, 8, ["data"]), t(g, {
+        visible: a.dialogVisible,
+        "onUpdate:visible": e[0] || (e[0] = c => a.dialogVisible = c),
+        row: a.currentRow,
         onOnSuccess: o.handleUpdateSuccess
     }, null, 8, ["visible", "row", "onOnSuccess"])])
 }
-const _e = v(de, [
-        ["render", me]
+const fe = v(me, [
+        ["render", pe]
     ]),
-    pe = {
+    he = {
         name: "issue-certificate-list",
         props: {},
         components: {
-            DataFormDialog: I,
-            DataTable: _e
+            DataFormDialog: T,
+            DataTable: fe
         },
         data() {
             return {
                 list: [],
                 total: 0,
                 page: 1,
                 size: 20,
@@ -733,15 +829,15 @@
                 let i = {
                     page: this.page,
                     size: this.size,
                     keyword: this.keyword
                 };
                 try {
                     const e = await this.$http.getCertificateList(i);
-                    e.code == 0 && (this.list = e.data.list.map(t => (t.show_status = null, t.status_label = "\u672A\u77E5", t.status == "pending" ? (t.show_status = !1, t.status_label = "\u672A\u9A8C\u8BC1") : t.status == "valid" && (t.show_status = !0, t.status_label = "\u5DF2\u9A8C\u8BC1"), t)), this.total = e.data.total)
+                    e.code == 0 && (this.list = e.data.list.map(s => (s.show_status = null, s.status_label = "\u672A\u77E5", s.status == "pending" ? (s.show_status = !1, s.status_label = "\u672A\u9A8C\u8BC1") : s.status == "valid" && (s.show_status = !0, s.status_label = "\u5DF2\u9A8C\u8BC1"), s)), this.total = e.data.total)
                 } catch (e) {
                     console.log(e)
                 } finally {
                     this.loading = !1
                 }
             },
             handleAddRow() {
@@ -754,85 +850,85 @@
                 this.resetData()
             }
         },
         created() {
             this.getData()
         }
     },
-    fe = {
+    ge = {
         class: "app-container"
     },
-    he = {
+    be = {
         class: "margin-bottom--20"
     };
 
-function ge(i, e, t, C, l, o) {
-    const r = a("Plus"),
-        u = a("el-icon"),
-        m = a("el-button"),
-        _ = a("Search"),
-        f = a("el-input"),
-        b = a("DataTable"),
-        S = a("el-pagination"),
-        c = a("DataFormDialog"),
-        D = T("loading");
-    return d(), h("div", fe, [p("div", he, [s(m, {
+function Se(i, e, s, C, a, o) {
+    const r = l("Plus"),
+        _ = l("el-icon"),
+        p = l("el-button"),
+        u = l("Search"),
+        f = l("el-input"),
+        b = l("DataTable"),
+        g = l("el-pagination"),
+        c = l("DataFormDialog"),
+        x = R("loading");
+    return m(), h("div", ge, [d("div", be, [t(p, {
         type: "primary",
         onClick: o.handleAddRow
     }, {
-        default: n(() => [s(u, null, {
-            default: n(() => [s(r)]),
+        default: n(() => [t(_, null, {
+            default: n(() => [t(r)]),
             _: 1
-        }), y("\u7533\u8BF7")]),
+        }), w("\u7533\u8BF7")]),
         _: 1
-    }, 8, ["onClick"]), s(f, {
+    }, 8, ["onClick"]), t(f, {
         class: "ml-sm",
         style: {
             width: "260px"
         },
-        modelValue: l.keyword,
-        "onUpdate:modelValue": e[0] || (e[0] = w => l.keyword = w),
+        modelValue: a.keyword,
+        "onUpdate:modelValue": e[0] || (e[0] = y => a.keyword = y),
         placeholder: "\u8F93\u5165\u57DF\u540D",
         clearable: "",
-        onKeypress: U(o.handleSearch, ["enter"]),
+        onKeypress: F(o.handleSearch, ["enter"]),
         onClear: o.handleSearch
     }, {
-        append: n(() => [s(m, {
+        append: n(() => [t(p, {
             onClick: o.handleSearch
         }, {
-            default: n(() => [s(u, null, {
-                default: n(() => [s(_)]),
+            default: n(() => [t(_, null, {
+                default: n(() => [t(u)]),
                 _: 1
             })]),
             _: 1
         }, 8, ["onClick"])]),
         _: 1
-    }, 8, ["modelValue", "onKeypress", "onClear"])]), z(s(b, {
+    }, 8, ["modelValue", "onKeypress", "onClear"])]), E(t(b, {
         class: "mt-md",
-        list: l.list,
+        list: a.list,
         onOnSuccess: o.resetData,
         onOnEditRow: i.handleEditRow
     }, null, 8, ["list", "onOnSuccess", "onOnEditRow"]), [
-        [D, l.loading]
-    ]), s(S, {
+        [x, a.loading]
+    ]), t(g, {
         class: "mt-md justify-center",
         background: "",
         layout: "total, prev, pager, next",
-        total: l.total,
-        "page-size": l.size,
-        "onUpdate:pageSize": e[1] || (e[1] = w => l.size = w),
-        "current-page": l.page,
-        "onUpdate:currentPage": e[2] || (e[2] = w => l.page = w),
+        total: a.total,
+        "page-size": a.size,
+        "onUpdate:pageSize": e[1] || (e[1] = y => a.size = y),
+        "current-page": a.page,
+        "onUpdate:currentPage": e[2] || (e[2] = y => a.page = y),
         onCurrentChange: o.getData
-    }, null, 8, ["total", "page-size", "current-page", "onCurrentChange"]), s(c, {
-        visible: l.dialogVisible,
-        "onUpdate:visible": e[3] || (e[3] = w => l.dialogVisible = w),
+    }, null, 8, ["total", "page-size", "current-page", "onCurrentChange"]), t(c, {
+        visible: a.dialogVisible,
+        "onUpdate:visible": e[3] || (e[3] = y => a.dialogVisible = y),
         onOnSuccess: o.handleAddSuccess
     }, null, 8, ["visible", "onOnSuccess"])])
 }
-const ke = v(pe, [
-    ["render", ge]
+const Ve = v(he, [
+    ["render", Se]
 ]);
 export {
-    ke as
+    Ve as
     default
 };
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.ab38e8b8.js` & `domain-admin-1.5.8/domain_admin/public/js/index.0963ab53.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     C as S
-} from "./ConnectStatus.89654d5c.js";
+} from "./ConnectStatus.a429b01b.js";
 import {
     _ as m
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ah as o,
     o as _,
     c as f,
     V as s,
     P as n,
     a as i,
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.b84878f9.js` & `domain-admin-1.5.8/domain_admin/public/js/index.5f8ece3f.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     C as w
-} from "./ConnectStatus.89654d5c.js";
+} from "./ConnectStatus.a429b01b.js";
 import {
     _ as m
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ah as l,
     o as _,
     c as f,
     V as a,
     P as n,
     a as c,
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.c05aa8e8.js` & `domain-admin-1.5.8/domain_admin/public/js/index.2ab02c40.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
     T as f,
     U as u,
     az as I,
     aA as k
 } from "./vendor-vue.9e61e0af.js";
 import {
     _ as C
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.76301fc3.js";
 import "./element-plus.30eb1cab.js";
 const V = {
         name: "index",
         props: {},
         components: {},
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/index.c512b8f1.js` & `domain-admin-1.5.8/domain_admin/public/js/index.af06b2dc.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 import {
     i as Y,
     E as M
 } from "./event-enums.6c6f25e7.js";
 import {
     S as N,
     u as z
-} from "./SelectGroup.d7e6e540.js";
+} from "./SelectGroup.53d83114.js";
 import {
     _ as v,
     R as $,
     d as L,
     r as W
-} from "./index.12198a8e.js";
+} from "./index.165f9ce1.js";
 import {
     ah as s,
     ar as P,
     Q as G,
     o as u,
     c as g,
     V as o,
@@ -33,18 +33,18 @@
 } from "./vendor-vue.9e61e0af.js";
 import {
     E as q,
     A as J,
     a as Z,
     b as ee,
     C as te
-} from "./ConditionFilterGroup.340936f7.js";
+} from "./ConditionFilterGroup.3c6ac067.js";
 import {
     C as oe
-} from "./ConnectStatus.89654d5c.js";
+} from "./ConnectStatus.a429b01b.js";
 import {
     F as le
 } from "./vendor-lib.76301fc3.js";
 import {
     b as ie
 } from "./element-plus.30eb1cab.js";
 import "./element-icon.1ce1c350.js";
```

### Comparing `domain-admin-1.5.7/domain_admin/public/js/vendor-lib.76301fc3.js` & `domain-admin-1.5.8/domain_admin/public/js/vendor-lib.76301fc3.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/js/vendor-vue.9e61e0af.js` & `domain-admin-1.5.8/domain_admin/public/js/vendor-vue.9e61e0af.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/commit-msg.sample` & `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-commit.sample` & `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-push.sample` & `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-rebase.sample` & `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-receive.sample` & `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/push-to-checkout.sample` & `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/sendemail-validate.sample` & `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/update.sample` & `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3` & `domain-admin-1.5.8/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/common-c7dd5d89.css` & `domain-admin-1.5.8/domain_admin/public/m/assets/common-c7dd5d89.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/common.6194c42f.js` & `domain-admin-1.5.8/domain_admin/public/m/assets/common.6194c42f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/index-5eda257b.css` & `domain-admin-1.5.8/domain_admin/public/m/assets/index-5eda257b.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/index-958ae3a0.css` & `domain-admin-1.5.8/domain_admin/public/m/assets/index-958ae3a0.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/index-9c365a03.js` & `domain-admin-1.5.8/domain_admin/public/m/assets/index-9c365a03.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/index-ad047368.css` & `domain-admin-1.5.8/domain_admin/public/m/assets/index-ad047368.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/index-e8224928.css` & `domain-admin-1.5.8/domain_admin/public/m/assets/index-e8224928.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/index-f79acb3d.css` & `domain-admin-1.5.8/domain_admin/public/m/assets/index-f79acb3d.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/index.1a0d1182.js` & `domain-admin-1.5.8/domain_admin/public/m/assets/index.1a0d1182.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/index.1d067866.js` & `domain-admin-1.5.8/domain_admin/public/m/assets/index.1d067866.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/index.daaf9893.js` & `domain-admin-1.5.8/domain_admin/public/m/assets/index.daaf9893.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/index.feef7c0f.js` & `domain-admin-1.5.8/domain_admin/public/m/assets/index.feef7c0f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/login-cb9f43ad.css` & `domain-admin-1.5.8/domain_admin/public/m/assets/login-cb9f43ad.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js` & `domain-admin-1.5.8/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js` & `domain-admin-1.5.8/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/pages-login-login.09426b90.js` & `domain-admin-1.5.8/domain_admin/public/m/assets/pages-login-login.09426b90.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js` & `domain-admin-1.5.8/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/uni.06dd3c8e.css` & `domain-admin-1.5.8/domain_admin/public/m/assets/uni.06dd3c8e.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/assets/user-index-be7005ab.css` & `domain-admin-1.5.8/domain_admin/public/m/assets/user-index-be7005ab.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/index.html` & `domain-admin-1.5.8/domain_admin/public/m/index.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/m/static/user-avatar.gif` & `domain-admin-1.5.8/domain_admin/public/m/static/user-avatar.gif`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/public/svg/logo.184a2d7d.svg` & `domain-admin-1.5.8/domain_admin/public/svg/logo.184a2d7d.svg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/router/api_map.py` & `domain-admin-1.5.8/domain_admin/router/api_map.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/router/permission.py` & `domain-admin-1.5.8/domain_admin/router/permission.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/async_task_service.py` & `domain-admin-1.5.8/domain_admin/service/async_task_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/auth_service.py` & `domain-admin-1.5.8/domain_admin/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/common_service.py` & `domain-admin-1.5.8/domain_admin/service/common_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/domain_info_service.py` & `domain-admin-1.5.8/domain_admin/service/domain_info_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/domain_service.py` & `domain-admin-1.5.8/domain_admin/service/domain_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/file_service.py` & `domain-admin-1.5.8/domain_admin/service/file_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/group_service.py` & `domain-admin-1.5.8/domain_admin/service/group_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/group_user_service.py` & `domain-admin-1.5.8/domain_admin/service/group_user_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/issue_certificate_service.py` & `domain-admin-1.5.8/domain_admin/service/issue_certificate_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/notify_service.py` & `domain-admin-1.5.8/domain_admin/service/notify_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/operation_service.py` & `domain-admin-1.5.8/domain_admin/service/operation_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/scheduler_service.py` & `domain-admin-1.5.8/domain_admin/service/scheduler_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
     scheduler.start()
 
 
 def update_job(cron_exp):
     scheduler.remove_all_jobs()
 
     # cron 定时任务
-    minute, hour, day, month, day_of_week = cron_exp.split(' ')
+    # Bugfix: 用户输入的cron表达式有多余的空格
+    minute, hour, day, month, day_of_week = cron_exp.split()
 
     scheduler.add_job(
         func=task,
         trigger='cron',
         minute=minute,
         hour=hour,
         day=day,
```

### Comparing `domain-admin-1.5.7/domain_admin/service/system_service.py` & `domain-admin-1.5.8/domain_admin/service/system_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/token_service.py` & `domain-admin-1.5.8/domain_admin/service/token_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/service/version_service.py` & `domain-admin-1.5.8/domain_admin/service/version_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/templates/cert-email.html` & `domain-admin-1.5.8/domain_admin/templates/cert-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/templates/domain-email.html` & `domain-admin-1.5.8/domain_admin/templates/domain-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/acme_util/acme_v2_api.py` & `domain-admin-1.5.8/domain_admin/utils/acme_util/acme_v2_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/bcrypt_util.py` & `domain-admin-1.5.8/domain_admin/utils/bcrypt_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/cert_util/cert_common.py` & `domain-admin-1.5.8/domain_admin/utils/cert_util/cert_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/cert_util/cert_openssl_v2.py` & `domain-admin-1.5.8/domain_admin/utils/cert_util/cert_openssl_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/cert_util/cert_socket.py` & `domain-admin-1.5.8/domain_admin/utils/cert_util/cert_socket.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/cert_util/cert_socket_v2.py` & `domain-admin-1.5.8/domain_admin/utils/cert_util/cert_socket_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/datetime_util.py` & `domain-admin-1.5.8/domain_admin/utils/datetime_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/domain_util.py` & `domain-admin-1.5.8/domain_admin/utils/domain_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/email_util.py` & `domain-admin-1.5.8/domain_admin/utils/email_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/flask_ext/api_result.py` & `domain-admin-1.5.8/domain_admin/utils/flask_ext/api_result.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/flask_ext/app_exception.py` & `domain-admin-1.5.8/domain_admin/utils/flask_ext/app_exception.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/flask_ext/flask_app.py` & `domain-admin-1.5.8/domain_admin/utils/flask_ext/flask_app.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/flask_ext/handler.py` & `domain-admin-1.5.8/domain_admin/utils/flask_ext/handler.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/flask_ext/json/default.py` & `domain-admin-1.5.8/domain_admin/utils/flask_ext/json/default.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/flask_ext/json/json_encoder.py` & `domain-admin-1.5.8/domain_admin/utils/flask_ext/json/json_encoder.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/flask_ext/json/json_provider.py` & `domain-admin-1.5.8/domain_admin/utils/flask_ext/json/json_provider.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/icp_util.py` & `domain-admin-1.5.8/domain_admin/utils/icp_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/ip_util.py` & `domain-admin-1.5.8/domain_admin/utils/ip_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/json_util.py` & `domain-admin-1.5.8/domain_admin/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/open_api/crtsh_api.py` & `domain-admin-1.5.8/domain_admin/utils/open_api/crtsh_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/open_api/ding_talk_api.py` & `domain-admin-1.5.8/domain_admin/utils/open_api/ding_talk_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/open_api/feishu_api.py` & `domain-admin-1.5.8/domain_admin/utils/open_api/feishu_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/open_api/work_weixin_api.py` & `domain-admin-1.5.8/domain_admin/utils/open_api/work_weixin_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/peewee_ext/model_util.py` & `domain-admin-1.5.8/domain_admin/utils/peewee_ext/model_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/secret_util.py` & `domain-admin-1.5.8/domain_admin/utils/secret_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/text_util.py` & `domain-admin-1.5.8/domain_admin/utils/text_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/time_util.py` & `domain-admin-1.5.8/domain_admin/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/whois_util/config.py` & `domain-admin-1.5.8/domain_admin/utils/whois_util/config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/whois_util/util.py` & `domain-admin-1.5.8/domain_admin/utils/whois_util/util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/whois_util/whois-servers.txt` & `domain-admin-1.5.8/domain_admin/utils/whois_util/whois-servers.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin/utils/whois_util/whois_util.py` & `domain-admin-1.5.8/domain_admin/utils/whois_util/whois_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.7/domain_admin.egg-info/PKG-INFO` & `domain-admin-1.5.8/domain_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.5.7
+Version: 1.5.8
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain,ssl,cert,web,monitor
 Platform: any
```

### Comparing `domain-admin-1.5.7/domain_admin.egg-info/SOURCES.txt` & `domain-admin-1.5.8/domain_admin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -96,98 +96,100 @@
 domain_admin/public/.git/hooks/push-to-checkout.sample
 domain_admin/public/.git/hooks/sendemail-validate.sample
 domain_admin/public/.git/hooks/update.sample
 domain_admin/public/.git/info/exclude
 domain_admin/public/.git/logs/HEAD
 domain_admin/public/.git/logs/refs/heads/dist
 domain_admin/public/.git/logs/refs/remotes/origin/dist
-domain_admin/public/.git/objects/01/9bb44cfca57b7aa35ea7f5b6f99c3ef48e8d8f
 domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
-domain_admin/public/.git/objects/1e/270d8f3cc5167242582434675642b5858ba482
 domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
-domain_admin/public/.git/objects/30/0478ea1f19f5a14d6a7167e9f71f5848707d76
+domain_admin/public/.git/objects/2b/3195083ee5802a2c60fdb9919fbf35e18e6478
+domain_admin/public/.git/objects/32/dd3b54be707f423bd7375381bbc2baede37f8c
+domain_admin/public/.git/objects/37/11576f2b615224b9477da0a0a9a43c17539d12
 domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
 domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1
-domain_admin/public/.git/objects/40/03c2e07280d146ee3443587c38ea2d264c07ca
-domain_admin/public/.git/objects/50/c771a9bca6f87a2fb3381719fe0622eeae23bf
+domain_admin/public/.git/objects/3e/24054f5e3a680f56b9276efe009e73b7133a99
+domain_admin/public/.git/objects/4b/f6af202944cd3e22f8a375977737ce52b17763
 domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
-domain_admin/public/.git/objects/53/0864cbe282ec11e8564a8a3ce33756977d59ee
 domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
-domain_admin/public/.git/objects/58/1d5e80145e76e2ba0d08b038e1a2fefebef3bb
+domain_admin/public/.git/objects/57/bd1a9bfce972b50e5efecf11f71a3f5b2ec3d3
 domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
+domain_admin/public/.git/objects/60/727d43f26f701780e7c55e90cb084973a1be9e
 domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a
 domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
+domain_admin/public/.git/objects/6c/f21ee6e3a69b2e234f6012f1636e3621d25db8
 domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
-domain_admin/public/.git/objects/77/bb86f804268cc8045d2cd2547ec17c22a0d166
+domain_admin/public/.git/objects/71/6b5718c659ed5a85d4f93a2cf25fc5ff5031cb
 domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b
+domain_admin/public/.git/objects/7c/7a565bed760068496030f030f2b05ede1bec4b
 domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
+domain_admin/public/.git/objects/88/eed16a647060a310c6f8fd8cbf109ad11d1211
 domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
 domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
-domain_admin/public/.git/objects/90/4a4570929957b2678d3c499a9cd83658a6675e
-domain_admin/public/.git/objects/91/dcfad5270425be228e01a34e9c9b11ef3a0c4e
+domain_admin/public/.git/objects/8f/3fc862ebdfdd80953e51ae5e44e7862b79ad63
 domain_admin/public/.git/objects/92/cfface0a460c51331fb8f25083a09948e00cbf
-domain_admin/public/.git/objects/93/522d98a7fe61eb676e55f33d92d8d090b967e4
 domain_admin/public/.git/objects/95/f07af46d709638b20c0b2c66cdf6de8e89a7e4
-domain_admin/public/.git/objects/a0/e9b4ee6e91d304066df26b1bc6218de181c2c2
-domain_admin/public/.git/objects/a2/86b0b36b3538d177580f0c25e8e3a3a9f007b7
-domain_admin/public/.git/objects/ab/2ba13bd2bd0cbf3e5b764ff0a29fd5872380c5
-domain_admin/public/.git/objects/b1/115cb42fa8938fe1dbebccc9584aa03a895df0
+domain_admin/public/.git/objects/9a/44f010e55bd5cd3a7d60bcd86ee9b8e7ef2cef
+domain_admin/public/.git/objects/9a/4e8fcc1912f0c1af9a1836ebd9847d8b0e3118
+domain_admin/public/.git/objects/a5/6b22c2eacca280122dde700a98068ebdd8c5af
+domain_admin/public/.git/objects/a7/49320e6e50d7593d7d1d30ee0159023cd4e422
+domain_admin/public/.git/objects/ae/1c9a7def175d7a6389679bf822a6a9219c3ca3
+domain_admin/public/.git/objects/b2/9b2820070fd0808f478afc2a5995aaee9cd79f
 domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
-domain_admin/public/.git/objects/bb/ecd10fc84228b6f4a1c2e0c90e2b68d4aa6bf2
-domain_admin/public/.git/objects/c0/76a86e24db79ccf75f79903b19cf145419d4bf
-domain_admin/public/.git/objects/c1/ff198374b288725eab95bc1294e1f04fe5c561
 domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
+domain_admin/public/.git/objects/c9/3d3f53fd06fdbc8587e3a8f37876356c5cdb56
 domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9
-domain_admin/public/.git/objects/ce/dcd8ba4511fabecdc11df81e55d82ca8b96ca3
-domain_admin/public/.git/objects/cf/1eea719ca3a291ef7edaa6c60eaa808ca6e4ae
-domain_admin/public/.git/objects/d4/9eb5d776f5b92a02189cebbe590f76db9575bd
-domain_admin/public/.git/objects/d8/1e4838c9ac36863e037e68a2f3552f736c5c8f
+domain_admin/public/.git/objects/d2/5bbe60e329a2e662af042df10825c9dcdc3887
+domain_admin/public/.git/objects/e0/6f4cc670d4bb8f606c4edfb9d7aa51becaaf2a
 domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
-domain_admin/public/.git/objects/e4/c5465d396f947d57739ed8266597d6a47ef51b
-domain_admin/public/.git/objects/e6/72b6afc2744b043e6fbdf3031eb086a109ec3c
-domain_admin/public/.git/objects/e6/e5ddee110d6ed47cbb0a4f30db3d055efd21da
+domain_admin/public/.git/objects/e6/8884f9d8cc37153041b8b82943d995c95ba1aa
+domain_admin/public/.git/objects/e6/e9c9b85a9477efa2c8f05874bd09fa93a6b34c
+domain_admin/public/.git/objects/e9/8d4dd298d6c05d0bfa2fbe9182ec7cddde7926
+domain_admin/public/.git/objects/f9/78f4b33c1fdc0cb74f1df45d0fc049f5da1c89
+domain_admin/public/.git/objects/fb/ac0b57e4138b4fca9c9f5babf558611a38e6d0
 domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
 domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
 domain_admin/public/.git/refs/heads/dist
 domain_admin/public/.git/refs/remotes/origin/dist
 domain_admin/public/css/ConditionFilterGroup.a91875e6.css
 domain_admin/public/css/index.302e10d7.css
 domain_admin/public/css/index.69a97337.css
-domain_admin/public/css/index.75ef7015.css
+domain_admin/public/css/index.93c714bb.css
 domain_admin/public/css/index.a676cc2e.css
 domain_admin/public/css/index.b285e10a.css
 domain_admin/public/css/index.cf805e1c.css
 domain_admin/public/css/index.d028ae37.css
 domain_admin/public/gif/user-avatar.ea67286d.gif
 domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
 domain_admin/public/jpg/chatpet.fce5580e.jpg
-domain_admin/public/js/ConditionFilterGroup.340936f7.js
-domain_admin/public/js/ConnectStatus.89654d5c.js
-domain_admin/public/js/SearchUser.983b7494.js
-domain_admin/public/js/SelectGroup.d7e6e540.js
+domain_admin/public/js/ConditionFilterGroup.3c6ac067.js
+domain_admin/public/js/ConnectStatus.a429b01b.js
+domain_admin/public/js/SearchUser.f8e52158.js
+domain_admin/public/js/SelectGroup.53d83114.js
 domain_admin/public/js/codemirror-lib.a3a39aa0.js
 domain_admin/public/js/element-icon.1ce1c350.js
 domain_admin/public/js/element-plus.30eb1cab.js
 domain_admin/public/js/event-enums.6c6f25e7.js
 domain_admin/public/js/highlight-lib.3654f6d3.js
-domain_admin/public/js/index.075c6a16.js
-domain_admin/public/js/index.12198a8e.js
-domain_admin/public/js/index.127485d4.js
-domain_admin/public/js/index.16184f42.js
-domain_admin/public/js/index.2e3ad8c8.js
-domain_admin/public/js/index.34096d0f.js
-domain_admin/public/js/index.4704b0d3.js
-domain_admin/public/js/index.51aeadc3.js
-domain_admin/public/js/index.58059e0f.js
-domain_admin/public/js/index.86cef4dd.js
-domain_admin/public/js/index.a3947126.js
-domain_admin/public/js/index.ab38e8b8.js
-domain_admin/public/js/index.b84878f9.js
-domain_admin/public/js/index.c05aa8e8.js
-domain_admin/public/js/index.c512b8f1.js
+domain_admin/public/js/highlight-util.a4f1867f.js
+domain_admin/public/js/index.0963ab53.js
+domain_admin/public/js/index.0d4c27ce.js
+domain_admin/public/js/index.165f9ce1.js
+domain_admin/public/js/index.24e255af.js
+domain_admin/public/js/index.2ab02c40.js
+domain_admin/public/js/index.3b5a616c.js
+domain_admin/public/js/index.5b4cd516.js
+domain_admin/public/js/index.5f8ece3f.js
+domain_admin/public/js/index.654f7830.js
+domain_admin/public/js/index.8c31b31b.js
+domain_admin/public/js/index.a8bb8abf.js
+domain_admin/public/js/index.af06b2dc.js
+domain_admin/public/js/index.c22f6489.js
+domain_admin/public/js/index.deff2c63.js
+domain_admin/public/js/index.ef82c865.js
 domain_admin/public/js/vendor-lib.76301fc3.js
 domain_admin/public/js/vendor-vue.9e61e0af.js
 domain_admin/public/m/index.html
 domain_admin/public/m/.git/FETCH_HEAD
 domain_admin/public/m/.git/HEAD
 domain_admin/public/m/.git/config
 domain_admin/public/m/.git/description
```

### Comparing `domain-admin-1.5.7/setup.py` & `domain-admin-1.5.8/setup.py`

 * *Files identical despite different names*

