# Comparing `tmp/fullctl-1.4.0.tar.gz` & `tmp/fullctl-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullctl-1.4.0.tar", max compression
+gzip compressed data, was "fullctl-1.5.0.tar", max compression
```

## Comparing `fullctl-1.4.0.tar` & `fullctl-1.5.0.tar`

### file list

```diff
@@ -1,311 +1,317 @@
--rw-r--r--   0        0        0    11357 2021-04-22 13:27:52.952758 fullctl-1.4.0/LICENSE
--rw-r--r--   0        0        0     1203 2023-04-18 23:41:07.569197 fullctl-1.4.0/README.md
--rw-r--r--   0        0        0     2213 2023-06-30 20:48:24.070788 fullctl-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.4.0/src/fullctl/__init__.py
--rwxr-xr-x   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.4.0/src/fullctl/django/__init__.py
--rw-r--r--   0        0        0     5719 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/admin.py
--rw-r--r--   0        0        0      259 2021-10-21 03:49:59.920722 fullctl-1.4.0/src/fullctl/django/apps.py
--rw-r--r--   0        0        0     7188 2023-02-27 05:27:02.246818 fullctl-1.4.0/src/fullctl/django/auditlog.py
--rw-r--r--   0        0        0     4966 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/auth.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.4.0/src/fullctl/django/autocomplete/__init__.py
--rw-r--r--   0        0        0     1231 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/autocomplete/devicectl.py
--rw-r--r--   0        0        0      954 2023-02-27 05:27:02.247818 fullctl-1.4.0/src/fullctl/django/autocomplete/pdb.py
--rw-r--r--   0        0        0     2518 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/context.py
--rw-r--r--   0        0        0     3389 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/context_processors.py
--rw-r--r--   0        0        0     3102 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/decorators.py
--rw-r--r--   0        0        0      233 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/enum.py
--rw-r--r--   0        0        0      283 2022-10-14 13:57:25.205745 fullctl-1.4.0/src/fullctl/django/exceptions.py
--rw-r--r--   0        0        0      650 2022-10-14 13:57:25.205745 fullctl-1.4.0/src/fullctl/django/fields/__init__.py
--rw-r--r--   0        0        0     4351 2023-02-27 05:27:02.248818 fullctl-1.4.0/src/fullctl/django/fields/service_bridge/__init__.py
--rw-r--r--   0        0        0      317 2023-02-27 05:27:02.248818 fullctl-1.4.0/src/fullctl/django/fields/service_bridge/prefixctl.py
--rw-r--r--   0        0        0       79 2021-06-15 13:03:05.246145 fullctl-1.4.0/src/fullctl/django/forms.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.4.0/src/fullctl/django/inet/__init__.py
--rw-r--r--   0        0        0      325 2021-04-22 13:27:52.954758 fullctl-1.4.0/src/fullctl/django/inet/const.py
--rw-r--r--   0        0        0      186 2021-04-22 13:27:52.955758 fullctl-1.4.0/src/fullctl/django/inet/exceptions.py
--rw-r--r--   0        0        0      761 2021-06-15 13:03:05.246145 fullctl-1.4.0/src/fullctl/django/inet/fields.py
--rw-r--r--   0        0        0      519 2021-06-15 13:03:05.246145 fullctl-1.4.0/src/fullctl/django/inet/util.py
--rw-r--r--   0        0        0     3738 2021-06-15 13:03:05.246145 fullctl-1.4.0/src/fullctl/django/inet/validators.py
--rw-r--r--   0        0        0      307 2023-02-27 05:27:02.248818 fullctl-1.4.0/src/fullctl/django/mail.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.4.0/src/fullctl/django/management/__init__.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.4.0/src/fullctl/django/management/commands/__init__.py
--rw-r--r--   0        0        0     4128 2021-10-29 12:45:46.921418 fullctl-1.4.0/src/fullctl/django/management/commands/base.py
--rw-r--r--   0        0        0     1867 2023-02-27 05:27:02.248818 fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py
--rw-r--r--   0        0        0     4750 2023-02-27 05:27:02.249818 fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py
--rw-r--r--   0        0        0      620 2023-02-27 05:27:02.249818 fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_promote_user.py
--rw-r--r--   0        0        0      763 2023-02-27 05:27:02.249818 fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_work_task.py
--rw-r--r--   0        0        0     4373 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/middleware.py
--rw-r--r--   0        0        0     8661 2023-02-27 05:27:02.250818 fullctl-1.4.0/src/fullctl/django/migrations/0001_initial.py
--rw-r--r--   0        0        0      291 2023-02-27 05:27:02.250818 fullctl-1.4.0/src/fullctl/django/migrations/0002_delete_apikey.py
--rw-r--r--   0        0        0     2216 2023-02-27 05:27:02.250818 fullctl-1.4.0/src/fullctl/django/migrations/0003_auditlog.py
--rw-r--r--   0        0        0     1081 2023-02-27 05:27:02.250818 fullctl-1.4.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py
--rw-r--r--   0        0        0      625 2023-02-27 05:27:02.250818 fullctl-1.4.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py
--rw-r--r--   0        0        0     1374 2023-02-27 05:27:02.251818 fullctl-1.4.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py
--rw-r--r--   0        0        0      485 2023-02-27 05:27:02.251818 fullctl-1.4.0/src/fullctl/django/migrations/0007_auditlog_ip_address.py
--rw-r--r--   0        0        0     4435 2023-02-27 05:27:02.251818 fullctl-1.4.0/src/fullctl/django/migrations/0008_managementtask.py
--rw-r--r--   0        0        0     2341 2023-02-27 05:27:02.251818 fullctl-1.4.0/src/fullctl/django/migrations/0009_taskclaim.py
--rw-r--r--   0        0        0      557 2023-02-27 05:27:02.251818 fullctl-1.4.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py
--rw-r--r--   0        0        0      749 2023-02-27 05:27:02.252818 fullctl-1.4.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py
--rw-r--r--   0        0        0     5399 2023-02-27 05:27:02.252818 fullctl-1.4.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py
--rw-r--r--   0        0        0      723 2023-02-27 05:27:02.252818 fullctl-1.4.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py
--rw-r--r--   0        0        0      516 2023-02-27 05:27:02.252818 fullctl-1.4.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py
--rw-r--r--   0        0        0      625 2023-02-27 05:27:02.252818 fullctl-1.4.0/src/fullctl/django/migrations/0015_alter_task_parent.py
--rw-r--r--   0        0        0      414 2023-02-27 05:27:02.253818 fullctl-1.4.0/src/fullctl/django/migrations/0016_task_limit_id.py
--rw-r--r--   0        0        0      463 2023-02-27 05:27:02.253818 fullctl-1.4.0/src/fullctl/django/migrations/0017_alter_organizationuser_options.py
--rw-r--r--   0        0        0     4271 2023-02-27 05:27:02.253818 fullctl-1.4.0/src/fullctl/django/migrations/0018_task_schedule.py
--rw-r--r--   0        0        0      402 2023-02-27 05:27:02.253818 fullctl-1.4.0/src/fullctl/django/migrations/0019_default_org.py
--rw-r--r--   0        0        0      389 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0020_auditlog_action_length.py
--rw-r--r--   0        0        0     3330 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0021_servicebridgeaction.py
--rw-r--r--   0        0        0     1077 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py
--rw-r--r--   0        0        0     1050 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py
--rw-r--r--   0        0        0     2539 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py
--rw-r--r--   0        0        0      900 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py
--rw-r--r--   0        0        0      837 2023-02-27 05:27:02.255818 fullctl-1.4.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py
--rw-r--r--   0        0        0     4518 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/migrations/0027_request_response.py
--rw-r--r--   0        0        0      457 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/migrations/0028_request_identifier.py
--rw-r--r--   0        0        0      427 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/migrations/0029_response_content.py
--rw-r--r--   0        0        0      550 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/migrations/0030_alter_response_content.py
--rw-r--r--   0        0        0     2496 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.4.0/src/fullctl/django/migrations/__init__.py
--rw-r--r--   0        0        0      218 2021-10-21 03:49:59.989723 fullctl-1.4.0/src/fullctl/django/models/__init__.py
--rw-r--r--   0        0        0      150 2022-10-14 13:57:25.208745 fullctl-1.4.0/src/fullctl/django/models/abstract/__init__.py
--rw-r--r--   0        0        0     3282 2022-06-14 21:13:57.268730 fullctl-1.4.0/src/fullctl/django/models/abstract/alert.py
--rw-r--r--   0        0        0     3337 2022-10-14 13:57:25.209745 fullctl-1.4.0/src/fullctl/django/models/abstract/base.py
--rw-r--r--   0        0        0    14848 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/models/abstract/meta.py
--rw-r--r--   0        0        0     7822 2023-02-27 05:27:02.255818 fullctl-1.4.0/src/fullctl/django/models/abstract/service_bridge.py
--rw-r--r--   0        0        0     2682 2023-02-27 05:27:02.256818 fullctl-1.4.0/src/fullctl/django/models/abstract/template.py
--rw-r--r--   0        0        0      288 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/models/concrete/__init__.py
--rw-r--r--   0        0        0     7437 2023-02-27 05:27:02.256818 fullctl-1.4.0/src/fullctl/django/models/concrete/account.py
--rw-r--r--   0        0        0     1884 2023-02-27 05:27:02.256818 fullctl-1.4.0/src/fullctl/django/models/concrete/auditlog.py
--rw-r--r--   0        0        0     1808 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/models/concrete/meta.py
--rw-r--r--   0        0        0     7811 2023-02-27 05:27:02.257818 fullctl-1.4.0/src/fullctl/django/models/concrete/service_bridge.py
--rw-r--r--   0        0        0    16238 2023-04-15 16:24:16.031446 fullctl-1.4.0/src/fullctl/django/models/concrete/tasks.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.4.0/src/fullctl/django/rest/__init__.py
--rw-r--r--   0        0        0     8217 2023-02-27 05:27:02.257818 fullctl-1.4.0/src/fullctl/django/rest/api_schema.py
--rw-r--r--   0        0        0     1143 2021-10-29 12:45:46.966419 fullctl-1.4.0/src/fullctl/django/rest/authentication.py
--rw-r--r--   0        0        0     1831 2021-06-15 13:03:05.250145 fullctl-1.4.0/src/fullctl/django/rest/core.py
--rw-r--r--   0        0        0     8517 2023-02-27 05:27:02.258818 fullctl-1.4.0/src/fullctl/django/rest/decorators.py
--rw-r--r--   0        0        0      328 2023-02-27 05:27:02.258818 fullctl-1.4.0/src/fullctl/django/rest/fields.py
--rw-r--r--   0        0        0     1074 2021-10-21 03:50:00.023724 fullctl-1.4.0/src/fullctl/django/rest/filters.py
--rw-r--r--   0        0        0     1486 2022-10-14 13:57:25.257745 fullctl-1.4.0/src/fullctl/django/rest/mixins.py
--rw-r--r--   0        0        0     2148 2021-10-29 12:45:46.983419 fullctl-1.4.0/src/fullctl/django/rest/renderers.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.957758 fullctl-1.4.0/src/fullctl/django/rest/route/__init__.py
--rw-r--r--   0        0        0      352 2023-02-27 05:27:02.258818 fullctl-1.4.0/src/fullctl/django/rest/route/aaactl_sync.py
--rw-r--r--   0        0        0      298 2021-10-21 03:50:00.070725 fullctl-1.4.0/src/fullctl/django/rest/route/account.py
--rw-r--r--   0        0        0      426 2023-02-27 05:27:02.258818 fullctl-1.4.0/src/fullctl/django/rest/route/service_bridge.py
--rw-r--r--   0        0        0      342 2023-02-27 05:27:02.259818 fullctl-1.4.0/src/fullctl/django/rest/route/usage.py
--rw-r--r--   0        0        0     1558 2023-02-27 05:27:02.259818 fullctl-1.4.0/src/fullctl/django/rest/serializers/__init__.py
--rw-r--r--   0        0        0     2136 2023-04-15 16:24:16.031446 fullctl-1.4.0/src/fullctl/django/rest/serializers/aaactl_sync.py
--rw-r--r--   0        0        0     2523 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/rest/serializers/account.py
--rw-r--r--   0        0        0      518 2023-04-15 16:24:16.032446 fullctl-1.4.0/src/fullctl/django/rest/serializers/meta.py
--rw-r--r--   0        0        0      807 2022-10-14 13:57:25.258745 fullctl-1.4.0/src/fullctl/django/rest/serializers/org.py
--rw-r--r--   0        0        0      233 2023-02-27 05:27:02.260818 fullctl-1.4.0/src/fullctl/django/rest/serializers/service_bridge.py
--rw-r--r--   0        0        0      688 2022-10-14 13:57:25.258745 fullctl-1.4.0/src/fullctl/django/rest/serializers/template.py
--rw-r--r--   0        0        0      440 2023-02-27 05:27:02.260818 fullctl-1.4.0/src/fullctl/django/rest/serializers/usage.py
--rw-r--r--   0        0        0      395 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/rest/throttle.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.4.0/src/fullctl/django/rest/urls/__init__.py
--rw-r--r--   0        0        0      222 2021-10-21 03:50:00.135727 fullctl-1.4.0/src/fullctl/django/rest/urls/aaactl_sync.py
--rw-r--r--   0        0        0      210 2021-06-15 13:03:05.251145 fullctl-1.4.0/src/fullctl/django/rest/urls/account.py
--rw-r--r--   0        0        0      491 2021-10-29 12:45:46.983419 fullctl-1.4.0/src/fullctl/django/rest/urls/service_bridge.py
--rw-r--r--   0        0        0     2161 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/rest/urls/service_bridge_proxy.py
--rw-r--r--   0        0        0      204 2021-06-15 13:03:05.251145 fullctl-1.4.0/src/fullctl/django/rest/urls/usage.py
--rw-r--r--   0        0        0      419 2021-06-15 13:03:05.251145 fullctl-1.4.0/src/fullctl/django/rest/usage.py
--rw-r--r--   0        0        0        0 2021-06-15 13:03:05.251145 fullctl-1.4.0/src/fullctl/django/rest/views/__init__.py
--rw-r--r--   0        0        0     3258 2022-10-14 13:57:25.258745 fullctl-1.4.0/src/fullctl/django/rest/views/aaactl_sync.py
--rw-r--r--   0        0        0     2576 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/rest/views/account.py
--rw-r--r--   0        0        0     7159 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/rest/views/service_bridge.py
--rw-r--r--   0        0        0      994 2023-02-27 05:27:02.261818 fullctl-1.4.0/src/fullctl/django/rest/views/template.py
--rw-r--r--   0        0        0     1410 2023-02-27 05:27:02.261818 fullctl-1.4.0/src/fullctl/django/rest/views/usage.py
--rw-r--r--   0        0        0    16540 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/settings/__init__.py
--rw-r--r--   0        0        0     2655 2023-02-27 05:27:02.262818 fullctl-1.4.0/src/fullctl/django/settings/default.py
--rw-r--r--   0        0        0     1215 2023-02-27 05:27:02.262818 fullctl-1.4.0/src/fullctl/django/signals.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.4.0/src/fullctl/django/social/__init__.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.4.0/src/fullctl/django/social/backends/__init__.py
--rw-r--r--   0        0        0     1206 2021-06-15 13:03:05.252145 fullctl-1.4.0/src/fullctl/django/social/backends/peeringdb.py
--rw-r--r--   0        0        0     1589 2021-10-21 03:50:00.137727 fullctl-1.4.0/src/fullctl/django/social/backends/twentyc.py
--rw-r--r--   0        0        0      388 2021-06-15 13:03:05.252145 fullctl-1.4.0/src/fullctl/django/social/pipelines/__init__.py
--rw-r--r--   0        0        0     4237 2021-04-22 13:27:52.959758 fullctl-1.4.0/src/fullctl/django/static/common/20c/twentyc.core.min.js
--rw-r--r--   0        0        0    59951 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/static/common/20c/twentyc.rest.js
--rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.959758 fullctl-1.4.0/src/fullctl/django/static/common/20c-logo-filled.svg
--rw-r--r--   0        0        0    21299 2023-02-27 05:27:02.264818 fullctl-1.4.0/src/fullctl/django/static/common/app.css
--rw-r--r--   0        0        0    19449 2023-02-27 05:27:02.265818 fullctl-1.4.0/src/fullctl/django/static/common/app.js
--rwxr-xr-x   0        0        0   372526 2021-10-29 12:45:47.007420 fullctl-1.4.0/src/fullctl/django/static/common/favicon.ico
--rw-r--r--   0        0        0     3380 2021-04-22 13:27:52.960758 fullctl-1.4.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg
--rw-r--r--   0        0        0     3657 2021-04-22 13:27:52.960758 fullctl-1.4.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg
--rw-r--r--   0        0        0     3430 2021-04-22 13:27:52.960758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/add.svg
--rw-r--r--   0        0        0     3819 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/alerts.svg
--rw-r--r--   0        0        0     2838 2022-06-14 21:13:57.362731 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/api.svg
--rw-r--r--   0        0        0     1303 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg
--rw-r--r--   0        0        0     2681 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/delete.svg
--rw-r--r--   0        0        0     5490 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/edit.svg
--rwxr-xr-x   0        0        0     1172 2021-10-29 12:45:47.024420 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/launch.svg
--rw-r--r--   0        0        0     1601 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/light-mode.svg
--rw-r--r--   0        0        0     3357 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/list.svg
--rwxr-xr-x   0        0        0     1721 2022-06-14 21:13:57.362731 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/location.svg
--rw-r--r--   0        0        0     2617 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/logout.svg
--rwxr-xr-x   0        0        0      726 2021-10-29 12:45:47.026420 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/mail.svg
--rw-r--r--   0        0        0     2761 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/org.svg
--rw-r--r--   0        0        0     1597 2022-06-14 21:13:57.599734 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/refresh.svg
--rw-r--r--   0        0        0     1515 2022-06-14 21:13:57.623735 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/report.svg
--rw-r--r--   0        0        0     8263 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/settings.svg
--rw-r--r--   0        0        0     4138 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/user.svg
--rwxr-xr-x   0        0        0     2782 2021-10-29 12:45:47.035421 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/view.svg
--rw-r--r--   0        0        0     3689 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg
--rw-r--r--   0        0        0      169 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/md-add.svg
--rw-r--r--   0        0        0      275 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/md-create.svg
--rw-r--r--   0        0        0      272 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/md-list-box.svg
--rw-r--r--   0        0        0      240 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/md-trash.svg
--rw-r--r--   0        0        0     5957 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg
--rw-r--r--   0        0        0      954 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg
--rw-r--r--   0        0        0      818 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/ui-close.svg
--rw-r--r--   0        0        0     4482 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/static/common/logos/aaactl-dark.svg
--rw-r--r--   0        0        0     4484 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/static/common/logos/aaactl-light.svg
--rw-r--r--   0        0        0     4512 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/static/common/logos/aclctl-dark.svg
--rw-r--r--   0        0        0     2625 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/aclctl-light.svg
--rwxr-xr-x   0        0        0     3333 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/auditctl-dark.svg
--rwxr-xr-x   0        0        0     3333 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/auditctl-light.svg
--rwxr-xr-x   0        0        0    36084 2023-04-15 16:24:16.033446 fullctl-1.4.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png
--rwxr-xr-x   0        0        0    36307 2023-04-15 16:24:16.033446 fullctl-1.4.0/src/fullctl/django/static/common/logos/ctl-mark-light.png
--rwxr-xr-x   0        0        0     4680 2022-10-14 13:57:25.295745 fullctl-1.4.0/src/fullctl/django/static/common/logos/devicectl-dark.svg
--rw-r--r--   0        0        0     4682 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/devicectl-light.svg
--rwxr-xr-x   0        0        0     2579 2021-10-29 12:45:47.035421 fullctl-1.4.0/src/fullctl/django/static/common/logos/ixctl-dark.svg
--rw-r--r--   0        0        0     2581 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/ixctl-light.svg
--rwxr-xr-x   0        0        0     3857 2021-10-29 12:45:47.035421 fullctl-1.4.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg
--rw-r--r--   0        0        0     3859 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/pdbctl-light.svg
--rwxr-xr-x   0        0        0     4166 2021-10-29 12:45:47.036420 fullctl-1.4.0/src/fullctl/django/static/common/logos/peerctl-dark.svg
--rw-r--r--   0        0        0     4168 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/peerctl-light.svg
--rwxr-xr-x   0        0        0     4336 2022-06-14 21:13:57.623735 fullctl-1.4.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg
--rw-r--r--   0        0        0     4338 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/prefixctl-light.svg
--rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/oauth/20c.svg
--rw-r--r--   0        0        0      689 2021-04-22 13:27:52.963758 fullctl-1.4.0/src/fullctl/django/static/common/oauth/google.svg
--rw-r--r--   0        0        0     5222 2023-04-15 16:24:16.033446 fullctl-1.4.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png
--rw-r--r--   0        0        0     9186 2021-04-22 13:27:52.963758 fullctl-1.4.0/src/fullctl/django/static/common/oauth/peeringdb.png
--rw-r--r--   0        0        0     4323 2021-10-21 03:50:00.180728 fullctl-1.4.0/src/fullctl/django/static/common/service_bridge.js
--rw-r--r--   0        0        0    11545 2023-02-27 05:27:02.266818 fullctl-1.4.0/src/fullctl/django/static/common/themes/dark.css
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.963758 fullctl-1.4.0/src/fullctl/django/static/common/themes/light.css
--rw-r--r--   0        0        0    31266 2023-06-30 20:48:24.072788 fullctl-1.4.0/src/fullctl/django/static/common/v2/app.css
--rw-r--r--   0        0        0    50966 2023-06-30 20:48:24.072788 fullctl-1.4.0/src/fullctl/django/static/common/v2/app.js
--rw-r--r--   0        0        0     9584 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/static/common/v2/graph.js
--rw-r--r--   0        0        0      644 2023-02-27 05:27:02.268818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/add.svg
--rw-r--r--   0        0        0     4812 2023-02-27 05:27:02.268818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/api.svg
--rw-r--r--   0        0        0      352 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/arrow-clockwise.svg
--rw-r--r--   0        0        0      232 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/arrow.svg
--rw-r--r--   0        0        0      532 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg
--rw-r--r--   0        0        0      423 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/cancel.svg
--rw-r--r--   0        0        0      274 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/close.svg
--rw-r--r--   0        0        0     1229 2023-04-15 16:24:16.034446 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/database.svg
--rw-r--r--   0        0        0      427 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/download.svg
--rw-r--r--   0        0        0      438 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/envelope.svg
--rw-r--r--   0        0        0      569 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/eye.svg
--rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/file-earmark-text.svg
--rw-r--r--   0        0        0      404 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/funnel.svg
--rw-r--r--   0        0        0     1530 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/gear.svg
--rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/geo-alt.svg
--rw-r--r--   0        0        0     1975 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/help.svg
--rw-r--r--   0        0        0      582 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list/delete.svg
--rw-r--r--   0        0        0      438 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list/edit.svg
--rw-r--r--   0        0        0      818 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list/options.svg
--rw-r--r--   0        0        0      447 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list-ul.svg
--rw-r--r--   0        0        0      553 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/logout.svg
--rw-r--r--   0        0        0      749 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/org.svg
--rw-r--r--   0        0        0      331 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/search.svg
--rw-r--r--   0        0        0     1465 2023-02-27 05:27:02.272818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg
--rw-r--r--   0        0        0      298 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/triangle-fill.svg
--rw-r--r--   0        0        0      465 2023-02-27 05:27:02.272818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/ui-caret/dbl-select.svg
--rw-r--r--   0        0        0      190 2023-02-27 05:27:02.272818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/ui-caret/down.svg
--rw-r--r--   0        0        0     4138 2023-02-27 05:27:02.272818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/user.svg
--rw-r--r--   0        0        0     3986 2023-02-27 05:27:02.272818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/view-settings.svg
--rw-r--r--   0        0        0    61189 2023-02-27 05:27:02.273818 fullctl-1.4.0/src/fullctl/django/static/common/v2/imgs/help.png
--rw-r--r--   0        0        0   426086 2023-04-15 16:24:16.037446 fullctl-1.4.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png
--rw-r--r--   0        0        0    18080 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/static/common/v2/themes/dark.css
--rw-r--r--   0        0        0        0 2023-02-27 05:27:02.273818 fullctl-1.4.0/src/fullctl/django/static/common/v2/themes/light.css
--rw-r--r--   0        0        0      921 2023-02-27 05:27:02.274818 fullctl-1.4.0/src/fullctl/django/tasks/__init__.py
--rw-r--r--   0        0        0      740 2021-10-21 03:50:00.186728 fullctl-1.4.0/src/fullctl/django/tasks/celery.py
--rw-r--r--   0        0        0     2385 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/tasks/orm.py
--rw-r--r--   0        0        0     2232 2023-04-22 03:42:18.733445 fullctl-1.4.0/src/fullctl/django/tasks/qualifiers.py
--rw-r--r--   0        0        0      374 2023-02-27 05:27:02.274818 fullctl-1.4.0/src/fullctl/django/tasks/util.py
--rw-r--r--   0        0        0      658 2022-10-14 13:57:25.296744 fullctl-1.4.0/src/fullctl/django/templates/common/apidocs/redoc.html
--rw-r--r--   0        0        0      856 2022-10-14 13:57:25.296744 fullctl-1.4.0/src/fullctl/django/templates/common/apidocs/swagger.html
--rw-r--r--   0        0        0     8871 2022-10-14 13:57:25.296744 fullctl-1.4.0/src/fullctl/django/templates/common/app/base.html
--rw-r--r--   0        0        0      211 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/checkbox.html
--rw-r--r--   0        0        0     1935 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html
--rw-r--r--   0        0        0      726 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/import-org.html
--rw-r--r--   0        0        0      494 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/invite.html
--rw-r--r--   0        0        0      792 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/org-create.html
--rw-r--r--   0        0        0     3826 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/org-prefs.html
--rw-r--r--   0        0        0      355 2021-06-15 13:03:05.254145 fullctl-1.4.0/src/fullctl/django/templates/common/app/index.html
--rw-r--r--   0        0        0     1974 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/manage/permissions.html
--rw-r--r--   0        0        0     4752 2022-10-14 13:57:25.297744 fullctl-1.4.0/src/fullctl/django/templates/common/app/modal.html
--rw-r--r--   0        0        0     2668 2021-04-22 13:27:52.965758 fullctl-1.4.0/src/fullctl/django/templates/common/app/navbar.html
--rw-r--r--   0        0        0      371 2023-02-27 05:27:02.275818 fullctl-1.4.0/src/fullctl/django/templates/common/app/templates.html
--rw-r--r--   0        0        0     3101 2022-10-14 13:57:25.297744 fullctl-1.4.0/src/fullctl/django/templates/common/auth/login.html
--rw-r--r--   0        0        0      880 2021-04-22 13:27:52.965758 fullctl-1.4.0/src/fullctl/django/templates/common/auth/oauth-badge.html
--rw-r--r--   0        0        0     1110 2021-04-22 13:27:52.965758 fullctl-1.4.0/src/fullctl/django/templates/common/auth/oauth.html
--rw-r--r--   0        0        0     1996 2023-04-15 16:24:16.038446 fullctl-1.4.0/src/fullctl/django/templates/common/base.html
--rw-r--r--   0        0        0      333 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/400.html
--rw-r--r--   0        0        0      367 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/401.html
--rw-r--r--   0        0        0      375 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/403.html
--rw-r--r--   0        0        0      377 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/404.html
--rw-r--r--   0        0        0      456 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/500.html
--rw-r--r--   0        0        0      597 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/templates/common/errors/base.html
--rw-r--r--   0        0        0      351 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/details.html
--rw-r--r--   0        0        0     1229 2022-06-14 21:13:57.992740 fullctl-1.4.0/src/fullctl/django/templates/common/snippets.html
--rw-r--r--   0        0        0      234 2021-04-22 13:27:52.965758 fullctl-1.4.0/src/fullctl/django/templates/common/tool_base.html
--rw-r--r--   0        0        0      658 2023-02-27 05:27:02.276818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html
--rw-r--r--   0        0        0      856 2023-02-27 05:27:02.276818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html
--rw-r--r--   0        0        0    12350 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/base.html
--rw-r--r--   0        0        0      211 2023-02-27 05:27:02.277818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/checkbox.html
--rw-r--r--   0        0        0     2092 2023-04-15 17:32:55.632524 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html
--rw-r--r--   0        0        0      357 2023-02-27 05:27:02.277818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/delete_selected.html
--rw-r--r--   0        0        0     1945 2023-04-22 03:42:18.733445 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/footer.html
--rw-r--r--   0        0        0     1935 2023-02-27 05:27:02.278818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html
--rw-r--r--   0        0        0      430 2023-04-15 17:32:55.632524 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/feature-request.html
--rw-r--r--   0        0        0      726 2023-02-27 05:27:02.278818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html
--rw-r--r--   0        0        0      494 2023-02-27 05:27:02.278818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/invite.html
--rw-r--r--   0        0        0      792 2023-02-27 05:27:02.278818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html
--rw-r--r--   0        0        0     3826 2023-02-27 05:27:02.278818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html
--rw-r--r--   0        0        0      358 2023-02-27 05:27:02.279818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/index.html
--rw-r--r--   0        0        0     1974 2023-02-27 05:27:02.279818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html
--rw-r--r--   0        0        0     6317 2023-04-15 16:24:16.038446 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/modal.html
--rw-r--r--   0        0        0     2668 2023-02-27 05:27:02.280818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/navbar.html
--rw-r--r--   0        0        0      413 2023-02-27 05:27:02.280818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/templates.html
--rw-r--r--   0        0        0     3048 2023-02-27 05:27:02.280818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/login.html
--rw-r--r--   0        0        0     1109 2023-04-15 16:24:16.038446 fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html
--rw-r--r--   0        0        0     1339 2023-04-15 16:24:16.038446 fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/oauth.html
--rw-r--r--   0        0        0     1977 2023-04-15 16:24:16.038446 fullctl-1.4.0/src/fullctl/django/templates/common/v2/base.html
--rw-r--r--   0        0        0      339 2023-02-27 05:27:02.281818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/400.html
--rw-r--r--   0        0        0      373 2023-02-27 05:27:02.281818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/401.html
--rw-r--r--   0        0        0      381 2023-02-27 05:27:02.281818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/403.html
--rw-r--r--   0        0        0      383 2023-02-27 05:27:02.281818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/404.html
--rw-r--r--   0        0        0      462 2023-02-27 05:27:02.281818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/500.html
--rw-r--r--   0        0        0      568 2023-02-27 05:27:02.282818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/base.html
--rw-r--r--   0        0        0      351 2023-02-27 05:27:02.282818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/details.html
--rw-r--r--   0        0        0     1661 2023-04-15 16:24:16.039446 fullctl-1.4.0/src/fullctl/django/templates/common/v2/snippets.html
--rw-r--r--   0        0        0      234 2023-02-27 05:27:02.282818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/tool_base.html
--rw-r--r--   0        0        0      249 2023-02-27 05:27:02.282818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/tool_base_sidebar.html
--rw-r--r--   0        0        0        0 2022-06-14 21:13:57.992740 fullctl-1.4.0/src/fullctl/django/templatetags/__init__.py
--rw-r--r--   0        0        0     3398 2023-04-15 16:24:16.039446 fullctl-1.4.0/src/fullctl/django/templatetags/fullctl_util.py
--rw-r--r--   0        0        0     3152 2023-02-27 05:27:02.283818 fullctl-1.4.0/src/fullctl/django/testutil.py
--rw-r--r--   0        0        0     3690 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/urls.py
--rw-r--r--   0        0        0     1171 2023-02-27 05:27:02.283818 fullctl-1.4.0/src/fullctl/django/util.py
--rw-r--r--   0        0        0     1193 2022-10-14 13:57:25.299744 fullctl-1.4.0/src/fullctl/django/validators.py
--rw-r--r--   0        0        0     2885 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/django/views/__init__.py
--rw-r--r--   0        0        0      199 2022-10-14 13:57:25.300744 fullctl-1.4.0/src/fullctl/django/views/api_schema.py
--rw-r--r--   0        0        0      927 2023-04-15 17:32:55.633525 fullctl-1.4.0/src/fullctl/django/views/template.py
--rw-r--r--   0        0        0        0 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/graph/mrtg/__init__.py
--rw-r--r--   0        0        0     1420 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/graph/mrtg/mock.py
--rw-r--r--   0        0        0     7664 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/graph/mrtg/rrd.py
--rw-r--r--   0        0        0        0 2021-06-15 13:03:05.256145 fullctl-1.4.0/src/fullctl/service_bridge/__init__.py
--rw-r--r--   0        0        0     2706 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/service_bridge/aaactl.py
--rw-r--r--   0        0        0      940 2023-04-22 03:42:18.733445 fullctl-1.4.0/src/fullctl/service_bridge/auditctl.py
--rw-r--r--   0        0        0     8510 2023-04-15 16:24:16.052446 fullctl-1.4.0/src/fullctl/service_bridge/client.py
--rw-r--r--   0        0        0     3419 2023-02-27 05:27:02.285818 fullctl-1.4.0/src/fullctl/service_bridge/data.py
--rw-r--r--   0        0        0     3239 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/service_bridge/devicectl.py
--rw-r--r--   0        0        0     2577 2023-04-15 16:24:16.053446 fullctl-1.4.0/src/fullctl/service_bridge/ixctl.py
--rw-r--r--   0        0        0     2651 2023-02-27 05:27:02.286818 fullctl-1.4.0/src/fullctl/service_bridge/nautobot.py
--rw-r--r--   0        0        0     1699 2023-04-15 16:24:16.054446 fullctl-1.4.0/src/fullctl/service_bridge/pdbctl.py
--rw-r--r--   0        0        0     1037 2023-04-15 16:24:16.063447 fullctl-1.4.0/src/fullctl/service_bridge/peerctl.py
--rw-r--r--   0        0        0     1076 2023-04-15 16:24:16.097447 fullctl-1.4.0/src/fullctl/service_bridge/prefixctl.py
--rw-r--r--   0        0        0     6952 2023-04-15 16:24:16.097447 fullctl-1.4.0/src/fullctl/service_bridge/sot.py
--rw-r--r--   0        0        0      323 2022-10-14 13:57:25.408743 fullctl-1.4.0/src/fullctl/utils/__init__.py
--rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 fullctl-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-10-06 05:10:14.129326 fullctl-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1203 2023-07-24 02:51:17.174429 fullctl-1.5.0/README.md
+-rw-r--r--   0        0        0     2304 2023-07-24 03:03:46.386276 fullctl-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.131326 fullctl-1.5.0/src/fullctl/__init__.py
+-rwxr-xr-x   0        0        0        0 2021-10-06 05:10:14.131326 fullctl-1.5.0/src/fullctl/django/__init__.py
+-rw-r--r--   0        0        0     6909 2023-07-24 03:03:46.386276 fullctl-1.5.0/src/fullctl/django/admin.py
+-rw-r--r--   0        0        0      259 2021-10-06 05:10:14.132326 fullctl-1.5.0/src/fullctl/django/apps.py
+-rw-r--r--   0        0        0     7188 2023-07-24 02:51:17.181429 fullctl-1.5.0/src/fullctl/django/auditlog.py
+-rw-r--r--   0        0        0     4966 2023-07-24 02:51:17.182429 fullctl-1.5.0/src/fullctl/django/auth.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.132326 fullctl-1.5.0/src/fullctl/django/autocomplete/__init__.py
+-rw-r--r--   0        0        0     1231 2023-07-24 02:51:17.198429 fullctl-1.5.0/src/fullctl/django/autocomplete/devicectl.py
+-rw-r--r--   0        0        0      954 2023-07-24 02:51:17.200429 fullctl-1.5.0/src/fullctl/django/autocomplete/pdb.py
+-rw-r--r--   0        0        0     2518 2023-07-24 02:51:17.202429 fullctl-1.5.0/src/fullctl/django/context.py
+-rw-r--r--   0        0        0     3389 2023-07-24 02:51:17.202429 fullctl-1.5.0/src/fullctl/django/context_processors.py
+-rw-r--r--   0        0        0     3102 2023-07-24 02:51:17.203429 fullctl-1.5.0/src/fullctl/django/decorators.py
+-rw-r--r--   0        0        0      233 2023-07-24 02:51:17.203429 fullctl-1.5.0/src/fullctl/django/enum.py
+-rw-r--r--   0        0        0      283 2023-07-24 02:51:17.204429 fullctl-1.5.0/src/fullctl/django/exceptions.py
+-rw-r--r--   0        0        0      650 2023-07-24 02:51:17.204429 fullctl-1.5.0/src/fullctl/django/fields/__init__.py
+-rw-r--r--   0        0        0     4351 2023-07-24 02:51:17.204429 fullctl-1.5.0/src/fullctl/django/fields/service_bridge/__init__.py
+-rw-r--r--   0        0        0      317 2023-07-24 02:51:17.205429 fullctl-1.5.0/src/fullctl/django/fields/service_bridge/prefixctl.py
+-rw-r--r--   0        0        0       79 2021-10-06 05:10:14.133326 fullctl-1.5.0/src/fullctl/django/forms.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.133326 fullctl-1.5.0/src/fullctl/django/inet/__init__.py
+-rw-r--r--   0        0        0      325 2021-10-06 05:10:14.133326 fullctl-1.5.0/src/fullctl/django/inet/const.py
+-rw-r--r--   0        0        0      186 2021-10-06 05:10:14.133326 fullctl-1.5.0/src/fullctl/django/inet/exceptions.py
+-rw-r--r--   0        0        0      761 2021-10-06 05:10:14.133326 fullctl-1.5.0/src/fullctl/django/inet/fields.py
+-rw-r--r--   0        0        0      519 2021-10-06 05:10:14.133326 fullctl-1.5.0/src/fullctl/django/inet/util.py
+-rw-r--r--   0        0        0     3738 2021-10-06 05:10:14.133326 fullctl-1.5.0/src/fullctl/django/inet/validators.py
+-rw-r--r--   0        0        0      307 2023-07-24 02:51:17.205429 fullctl-1.5.0/src/fullctl/django/mail.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.134326 fullctl-1.5.0/src/fullctl/django/management/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.134326 fullctl-1.5.0/src/fullctl/django/management/commands/__init__.py
+-rw-r--r--   0        0        0     4128 2023-07-24 02:51:17.205429 fullctl-1.5.0/src/fullctl/django/management/commands/base.py
+-rw-r--r--   0        0        0     1867 2023-07-24 02:51:17.206429 fullctl-1.5.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py
+-rw-r--r--   0        0        0     4750 2023-07-24 02:51:17.206429 fullctl-1.5.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py
+-rw-r--r--   0        0        0      620 2023-07-24 02:51:17.206429 fullctl-1.5.0/src/fullctl/django/management/commands/fullctl_promote_user.py
+-rw-r--r--   0        0        0      763 2023-07-24 02:51:17.207429 fullctl-1.5.0/src/fullctl/django/management/commands/fullctl_work_task.py
+-rw-r--r--   0        0        0     4373 2023-07-24 02:51:17.207429 fullctl-1.5.0/src/fullctl/django/middleware.py
+-rw-r--r--   0        0        0     8661 2023-07-24 02:51:17.207429 fullctl-1.5.0/src/fullctl/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0      291 2023-07-24 02:51:17.208429 fullctl-1.5.0/src/fullctl/django/migrations/0002_delete_apikey.py
+-rw-r--r--   0        0        0     2216 2023-07-24 02:51:17.208429 fullctl-1.5.0/src/fullctl/django/migrations/0003_auditlog.py
+-rw-r--r--   0        0        0     1081 2023-07-24 02:51:17.208429 fullctl-1.5.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py
+-rw-r--r--   0        0        0      625 2023-07-24 02:51:17.209429 fullctl-1.5.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py
+-rw-r--r--   0        0        0     1374 2023-07-24 02:51:17.209429 fullctl-1.5.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py
+-rw-r--r--   0        0        0      485 2023-07-24 02:51:17.209429 fullctl-1.5.0/src/fullctl/django/migrations/0007_auditlog_ip_address.py
+-rw-r--r--   0        0        0     4435 2023-07-24 02:51:17.209429 fullctl-1.5.0/src/fullctl/django/migrations/0008_managementtask.py
+-rw-r--r--   0        0        0     2341 2023-07-24 02:51:17.210429 fullctl-1.5.0/src/fullctl/django/migrations/0009_taskclaim.py
+-rw-r--r--   0        0        0      557 2023-07-24 02:51:17.210429 fullctl-1.5.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py
+-rw-r--r--   0        0        0      749 2023-07-24 02:51:17.210429 fullctl-1.5.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py
+-rw-r--r--   0        0        0     5399 2023-07-24 02:51:17.210429 fullctl-1.5.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py
+-rw-r--r--   0        0        0      723 2023-07-24 02:51:17.211429 fullctl-1.5.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py
+-rw-r--r--   0        0        0      516 2023-07-24 02:51:17.211429 fullctl-1.5.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py
+-rw-r--r--   0        0        0      625 2023-07-24 02:51:17.211429 fullctl-1.5.0/src/fullctl/django/migrations/0015_alter_task_parent.py
+-rw-r--r--   0        0        0      414 2023-07-24 02:51:17.211429 fullctl-1.5.0/src/fullctl/django/migrations/0016_task_limit_id.py
+-rw-r--r--   0        0        0      463 2023-07-24 02:51:17.212429 fullctl-1.5.0/src/fullctl/django/migrations/0017_alter_organizationuser_options.py
+-rw-r--r--   0        0        0     4271 2023-07-24 02:51:17.212429 fullctl-1.5.0/src/fullctl/django/migrations/0018_task_schedule.py
+-rw-r--r--   0        0        0      402 2023-07-24 02:51:17.212429 fullctl-1.5.0/src/fullctl/django/migrations/0019_default_org.py
+-rw-r--r--   0        0        0      389 2023-07-24 02:51:17.212429 fullctl-1.5.0/src/fullctl/django/migrations/0020_auditlog_action_length.py
+-rw-r--r--   0        0        0     3330 2023-07-24 02:51:17.212429 fullctl-1.5.0/src/fullctl/django/migrations/0021_servicebridgeaction.py
+-rw-r--r--   0        0        0     1077 2023-07-24 02:51:17.213429 fullctl-1.5.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py
+-rw-r--r--   0        0        0     1050 2023-07-24 02:51:17.213429 fullctl-1.5.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py
+-rw-r--r--   0        0        0     2539 2023-07-24 02:51:17.213429 fullctl-1.5.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py
+-rw-r--r--   0        0        0      900 2023-07-24 02:51:17.213429 fullctl-1.5.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py
+-rw-r--r--   0        0        0      837 2023-07-24 02:51:17.213429 fullctl-1.5.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py
+-rw-r--r--   0        0        0     4518 2023-07-24 02:51:17.213429 fullctl-1.5.0/src/fullctl/django/migrations/0027_request_response.py
+-rw-r--r--   0        0        0      457 2023-07-24 02:51:17.214429 fullctl-1.5.0/src/fullctl/django/migrations/0028_request_identifier.py
+-rw-r--r--   0        0        0      427 2023-07-24 02:51:17.214429 fullctl-1.5.0/src/fullctl/django/migrations/0029_response_content.py
+-rw-r--r--   0        0        0      550 2023-07-24 02:51:17.214429 fullctl-1.5.0/src/fullctl/django/migrations/0030_alter_response_content.py
+-rw-r--r--   0        0        0     2496 2023-07-24 02:51:17.214429 fullctl-1.5.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py
+-rw-r--r--   0        0        0     2363 2023-07-24 03:03:46.387276 fullctl-1.5.0/src/fullctl/django/migrations/0032_auto_20230719_1049.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.137327 fullctl-1.5.0/src/fullctl/django/migrations/__init__.py
+-rw-r--r--   0        0        0      218 2021-10-06 05:10:14.137327 fullctl-1.5.0/src/fullctl/django/models/__init__.py
+-rw-r--r--   0        0        0      150 2023-07-24 02:51:17.215429 fullctl-1.5.0/src/fullctl/django/models/abstract/__init__.py
+-rw-r--r--   0        0        0     3282 2023-07-24 02:51:17.215429 fullctl-1.5.0/src/fullctl/django/models/abstract/alert.py
+-rw-r--r--   0        0        0     3337 2023-07-24 02:51:17.215429 fullctl-1.5.0/src/fullctl/django/models/abstract/base.py
+-rw-r--r--   0        0        0      445 2023-07-24 03:03:46.387276 fullctl-1.5.0/src/fullctl/django/models/abstract/file.py
+-rw-r--r--   0        0        0    14983 2023-07-24 03:03:46.388276 fullctl-1.5.0/src/fullctl/django/models/abstract/meta.py
+-rw-r--r--   0        0        0     7820 2023-07-24 03:03:46.389276 fullctl-1.5.0/src/fullctl/django/models/abstract/service_bridge.py
+-rw-r--r--   0        0        0     2682 2023-07-24 02:51:17.218429 fullctl-1.5.0/src/fullctl/django/models/abstract/template.py
+-rw-r--r--   0        0        0      358 2023-07-24 03:03:46.389276 fullctl-1.5.0/src/fullctl/django/models/concrete/__init__.py
+-rw-r--r--   0        0        0     7437 2023-07-24 02:51:17.219429 fullctl-1.5.0/src/fullctl/django/models/concrete/account.py
+-rw-r--r--   0        0        0     1884 2023-07-24 02:51:17.219429 fullctl-1.5.0/src/fullctl/django/models/concrete/auditlog.py
+-rw-r--r--   0        0        0      695 2023-07-24 03:03:46.390276 fullctl-1.5.0/src/fullctl/django/models/concrete/file.py
+-rw-r--r--   0        0        0     1808 2023-07-24 02:51:17.220429 fullctl-1.5.0/src/fullctl/django/models/concrete/meta.py
+-rw-r--r--   0        0        0     7811 2023-07-24 02:51:17.220429 fullctl-1.5.0/src/fullctl/django/models/concrete/service_bridge.py
+-rw-r--r--   0        0        0    16238 2023-07-24 02:51:17.221429 fullctl-1.5.0/src/fullctl/django/models/concrete/tasks.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.138327 fullctl-1.5.0/src/fullctl/django/rest/__init__.py
+-rw-r--r--   0        0        0     8217 2023-07-24 02:51:17.221429 fullctl-1.5.0/src/fullctl/django/rest/api_schema.py
+-rw-r--r--   0        0        0     1143 2023-07-24 02:51:17.221429 fullctl-1.5.0/src/fullctl/django/rest/authentication.py
+-rw-r--r--   0        0        0     1831 2021-10-06 05:10:14.139326 fullctl-1.5.0/src/fullctl/django/rest/core.py
+-rw-r--r--   0        0        0     8517 2023-07-24 02:51:17.222429 fullctl-1.5.0/src/fullctl/django/rest/decorators.py
+-rw-r--r--   0        0        0      328 2023-07-24 02:51:17.222429 fullctl-1.5.0/src/fullctl/django/rest/fields.py
+-rw-r--r--   0        0        0     1074 2021-10-06 05:10:14.139326 fullctl-1.5.0/src/fullctl/django/rest/filters.py
+-rw-r--r--   0        0        0     1486 2023-07-24 02:51:17.222429 fullctl-1.5.0/src/fullctl/django/rest/mixins.py
+-rw-r--r--   0        0        0     2148 2023-07-24 02:51:17.223429 fullctl-1.5.0/src/fullctl/django/rest/renderers.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.139326 fullctl-1.5.0/src/fullctl/django/rest/route/__init__.py
+-rw-r--r--   0        0        0      352 2023-07-24 02:51:17.223429 fullctl-1.5.0/src/fullctl/django/rest/route/aaactl_sync.py
+-rw-r--r--   0        0        0      298 2021-10-06 05:10:14.140327 fullctl-1.5.0/src/fullctl/django/rest/route/account.py
+-rw-r--r--   0        0        0      426 2023-07-24 02:51:17.223429 fullctl-1.5.0/src/fullctl/django/rest/route/service_bridge.py
+-rw-r--r--   0        0        0      342 2023-07-24 02:51:17.223429 fullctl-1.5.0/src/fullctl/django/rest/route/usage.py
+-rw-r--r--   0        0        0     1558 2023-07-24 02:51:17.224429 fullctl-1.5.0/src/fullctl/django/rest/serializers/__init__.py
+-rw-r--r--   0        0        0     3175 2023-07-24 03:03:46.390276 fullctl-1.5.0/src/fullctl/django/rest/serializers/aaactl_sync.py
+-rw-r--r--   0        0        0     2523 2023-07-24 02:51:17.225429 fullctl-1.5.0/src/fullctl/django/rest/serializers/account.py
+-rw-r--r--   0        0        0      518 2023-07-24 02:51:17.242429 fullctl-1.5.0/src/fullctl/django/rest/serializers/meta.py
+-rw-r--r--   0        0        0      807 2023-07-24 02:51:17.242429 fullctl-1.5.0/src/fullctl/django/rest/serializers/org.py
+-rw-r--r--   0        0        0      233 2023-07-24 02:51:17.242429 fullctl-1.5.0/src/fullctl/django/rest/serializers/service_bridge.py
+-rw-r--r--   0        0        0      688 2023-07-24 02:51:17.243429 fullctl-1.5.0/src/fullctl/django/rest/serializers/template.py
+-rw-r--r--   0        0        0      440 2023-07-24 02:51:17.243429 fullctl-1.5.0/src/fullctl/django/rest/serializers/usage.py
+-rw-r--r--   0        0        0      395 2023-07-24 02:51:17.243429 fullctl-1.5.0/src/fullctl/django/rest/throttle.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.140327 fullctl-1.5.0/src/fullctl/django/rest/urls/__init__.py
+-rw-r--r--   0        0        0      222 2021-10-06 05:10:14.141327 fullctl-1.5.0/src/fullctl/django/rest/urls/aaactl_sync.py
+-rw-r--r--   0        0        0      210 2021-10-06 05:10:14.141327 fullctl-1.5.0/src/fullctl/django/rest/urls/account.py
+-rw-r--r--   0        0        0      491 2023-07-24 02:51:17.243429 fullctl-1.5.0/src/fullctl/django/rest/urls/service_bridge.py
+-rw-r--r--   0        0        0     2161 2023-07-24 02:51:17.245429 fullctl-1.5.0/src/fullctl/django/rest/urls/service_bridge_proxy.py
+-rw-r--r--   0        0        0      204 2021-10-06 05:10:14.141327 fullctl-1.5.0/src/fullctl/django/rest/urls/usage.py
+-rw-r--r--   0        0        0      419 2021-10-06 05:10:14.141327 fullctl-1.5.0/src/fullctl/django/rest/usage.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.141327 fullctl-1.5.0/src/fullctl/django/rest/views/__init__.py
+-rw-r--r--   0        0        0     3704 2023-07-24 03:03:46.391276 fullctl-1.5.0/src/fullctl/django/rest/views/aaactl_sync.py
+-rw-r--r--   0        0        0     2576 2023-07-24 02:51:17.247429 fullctl-1.5.0/src/fullctl/django/rest/views/account.py
+-rw-r--r--   0        0        0     7159 2023-07-24 02:51:17.247429 fullctl-1.5.0/src/fullctl/django/rest/views/service_bridge.py
+-rw-r--r--   0        0        0      994 2023-07-24 02:51:17.248429 fullctl-1.5.0/src/fullctl/django/rest/views/template.py
+-rw-r--r--   0        0        0     1410 2023-07-24 02:51:17.248429 fullctl-1.5.0/src/fullctl/django/rest/views/usage.py
+-rw-r--r--   0        0        0    16540 2023-07-24 02:51:17.248429 fullctl-1.5.0/src/fullctl/django/settings/__init__.py
+-rw-r--r--   0        0        0     2655 2023-07-24 02:51:17.249429 fullctl-1.5.0/src/fullctl/django/settings/default.py
+-rw-r--r--   0        0        0     1215 2023-07-24 02:51:17.249429 fullctl-1.5.0/src/fullctl/django/signals.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.142326 fullctl-1.5.0/src/fullctl/django/social/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.142326 fullctl-1.5.0/src/fullctl/django/social/backends/__init__.py
+-rw-r--r--   0        0        0     1206 2021-10-06 05:10:14.142326 fullctl-1.5.0/src/fullctl/django/social/backends/peeringdb.py
+-rw-r--r--   0        0        0     1589 2021-10-06 05:10:14.142326 fullctl-1.5.0/src/fullctl/django/social/backends/twentyc.py
+-rw-r--r--   0        0        0      388 2021-10-06 05:10:14.142326 fullctl-1.5.0/src/fullctl/django/social/pipelines/__init__.py
+-rw-r--r--   0        0        0     4237 2021-10-06 05:10:14.143327 fullctl-1.5.0/src/fullctl/django/static/common/20c/twentyc.core.min.js
+-rw-r--r--   0        0        0    61051 2023-07-24 03:03:46.393276 fullctl-1.5.0/src/fullctl/django/static/common/20c/twentyc.rest.js
+-rw-r--r--   0        0        0     9475 2021-10-06 05:10:14.143327 fullctl-1.5.0/src/fullctl/django/static/common/20c-logo-filled.svg
+-rw-r--r--   0        0        0    21299 2023-07-24 02:51:17.274429 fullctl-1.5.0/src/fullctl/django/static/common/app.css
+-rw-r--r--   0        0        0    19449 2023-07-24 02:51:17.276429 fullctl-1.5.0/src/fullctl/django/static/common/app.js
+-rwxr-xr-x   0        0        0   372526 2023-07-24 02:51:17.281429 fullctl-1.5.0/src/fullctl/django/static/common/favicon.ico
+-rw-r--r--   0        0        0     3380 2021-10-06 05:10:14.144327 fullctl-1.5.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg
+-rw-r--r--   0        0        0     3657 2021-10-06 05:10:14.144327 fullctl-1.5.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg
+-rw-r--r--   0        0        0     3430 2021-10-06 05:10:14.144327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/add.svg
+-rw-r--r--   0        0        0     3819 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/alerts.svg
+-rw-r--r--   0        0        0     2838 2023-07-24 02:51:17.282429 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/api.svg
+-rw-r--r--   0        0        0     1303 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg
+-rw-r--r--   0        0        0     2681 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/delete.svg
+-rw-r--r--   0        0        0     5490 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/edit.svg
+-rwxr-xr-x   0        0        0     1172 2023-07-24 02:51:17.283429 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/launch.svg
+-rw-r--r--   0        0        0     1601 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/light-mode.svg
+-rw-r--r--   0        0        0     3357 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/list.svg
+-rwxr-xr-x   0        0        0     1721 2023-07-24 02:51:17.283429 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/location.svg
+-rw-r--r--   0        0        0     2617 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/logout.svg
+-rwxr-xr-x   0        0        0      726 2023-07-24 02:51:17.283429 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/mail.svg
+-rw-r--r--   0        0        0     2761 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/org.svg
+-rw-r--r--   0        0        0     1597 2023-07-24 02:51:17.284429 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/refresh.svg
+-rw-r--r--   0        0        0     1515 2023-07-24 02:51:17.284429 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/report.svg
+-rw-r--r--   0        0        0     8263 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/settings.svg
+-rw-r--r--   0        0        0     4138 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/user.svg
+-rwxr-xr-x   0        0        0     2782 2023-07-24 02:51:17.284429 fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/view.svg
+-rw-r--r--   0        0        0     3689 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg
+-rw-r--r--   0        0        0      169 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/md-add.svg
+-rw-r--r--   0        0        0      275 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/md-create.svg
+-rw-r--r--   0        0        0      272 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/md-list-box.svg
+-rw-r--r--   0        0        0      240 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/md-trash.svg
+-rw-r--r--   0        0        0     5957 2021-10-06 05:10:14.146327 fullctl-1.5.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg
+-rw-r--r--   0        0        0      954 2021-10-06 05:10:14.147327 fullctl-1.5.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg
+-rw-r--r--   0        0        0      818 2021-10-06 05:10:14.147327 fullctl-1.5.0/src/fullctl/django/static/common/icons/ui-close.svg
+-rw-r--r--   0        0        0     4482 2023-07-24 02:51:17.284429 fullctl-1.5.0/src/fullctl/django/static/common/logos/aaactl-dark.svg
+-rw-r--r--   0        0        0     4484 2023-07-24 02:51:17.285429 fullctl-1.5.0/src/fullctl/django/static/common/logos/aaactl-light.svg
+-rw-r--r--   0        0        0     4512 2023-07-24 02:51:17.285429 fullctl-1.5.0/src/fullctl/django/static/common/logos/aclctl-dark.svg
+-rw-r--r--   0        0        0     2625 2023-07-24 02:51:17.286429 fullctl-1.5.0/src/fullctl/django/static/common/logos/aclctl-light.svg
+-rwxr-xr-x   0        0        0     3333 2023-07-24 02:51:17.288429 fullctl-1.5.0/src/fullctl/django/static/common/logos/auditctl-dark.svg
+-rwxr-xr-x   0        0        0     3333 2023-07-24 02:51:17.289429 fullctl-1.5.0/src/fullctl/django/static/common/logos/auditctl-light.svg
+-rwxr-xr-x   0        0        0    36084 2023-07-24 02:51:17.292429 fullctl-1.5.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png
+-rwxr-xr-x   0        0        0    36307 2023-07-24 02:51:17.293429 fullctl-1.5.0/src/fullctl/django/static/common/logos/ctl-mark-light.png
+-rwxr-xr-x   0        0        0     4680 2023-07-24 02:51:17.294429 fullctl-1.5.0/src/fullctl/django/static/common/logos/devicectl-dark.svg
+-rw-r--r--   0        0        0     4682 2023-07-24 02:51:17.295429 fullctl-1.5.0/src/fullctl/django/static/common/logos/devicectl-light.svg
+-rwxr-xr-x   0        0        0     2579 2023-07-24 02:51:17.305429 fullctl-1.5.0/src/fullctl/django/static/common/logos/ixctl-dark.svg
+-rw-r--r--   0        0        0     2581 2023-07-24 02:51:17.318429 fullctl-1.5.0/src/fullctl/django/static/common/logos/ixctl-light.svg
+-rwxr-xr-x   0        0        0     3857 2023-07-24 02:51:17.319429 fullctl-1.5.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg
+-rw-r--r--   0        0        0     3859 2023-07-24 02:51:17.320429 fullctl-1.5.0/src/fullctl/django/static/common/logos/pdbctl-light.svg
+-rwxr-xr-x   0        0        0     4166 2023-07-24 02:51:17.322430 fullctl-1.5.0/src/fullctl/django/static/common/logos/peerctl-dark.svg
+-rw-r--r--   0        0        0     4168 2023-07-24 02:51:17.323429 fullctl-1.5.0/src/fullctl/django/static/common/logos/peerctl-light.svg
+-rwxr-xr-x   0        0        0     4336 2023-07-24 02:51:17.323429 fullctl-1.5.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg
+-rw-r--r--   0        0        0     4338 2023-07-24 02:51:17.325430 fullctl-1.5.0/src/fullctl/django/static/common/logos/prefixctl-light.svg
+-rw-r--r--   0        0        0     9475 2021-10-06 05:10:14.147327 fullctl-1.5.0/src/fullctl/django/static/common/oauth/20c.svg
+-rw-r--r--   0        0        0      689 2021-10-06 05:10:14.147327 fullctl-1.5.0/src/fullctl/django/static/common/oauth/google.svg
+-rw-r--r--   0        0        0     5222 2023-07-24 02:51:17.325430 fullctl-1.5.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png
+-rw-r--r--   0        0        0     9186 2021-10-06 05:10:14.147327 fullctl-1.5.0/src/fullctl/django/static/common/oauth/peeringdb.png
+-rw-r--r--   0        0        0     4323 2021-10-06 05:10:14.147327 fullctl-1.5.0/src/fullctl/django/static/common/service_bridge.js
+-rw-r--r--   0        0        0    11545 2023-07-24 02:51:17.333429 fullctl-1.5.0/src/fullctl/django/static/common/themes/dark.css
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.148327 fullctl-1.5.0/src/fullctl/django/static/common/themes/light.css
+-rw-r--r--   0        0        0    31401 2023-07-24 03:03:46.394276 fullctl-1.5.0/src/fullctl/django/static/common/v2/app.css
+-rw-r--r--   0        0        0    50853 2023-07-24 03:03:46.396276 fullctl-1.5.0/src/fullctl/django/static/common/v2/app.js
+-rw-r--r--   0        0        0    14838 2023-07-24 03:03:46.396276 fullctl-1.5.0/src/fullctl/django/static/common/v2/graph.js
+-rw-r--r--   0        0        0      644 2023-07-24 02:51:17.369430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/add.svg
+-rw-r--r--   0        0        0     4812 2023-07-24 02:51:17.369430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/api.svg
+-rw-r--r--   0        0        0      352 2023-07-24 02:51:17.377430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/arrow-clockwise.svg
+-rw-r--r--   0        0        0      232 2023-07-24 02:51:17.377430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/arrow.svg
+-rw-r--r--   0        0        0      532 2023-07-24 02:51:17.378430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg
+-rw-r--r--   0        0        0      423 2023-07-24 02:51:17.378430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/cancel.svg
+-rw-r--r--   0        0        0      274 2023-07-24 02:51:17.378430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/close.svg
+-rw-r--r--   0        0        0     1229 2023-07-24 02:51:17.378430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/database.svg
+-rw-r--r--   0        0        0      427 2023-07-24 02:51:17.378430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/download.svg
+-rw-r--r--   0        0        0      438 2023-07-24 02:51:17.378430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/envelope.svg
+-rw-r--r--   0        0        0      569 2023-07-24 02:51:17.379430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/eye.svg
+-rw-r--r--   0        0        0      483 2023-07-24 02:51:17.401430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/file-earmark-text.svg
+-rw-r--r--   0        0        0      404 2023-07-24 02:51:17.402430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/funnel.svg
+-rw-r--r--   0        0        0     1530 2023-07-24 02:51:17.402430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/gear.svg
+-rw-r--r--   0        0        0      483 2023-07-24 02:51:17.404430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/geo-alt.svg
+-rw-r--r--   0        0        0     1975 2023-07-24 02:51:17.404430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/help.svg
+-rw-r--r--   0        0        0      582 2023-07-24 02:51:17.405430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/list/delete.svg
+-rw-r--r--   0        0        0      438 2023-07-24 02:51:17.405430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/list/edit.svg
+-rw-r--r--   0        0        0      818 2023-07-24 02:51:17.405430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/list/options.svg
+-rw-r--r--   0        0        0      447 2023-07-24 02:51:17.404430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/list-ul.svg
+-rw-r--r--   0        0        0      553 2023-07-24 02:51:17.407430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/logout.svg
+-rw-r--r--   0        0        0      749 2023-07-24 02:51:17.407430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/org.svg
+-rw-r--r--   0        0        0      331 2023-07-24 02:51:17.407430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/search.svg
+-rw-r--r--   0        0        0     1465 2023-07-24 02:51:17.408430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg
+-rw-r--r--   0        0        0      298 2023-07-24 02:51:17.409430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/triangle-fill.svg
+-rw-r--r--   0        0        0      465 2023-07-24 02:51:17.409430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/ui-caret/dbl-select.svg
+-rw-r--r--   0        0        0      190 2023-07-24 02:51:17.410430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/ui-caret/down.svg
+-rw-r--r--   0        0        0     4138 2023-07-24 02:51:17.410430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/user.svg
+-rw-r--r--   0        0        0     3986 2023-07-24 02:51:17.410430 fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/view-settings.svg
+-rw-r--r--   0        0        0    61189 2023-07-24 02:51:17.412430 fullctl-1.5.0/src/fullctl/django/static/common/v2/imgs/help.png
+-rw-r--r--   0        0        0   426086 2023-07-24 02:51:17.421430 fullctl-1.5.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png
+-rw-r--r--   0        0        0    18588 2023-07-24 03:03:46.397276 fullctl-1.5.0/src/fullctl/django/static/common/v2/themes/dark.css
+-rw-r--r--   0        0        0        0 2023-07-24 02:51:17.424430 fullctl-1.5.0/src/fullctl/django/static/common/v2/themes/light.css
+-rw-r--r--   0        0        0      921 2023-07-24 02:51:17.424430 fullctl-1.5.0/src/fullctl/django/tasks/__init__.py
+-rw-r--r--   0        0        0      740 2021-10-06 05:10:14.148327 fullctl-1.5.0/src/fullctl/django/tasks/celery.py
+-rw-r--r--   0        0        0     2385 2023-07-24 02:51:17.434430 fullctl-1.5.0/src/fullctl/django/tasks/orm.py
+-rw-r--r--   0        0        0     2232 2023-07-24 02:51:17.435430 fullctl-1.5.0/src/fullctl/django/tasks/qualifiers.py
+-rw-r--r--   0        0        0      374 2023-07-24 02:51:17.435430 fullctl-1.5.0/src/fullctl/django/tasks/util.py
+-rw-r--r--   0        0        0      658 2023-07-24 02:51:17.436430 fullctl-1.5.0/src/fullctl/django/templates/common/apidocs/redoc.html
+-rw-r--r--   0        0        0      856 2023-07-24 02:51:17.436430 fullctl-1.5.0/src/fullctl/django/templates/common/apidocs/swagger.html
+-rw-r--r--   0        0        0     8871 2023-07-24 02:51:17.437430 fullctl-1.5.0/src/fullctl/django/templates/common/app/base.html
+-rw-r--r--   0        0        0      211 2021-10-06 05:10:14.149327 fullctl-1.5.0/src/fullctl/django/templates/common/app/checkbox.html
+-rw-r--r--   0        0        0     1935 2021-10-06 05:10:14.150327 fullctl-1.5.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html
+-rw-r--r--   0        0        0      726 2021-10-06 05:10:14.150327 fullctl-1.5.0/src/fullctl/django/templates/common/app/forms/import-org.html
+-rw-r--r--   0        0        0      494 2021-10-06 05:10:14.150327 fullctl-1.5.0/src/fullctl/django/templates/common/app/forms/invite.html
+-rw-r--r--   0        0        0      792 2021-10-06 05:10:14.150327 fullctl-1.5.0/src/fullctl/django/templates/common/app/forms/org-create.html
+-rw-r--r--   0        0        0     3826 2021-10-06 05:10:14.150327 fullctl-1.5.0/src/fullctl/django/templates/common/app/forms/org-prefs.html
+-rw-r--r--   0        0        0      355 2021-10-06 05:10:14.150327 fullctl-1.5.0/src/fullctl/django/templates/common/app/index.html
+-rw-r--r--   0        0        0     1974 2021-10-06 05:10:14.150327 fullctl-1.5.0/src/fullctl/django/templates/common/app/manage/permissions.html
+-rw-r--r--   0        0        0     4752 2023-07-24 02:51:17.438430 fullctl-1.5.0/src/fullctl/django/templates/common/app/modal.html
+-rw-r--r--   0        0        0     2668 2021-10-06 05:10:14.151327 fullctl-1.5.0/src/fullctl/django/templates/common/app/navbar.html
+-rw-r--r--   0        0        0      371 2023-07-24 02:51:17.438430 fullctl-1.5.0/src/fullctl/django/templates/common/app/templates.html
+-rw-r--r--   0        0        0     3101 2023-07-24 02:51:17.438430 fullctl-1.5.0/src/fullctl/django/templates/common/auth/login.html
+-rw-r--r--   0        0        0      880 2021-10-06 05:10:14.151327 fullctl-1.5.0/src/fullctl/django/templates/common/auth/oauth-badge.html
+-rw-r--r--   0        0        0     1110 2021-10-06 05:10:14.151327 fullctl-1.5.0/src/fullctl/django/templates/common/auth/oauth.html
+-rw-r--r--   0        0        0     1996 2023-07-24 02:51:17.454430 fullctl-1.5.0/src/fullctl/django/templates/common/base.html
+-rw-r--r--   0        0        0      333 2021-10-06 05:10:14.151327 fullctl-1.5.0/src/fullctl/django/templates/common/errors/400.html
+-rw-r--r--   0        0        0      367 2021-10-06 05:10:14.151327 fullctl-1.5.0/src/fullctl/django/templates/common/errors/401.html
+-rw-r--r--   0        0        0      375 2021-10-06 05:10:14.152327 fullctl-1.5.0/src/fullctl/django/templates/common/errors/403.html
+-rw-r--r--   0        0        0      377 2021-10-06 05:10:14.152327 fullctl-1.5.0/src/fullctl/django/templates/common/errors/404.html
+-rw-r--r--   0        0        0      456 2021-10-06 05:10:14.152327 fullctl-1.5.0/src/fullctl/django/templates/common/errors/500.html
+-rw-r--r--   0        0        0      597 2023-07-24 02:51:17.456430 fullctl-1.5.0/src/fullctl/django/templates/common/errors/base.html
+-rw-r--r--   0        0        0      351 2021-10-06 05:10:14.152327 fullctl-1.5.0/src/fullctl/django/templates/common/errors/details.html
+-rw-r--r--   0        0        0     1229 2023-07-24 02:51:17.456430 fullctl-1.5.0/src/fullctl/django/templates/common/snippets.html
+-rw-r--r--   0        0        0      234 2021-10-06 05:10:14.152327 fullctl-1.5.0/src/fullctl/django/templates/common/tool_base.html
+-rw-r--r--   0        0        0      658 2023-07-24 02:51:17.456430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html
+-rw-r--r--   0        0        0      856 2023-07-24 02:51:17.457430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html
+-rw-r--r--   0        0        0    12350 2023-07-24 02:51:17.458430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/base.html
+-rw-r--r--   0        0        0      211 2023-07-24 02:51:17.458430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/checkbox.html
+-rw-r--r--   0        0        0     2092 2023-07-24 02:51:17.459430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html
+-rw-r--r--   0        0        0      357 2023-07-24 02:51:17.479430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/delete_selected.html
+-rw-r--r--   0        0        0     1945 2023-07-24 02:51:17.480430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/footer.html
+-rw-r--r--   0        0        0     1935 2023-07-24 02:51:17.481430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html
+-rw-r--r--   0        0        0      430 2023-07-24 02:51:17.481430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/forms/feature-request.html
+-rw-r--r--   0        0        0      726 2023-07-24 02:51:17.481430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html
+-rw-r--r--   0        0        0      494 2023-07-24 02:51:17.481430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/forms/invite.html
+-rw-r--r--   0        0        0      792 2023-07-24 02:51:17.481430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html
+-rw-r--r--   0        0        0     3826 2023-07-24 02:51:17.482430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html
+-rw-r--r--   0        0        0      358 2023-07-24 02:51:17.482430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/index.html
+-rw-r--r--   0        0        0     1974 2023-07-24 02:51:17.482430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html
+-rw-r--r--   0        0        0     6217 2023-07-24 03:03:46.398276 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/modal.html
+-rw-r--r--   0        0        0     2668 2023-07-24 02:51:17.483430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/navbar.html
+-rw-r--r--   0        0        0      413 2023-07-24 02:51:17.483430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/templates.html
+-rw-r--r--   0        0        0     3048 2023-07-24 02:51:17.483430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/auth/login.html
+-rw-r--r--   0        0        0     1109 2023-07-24 02:51:17.483430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html
+-rw-r--r--   0        0        0     1339 2023-07-24 02:51:17.484430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/auth/oauth.html
+-rw-r--r--   0        0        0     1977 2023-07-24 02:51:17.484430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/base.html
+-rw-r--r--   0        0        0      339 2023-07-24 02:51:17.484430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/errors/400.html
+-rw-r--r--   0        0        0      373 2023-07-24 02:51:17.484430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/errors/401.html
+-rw-r--r--   0        0        0      381 2023-07-24 02:51:17.484430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/errors/403.html
+-rw-r--r--   0        0        0      383 2023-07-24 02:51:17.485430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/errors/404.html
+-rw-r--r--   0        0        0      462 2023-07-24 02:51:17.485430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/errors/500.html
+-rw-r--r--   0        0        0      568 2023-07-24 02:51:17.485430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/errors/base.html
+-rw-r--r--   0        0        0      351 2023-07-24 02:51:17.485430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/errors/details.html
+-rw-r--r--   0        0        0     1661 2023-07-24 02:51:17.485430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/snippets.html
+-rw-r--r--   0        0        0      234 2023-07-24 02:51:17.485430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/tool_base.html
+-rw-r--r--   0        0        0      249 2023-07-24 02:51:17.486430 fullctl-1.5.0/src/fullctl/django/templates/common/v2/tool_base_sidebar.html
+-rw-r--r--   0        0        0        0 2023-07-24 02:51:17.486430 fullctl-1.5.0/src/fullctl/django/templatetags/__init__.py
+-rw-r--r--   0        0        0     3398 2023-07-24 02:51:17.486430 fullctl-1.5.0/src/fullctl/django/templatetags/fullctl_util.py
+-rw-r--r--   0        0        0     3152 2023-07-24 02:51:17.486430 fullctl-1.5.0/src/fullctl/django/testutil.py
+-rw-r--r--   0        0        0     3854 2023-07-24 03:03:46.399276 fullctl-1.5.0/src/fullctl/django/urls.py
+-rw-r--r--   0        0        0     1171 2023-07-24 02:51:17.487430 fullctl-1.5.0/src/fullctl/django/util.py
+-rw-r--r--   0        0        0     1193 2023-07-24 02:51:17.488430 fullctl-1.5.0/src/fullctl/django/validators.py
+-rw-r--r--   0        0        0     4002 2023-07-24 03:03:46.399276 fullctl-1.5.0/src/fullctl/django/views/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-24 02:51:17.489430 fullctl-1.5.0/src/fullctl/django/views/api_schema.py
+-rw-r--r--   0        0        0      927 2023-07-24 02:51:17.489430 fullctl-1.5.0/src/fullctl/django/views/template.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:51:17.489430 fullctl-1.5.0/src/fullctl/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:51:17.489430 fullctl-1.5.0/src/fullctl/graph/mrtg/__init__.py
+-rw-r--r--   0        0        0     1420 2023-07-24 02:51:17.490430 fullctl-1.5.0/src/fullctl/graph/mrtg/mock.py
+-rw-r--r--   0        0        0    11196 2023-07-24 03:03:46.400276 fullctl-1.5.0/src/fullctl/graph/mrtg/rrd.py
+-rw-r--r--   0        0        0        0 2023-07-24 03:03:46.400276 fullctl-1.5.0/src/fullctl/graph/render/__init__.py
+-rw-r--r--   0        0        0     5327 2023-07-24 03:03:46.401276 fullctl-1.5.0/src/fullctl/graph/render/traffic.py
+-rw-r--r--   0        0        0     1536 2023-07-24 03:03:46.401276 fullctl-1.5.0/src/fullctl/graph/render/util.py
+-rw-r--r--   0        0        0        0 2021-10-06 05:10:14.153327 fullctl-1.5.0/src/fullctl/service_bridge/__init__.py
+-rw-r--r--   0        0        0     2706 2023-07-24 02:51:17.491430 fullctl-1.5.0/src/fullctl/service_bridge/aaactl.py
+-rw-r--r--   0        0        0      940 2023-07-24 02:51:17.493430 fullctl-1.5.0/src/fullctl/service_bridge/auditctl.py
+-rw-r--r--   0        0        0     8510 2023-07-24 02:51:17.494430 fullctl-1.5.0/src/fullctl/service_bridge/client.py
+-rw-r--r--   0        0        0     3419 2023-07-24 02:51:17.494430 fullctl-1.5.0/src/fullctl/service_bridge/data.py
+-rw-r--r--   0        0        0     3562 2023-07-24 03:03:46.402276 fullctl-1.5.0/src/fullctl/service_bridge/devicectl.py
+-rw-r--r--   0        0        0     2894 2023-07-24 03:03:46.402276 fullctl-1.5.0/src/fullctl/service_bridge/ixctl.py
+-rw-r--r--   0        0        0     2651 2023-07-24 02:51:17.498430 fullctl-1.5.0/src/fullctl/service_bridge/nautobot.py
+-rw-r--r--   0        0        0     1699 2023-07-24 02:51:17.499430 fullctl-1.5.0/src/fullctl/service_bridge/pdbctl.py
+-rw-r--r--   0        0        0     1037 2023-07-24 02:51:17.500430 fullctl-1.5.0/src/fullctl/service_bridge/peerctl.py
+-rw-r--r--   0        0        0     1076 2023-07-24 02:51:17.501430 fullctl-1.5.0/src/fullctl/service_bridge/prefixctl.py
+-rw-r--r--   0        0        0     6952 2023-07-24 02:51:17.502430 fullctl-1.5.0/src/fullctl/service_bridge/sot.py
+-rw-r--r--   0        0        0      323 2023-07-24 02:51:17.502430 fullctl-1.5.0/src/fullctl/utils/__init__.py
+-rw-r--r--   0        0        0     2837 1970-01-01 00:00:00.000000 fullctl-1.5.0/PKG-INFO
```

### Comparing `fullctl-1.4.0/LICENSE` & `fullctl-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/README.md` & `fullctl-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/pyproject.toml` & `fullctl-1.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "fullctl"
 repository = "https://github.com/fullctl/fullctl"
