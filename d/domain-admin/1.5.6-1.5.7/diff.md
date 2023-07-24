# Comparing `tmp/domain-admin-1.5.6.tar.gz` & `tmp/domain-admin-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domain-admin-1.5.6.tar", last modified: Sun Jul 23 14:37:36 2023, max compression
+gzip compressed data, was "domain-admin-1.5.7.tar", last modified: Mon Jul 24 05:27:45 2023, max compression
```

## Comparing `domain-admin-1.5.6.tar` & `domain-admin-1.5.7.tar`

### file list

```diff
@@ -1,457 +1,457 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.916354 domain-admin-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-23 14:37:24.000000 domain-admin-1.5.6/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-23 14:37:24.000000 domain-admin-1.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-23 14:37:36.916354 domain-admin-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-07-23 14:37:24.000000 domain-admin-1.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.864354 domain-admin-1.5.6/domain_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.868353 domain-admin-1.5.6/domain_admin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/address_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/cert_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/domain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16941 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/domain_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/group_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/ip_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/issue_certificate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/log_async_task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/log_operation_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/log_scheduler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/notify_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/prometheus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/api/whois_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.868353 domain-admin-1.5.6/domain_admin/config/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/config/default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/config/env_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/config/runtime_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.868353 domain-admin-1.5.6/domain_admin/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/enums/config_key_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/enums/event_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/enums/notify_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/enums/operation_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/enums/role_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/enums/status_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/enums/version_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.872353 domain-admin-1.5.6/domain_admin/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_102_to_103.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_106_to_110.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_110_to_1212.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_1212_to_1213.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_1213_to_131.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_136_to_140_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_140_alpha_to_140.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_1413_to_1414.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_1422_to_1423.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_143_to_144.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_145_to_146.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_151_to_152.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_154_to_155.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/migrate/migrate_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.872353 domain-admin-1.5.6/domain_admin/model/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/address_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/domain_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/group_user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/issue_certificate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/log_async_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/log_operation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/log_scheduler_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/notify_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/system_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/model/version_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.872353 domain-admin-1.5.6/domain_admin/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-23 14:37:33.000000 domain-admin-1.5.6/domain_admin/public/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.856353 domain-admin-1.5.6/domain_admin/public/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.856353 domain-admin-1.5.6/domain_admin/public/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.860353 domain-admin-1.5.6/domain_admin/public/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/objects/01/
--r--r--r--   0 runner    (1001) docker     (123)     1738 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/01/9bb44cfca57b7aa35ea7f5b6f99c3ef48e8d8f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/objects/19/
--r--r--r--   0 runner    (1001) docker     (123)    64350 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/objects/1e/
--r--r--r--   0 runner    (1001) docker     (123)      984 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/1e/270d8f3cc5167242582434675642b5858ba482
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/objects/21/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.876354 domain-admin-1.5.6/domain_admin/public/.git/objects/30/
--r--r--r--   0 runner    (1001) docker     (123)     7634 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/30/0478ea1f19f5a14d6a7167e9f71f5848707d76
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/3c/
--r--r--r--   0 runner    (1001) docker     (123)     3081 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
--r--r--r--   0 runner    (1001) docker     (123)   148706 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/40/
--r--r--r--   0 runner    (1001) docker     (123)      637 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/40/03c2e07280d146ee3443587c38ea2d264c07ca
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/50/
--r--r--r--   0 runner    (1001) docker     (123)     1895 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/50/c771a9bca6f87a2fb3381719fe0622eeae23bf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/52/
--r--r--r--   0 runner    (1001) docker     (123)    62564 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/53/
--r--r--r--   0 runner    (1001) docker     (123)      221 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/53/0864cbe282ec11e8564a8a3ce33756977d59ee
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/55/
--r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/58/
--r--r--r--   0 runner    (1001) docker     (123)    11674 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/58/1d5e80145e76e2ba0d08b038e1a2fefebef3bb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/5f/
--r--r--r--   0 runner    (1001) docker     (123)      530 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/69/
--r--r--r--   0 runner    (1001) docker     (123)   279936 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/6c/
--r--r--r--   0 runner    (1001) docker     (123)      155 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/6d/
--r--r--r--   0 runner    (1001) docker     (123)      612 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/77/
--r--r--r--   0 runner    (1001) docker     (123)     1436 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/77/bb86f804268cc8045d2cd2547ec17c22a0d166
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/79/
--r--r--r--   0 runner    (1001) docker     (123)   105817 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/7f/
--r--r--r--   0 runner    (1001) docker     (123)      368 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/89/
--r--r--r--   0 runner    (1001) docker     (123)      106 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/8c/
--r--r--r--   0 runner    (1001) docker     (123)       69 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/90/
--r--r--r--   0 runner    (1001) docker     (123)     2691 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/90/4a4570929957b2678d3c499a9cd83658a6675e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/91/
--r--r--r--   0 runner    (1001) docker     (123)      310 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/91/dcfad5270425be228e01a34e9c9b11ef3a0c4e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/92/
--r--r--r--   0 runner    (1001) docker     (123)      200 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/92/cfface0a460c51331fb8f25083a09948e00cbf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/93/
--r--r--r--   0 runner    (1001) docker     (123)     8844 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/93/522d98a7fe61eb676e55f33d92d8d090b967e4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/95/
--r--r--r--   0 runner    (1001) docker     (123)      118 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/95/f07af46d709638b20c0b2c66cdf6de8e89a7e4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/a0/
--r--r--r--   0 runner    (1001) docker     (123)     1814 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/a0/e9b4ee6e91d304066df26b1bc6218de181c2c2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/a2/
--r--r--r--   0 runner    (1001) docker     (123)    17343 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/a2/86b0b36b3538d177580f0c25e8e3a3a9f007b7
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.880354 domain-admin-1.5.6/domain_admin/public/.git/objects/ab/
--r--r--r--   0 runner    (1001) docker     (123)     1701 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/ab/2ba13bd2bd0cbf3e5b764ff0a29fd5872380c5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/b1/
--r--r--r--   0 runner    (1001) docker     (123)     6011 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/b1/115cb42fa8938fe1dbebccc9584aa03a895df0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/b3/
--r--r--r--   0 runner    (1001) docker     (123)    41902 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/bb/
--r--r--r--   0 runner    (1001) docker     (123)      474 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/bb/ecd10fc84228b6f4a1c2e0c90e2b68d4aa6bf2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/c0/
--r--r--r--   0 runner    (1001) docker     (123)      100 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/c0/76a86e24db79ccf75f79903b19cf145419d4bf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/c1/
--r--r--r--   0 runner    (1001) docker     (123)      694 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/c1/ff198374b288725eab95bc1294e1f04fe5c561
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/c4/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/cc/
--r--r--r--   0 runner    (1001) docker     (123)   361458 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/ce/
--r--r--r--   0 runner    (1001) docker     (123)     4311 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/ce/dcd8ba4511fabecdc11df81e55d82ca8b96ca3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/cf/
--r--r--r--   0 runner    (1001) docker     (123)     5817 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/cf/1eea719ca3a291ef7edaa6c60eaa808ca6e4ae
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/d4/
--r--r--r--   0 runner    (1001) docker     (123)     1026 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/d4/9eb5d776f5b92a02189cebbe590f76db9575bd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/d8/
--r--r--r--   0 runner    (1001) docker     (123)      464 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/d8/1e4838c9ac36863e037e68a2f3552f736c5c8f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/e1/
--r--r--r--   0 runner    (1001) docker     (123)    23927 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/e4/
--r--r--r--   0 runner    (1001) docker     (123)     3441 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/e4/c5465d396f947d57739ed8266597d6a47ef51b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/e6/
--r--r--r--   0 runner    (1001) docker     (123)     4593 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/e6/72b6afc2744b043e6fbdf3031eb086a109ec3c
--r--r--r--   0 runner    (1001) docker     (123)      227 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/e6/e5ddee110d6ed47cbb0a4f30db3d055efd21da
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/fd/
--r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/objects/ff/
--r--r--r--   0 runner    (1001) docker     (123)    13943 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.860353 domain-admin-1.5.6/domain_admin/public/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.860353 domain-admin-1.5.6/domain_admin/public/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.884353 domain-admin-1.5.6/domain_admin/public/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.888354 domain-admin-1.5.6/domain_admin/public/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/css/index.302e10d7.css
--rw-r--r--   0 runner    (1001) docker     (123)   331526 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/css/index.69a97337.css
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/css/index.75ef7015.css
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/css/index.a676cc2e.css
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/css/index.b285e10a.css
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/css/index.cf805e1c.css
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/css/index.d028ae37.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.888354 domain-admin-1.5.6/domain_admin/public/gif/
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/gif/user-avatar.ea67286d.gif
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.888354 domain-admin-1.5.6/domain_admin/public/jpg/
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/jpg/chatpet.fce5580e.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.896354 domain-admin-1.5.6/domain_admin/public/js/
--rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/ConditionFilterGroup.340936f7.js
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/ConnectStatus.89654d5c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/SearchUser.983b7494.js
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/SelectGroup.d7e6e540.js
--rw-r--r--   0 runner    (1001) docker     (123)   390997 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/codemirror-lib.a3a39aa0.js
--rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/element-icon.1ce1c350.js
--rw-r--r--   0 runner    (1001) docker     (123)   749914 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/element-plus.30eb1cab.js
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/event-enums.6c6f25e7.js
--rw-r--r--   0 runner    (1001) docker     (123)  1058329 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/highlight-lib.3654f6d3.js
--rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.075c6a16.js
--rw-r--r--   0 runner    (1001) docker     (123)    64823 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.12198a8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.127485d4.js
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.16184f42.js
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.2e3ad8c8.js
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.34096d0f.js
--rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.4704b0d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.51aeadc3.js
--rw-r--r--   0 runner    (1001) docker     (123)    28081 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.58059e0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.86cef4dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.a3947126.js
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.ab38e8b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.b84878f9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.c05aa8e8.js
--rw-r--r--   0 runner    (1001) docker     (123)    28958 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/index.c512b8f1.js
--rw-r--r--   0 runner    (1001) docker     (123)   312580 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/vendor-lib.76301fc3.js
--rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/js/vendor-vue.9e61e0af.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.896354 domain-admin-1.5.6/domain_admin/public/m/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.896354 domain-admin-1.5.6/domain_admin/public/m/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.896354 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.896354 domain-admin-1.5.6/domain_admin/public/m/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/m/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.896354 domain-admin-1.5.6/domain_admin/public/m/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.860353 domain-admin-1.5.6/domain_admin/public/m/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.896354 domain-admin-1.5.6/domain_admin/public/m/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.860353 domain-admin-1.5.6/domain_admin/public/m/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.896354 domain-admin-1.5.6/domain_admin/public/m/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.860353 domain-admin-1.5.6/domain_admin/public/m/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.896354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/2d/
--r--r--r--   0 runner    (1001) docker     (123)      814 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.896354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/43/
--r--r--r--   0 runner    (1001) docker     (123)     1262 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/4b/
--r--r--r--   0 runner    (1001) docker     (123)     5351 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/5c/
--r--r--r--   0 runner    (1001) docker     (123)       60 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/5c/98d16331bcc99b0cbbe89a3ffb23e3f5918ff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/61/
--r--r--r--   0 runner    (1001) docker     (123)      421 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/61/05f9fd4f4b11812fcca0d2e0704e4c8dd6e7a3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/62/
--r--r--r--   0 runner    (1001) docker     (123)      222 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/62/59838c4de171bc95a934ee2384d626eeb3040a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/67/
--r--r--r--   0 runner    (1001) docker     (123)      478 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/67/d2a69f1213016d777c02e0c99a38871d07da5b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/6f/
--r--r--r--   0 runner    (1001) docker     (123)      725 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/71/
--r--r--r--   0 runner    (1001) docker     (123)     2231 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/7a/
--r--r--r--   0 runner    (1001) docker     (123)     2494 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329
--r--r--r--   0 runner    (1001) docker     (123)      968 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/8e/
--r--r--r--   0 runner    (1001) docker     (123)     2655 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/93/
--r--r--r--   0 runner    (1001) docker     (123)     1108 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6
--r--r--r--   0 runner    (1001) docker     (123)     4673 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/98/
--r--r--r--   0 runner    (1001) docker     (123)     5141 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/a9/
--r--r--r--   0 runner    (1001) docker     (123)     1110 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/b0/
--r--r--r--   0 runner    (1001) docker     (123)     1821 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/c2/
--r--r--r--   0 runner    (1001) docker     (123)      505 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/c2/c748e84bc4d5118b0e33d6e0073e315a36d034
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/c7/
--r--r--r--   0 runner    (1001) docker     (123)    31300 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/c8/
--r--r--r--   0 runner    (1001) docker     (123)   143922 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/d9/
--r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/d9/d9ca2809d6994fef91c1ee2d22bc7a54b8b4a5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/ed/
--r--r--r--   0 runner    (1001) docker     (123)      979 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.900354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/f0/
--r--r--r--   0 runner    (1001) docker     (123)      755 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.904354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/f8/
--r--r--r--   0 runner    (1001) docker     (123)     1082 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.904354 domain-admin-1.5.6/domain_admin/public/m/.git/objects/fd/
--r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.860353 domain-admin-1.5.6/domain_admin/public/m/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.904354 domain-admin-1.5.6/domain_admin/public/m/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.860353 domain-admin-1.5.6/domain_admin/public/m/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.904354 domain-admin-1.5.6/domain_admin/public/m/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.904354 domain-admin-1.5.6/domain_admin/public/m/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/common-c7dd5d89.css
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/common.6194c42f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/index-5eda257b.css
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/index-958ae3a0.css
--rw-r--r--   0 runner    (1001) docker     (123)   379599 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/index-9c365a03.js
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/index-ad047368.css
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/index-e8224928.css
--rw-r--r--   0 runner    (1001) docker     (123)    53115 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/index-f79acb3d.css
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/index.1a0d1182.js
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/index.1d067866.js
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/index.daaf9893.js
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/index.feef7c0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/login-cb9f43ad.css
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/pages-login-login.09426b90.js
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/uni.06dd3c8e.css
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/assets/user-index-be7005ab.css
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.904354 domain-admin-1.5.6/domain_admin/public/m/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6334 2023-07-23 14:37:35.000000 domain-admin-1.5.6/domain_admin/public/m/static/user-avatar.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.904354 domain-admin-1.5.6/domain_admin/public/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-23 14:37:34.000000 domain-admin-1.5.6/domain_admin/public/svg/logo.184a2d7d.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.908354 domain-admin-1.5.6/domain_admin/router/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/router/api_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/router/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.908354 domain-admin-1.5.6/domain_admin/service/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/async_task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/common_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/domain_info_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/group_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/group_user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/issue_certificate_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/notify_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/operation_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/render_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/scheduler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/system_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/service/version_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.908354 domain-admin-1.5.6/domain_admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/templates/cert-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/templates/cert-export.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/templates/domain-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/templates/domain-export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.912354 domain-admin-1.5.6/domain_admin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.912354 domain-admin-1.5.6/domain_admin/utils/acme_util/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/acme_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/acme_util/acme_v2_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/bcrypt_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.912354 domain-admin-1.5.6/domain_admin/utils/cert_util/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/cert_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/cert_util/cert_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/cert_util/cert_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/cert_util/cert_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/cert_util/cert_openssl_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/cert_util/cert_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/cert_util/cert_socket_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/datetime_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/domain_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.912354 domain-admin-1.5.6/domain_admin/utils/flask_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/api_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/app_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/flask_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/http_code_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.912354 domain-admin-1.5.6/domain_admin/utils/flask_ext/json/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/json/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/json/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/json/json_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/flask_ext/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/icp_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/md5_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.912354 domain-admin-1.5.6/domain_admin/utils/open_api/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/open_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/open_api/crtsh_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/open_api/ding_talk_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/open_api/feishu_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/open_api/work_weixin_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.912354 domain-admin-1.5.6/domain_admin/utils/peewee_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/peewee_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/peewee_ext/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/secret_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/text_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.916354 domain-admin-1.5.6/domain_admin/utils/whois_util/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/whois_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/whois_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/whois_util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/whois_util/whois-servers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/utils/whois_util/whois_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-07-23 14:37:24.000000 domain-admin-1.5.6/domain_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.864354 domain-admin-1.5.6/domain_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-23 14:37:36.000000 domain-admin-1.5.6/domain_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16145 2023-07-23 14:37:36.000000 domain-admin-1.5.6/domain_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 14:37:36.000000 domain-admin-1.5.6/domain_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-23 14:37:36.000000 domain-admin-1.5.6/domain_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-23 14:37:36.000000 domain-admin-1.5.6/domain_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 14:37:36.000000 domain-admin-1.5.6/domain_admin.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:37:36.916354 domain-admin-1.5.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-23 14:37:24.000000 domain-admin-1.5.6/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 14:37:36.916354 domain-admin-1.5.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3190 2023-07-23 14:37:24.000000 domain-admin-1.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 05:27:30.000000 domain-admin-1.5.7/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-24 05:27:30.000000 domain-admin-1.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-24 05:27:45.933064 domain-admin-1.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-07-24 05:27:30.000000 domain-admin-1.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.897063 domain-admin-1.5.7/domain_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.901063 domain-admin-1.5.7/domain_admin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/address_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/cert_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/domain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16941 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/domain_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/group_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/ip_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/issue_certificate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/log_async_task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/log_operation_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/log_scheduler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/notify_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/prometheus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/api/whois_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.901063 domain-admin-1.5.7/domain_admin/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/config/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/config/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/config/runtime_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.901063 domain-admin-1.5.7/domain_admin/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/config_key_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/event_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/notify_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/operation_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/enums/version_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.901063 domain-admin-1.5.7/domain_admin/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_102_to_103.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_106_to_110.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_110_to_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_1212_to_1213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_1213_to_131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_136_to_140_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_140_alpha_to_140.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_1413_to_1414.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_1422_to_1423.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_143_to_144.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_145_to_146.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_151_to_152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_154_to_155.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/migrate/migrate_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/address_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/domain_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/group_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/issue_certificate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/log_async_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/log_operation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/log_scheduler_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/notify_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/system_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/model/version_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-24 05:27:42.000000 domain-admin-1.5.7/domain_admin/public/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.889063 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.889063 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.893063 domain-admin-1.5.7/domain_admin/public/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/objects/01/
+-r--r--r--   0 runner    (1001) docker     (123)     1738 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/01/9bb44cfca57b7aa35ea7f5b6f99c3ef48e8d8f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/objects/19/
+-r--r--r--   0 runner    (1001) docker     (123)    64350 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/objects/1e/
+-r--r--r--   0 runner    (1001) docker     (123)      984 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/1e/270d8f3cc5167242582434675642b5858ba482
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/objects/21/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.905063 domain-admin-1.5.7/domain_admin/public/.git/objects/30/
+-r--r--r--   0 runner    (1001) docker     (123)     7634 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/30/0478ea1f19f5a14d6a7167e9f71f5848707d76
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/3c/
+-r--r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
+-r--r--r--   0 runner    (1001) docker     (123)   148706 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/40/
+-r--r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/40/03c2e07280d146ee3443587c38ea2d264c07ca
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/50/
+-r--r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/50/c771a9bca6f87a2fb3381719fe0622eeae23bf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/52/
+-r--r--r--   0 runner    (1001) docker     (123)    62564 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/53/
+-r--r--r--   0 runner    (1001) docker     (123)      221 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/53/0864cbe282ec11e8564a8a3ce33756977d59ee
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/55/
+-r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/58/
+-r--r--r--   0 runner    (1001) docker     (123)    11674 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/58/1d5e80145e76e2ba0d08b038e1a2fefebef3bb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/5f/
+-r--r--r--   0 runner    (1001) docker     (123)      530 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/69/
+-r--r--r--   0 runner    (1001) docker     (123)   279936 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/6c/
+-r--r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/6d/
+-r--r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/77/
+-r--r--r--   0 runner    (1001) docker     (123)     1436 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/77/bb86f804268cc8045d2cd2547ec17c22a0d166
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/79/
+-r--r--r--   0 runner    (1001) docker     (123)   105817 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/7f/
+-r--r--r--   0 runner    (1001) docker     (123)      368 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/89/
+-r--r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/8c/
+-r--r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/90/
+-r--r--r--   0 runner    (1001) docker     (123)     2691 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/90/4a4570929957b2678d3c499a9cd83658a6675e
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/91/
+-r--r--r--   0 runner    (1001) docker     (123)      310 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/91/dcfad5270425be228e01a34e9c9b11ef3a0c4e
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/92/
+-r--r--r--   0 runner    (1001) docker     (123)      200 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/92/cfface0a460c51331fb8f25083a09948e00cbf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/93/
+-r--r--r--   0 runner    (1001) docker     (123)     8844 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/93/522d98a7fe61eb676e55f33d92d8d090b967e4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/95/
+-r--r--r--   0 runner    (1001) docker     (123)      118 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/95/f07af46d709638b20c0b2c66cdf6de8e89a7e4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/a0/
+-r--r--r--   0 runner    (1001) docker     (123)     1814 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/a0/e9b4ee6e91d304066df26b1bc6218de181c2c2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/a2/
+-r--r--r--   0 runner    (1001) docker     (123)    17343 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/a2/86b0b36b3538d177580f0c25e8e3a3a9f007b7
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/ab/
+-r--r--r--   0 runner    (1001) docker     (123)     1701 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/ab/2ba13bd2bd0cbf3e5b764ff0a29fd5872380c5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/b1/
+-r--r--r--   0 runner    (1001) docker     (123)     6011 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/b1/115cb42fa8938fe1dbebccc9584aa03a895df0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/b3/
+-r--r--r--   0 runner    (1001) docker     (123)    41902 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/bb/
+-r--r--r--   0 runner    (1001) docker     (123)      474 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/bb/ecd10fc84228b6f4a1c2e0c90e2b68d4aa6bf2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/c0/
+-r--r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/c0/76a86e24db79ccf75f79903b19cf145419d4bf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/c1/
+-r--r--r--   0 runner    (1001) docker     (123)      694 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/c1/ff198374b288725eab95bc1294e1f04fe5c561
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/c4/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.909063 domain-admin-1.5.7/domain_admin/public/.git/objects/cc/
+-r--r--r--   0 runner    (1001) docker     (123)   361458 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/ce/
+-r--r--r--   0 runner    (1001) docker     (123)     4311 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/ce/dcd8ba4511fabecdc11df81e55d82ca8b96ca3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/cf/
+-r--r--r--   0 runner    (1001) docker     (123)     5817 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/cf/1eea719ca3a291ef7edaa6c60eaa808ca6e4ae
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/d4/
+-r--r--r--   0 runner    (1001) docker     (123)     1026 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/d4/9eb5d776f5b92a02189cebbe590f76db9575bd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/d8/
+-r--r--r--   0 runner    (1001) docker     (123)      464 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/d8/1e4838c9ac36863e037e68a2f3552f736c5c8f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/e1/
+-r--r--r--   0 runner    (1001) docker     (123)    23927 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/e4/
+-r--r--r--   0 runner    (1001) docker     (123)     3441 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/e4/c5465d396f947d57739ed8266597d6a47ef51b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/e6/
+-r--r--r--   0 runner    (1001) docker     (123)     4593 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/e6/72b6afc2744b043e6fbdf3031eb086a109ec3c
+-r--r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/e6/e5ddee110d6ed47cbb0a4f30db3d055efd21da
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/fd/
+-r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/objects/ff/
+-r--r--r--   0 runner    (1001) docker     (123)    13943 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.893063 domain-admin-1.5.7/domain_admin/public/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.893063 domain-admin-1.5.7/domain_admin/public/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.302e10d7.css
+-rw-r--r--   0 runner    (1001) docker     (123)   331526 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.69a97337.css
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.75ef7015.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.a676cc2e.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.b285e10a.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.cf805e1c.css
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/css/index.d028ae37.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/gif/
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/gif/user-avatar.ea67286d.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.913063 domain-admin-1.5.7/domain_admin/public/jpg/
+-rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/jpg/chatpet.fce5580e.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/ConditionFilterGroup.340936f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/ConnectStatus.89654d5c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/SearchUser.983b7494.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/SelectGroup.d7e6e540.js
+-rw-r--r--   0 runner    (1001) docker     (123)   390997 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/codemirror-lib.a3a39aa0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/element-icon.1ce1c350.js
+-rw-r--r--   0 runner    (1001) docker     (123)   749914 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/element-plus.30eb1cab.js
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/event-enums.6c6f25e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1058329 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/highlight-lib.3654f6d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.075c6a16.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64823 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.12198a8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.127485d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.16184f42.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.2e3ad8c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.34096d0f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.4704b0d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.51aeadc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28081 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.58059e0f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.86cef4dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.a3947126.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.ab38e8b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.b84878f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.c05aa8e8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28958 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/index.c512b8f1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   312580 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/vendor-lib.76301fc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/js/vendor-vue.9e61e0af.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.893063 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.893063 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.897063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/2d/
+-r--r--r--   0 runner    (1001) docker     (123)      814 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/43/
+-r--r--r--   0 runner    (1001) docker     (123)     1262 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/4b/
+-r--r--r--   0 runner    (1001) docker     (123)     5351 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/5c/
+-r--r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/5c/98d16331bcc99b0cbbe89a3ffb23e3f5918ff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/61/
+-r--r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/61/05f9fd4f4b11812fcca0d2e0704e4c8dd6e7a3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/62/
+-r--r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/62/59838c4de171bc95a934ee2384d626eeb3040a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/67/
+-r--r--r--   0 runner    (1001) docker     (123)      478 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/67/d2a69f1213016d777c02e0c99a38871d07da5b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/6f/
+-r--r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/71/
+-r--r--r--   0 runner    (1001) docker     (123)     2231 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/7a/
+-r--r--r--   0 runner    (1001) docker     (123)     2494 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329
+-r--r--r--   0 runner    (1001) docker     (123)      968 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/8e/
+-r--r--r--   0 runner    (1001) docker     (123)     2655 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/93/
+-r--r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6
+-r--r--r--   0 runner    (1001) docker     (123)     4673 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/98/
+-r--r--r--   0 runner    (1001) docker     (123)     5141 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/a9/
+-r--r--r--   0 runner    (1001) docker     (123)     1110 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.921063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/b0/
+-r--r--r--   0 runner    (1001) docker     (123)     1821 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c2/
+-r--r--r--   0 runner    (1001) docker     (123)      505 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c2/c748e84bc4d5118b0e33d6e0073e315a36d034
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c7/
+-r--r--r--   0 runner    (1001) docker     (123)    31300 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c8/
+-r--r--r--   0 runner    (1001) docker     (123)   143922 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/d9/
+-r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/d9/d9ca2809d6994fef91c1ee2d22bc7a54b8b4a5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/ed/
+-r--r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/f0/
+-r--r--r--   0 runner    (1001) docker     (123)      755 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/f8/
+-r--r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/objects/fd/
+-r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.897063 domain-admin-1.5.7/domain_admin/public/m/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.897063 domain-admin-1.5.7/domain_admin/public/m/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/common-c7dd5d89.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/common.6194c42f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-5eda257b.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-958ae3a0.css
+-rw-r--r--   0 runner    (1001) docker     (123)   379599 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-9c365a03.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-ad047368.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-e8224928.css
+-rw-r--r--   0 runner    (1001) docker     (123)    53115 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index-f79acb3d.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index.1a0d1182.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index.1d067866.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index.daaf9893.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/index.feef7c0f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/login-cb9f43ad.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/pages-login-login.09426b90.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/uni.06dd3c8e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/assets/user-index-be7005ab.css
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/m/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6334 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/m/static/user-avatar.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.925063 domain-admin-1.5.7/domain_admin/public/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-24 05:27:43.000000 domain-admin-1.5.7/domain_admin/public/svg/logo.184a2d7d.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.929063 domain-admin-1.5.7/domain_admin/router/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/router/api_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/router/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.929063 domain-admin-1.5.7/domain_admin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/async_task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/common_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/domain_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/group_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/group_user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/issue_certificate_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/notify_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/operation_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/render_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/scheduler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/system_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/service/version_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.929063 domain-admin-1.5.7/domain_admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/templates/cert-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/templates/cert-export.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/templates/domain-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/templates/domain-export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.929063 domain-admin-1.5.7/domain_admin/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.929063 domain-admin-1.5.7/domain_admin/utils/acme_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/acme_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/acme_util/acme_v2_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/bcrypt_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/cert_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_openssl_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/cert_util/cert_socket_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/datetime_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/domain_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/flask_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/api_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/app_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/http_code_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/flask_ext/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/json/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/json/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/json/json_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/flask_ext/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/icp_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/md5_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/open_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/open_api/crtsh_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/open_api/ding_talk_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/open_api/feishu_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/open_api/work_weixin_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/peewee_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/peewee_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/peewee_ext/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/secret_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/text_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/domain_admin/utils/whois_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/whois_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/whois_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/whois_util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/whois_util/whois-servers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/utils/whois_util/whois_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-07-24 05:27:30.000000 domain-admin-1.5.7/domain_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.897063 domain-admin-1.5.7/domain_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16145 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:27:45.000000 domain-admin-1.5.7/domain_admin.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:27:45.933064 domain-admin-1.5.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-24 05:27:30.000000 domain-admin-1.5.7/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 05:27:45.933064 domain-admin-1.5.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3190 2023-07-24 05:27:30.000000 domain-admin-1.5.7/setup.py
```

### Comparing `domain-admin-1.5.6/LICENSE` & `domain-admin-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/PKG-INFO` & `domain-admin-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.5.6
+Version: 1.5.7
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain,ssl,cert,web,monitor
 Platform: any