-version = "1.4.0"
+version = "1.5.0"
 description = "Core classes and functions for service applications"
 authors = ["FullCtl <code@fullctl.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
@@ -47,49 +47,53 @@
 # only needed for ixctl now, compare vs django-inet?
 django-netfields = "<2"
 
 # needed for verified asns
 django-peeringdb = "^2.8"
 
 # prod serving
-whitenoise = "^6"
-pyuwsgi = "^2.0.19"
+whitenoise = ">=6"
+pyuwsgi = ">=2.0.19"
 
 confu = "^1.5"
 grainy = "^1.8.1"
 psycopg2-binary = "^2.8"
-# psycopg = {extras = ["binary"], version = "^3.0.14"}
+# psycopg3 requires django 4.2
+# psycopg = {extras = ["binary"], version = "^3.1.8"}
 # force update
 pyyaml = ">=5"
 munge = ">=1.3.0"
 
 [tool.poetry.dev-dependencies]
 # tests
 coverage = ">=5"
 pytest = ">=6"
 pytest-django = ">=3.8"
 pytest-cov = "*"
+requests-mock = ">=1.11"
+tox = ">=3.20"
+tox-gh-actions = ">=2.9.1"
 
 # linting
 black = ">=20"
 isort = ">=5.7"
 flake8 = ">=3.8"
 pre-commit = ">=2.13"
 pyupgrade = ">=2.19"
 
 # docs
 markdown = "*"
-markdown-include = ">=0.5,<1"
-mkdocs = "^1.2.3"
+markdown-include = ">=0.5"
+mkdocs = ">=1.2.3"
 uritemplate = "*"
 
 # ctl
-ctl = { git = "https://github.com/20c/ctl.git", branch = "prep-release" }
-jinja2 = "^3"
-tmpl = "^1"
+ctl = { git = "https://github.com/20c/ctl.git", branch = "main" }
+jinja2 = ">=3"
+tmpl = ">=1"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.plugins."markdown.extensions"]
 pymdgen = "pymdgen.md:Extension"