```

### Comparing `domain-admin-1.5.6/README.md` & `domain-admin-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/address_api.py` & `domain-admin-1.5.7/domain_admin/api/address_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/auth_api.py` & `domain-admin-1.5.7/domain_admin/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/cert_api.py` & `domain-admin-1.5.7/domain_admin/api/cert_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/domain_api.py` & `domain-admin-1.5.7/domain_admin/api/domain_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/domain_info_api.py` & `domain-admin-1.5.7/domain_admin/api/domain_info_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/group_api.py` & `domain-admin-1.5.7/domain_admin/api/group_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/group_user_api.py` & `domain-admin-1.5.7/domain_admin/api/group_user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/issue_certificate_api.py` & `domain-admin-1.5.7/domain_admin/api/issue_certificate_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/log_async_task_api.py` & `domain-admin-1.5.7/domain_admin/api/log_async_task_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/log_operation_api.py` & `domain-admin-1.5.7/domain_admin/api/log_operation_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/log_scheduler_api.py` & `domain-admin-1.5.7/domain_admin/api/log_scheduler_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/notify_api.py` & `domain-admin-1.5.7/domain_admin/api/notify_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/prometheus_api.py` & `domain-admin-1.5.7/domain_admin/api/prometheus_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/system_api.py` & `domain-admin-1.5.7/domain_admin/api/system_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/user_api.py` & `domain-admin-1.5.7/domain_admin/api/user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/api/whois_api.py` & `domain-admin-1.5.7/domain_admin/api/whois_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/compat.py` & `domain-admin-1.5.7/domain_admin/compat.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/config/default_config.py` & `domain-admin-1.5.7/domain_admin/config/default_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/config/env_config.py` & `domain-admin-1.5.7/domain_admin/config/env_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/config/runtime_config.py` & `domain-admin-1.5.7/domain_admin/config/runtime_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/enums/config_key_enum.py` & `domain-admin-1.5.7/domain_admin/enums/config_key_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/enums/operation_enum.py` & `domain-admin-1.5.7/domain_admin/enums/operation_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/enums/version_enum.py` & `domain-admin-1.5.7/domain_admin/enums/version_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/log.py` & `domain-admin-1.5.7/domain_admin/log.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/main.py` & `domain-admin-1.5.7/domain_admin/main.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_102_to_103.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_102_to_103.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_106_to_110.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_106_to_110.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_110_to_1212.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_110_to_1212.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_1212_to_1213.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_1212_to_1213.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_1213_to_131.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_1213_to_131.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_136_to_140_alpha.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_136_to_140_alpha.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_140_alpha_to_140.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_140_alpha_to_140.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_1413_to_1414.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_1413_to_1414.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_1422_to_1423.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_1422_to_1423.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_143_to_144.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_143_to_144.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_145_to_146.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_145_to_146.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_151_to_152.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_151_to_152.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_154_to_155.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_154_to_155.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/migrate/migrate_common.py` & `domain-admin-1.5.7/domain_admin/migrate/migrate_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/address_model.py` & `domain-admin-1.5.7/domain_admin/model/address_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/base_model.py` & `domain-admin-1.5.7/domain_admin/model/base_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/database.py` & `domain-admin-1.5.7/domain_admin/model/database.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/domain_info_model.py` & `domain-admin-1.5.7/domain_admin/model/domain_info_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/domain_model.py` & `domain-admin-1.5.7/domain_admin/model/domain_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/group_model.py` & `domain-admin-1.5.7/domain_admin/model/group_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/group_user_model.py` & `domain-admin-1.5.7/domain_admin/model/group_user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/issue_certificate_model.py` & `domain-admin-1.5.7/domain_admin/model/issue_certificate_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/log_async_task_model.py` & `domain-admin-1.5.7/domain_admin/model/log_async_task_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/log_operation_model.py` & `domain-admin-1.5.7/domain_admin/model/log_operation_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/log_scheduler_model.py` & `domain-admin-1.5.7/domain_admin/model/log_scheduler_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/notify_model.py` & `domain-admin-1.5.7/domain_admin/model/notify_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/system_model.py` & `domain-admin-1.5.7/domain_admin/model/system_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/user_model.py` & `domain-admin-1.5.7/domain_admin/model/user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/model/version_model.py` & `domain-admin-1.5.7/domain_admin/model/version_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/hooks/commit-msg.sample` & `domain-admin-1.5.7/domain_admin/public/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.5.7/domain_admin/public/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/hooks/pre-commit.sample` & `domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/hooks/pre-push.sample` & `domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/hooks/pre-rebase.sample` & `domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/hooks/pre-receive.sample` & `domain-admin-1.5.7/domain_admin/public/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.5.7/domain_admin/public/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/hooks/push-to-checkout.sample` & `domain-admin-1.5.7/domain_admin/public/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/hooks/sendemail-validate.sample` & `domain-admin-1.5.7/domain_admin/public/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/hooks/update.sample` & `domain-admin-1.5.7/domain_admin/public/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/01/9bb44cfca57b7aa35ea7f5b6f99c3ef48e8d8f` & `domain-admin-1.5.7/domain_admin/public/.git/objects/01/9bb44cfca57b7aa35ea7f5b6f99c3ef48e8d8f`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63` & `domain-admin-1.5.7/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/1e/270d8f3cc5167242582434675642b5858ba482` & `domain-admin-1.5.7/domain_admin/public/.git/objects/1e/270d8f3cc5167242582434675642b5858ba482`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/30/0478ea1f19f5a14d6a7167e9f71f5848707d76` & `domain-admin-1.5.7/domain_admin/public/.git/objects/30/0478ea1f19f5a14d6a7167e9f71f5848707d76`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949` & `domain-admin-1.5.7/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1` & `domain-admin-1.5.7/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/40/03c2e07280d146ee3443587c38ea2d264c07ca` & `domain-admin-1.5.7/domain_admin/public/.git/objects/40/03c2e07280d146ee3443587c38ea2d264c07ca`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/50/c771a9bca6f87a2fb3381719fe0622eeae23bf` & `domain-admin-1.5.7/domain_admin/public/.git/objects/50/c771a9bca6f87a2fb3381719fe0622eeae23bf`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462` & `domain-admin-1.5.7/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/58/1d5e80145e76e2ba0d08b038e1a2fefebef3bb` & `domain-admin-1.5.7/domain_admin/public/.git/objects/58/1d5e80145e76e2ba0d08b038e1a2fefebef3bb`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34` & `domain-admin-1.5.7/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a` & `domain-admin-1.5.7/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc` & `domain-admin-1.5.7/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/77/bb86f804268cc8045d2cd2547ec17c22a0d166` & `domain-admin-1.5.7/domain_admin/public/.git/objects/77/bb86f804268cc8045d2cd2547ec17c22a0d166`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b` & `domain-admin-1.5.7/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/90/4a4570929957b2678d3c499a9cd83658a6675e` & `domain-admin-1.5.7/domain_admin/public/.git/objects/90/4a4570929957b2678d3c499a9cd83658a6675e`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/93/522d98a7fe61eb676e55f33d92d8d090b967e4` & `domain-admin-1.5.7/domain_admin/public/.git/objects/93/522d98a7fe61eb676e55f33d92d8d090b967e4`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/a0/e9b4ee6e91d304066df26b1bc6218de181c2c2` & `domain-admin-1.5.7/domain_admin/public/.git/objects/a0/e9b4ee6e91d304066df26b1bc6218de181c2c2`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/a2/86b0b36b3538d177580f0c25e8e3a3a9f007b7` & `domain-admin-1.5.7/domain_admin/public/.git/objects/a2/86b0b36b3538d177580f0c25e8e3a3a9f007b7`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/ab/2ba13bd2bd0cbf3e5b764ff0a29fd5872380c5` & `domain-admin-1.5.7/domain_admin/public/.git/objects/ab/2ba13bd2bd0cbf3e5b764ff0a29fd5872380c5`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/b1/115cb42fa8938fe1dbebccc9584aa03a895df0` & `domain-admin-1.5.7/domain_admin/public/.git/objects/b1/115cb42fa8938fe1dbebccc9584aa03a895df0`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad` & `domain-admin-1.5.7/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/c1/ff198374b288725eab95bc1294e1f04fe5c561` & `domain-admin-1.5.7/domain_admin/public/.git/objects/c1/ff198374b288725eab95bc1294e1f04fe5c561`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9` & `domain-admin-1.5.7/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/ce/dcd8ba4511fabecdc11df81e55d82ca8b96ca3` & `domain-admin-1.5.7/domain_admin/public/.git/objects/ce/dcd8ba4511fabecdc11df81e55d82ca8b96ca3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/cf/1eea719ca3a291ef7edaa6c60eaa808ca6e4ae` & `domain-admin-1.5.7/domain_admin/public/.git/objects/cf/1eea719ca3a291ef7edaa6c60eaa808ca6e4ae`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/d4/9eb5d776f5b92a02189cebbe590f76db9575bd` & `domain-admin-1.5.7/domain_admin/public/.git/objects/d4/9eb5d776f5b92a02189cebbe590f76db9575bd`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b` & `domain-admin-1.5.7/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/e4/c5465d396f947d57739ed8266597d6a47ef51b` & `domain-admin-1.5.7/domain_admin/public/.git/objects/e4/c5465d396f947d57739ed8266597d6a47ef51b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/e6/72b6afc2744b043e6fbdf3031eb086a109ec3c` & `domain-admin-1.5.7/domain_admin/public/.git/objects/e6/72b6afc2744b043e6fbdf3031eb086a109ec3c`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3` & `domain-admin-1.5.7/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd` & `domain-admin-1.5.7/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/css/ConditionFilterGroup.a91875e6.css` & `domain-admin-1.5.7/domain_admin/public/css/ConditionFilterGroup.a91875e6.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/css/index.69a97337.css` & `domain-admin-1.5.7/domain_admin/public/css/index.69a97337.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/favicon.ico` & `domain-admin-1.5.7/domain_admin/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/gif/user-avatar.ea67286d.gif` & `domain-admin-1.5.7/domain_admin/public/gif/user-avatar.ea67286d.gif`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/index.html` & `domain-admin-1.5.7/domain_admin/public/index.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg` & `domain-admin-1.5.7/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/jpg/chatpet.fce5580e.jpg` & `domain-admin-1.5.7/domain_admin/public/jpg/chatpet.fce5580e.jpg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/ConditionFilterGroup.340936f7.js` & `domain-admin-1.5.7/domain_admin/public/js/ConditionFilterGroup.340936f7.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/ConnectStatus.89654d5c.js` & `domain-admin-1.5.7/domain_admin/public/js/ConnectStatus.89654d5c.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/SearchUser.983b7494.js` & `domain-admin-1.5.7/domain_admin/public/js/SearchUser.983b7494.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/SelectGroup.d7e6e540.js` & `domain-admin-1.5.7/domain_admin/public/js/SelectGroup.d7e6e540.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/codemirror-lib.a3a39aa0.js` & `domain-admin-1.5.7/domain_admin/public/js/codemirror-lib.a3a39aa0.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/element-icon.1ce1c350.js` & `domain-admin-1.5.7/domain_admin/public/js/element-icon.1ce1c350.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/element-plus.30eb1cab.js` & `domain-admin-1.5.7/domain_admin/public/js/element-plus.30eb1cab.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/event-enums.6c6f25e7.js` & `domain-admin-1.5.7/domain_admin/public/js/event-enums.6c6f25e7.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/highlight-lib.3654f6d3.js` & `domain-admin-1.5.7/domain_admin/public/js/highlight-lib.3654f6d3.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.075c6a16.js` & `domain-admin-1.5.7/domain_admin/public/js/index.075c6a16.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.12198a8e.js` & `domain-admin-1.5.7/domain_admin/public/js/index.12198a8e.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.127485d4.js` & `domain-admin-1.5.7/domain_admin/public/js/index.127485d4.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.16184f42.js` & `domain-admin-1.5.7/domain_admin/public/js/index.16184f42.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.2e3ad8c8.js` & `domain-admin-1.5.7/domain_admin/public/js/index.2e3ad8c8.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.34096d0f.js` & `domain-admin-1.5.7/domain_admin/public/js/index.34096d0f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.4704b0d3.js` & `domain-admin-1.5.7/domain_admin/public/js/index.4704b0d3.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.51aeadc3.js` & `domain-admin-1.5.7/domain_admin/public/js/index.51aeadc3.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.58059e0f.js` & `domain-admin-1.5.7/domain_admin/public/js/index.58059e0f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.86cef4dd.js` & `domain-admin-1.5.7/domain_admin/public/js/index.86cef4dd.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.a3947126.js` & `domain-admin-1.5.7/domain_admin/public/js/index.a3947126.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.ab38e8b8.js` & `domain-admin-1.5.7/domain_admin/public/js/index.ab38e8b8.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.b84878f9.js` & `domain-admin-1.5.7/domain_admin/public/js/index.b84878f9.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.c05aa8e8.js` & `domain-admin-1.5.7/domain_admin/public/js/index.c05aa8e8.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/index.c512b8f1.js` & `domain-admin-1.5.7/domain_admin/public/js/index.c512b8f1.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/vendor-lib.76301fc3.js` & `domain-admin-1.5.7/domain_admin/public/js/vendor-lib.76301fc3.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/js/vendor-vue.9e61e0af.js` & `domain-admin-1.5.7/domain_admin/public/js/vendor-vue.9e61e0af.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/hooks/commit-msg.sample` & `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/hooks/pre-commit.sample` & `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/hooks/pre-push.sample` & `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/hooks/pre-rebase.sample` & `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/hooks/pre-receive.sample` & `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/hooks/push-to-checkout.sample` & `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/hooks/sendemail-validate.sample` & `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/hooks/update.sample` & `domain-admin-1.5.7/domain_admin/public/m/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3` & `domain-admin-1.5.7/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/common-c7dd5d89.css` & `domain-admin-1.5.7/domain_admin/public/m/assets/common-c7dd5d89.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/common.6194c42f.js` & `domain-admin-1.5.7/domain_admin/public/m/assets/common.6194c42f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/index-5eda257b.css` & `domain-admin-1.5.7/domain_admin/public/m/assets/index-5eda257b.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/index-958ae3a0.css` & `domain-admin-1.5.7/domain_admin/public/m/assets/index-958ae3a0.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/index-9c365a03.js` & `domain-admin-1.5.7/domain_admin/public/m/assets/index-9c365a03.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/index-ad047368.css` & `domain-admin-1.5.7/domain_admin/public/m/assets/index-ad047368.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/index-e8224928.css` & `domain-admin-1.5.7/domain_admin/public/m/assets/index-e8224928.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/index-f79acb3d.css` & `domain-admin-1.5.7/domain_admin/public/m/assets/index-f79acb3d.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/index.1a0d1182.js` & `domain-admin-1.5.7/domain_admin/public/m/assets/index.1a0d1182.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/index.1d067866.js` & `domain-admin-1.5.7/domain_admin/public/m/assets/index.1d067866.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/index.daaf9893.js` & `domain-admin-1.5.7/domain_admin/public/m/assets/index.daaf9893.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/index.feef7c0f.js` & `domain-admin-1.5.7/domain_admin/public/m/assets/index.feef7c0f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/login-cb9f43ad.css` & `domain-admin-1.5.7/domain_admin/public/m/assets/login-cb9f43ad.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js` & `domain-admin-1.5.7/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js` & `domain-admin-1.5.7/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/pages-login-login.09426b90.js` & `domain-admin-1.5.7/domain_admin/public/m/assets/pages-login-login.09426b90.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js` & `domain-admin-1.5.7/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/uni.06dd3c8e.css` & `domain-admin-1.5.7/domain_admin/public/m/assets/uni.06dd3c8e.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/assets/user-index-be7005ab.css` & `domain-admin-1.5.7/domain_admin/public/m/assets/user-index-be7005ab.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/index.html` & `domain-admin-1.5.7/domain_admin/public/m/index.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/m/static/user-avatar.gif` & `domain-admin-1.5.7/domain_admin/public/m/static/user-avatar.gif`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/public/svg/logo.184a2d7d.svg` & `domain-admin-1.5.7/domain_admin/public/svg/logo.184a2d7d.svg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/router/api_map.py` & `domain-admin-1.5.7/domain_admin/router/api_map.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/router/permission.py` & `domain-admin-1.5.7/domain_admin/router/permission.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/async_task_service.py` & `domain-admin-1.5.7/domain_admin/service/async_task_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/auth_service.py` & `domain-admin-1.5.7/domain_admin/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/common_service.py` & `domain-admin-1.5.7/domain_admin/service/common_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/domain_info_service.py` & `domain-admin-1.5.7/domain_admin/service/domain_info_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/domain_service.py` & `domain-admin-1.5.7/domain_admin/service/domain_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/file_service.py` & `domain-admin-1.5.7/domain_admin/service/file_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/group_service.py` & `domain-admin-1.5.7/domain_admin/service/group_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/group_user_service.py` & `domain-admin-1.5.7/domain_admin/service/group_user_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/issue_certificate_service.py` & `domain-admin-1.5.7/domain_admin/service/issue_certificate_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/notify_service.py` & `domain-admin-1.5.7/domain_admin/service/notify_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/operation_service.py` & `domain-admin-1.5.7/domain_admin/service/operation_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/scheduler_service.py` & `domain-admin-1.5.7/domain_admin/service/scheduler_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/system_service.py` & `domain-admin-1.5.7/domain_admin/service/system_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/token_service.py` & `domain-admin-1.5.7/domain_admin/service/token_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/service/version_service.py` & `domain-admin-1.5.7/domain_admin/service/version_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/templates/cert-email.html` & `domain-admin-1.5.7/domain_admin/templates/cert-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/templates/domain-email.html` & `domain-admin-1.5.7/domain_admin/templates/domain-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/acme_util/acme_v2_api.py` & `domain-admin-1.5.7/domain_admin/utils/acme_util/acme_v2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 """
 @File    : acme_v2_api.py
 @Date    : 2023-07-23
 
+code from https://github.com/certbot/certbot/blob/master/acme/examples/http01_example.py
+
 https://datatracker.ietf.org/doc/html/rfc8555
 https://www.rfc-editor.org/rfc/rfc8555
 
 ref:
 acme-dns-tiny: https://gitlab.adorsaz.ch/adrien/acme-dns-tiny/-/tree/main
 
 https://pypi.org/project/acme/
 
 https://www.pyopenssl.org/en/latest/index.html
 
 https://zhuanlan.zhihu.com/p/75032510
 https://letsencrypt.org/zh-cn/docs/challenge-types/
 https://datatracker.ietf.org/doc/html/rfc8555
 
-code from https://github.com/certbot/certbot/blob/master/acme/examples/http01_example.py
 
 Example ACME-V2 API for HTTP-01 challenge.
 
 Brief:
 
 This a complete usage example of the python-acme API.
```