```

### Comparing `fullctl-1.4.0/src/fullctl/django/admin.py` & `fullctl-1.5.0/src/fullctl/django/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import reversion
 from django.conf.urls import url
 from django.contrib import admin
-from django.http import HttpResponseForbidden
+from django.http import FileResponse, HttpResponseForbidden
 from django.shortcuts import redirect
+from django.urls import path, reverse
+from django.utils.html import format_html
 from django_handleref.admin import VersionAdmin
 
 import fullctl.django.auditlog as auditlog
 from fullctl.django.models.concrete import (
     Attachment,
     AuditLog,
     Organization,
+    OrganizationFile,
     OrganizationUser,
     Request,
     Response,
     Task,
     TaskSchedule,
     UserSettings,
 )
@@ -50,14 +53,56 @@
 
 @admin.register(Organization)
 class OrganizationAdmin(BaseAdmin):
     list_display = ("id", "name", "slug")
     inlines = (OrganizationUserInline,)
 
 
+@admin.register(OrganizationFile)
+class OrganizationFileAdmin(BaseAdmin):
+    list_display = (
+        "id",
+        "name",
+        "org",
+        "public",
+        "created",
+        "updated",
+        "download_link",
+    )
+    search_fields = ("name", "org__name")
+
+    def download_link(self, obj):
+        return format_html(
+            '<a href="{}">Download</a>', reverse("admin:download_file", args=[obj.pk])
+        )
+
+    download_link.short_description = "Download Link"
+
+    def download_file(self, request, pk):
+        file = self.get_object(request, pk)
+        response = FileResponse(
+            file.content,
+            as_attachment=True,
+            filename=file.name,
+            content_type=file.content_type,
+        )
+        return response
+
+    def get_urls(self):
+        urls = super().get_urls()
+        custom_urls = [
+            path(
+                "<int:pk>/download/",
+                self.admin_site.admin_view(self.download_file),
+                name="download_file",
+            ),
+        ]
+        return custom_urls + urls
+
+
 @admin.register(Task)
 class TaskAdmin(BaseAdmin):
     list_display = (
         "id",
         "source",
         "queue_id",
         "parent",
```

### Comparing `fullctl-1.4.0/src/fullctl/django/auditlog.py` & `fullctl-1.5.0/src/fullctl/django/auditlog.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/auth.py` & `fullctl-1.5.0/src/fullctl/django/auth.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/autocomplete/devicectl.py` & `fullctl-1.5.0/src/fullctl/django/autocomplete/devicectl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/autocomplete/pdb.py` & `fullctl-1.5.0/src/fullctl/django/autocomplete/pdb.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/context.py` & `fullctl-1.5.0/src/fullctl/django/context.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/context_processors.py` & `fullctl-1.5.0/src/fullctl/django/context_processors.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/decorators.py` & `fullctl-1.5.0/src/fullctl/django/decorators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/fields/__init__.py` & `fullctl-1.5.0/src/fullctl/django/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/fields/service_bridge/__init__.py` & `fullctl-1.5.0/src/fullctl/django/fields/service_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/inet/fields.py` & `fullctl-1.5.0/src/fullctl/django/inet/fields.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/inet/util.py` & `fullctl-1.5.0/src/fullctl/django/inet/util.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/inet/validators.py` & `fullctl-1.5.0/src/fullctl/django/inet/validators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/management/commands/base.py` & `fullctl-1.5.0/src/fullctl/django/management/commands/base.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py` & `fullctl-1.5.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py` & `fullctl-1.5.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_promote_user.py` & `fullctl-1.5.0/src/fullctl/django/management/commands/fullctl_promote_user.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_work_task.py` & `fullctl-1.5.0/src/fullctl/django/management/commands/fullctl_work_task.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/middleware.py` & `fullctl-1.5.0/src/fullctl/django/middleware.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0001_initial.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0003_auditlog.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0003_auditlog.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0008_managementtask.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0008_managementtask.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0009_taskclaim.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0009_taskclaim.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0015_alter_task_parent.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0015_alter_task_parent.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0018_task_schedule.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0018_task_schedule.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0021_servicebridgeaction.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0021_servicebridgeaction.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0027_request_response.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0027_request_response.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0030_alter_response_content.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0030_alter_response_content.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py` & `fullctl-1.5.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/models/abstract/alert.py` & `fullctl-1.5.0/src/fullctl/django/models/abstract/alert.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/models/abstract/base.py` & `fullctl-1.5.0/src/fullctl/django/models/abstract/base.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/models/abstract/meta.py` & `fullctl-1.5.0/src/fullctl/django/models/abstract/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,15 +325,16 @@
                     request=req,
                 )
 
             # if a meta data class is defined for this request
             # we will write the meta data from the response
 
             try:
-                req.response.write_meta_data(req)
+                if http_status in cls.valid_http_status:
+                    req.response.write_meta_data(req)
             except NoMetaClassDefined:
                 pass
 
             return req
 
         return req
 
@@ -353,17 +354,17 @@
 
         if not cached:
             return None
 
         tdiff = time.time() - cached.updated.timestamp()
 
         if cached.http_status == 429:
-            if tdiff > 300:
-                # if the cached request is a 429 and it's older than 5 minutes
-                # we will ignore it and send a new request
+            if tdiff > 300 or tdiff > cls.cache_expiry(target):
+                # if the cached request is a 429 and it's older than 5 minutes or
+                # older than the normal cache expiry we will ignore it and send a new request
                 return None
 
         return cached
 
     @classmethod
     def get_cache_queryset(cls, target):
         target_field = cls.config("target_field")
```

### Comparing `fullctl-1.4.0/src/fullctl/django/models/abstract/service_bridge.py` & `fullctl-1.5.0/src/fullctl/django/models/abstract/service_bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
                 try:
                     if dest_value == type(dest_value)(src_value):
                         continue
                 except (ValueError, TypeError):
                     pass
 
                 changed = True
-                # print(f"{src_field} changed from {src_value} to {dest_value}")
+                print(f"{src_field} changed from {src_value} to {dest_value}")
                 setattr(self, src_field, dest_value)
 
         # print("sync from reference", self, changed)
 
         if changed and save:
             self.save()