### Comparing `domain-admin-1.5.6/domain_admin/utils/bcrypt_util.py` & `domain-admin-1.5.7/domain_admin/utils/bcrypt_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/cert_util/cert_common.py` & `domain-admin-1.5.7/domain_admin/utils/cert_util/cert_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/cert_util/cert_openssl_v2.py` & `domain-admin-1.5.7/domain_admin/utils/cert_util/cert_openssl_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/cert_util/cert_socket.py` & `domain-admin-1.5.7/domain_admin/utils/cert_util/cert_socket.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/cert_util/cert_socket_v2.py` & `domain-admin-1.5.7/domain_admin/utils/cert_util/cert_socket_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/datetime_util.py` & `domain-admin-1.5.7/domain_admin/utils/datetime_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 DATETIME_SHORT_FORMAT = "%Y-%m-%d %H:%M"
 
 DATE_FORMAT = "%Y-%m-%d"
 
 TIME_FORMAT = "%H:%M:%S"
 
 
+class TimeEnum(object):
+    Second = 1
+    Minute = 60 * Second
+    Hour = 60 * Minute
+    Day = 24 * Hour
+
+
 def get_timestamp(datetime_obj):
     """
     fix: Python 2.7 AttributeError: 'datetime.datetime' object has no attribute 'timestamp'
     ref: https://stackoverflow.com/questions/50650704/attributeerror-datetime-datetime-object-has-no-attribute-timestamp
 
     :param datetime_obj:
     :return: int
@@ -68,15 +75,15 @@
     """
     将时间格式化为: 1d 2h 3m 4s
     :param seconds:
     :return:
     """
     second = 1
     minute = second * 60
-    hour = minute * 12
+    hour = minute * 60
     day = hour * 24
 
     lst = []
 
     if seconds > day:
         days, seconds = divmod(seconds, day)
         lst.append(str(days) + 'd')
@@ -148,23 +155,7 @@
     """
     if start_date and end_date \
             and isinstance(start_date, datetime) \
             and isinstance(end_date, datetime):
         return get_timestamp(end_date) - get_timestamp(start_date)
     else:
         return 0