```

### Comparing `fullctl-1.4.0/src/fullctl/django/models/abstract/template.py` & `fullctl-1.5.0/src/fullctl/django/models/abstract/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/models/concrete/account.py` & `fullctl-1.5.0/src/fullctl/django/models/concrete/account.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/models/concrete/auditlog.py` & `fullctl-1.5.0/src/fullctl/django/models/concrete/auditlog.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/models/concrete/meta.py` & `fullctl-1.5.0/src/fullctl/django/models/concrete/meta.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/models/concrete/service_bridge.py` & `fullctl-1.5.0/src/fullctl/django/models/concrete/service_bridge.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/models/concrete/tasks.py` & `fullctl-1.5.0/src/fullctl/django/models/concrete/tasks.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/api_schema.py` & `fullctl-1.5.0/src/fullctl/django/rest/api_schema.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/authentication.py` & `fullctl-1.5.0/src/fullctl/django/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/core.py` & `fullctl-1.5.0/src/fullctl/django/rest/core.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/decorators.py` & `fullctl-1.5.0/src/fullctl/django/rest/decorators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/filters.py` & `fullctl-1.5.0/src/fullctl/django/rest/filters.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/mixins.py` & `fullctl-1.5.0/src/fullctl/django/rest/mixins.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/renderers.py` & `fullctl-1.5.0/src/fullctl/django/rest/renderers.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/serializers/__init__.py` & `fullctl-1.5.0/src/fullctl/django/rest/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/serializers/aaactl_sync.py` & `fullctl-1.5.0/src/fullctl/django/rest/serializers/aaactl_sync.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.contrib.auth import get_user_model
 from rest_framework import serializers
+from social_django.models import UserSocialAuth
 
 import fullctl.django.models as models
 from fullctl.django.rest.decorators import serializer_registry
 from fullctl.django.rest.serializers import ModelSerializer
 
 Serializers, register = serializer_registry()
 
@@ -19,14 +20,45 @@
             "first_name",
             "last_name",
             "email",
             "is_superuser",
             "is_staff",
         ]
 
+    def save(self):
+        if self.instance and self.instance.id:
+            # for updates we can just call super
+            return super().save()
+
+        # create new user
+
+        remote_id = self.context["remote_id"]
+
+        user = get_user_model().objects.create_user(
+            username=self.validated_data["username"],
+            email=self.validated_data["email"],
+            first_name=self.validated_data["first_name"],
+            last_name=self.validated_data["last_name"],
+            is_superuser=self.validated_data["is_superuser"],
+            is_staff=self.validated_data["is_staff"],
+        )
+
+        # create social auth entry for aaactl (this is not
+        # a valid auth at this point and the user will
+        # be prompted to login with aaactl - this just
+        # allows us to link the user to aaactl
+
+        UserSocialAuth.objects.create(
+            user=user,
+            uid=remote_id,
+            provider="twentyc",
+        )
+
+        return user
+
 
 @register
 class Organization(ModelSerializer):
     class Meta:
         model = models.Organization
         fields = ["name", "slug", "personal", "backend", "remote_id"]