-
-
-if __name__ == '__main__':
-    print(time_for_human(1665381270))
-    # 2天前
-
-    print(time_for_human(datetime.now()))
-    # 刚刚
-
-    print(time_for_human(time.time() - 100))
-    # 1分钟前
-
-    print(time_for_human('2022-10-10 13:33:11'))
-    # 2天前
-
-    print(get_timestamp(datetime.now()))
```

### Comparing `domain-admin-1.5.6/domain_admin/utils/domain_util.py` & `domain-admin-1.5.7/domain_admin/utils/domain_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/email_util.py` & `domain-admin-1.5.7/domain_admin/utils/email_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,18 @@
     """
     mail_username = mail_username or DEFAULT_MAIL_USERNAME
     mail_alias = mail_alias or mail_username
 
     # 构造邮件
     message = MIMEText(content, content_type, 'utf-8')
     # 邮箱昵称、发件人邮箱账号
-    message['From'] = formataddr((mail_alias, mail_username))
     message['Subject'] = Header(subject, 'utf-8')
+    message['From'] = formataddr((mail_alias, mail_username))
+    # bugfix: 显示收件人
+    message['To'] = ','.join(formataddr((mail, mail)) for mail in to_addresses)
 
     server = get_email_server(mail_host, mail_port)
 
     # 需要登录，否则匿名
     if mail_password:
         server.login(mail_username, mail_password)
```

### Comparing `domain-admin-1.5.6/domain_admin/utils/flask_ext/api_result.py` & `domain-admin-1.5.7/domain_admin/utils/flask_ext/api_result.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/flask_ext/app_exception.py` & `domain-admin-1.5.7/domain_admin/utils/flask_ext/app_exception.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/flask_ext/flask_app.py` & `domain-admin-1.5.7/domain_admin/utils/flask_ext/flask_app.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/flask_ext/handler.py` & `domain-admin-1.5.7/domain_admin/utils/flask_ext/handler.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/flask_ext/json/default.py` & `domain-admin-1.5.7/domain_admin/utils/flask_ext/json/default.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/flask_ext/json/json_encoder.py` & `domain-admin-1.5.7/domain_admin/utils/flask_ext/json/json_encoder.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/flask_ext/json/json_provider.py` & `domain-admin-1.5.7/domain_admin/utils/flask_ext/json/json_provider.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/icp_util.py` & `domain-admin-1.5.7/domain_admin/utils/icp_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 @File    : icp_util.py
 @Date    : 2023-06-30
+
+备案查询网站：https://www.beianx.cn/
 """
 from __future__ import print_function, unicode_literals, absolute_import, division
 
 import json
 import re
 
 import requests