```

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/serializers/account.py` & `fullctl-1.5.0/src/fullctl/django/rest/serializers/account.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/serializers/meta.py` & `fullctl-1.5.0/src/fullctl/django/rest/serializers/meta.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/serializers/org.py` & `fullctl-1.5.0/src/fullctl/django/rest/serializers/org.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/serializers/template.py` & `fullctl-1.5.0/src/fullctl/django/rest/serializers/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/urls/service_bridge_proxy.py` & `fullctl-1.5.0/src/fullctl/django/rest/urls/service_bridge_proxy.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/views/aaactl_sync.py` & `fullctl-1.5.0/src/fullctl/django/rest/views/aaactl_sync.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 These views require permissions to the `aaactl_sync` namespace which usually
 only exists on the internal api key used for service bridging
 """
 
 from django.contrib.auth import get_user_model
 from rest_framework import viewsets
+from rest_framework.decorators import action
 from rest_framework.response import Response
 
 import fullctl.django.models as models
 from fullctl.django.rest.core import BadRequest
 from fullctl.django.rest.decorators import grainy_endpoint
 from fullctl.django.rest.mixins import CachedObjectMixin
 from fullctl.django.rest.route.service_bridge import route
@@ -35,19 +36,31 @@
     queryset = get_user_model().objects.all()
 
     # this approach assumes that aaactl is the only authentication
     # provider
     lookup_field = "social_auth__uid"
     lookup_url_kwarg = "remote_id"
 
+    @action(detail=False, methods=["put"], url_path="(?P<aaactl_id>[^/.]+)")
     @grainy_endpoint("aaactl_sync.user")
-    def update(self, request, remote_id, *args, **kwargs):
-        user = self.get_object()
-        serializer = self.serializer_class(instance=user, data=request.data)
+    def create_or_update(self, request, aaactl_id, *args, **kwargs):
+        """
+        Creates / Updates user by their aaactl id (social_auth__uid)
+        """
+
+        try:
+            user = get_user_model().objects.get(social_auth__uid=aaactl_id)
+        except get_user_model().DoesNotExist:
+            user = None
+
+        serializer = self.serializer_class(
+            instance=user, data=request.data, context={"remote_id": aaactl_id}
+        )
         if not serializer.is_valid():
+            print(serializer.errors)
             return BadRequest(serializer.errors)
         serializer.save()
         return Response(serializer.data)
 
 
 @route
 class Organization(CachedObjectMixin, viewsets.GenericViewSet):
```

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/views/account.py` & `fullctl-1.5.0/src/fullctl/django/rest/views/account.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/views/service_bridge.py` & `fullctl-1.5.0/src/fullctl/django/rest/views/service_bridge.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/views/template.py` & `fullctl-1.5.0/src/fullctl/django/rest/views/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/rest/views/usage.py` & `fullctl-1.5.0/src/fullctl/django/rest/views/usage.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/settings/__init__.py` & `fullctl-1.5.0/src/fullctl/django/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/settings/default.py` & `fullctl-1.5.0/src/fullctl/django/settings/default.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/signals.py` & `fullctl-1.5.0/src/fullctl/django/signals.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/social/backends/peeringdb.py` & `fullctl-1.5.0/src/fullctl/django/social/backends/peeringdb.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/social/backends/twentyc.py` & `fullctl-1.5.0/src/fullctl/django/social/backends/twentyc.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/20c/twentyc.core.min.js` & `fullctl-1.5.0/src/fullctl/django/static/common/20c/twentyc.core.min.js`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/20c/twentyc.rest.js` & `fullctl-1.5.0/src/fullctl/django/static/common/20c/twentyc.rest.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -554,14 +554,15 @@
              * @param {String} method http request method
              * @returns {Promise}
              */
 
             write: function(endpoint, data, method, url = null) {
                 url = url || this.endpoint_url(endpoint);
                 method = method.toLowerCase();
+                const client = this;
 
                 $(this).trigger("api-request:before", [endpoint, data, method])
                 $(this).trigger("api-write:before", [endpoint, data, method])
                 $(this).trigger("api-" + method + ":before", [endpoint, data])
                 var request = new Promise(function(resolve, reject) {
                     $.ajax({
                         dataType: "json",
@@ -569,21 +570,22 @@
                         url: this.format_request_url(url, method),
                         data: this.encode(data),
                         headers: {
                             "Content-Type": "application/json",
                             "X-CSRFToken": twentyc.rest.config.csrf
                         },
                     }).done(function(result) {
-                        var response = new twentyc.rest.Response(result);
+                        const response = new twentyc.rest.Response(result);
+                        client.on_write_success(endpoint, data, response, method);
                         $(this).trigger("api-request:success", [endpoint, data, response, method]);
                         $(this).trigger("api-write:success", [endpoint, data, response, method]);
                         $(this).trigger("api-" + method + ":success", [endpoint, data, response]);
                         resolve(response);
                     }.bind(this)).fail(function(e) {
-                        var response = new twentyc.rest.Response(e.responseJSON, e.status);
+                        const response = new twentyc.rest.Response(e.responseJSON, e.status);
                         $(this).trigger("api-request:error", [endpoint, data, response, method]);
                         $(this).trigger("api-write:error", [endpoint, data, response, method]);
                         $(this).trigger("api-" + method + ":error", [endpoint, data, response]);
                         reject(response);
                     }.bind(this)).always(function(e) {
                         $(this).trigger("api-request:after", [endpoint, data, method]);
                         $(this).trigger("api-write:after", [endpoint, data, method]);
@@ -591,14 +593,27 @@
                     }.bind(this));
                 }.bind(this));
 
                 return request;
             },
 
             /**
+             * executed before hte `api-write:success` event if the POST, PUT or DELETE
+             * request returned with a succesful http status
+             *
+             * @method on_write_success
+             * @param {string} endpoint the api endpoint to be requested
+             * @param {object} data request payload
+             * @param {twentyc.rest.response} response
+             * @param {string} method request method
+             */
+
+            on_write_success: function(endpoint, data, response, method) {},
+
+            /**
              * Wrapper to perform a `GET` request on the api
              *
              * @method get
              * @param {String} endpoint
              * @param {Object} params url parameters
              * @returns {Promise}
              */
@@ -1056,18 +1071,20 @@
                 var k, empty = {};
                 for (k in this.payload()) {
                     empty[k] = ""
                 }
                 this.fill(empty);
             },
 
-            post_success: function(result) {
+            on_write_success: function() {
                 this.element.attr("data-submitted", "true")
             },
 
+            post_success: function(response) {},
+
             post_failure: function(response) {
                 response.field_errors(this.render_error.bind(this));
                 response.non_field_errors(this.render_non_field_errors.bind(this))
             },
 
             /**
              * Submit the form using the specified method
@@ -1187,22 +1204,20 @@
     /**
      * Base input widget class
      *
      * # required
      *
      * - data-api-base: api root or full path to endpoint
      *
-     * @class Button
+     * @class Input
      * @extends twentyc.rest.Widget
      * @namespace twentyc.rest
      * @param {jQuery result} jq jquery result holding the target element
      */
 
-
-
     twentyc.rest.Input = twentyc.cls.extend(
         "Input", {
             Input: function(jq) {
                 var base_url = jq.data("api-base");
                 this.Widget(base_url, jq);
             },
 
@@ -1283,15 +1298,21 @@
      *
      * The select element should have the following attributes set
      *
      * # required
      *
      * - data-api-base: api root or full path to endpoint
      *
-     * @class Button
+     * # optional
+     *
+     * - data-confirm: text to show to confirm confirm changing state of checkbox
+     * - data-confirm-off: text to show to confirm changing state of checkbox
+     * to unchecked
+     *
+     * @class Checkbox
      * @extends twentyc.rest.Input
      * @namespace twentyc.rest
      * @param {jQuery result} jq jquery result holding the button element
      */
 
 
     twentyc.rest.Checkbox = twentyc.cls.extend(
@@ -1302,30 +1323,37 @@
                 return pl;
             },
 
             bind: function(jq) {
                 this.Widget_bind(jq);
                 this.method = jq.data("api-method") || "POST";
 
-                this.element.on("change", function(ev) {
+                this.element.on("change", (ev) => {
+
+                    // use data-confirm-off to get confirmation when unchecking
+                    const confirm_off_required = this.element.data("confirm-off");
+                    if (confirm_off_required && !$(this.element).prop("checked") && !confirm(confirm_off_required)) {
+                        this.element.prop("checked", true);
+                        return;
+                    }
 
-                    var confirm_required = this.element.data("confirm");
+                    const confirm_required = this.element.data("confirm");
                     if (confirm_required && !confirm(confirm_required))
                         return;
 
                     this.clear_errors();
 
                     var action = this.action;
                     var fn = this[this.method.toLowerCase()].bind(this);
 
                     fn(action, this.payload()).then(
                         this.post_success.bind(this),
                         this.post_failure.bind(this)
                     );
-                }.bind(this));
+                });
 
             },
 
             post_failure: function(field, error) {
                 this.Input_post_failure(field, error);
 
                 // reset checkbox to previous state
```

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/20c-logo-filled.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/20c-logo-filled.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/app.css` & `fullctl-1.5.0/src/fullctl/django/static/common/app.css`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/app.js` & `fullctl-1.5.0/src/fullctl/django/static/common/app.js`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/favicon.ico` & `fullctl-1.5.0/src/fullctl/django/static/common/favicon.ico`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/add.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/add.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/alerts.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/alerts.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/api.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/api.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/delete.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/delete.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/edit.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/edit.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/launch.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/launch.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/light-mode.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/light-mode.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/list.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/list.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/location.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/location.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/logout.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/logout.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/mail.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/mail.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/org.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/org.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/refresh.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/refresh.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/report.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/report.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/settings.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/settings.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/user.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/user.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/view.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/icon/view.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/icons/ui-close.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/icons/ui-close.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/aaactl-dark.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/aaactl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/aaactl-light.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/aaactl-light.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/aclctl-dark.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/aclctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/aclctl-light.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/aclctl-light.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/auditctl-dark.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/auditctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/auditctl-light.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/auditctl-light.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/ctl-mark-light.png` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/ctl-mark-light.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/devicectl-dark.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/devicectl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/devicectl-light.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/devicectl-light.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/ixctl-dark.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/ixctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/ixctl-light.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/ixctl-light.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/pdbctl-light.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/pdbctl-light.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/peerctl-dark.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/peerctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/peerctl-light.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/peerctl-light.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/logos/prefixctl-light.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/logos/prefixctl-light.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/oauth/20c.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/oauth/20c.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/oauth/google.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/oauth/google.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png` & `fullctl-1.5.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/oauth/peeringdb.png` & `fullctl-1.5.0/src/fullctl/django/static/common/oauth/peeringdb.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/service_bridge.js` & `fullctl-1.5.0/src/fullctl/django/static/common/service_bridge.js`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/themes/dark.css` & `fullctl-1.5.0/src/fullctl/django/static/common/themes/dark.css`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/app.css` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/app.css`

 * *Files 1% similar despite different names*

```diff
@@ -657,14 +657,21 @@
   letter-spacing: 0;
   line-height: 20px;
   display: inline;
   margin-left: 1px;
   padding: 8px;
 }
 
+.infobar .toolbar-field {
+  border: 1px solid var(--clr-border-200);
+}
+
+.infobar .toolbar-field span.icon:not(.inactive) {
+  background-color: var(--clr-accent-400);
+}
 
 div.toolbar-field>span.value {
   font-size: 16px;
   font-weight: bold;
   letter-spacing: 0;
   line-height: 20px;
 }
@@ -1790,15 +1797,14 @@
 }
 
 .select2-selection.select2-selection--single {
   height: 42px;
   padding-left: var(--size-100);
   display: flex;
   align-items: center;
-  background-color: transparent;
 }
 
 .select2-container--default .select2-selection--single .select2-selection__arrow {
   right: 4px;
   top: initial;
 }
```

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/app.js` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/app.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1441,27 +1441,21 @@
      */
 
     fullctl.application.Searchbar = $tc.define(
         "Searchbar", {
             Searchbar: function(jq, filter_function, clear_filter_function) {
                 const filter_input =
                     this.filter_input =
-                    this.element =
-                    jq.find('[data-role="filter"]') ||
-                    jq.find('[data-element="filter"]');
+                    this.element = jq.find('[data-role="filter"]');
 
                 const search_btn =
-                    this.search_btn =
-                    jq.find('[data-role="filter_submit"]') ||
-                    jq.find('[data-element="filter_submit"]');
+                    this.search_btn = jq.find('[data-role="filter_submit"]');
 
                 const clear_search_btn =
-                    this.clear_search_btn =
-                    jq.find('[data-role="filter_clear"]') ||
-                    jq.find('[data-element="filter_clear"]');
+                    this.clear_search_btn = jq.find('[data-role="filter_clear"]');
 
                 this.filter_function = filter_function;
                 this.clear_filter_function = clear_filter_function;
 
                 const searchbar = this;
                 filter_input.on("keyup", function(event) {
                     if (event.key === "Enter") {
@@ -1764,21 +1758,21 @@
             if (opt.initial) {
 
                 // check if initial is callable
                 if (typeof opt.initial === "function") {
                     opt.initial((initial) => {
                         let option = $(new Option(initial.primary, initial.id, true, true))
                         option.data("selection_data", initial)
-                        jq.append(option.get(0)).trigger("change")
+                        jq.append(option.get(0)).trigger("change", ["on_load_change"]);
                     })
                 } else {
                     let initial = opt.initial;
                     let option = $(new Option(initial.primary, initial.id, true, true))
                     option.data("selection_data", initial)
-                    jq.append(option.get(0)).trigger("change")
+                    jq.append(option.get(0)).trigger("change", ["on_load_change"]);
                 }
 
             }
 
             if (opt.controls !== false)
                 this.setup_controls();
 
@@ -1789,15 +1783,15 @@
         },
 
         setup_controls: function() {
             // controls that allow removal of selected autocomplete element.
             let controls = $('<div>').addClass('autocomplete-controls').append(
                 $('<a>').addClass('action').text('remove')
             ).hide().on("click", () => {
-                this.element.val(null).trigger("change");
+                this.element.val(null).trigger("change", ["on_load_change"]);
                 controls.hide();
             });
 
             this.element.on("change", function(e) {
                 if ($(this).val()) {
                     controls.show();
                 } else {
```

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/add.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/add.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/api.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/api.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/database.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/database.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/eye.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/eye.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/gear.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/gear.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/help.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/help.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list/delete.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/list/delete.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list/options.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/list/options.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/logout.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/logout.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/org.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/org.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/user.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/user.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/view-settings.svg` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/icons/view-settings.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/imgs/help.png` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/imgs/help.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/static/common/v2/themes/dark.css` & `fullctl-1.5.0/src/fullctl/django/static/common/v2/themes/dark.css`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
   --clr-accent-500: #FD7E14;
   --clr-accent-600: red;
   --clr-accent-700: #1E90FF;
 
   --clr-bg-200: rgba(246, 248, 250, 1);
   --clr-bg-210: hsl(210, 14%, 95%);
   --clr-bg-300: #E5E5E5;
+  --clr-bg-400: #b3b3b3;
   --clr-bg-700: rgba(62, 70, 79, 1);
   --clr-bg-800: rgba(44, 47, 58, 0.96);
   --clr-bg-850: hsl(227, 12%, 14%);
   --clr-bg-900: #191B22;
 
   --clr-border-200: var(--clr-primary-500);
   --clr-border-400: var(--clr-primary-700);
@@ -62,14 +63,16 @@
   --source-of-truth-icon: url("../logos/ctl-mark-dark.png");
 
   --clr-bg-loading-indicator: #0c0e14;
   --default-input-bg: #3b3b3b;
 
   --graph-placeholder-bg: rgba(0,0,0,0.5);
 
+  --select2-selected-bg: var(--clr-bg-700);
+
   color-scheme: dark;
 }
 
 :root[data-theme="light"] {
   --theme-bg-secondary: #3E464F;
   --clr-border-400: var(--clr-primary-500);
   --theme-secondary-border-color: rgba(25, 27, 34, 0.15);
@@ -100,14 +103,16 @@
   --bs-link-color: rgb(13, 110, 253);
   --bs-link-hover-color: rgb(13, 110, 253);
 
   --clr-bg-loading-indicator: #d5d5d5;
 
   --graph-placeholder-bg: rgba(0,0,0,0.2);
 
+  --select2-selected-bg: var(--clr-bg-400);
+
   color-scheme: light;
 }
 
 /**
  * Basic styles
  */
 
@@ -618,14 +623,30 @@
 
 .modal span.select2-dropdown {
   border-color: var(--clr-border-400);
   background-color: var(--modal-bg);
   box-shadow: 5px 5px #0000004d;
 }
 
+.select2-selection.select2-selection--single {
+  background-color: transparent;
+}
+
+.select2-container--default .select2-results__option[aria-selected="true"] {
+  background: transparent;
+}
+
+.select2-results__option[aria-selected="true"] .autocomplete-item {
+  background-color: var(--select2-selected-bg);
+}
+
+.select2-container--default .select2-results__option--highlighted[aria-selected] {
+  color: foreground;
+}
+
 div.controls label {
   color: var(--th-clr);
 }
 
 div.menu div.menu-deco-border {
   background-color: var(--clr-border-400);
 }
@@ -834,19 +855,18 @@
  */
 .sidebar[data-element="menu"] .button {
   color: var(--foreground);
   background: transparent;
 }
 
 
-div.autocomplete-item .autocomplete-primary {
+div.autocomplete-item {
   color: var(--foreground);
 }
 
-
 /**
  * syntax hl
 */
 .syntax-highlight-transparent-bg pre {
   background-color: transparent !important;
 }
```

### Comparing `fullctl-1.4.0/src/fullctl/django/tasks/__init__.py` & `fullctl-1.5.0/src/fullctl/django/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/tasks/celery.py` & `fullctl-1.5.0/src/fullctl/django/tasks/celery.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/tasks/orm.py` & `fullctl-1.5.0/src/fullctl/django/tasks/orm.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/tasks/qualifiers.py` & `fullctl-1.5.0/src/fullctl/django/tasks/qualifiers.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/apidocs/redoc.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/apidocs/redoc.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/apidocs/swagger.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/apidocs/swagger.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/app/base.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/app/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/import-org.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/app/forms/import-org.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/org-create.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/app/forms/org-create.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/org-prefs.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/app/forms/org-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/app/manage/permissions.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/app/manage/permissions.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/app/modal.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/app/modal.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/app/navbar.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/app/navbar.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/auth/login.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/auth/login.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/auth/oauth-badge.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/auth/oauth-badge.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/auth/oauth.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/auth/oauth.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/base.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/errors/base.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/errors/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/snippets.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/snippets.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/base.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/footer.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/footer.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/modal.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/modal.html`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 <div class="modal" role="dialog" data-component="modal_no_button_lg">
   <div class="modal-dialog modal-lg" role="document">
     <div class="modal-content">
       <div class="modal-header">
         <h5 class="modal-title" data-element="title"></h5>
         <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close">
-          <span aria-hidden="true">&times;</span>
         </button>
       </div>
       <div class="modal-body controls" data-element="body">
       </div>
       <div class="modal-footer" data-element="footer">
       </div>
     </div>
@@ -159,15 +158,14 @@
 
 <div class="modal" role="dialog" id="modal-manage" data-component="modal_manage">
   <div class="modal-dialog modal-lg" role="document">
     <div class="modal-content">
       <div class="modal-header">
         <h5 class="modal-title"></h5>
         <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close">
-          <span aria-hidden="true">&times;</span>
         </button>
       </div>
       <div class="modal-body controls">
       </div>
       <div class="modal-footer">
       </div>
     </div>
```

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/navbar.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/app/navbar.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/login.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/auth/login.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/oauth.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/auth/oauth.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/base.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/base.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/errors/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templates/common/v2/snippets.html` & `fullctl-1.5.0/src/fullctl/django/templates/common/v2/snippets.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/templatetags/fullctl_util.py` & `fullctl-1.5.0/src/fullctl/django/templatetags/fullctl_util.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/testutil.py` & `fullctl-1.5.0/src/fullctl/django/testutil.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/urls.py` & `fullctl-1.5.0/src/fullctl/django/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,19 @@
     path(
         "api/",
         include(
             ("fullctl.django.rest.urls.service_bridge", "service_bridge_api"),
             namespace="service_bridge_api",
         ),
     ),
+    path(
+        "<str:org_tag>/file/<str:file_name>/",
+        fullctl.django.views.organization_file_download,
+        name="organization-file-download",
+    ),
     path("logout/", fullctl.django.views.logout, name="logout"),
     path("login/", fullctl.django.views.login, name="login"),
     path(
         "apidocs/swagger",
         TemplateView.as_view(
             template_name="common/apidocs/swagger.html",
         ),
```

### Comparing `fullctl-1.4.0/src/fullctl/django/util.py` & `fullctl-1.5.0/src/fullctl/django/util.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/validators.py` & `fullctl-1.5.0/src/fullctl/django/validators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/django/views/template.py` & `fullctl-1.5.0/src/fullctl/django/views/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/graph/mrtg/mock.py` & `fullctl-1.5.0/src/fullctl/graph/mrtg/mock.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/aaactl.py` & `fullctl-1.5.0/src/fullctl/service_bridge/aaactl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/auditctl.py` & `fullctl-1.5.0/src/fullctl/service_bridge/auditctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/client.py` & `fullctl-1.5.0/src/fullctl/service_bridge/client.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/data.py` & `fullctl-1.5.0/src/fullctl/service_bridge/data.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/devicectl.py` & `fullctl-1.5.0/src/fullctl/service_bridge/devicectl.py`

 * *Files 7% similar despite different names*

```diff
@@ -124,11 +124,24 @@
         ref_tag = "port_info"
 
 
 class VirtualPort(Devicectl):
     class Meta(Devicectl.Meta):
         ref_tag = "virtual_port"
 
+    def traffic(self, pk, start_time=None, duration=None):
+        params = {}
+        if start_time:
+            params["start_time"] = start_time
+
+        if duration:
+            params["duration"] = duration
+
+        return self.get(
+            f"data/virtual_port/{pk}/traffic",
+            params=params,
+        )
+
 
 class IPAddress(Devicectl):
     class Meta(Devicectl.Meta):
         ref_tag = "ip"
```

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/ixctl.py` & `fullctl-1.5.0/src/fullctl/service_bridge/ixctl.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,14 +78,27 @@
         data = {"md5": md5, "asn": asn, "source": source}
 
         member_ip = ipaddress.ip_interface(member_ip).ip
         router_ip = ipaddress.ip_interface(router_ip).ip
 
         self.put(f"data/member/sync/{asn}/{member_ip}/{router_ip}/md5", data=data)
 
+    def traffic(self, pk, start_time=None, duration=None):
+        params = {}
+        if start_time:
+            params["start_time"] = start_time
+
+        if duration:
+            params["duration"] = duration
+
+        return self.get(
+            f"data/member/{pk}/traffic",
+            params=params,
+        )
+
 
 class RouteserverObject(IxctlEntity):
     description = "Ixctl Route Server"
     relationships = {
         "ix": {"bridge": InternetExchange, "filter": ("ix", "ix_id")},
     }
```

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/nautobot.py` & `fullctl-1.5.0/src/fullctl/service_bridge/nautobot.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/pdbctl.py` & `fullctl-1.5.0/src/fullctl/service_bridge/pdbctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/peerctl.py` & `fullctl-1.5.0/src/fullctl/service_bridge/peerctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/prefixctl.py` & `fullctl-1.5.0/src/fullctl/service_bridge/prefixctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/src/fullctl/service_bridge/sot.py` & `fullctl-1.5.0/src/fullctl/service_bridge/sot.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.4.0/PKG-INFO` & `fullctl-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fullctl
-Version: 1.4.0
+Version: 1.5.0
 Summary: Core classes and functions for service applications
 Home-page: https://github.com/fullctl/fullctl
 License: Apache-2.0
 Author: FullCtl
 Author-email: code@fullctl.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,19 +28,19 @@
 Requires-Dist: django-recaptcha (>=2,<3)
 Requires-Dist: django-reversion (>=5,<6)
 Requires-Dist: django-structlog (>=2.1.3,<3.0.0)
 Requires-Dist: djangorestframework (>=3,<4)
 Requires-Dist: grainy (>=1.8.1,<2.0.0)
 Requires-Dist: munge (>=1.3.0)
 Requires-Dist: psycopg2-binary (>=2.8,<3.0)
-Requires-Dist: pyuwsgi (>=2.0.19,<3.0.0)
+Requires-Dist: pyuwsgi (>=2.0.19)
 Requires-Dist: pyyaml (>=5)
 Requires-Dist: setuptools
 Requires-Dist: social-auth-app-django (>=5.2)
-Requires-Dist: whitenoise (>=6,<7)
+Requires-Dist: whitenoise (>=6)
 Project-URL: Repository, https://github.com/fullctl/fullctl
 Description-Content-Type: text/markdown
 
 # FullCtl
 
 [![PyPI](https://img.shields.io/pypi/v/fullctl.svg?maxAge=60)](https://pypi.python.org/pypi/fullctl)
 [![PyPI](https://img.shields.io/pypi/pyversions/fullctl.svg?maxAge=600)](https://pypi.python.org/pypi/fullctl)
```