```

### Comparing `domain-admin-1.5.6/domain_admin/utils/ip_util.py` & `domain-admin-1.5.7/domain_admin/utils/ip_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/json_util.py` & `domain-admin-1.5.7/domain_admin/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/open_api/crtsh_api.py` & `domain-admin-1.5.7/domain_admin/utils/open_api/crtsh_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/open_api/ding_talk_api.py` & `domain-admin-1.5.7/domain_admin/utils/open_api/ding_talk_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/open_api/feishu_api.py` & `domain-admin-1.5.7/domain_admin/utils/open_api/feishu_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/open_api/work_weixin_api.py` & `domain-admin-1.5.7/domain_admin/utils/open_api/work_weixin_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/peewee_ext/model_util.py` & `domain-admin-1.5.7/domain_admin/utils/peewee_ext/model_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/secret_util.py` & `domain-admin-1.5.7/domain_admin/utils/secret_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/text_util.py` & `domain-admin-1.5.7/domain_admin/utils/text_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/time_util.py` & `domain-admin-1.5.7/domain_admin/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/whois_util/config.py` & `domain-admin-1.5.7/domain_admin/utils/whois_util/config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/whois_util/util.py` & `domain-admin-1.5.7/domain_admin/utils/whois_util/util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/whois_util/whois-servers.txt` & `domain-admin-1.5.7/domain_admin/utils/whois_util/whois-servers.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin/utils/whois_util/whois_util.py` & `domain-admin-1.5.7/domain_admin/utils/whois_util/whois_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/domain_admin.egg-info/PKG-INFO` & `domain-admin-1.5.7/domain_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.5.6
+Version: 1.5.7
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain,ssl,cert,web,monitor
 Platform: any
```

### Comparing `domain-admin-1.5.6/domain_admin.egg-info/SOURCES.txt` & `domain-admin-1.5.7/domain_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.6/setup.py` & `domain-admin-1.5.7/setup.py`

 * *Files identical despite different names*

