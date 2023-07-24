# Comparing `tmp/edx-enterprise-4.0.3.tar.gz` & `tmp/edx-enterprise-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-4.0.3.tar", last modified: Fri Jul 21 16:55:37 2023, max compression
+gzip compressed data, was "edx-enterprise-4.0.4.tar", last modified: Mon Jul 24 16:39:17 2023, max compression
```

## Comparing `edx-enterprise-4.0.3.tar` & `edx-enterprise-4.0.4.tar`

### file list

```diff
@@ -1,767 +1,768 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.073500 edx-enterprise-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)   137560 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)   186433 2023-07-21 16:55:37.077500 edx-enterprise-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.005498 edx-enterprise-4.0.3/consent/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.005498 edx-enterprise-4.0.3/consent/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.005498 edx-enterprise-4.0.3/consent/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.005498 edx-enterprise-4.0.3/consent/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.005498 edx-enterprise-4.0.3/consent/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/migrations/0002_migrate_to_new_data_sharing_consent.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/migrations/0003_historicaldatasharingconsent_history_change_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/migrations/0004_datasharingconsenttextoverrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/migrations/0005_auto_20230707_0755.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/consent/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.005498 edx-enterprise-4.0.3/edx_enterprise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)   186433 2023-07-21 16:55:36.000000 edx-enterprise-4.0.3/edx_enterprise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38833 2023-07-21 16:55:36.000000 edx-enterprise-4.0.3/edx_enterprise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:55:36.000000 edx-enterprise-4.0.3/edx_enterprise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:55:36.000000 edx-enterprise-4.0.3/edx_enterprise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-21 16:55:36.000000 edx-enterprise-4.0.3/edx_enterprise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 16:55:36.000000 edx-enterprise-4.0.3/edx_enterprise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.009498 edx-enterprise-4.0.3/enterprise/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.009498 edx-enterprise-4.0.3/enterprise/admin/
--rw-r--r--   0 runner    (1001) docker     (123)    32944 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/admin/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30210 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/admin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/admin/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/admin/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.009498 edx-enterprise-4.0.3/enterprise/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/throttles.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.009498 edx-enterprise-4.0.3/enterprise/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    57862 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.013498 edx-enterprise-4.0.3/enterprise/api/v1/views/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/base_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/coupon_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_catalog_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_course_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer_branding_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer_invite_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    28693 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/pending_enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api/v1/views/plotly_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.013498 edx-enterprise-4.0.3/enterprise/api_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api_client/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api_client/ecommerce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api_client/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api_client/enterprise_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/api_client/lms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:36.997498 edx-enterprise-4.0.3/enterprise/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:36.997498 edx-enterprise-4.0.3/enterprise/conf/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:36.997498 edx-enterprise-4.0.3/enterprise/conf/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.013498 edx-enterprise-4.0.3/enterprise/conf/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/conf/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.013498 edx-enterprise-4.0.3/enterprise/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/config/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.013498 edx-enterprise-4.0.3/enterprise/heartbeat/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/heartbeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/heartbeat/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/heartbeat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/heartbeat/throttles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/heartbeat/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/heartbeat/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:36.997498 edx-enterprise-4.0.3/enterprise/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:36.997498 edx-enterprise-4.0.3/enterprise/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.013498 edx-enterprise-4.0.3/enterprise/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    41500 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:36.997498 edx-enterprise-4.0.3/enterprise/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.013498 edx-enterprise-4.0.3/enterprise/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   104293 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:36.997498 edx-enterprise-4.0.3/enterprise/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.017499 edx-enterprise-4.0.3/enterprise/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/locale/es_419/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    45236 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/locale/es_419/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.017499 edx-enterprise-4.0.3/enterprise/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.017499 edx-enterprise-4.0.3/enterprise/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/backfill_learner_role_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/bulk_update_catalog_query_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/create_enterprise_course_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/create_missing_dsc_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/email_drip_for_missing_dsc_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/fix_dsc_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/migrate_enterprise_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32481 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/monthly_impact_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/revert_enrollment_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/save_enterprise_customer_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/seed_enterprise_devstack_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/unlink_enterprise_customer_learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/update_config_last_errored_at.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/management/commands/update_role_assignments_with_customers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.025499 edx-enterprise-4.0.3/enterprise/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0001_auto_20210111_1253.py
--rw-r--r--   0 runner    (1001) docker     (123)    52500 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0095_auto_20200507_1138.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0096_enterprise_catalog_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0097_auto_20200619_1130.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0098_auto_20200629_1756.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0099_auto_20200702_1537.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0101_move_data_to_saved_for_later.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0102_auto_20200708_1615.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0103_remove_marked_done.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0104_sync_query_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0105_add_branding_config_color_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0106_move_branding_config_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0107_remove_branding_config_banner_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0110_add_default_contract_discount.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0112_auto_20200914_0926.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0113_auto_20200914_2054.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0114_auto_20201020_0142.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0116_auto_20201116_0400.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0116_auto_20201208_1759.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0117_auto_20201215_0258.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0124_auto_20210301_1309.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0125_add_config_for_role_assign_backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0126_auto_20210308_1522.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0127_enterprisecatalogquery_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0129_enterprisecatalogquery_uuid_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0130_lms_customer_lp_search_help_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0131_auto_20210517_0924.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0132_auto_20210608_1921.py
--rw-r--r--   0 runner    (1001) docker     (123)    26436 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0133_auto_20210608_1931.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0136_auto_20210629_2129.py
--rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0137_enrollment_email_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0139_auto_20210803_1854.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0140_update_enrollment_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0142_auto_20210907_2059.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0143_auto_20210908_0559.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0144_auto_20211011_1030.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0145_auto_20211013_1018.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0146_enterprise_customer_invite_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0147_auto_20211129_1949.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0148_auto_20211129_2114.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0150_invite_key_expiry_required.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0151_add_is_active_to_invite_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0152_add_should_inactivate_other_customers.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0153_add_enable_browse_and_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0156_add_is_active_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0157_make_field_nullable_before_removal.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0158_remove_is_active_from_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0159_add_enable_learner_portal_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0163_auto_20220928_1611.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0166_auto_20221209_0819.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0167_auto_20230209_2108.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0168_auto_20230222_1621.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0169_auto_20230222_1621.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0170_auto_20230301_1627.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0171_auto_20230503_1413.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0172_auto_20230517_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0173_auto_20230531_1459.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/0174_auto_20230608_2041.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/migrations/unique_constraints_pending_users.py
--rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/roles_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.025499 edx-enterprise-4.0.3/enterprise/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:36.997498 edx-enterprise-4.0.3/enterprise/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:36.997498 edx-enterprise-4.0.3/enterprise/static/enterprise/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.025499 edx-enterprise-4.0.3/enterprise/static/enterprise/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/static/enterprise/admin/enterprise_customer_catalog.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.025499 edx-enterprise-4.0.3/enterprise/static/enterprise/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/static/enterprise/bundles/main-admin.style.css
--rw-r--r--   0 runner    (1001) docker     (123)   295145 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/static/enterprise/bundles/main.style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.029499 edx-enterprise-4.0.3/enterprise/static/enterprise/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/static/enterprise/js/course_modal.js
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/static/enterprise/js/enterprise_customer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/static/enterprise/js/enterprise_login_page.js
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/static/enterprise/js/enterprise_selection_page.js
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/static/enterprise/js/grant_data_sharing_permissions.js
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/static/enterprise/js/manage_learners.js
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/static/enterprise/js/program_enrollment_landing_page.js
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:36.997498 edx-enterprise-4.0.3/enterprise/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.029499 edx-enterprise-4.0.3/enterprise/templates/enterprise/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/_data_sharing_decline_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/_data_sharing_policy.html
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/_data_sharing_top_paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/_data_sharing_user_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/_enterprise_customer_sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.029499 edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/enterprise_course_enrollments_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/manage_learners.html
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/oauth_authorization_failed.html
--rw-r--r--   0 runner    (1001) docker     (123)    27091 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/oauth_authorization_successful.html
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/transmit_courses_metadata.html
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/enterprise_course_enrollment_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/enterprise_customer_login_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/enterprise_customer_select_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/enterprise_error_page_with_messages.html
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/enterprise_program_enrollment_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/grant_data_sharing_permissions.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.029499 edx-enterprise-4.0.3/enterprise/templates/enterprise/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/templatetags/alert_messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/templatetags/course_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/templatetags/expand_button.html
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/templatetags/fa_icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.029499 edx-enterprise-4.0.3/enterprise/templates/enterprise/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templates/enterprise/widgets/segment-io-django.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.029499 edx-enterprise-4.0.3/enterprise/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/templatetags/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/tpa_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    85180 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise/views_error_codes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/enterprise_learner_portal/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/enterprise_learner_portal/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/enterprise_learner_portal/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/enterprise_learner_portal/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/enterprise_learner_portal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/integrated_channels/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/integrated_channels/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/integrated_channels/api/v1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/integrated_channels/api/v1/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/blackboard/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/blackboard/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/blackboard/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/integrated_channels/api/v1/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/canvas/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/canvas/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/canvas/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/integrated_channels/api/v1/cornerstone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/cornerstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/cornerstone/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/cornerstone/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/cornerstone/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.033499 edx-enterprise-4.0.3/integrated_channels/api/v1/degreed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/degreed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/degreed/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/degreed/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/degreed/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.037499 edx-enterprise-4.0.3/integrated_channels/api/v1/degreed2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/degreed2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/degreed2/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/degreed2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/degreed2/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.037499 edx-enterprise-4.0.3/integrated_channels/api/v1/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/logs/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/logs/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/logs/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.037499 edx-enterprise-4.0.3/integrated_channels/api/v1/moodle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/moodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/moodle/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/moodle/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/moodle/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.037499 edx-enterprise-4.0.3/integrated_channels/api/v1/sap_success_factors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/sap_success_factors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/sap_success_factors/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/sap_success_factors/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/sap_success_factors/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/api/v1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.037499 edx-enterprise-4.0.3/integrated_channels/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.037499 edx-enterprise-4.0.3/integrated_channels/blackboard/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40081 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.037499 edx-enterprise-4.0.3/integrated_channels/blackboard/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.041499 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.041499 edx-enterprise-4.0.3/integrated_channels/blackboard/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/blackboard/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.041499 edx-enterprise-4.0.3/integrated_channels/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.041499 edx-enterprise-4.0.3/integrated_channels/canvas/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    38929 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.041499 edx-enterprise-4.0.3/integrated_channels/canvas/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.045499 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0003_delete_canvasglobalconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.045499 edx-enterprise-4.0.3/integrated_channels/canvas/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/canvas/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/catalog_service_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.045499 edx-enterprise-4.0.3/integrated_channels/cornerstone/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.045499 edx-enterprise-4.0.3/integrated_channels/cornerstone/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.045499 edx-enterprise-4.0.3/integrated_channels/cornerstone/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.049499 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0002_cornerstoneglobalconfiguration_subject_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0004_cornerstoneglobalconfiguration_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0017_alter_cornerstonelearnerdatatransmissionaudit_course_completed.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.049499 edx-enterprise-4.0.3/integrated_channels/cornerstone/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/cornerstone/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.049499 edx-enterprise-4.0.3/integrated_channels/degreed/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.049499 edx-enterprise-4.0.3/integrated_channels/degreed/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.049499 edx-enterprise-4.0.3/integrated_channels/degreed/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.053499 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.053499 edx-enterprise-4.0.3/integrated_channels/degreed/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed/transmitters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.053499 edx-enterprise-4.0.3/integrated_channels/degreed2/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.053499 edx-enterprise-4.0.3/integrated_channels/degreed2/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.053499 edx-enterprise-4.0.3/integrated_channels/degreed2/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.057499 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0008_degreed2learnerdatatransmissionaudit_course_completed.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.057499 edx-enterprise-4.0.3/integrated_channels/degreed2/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/degreed2/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.057499 edx-enterprise-4.0.3/integrated_channels/integrated_channel/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.057499 edx-enterprise-4.0.3/integrated_channels/integrated_channel/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/channel_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.057499 edx-enterprise-4.0.3/integrated_channels/integrated_channel/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    39607 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.057499 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.061499 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.061499 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0002_learnerdatatransmissionaudit_subsection_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0005_auto_20211005_1052.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0006_contentmetadataitemtransmission_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0007_delete_learnerdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0011_contentmetadataitemtransmission_plugin_configuration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0012_alter_contentmetadataitemtransmission_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_content_title.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0019_merge_20220928_1842.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0021_remove_contentmetadataitemtransmission_api_response_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0024_genericenterprisecustomerpluginconfiguration_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32216 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.061499 edx-enterprise-4.0.3/integrated_channels/integrated_channel/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    23829 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/integrated_channel/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/lms_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.065500 edx-enterprise-4.0.3/integrated_channels/moodle/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.065500 edx-enterprise-4.0.3/integrated_channels/moodle/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.065500 edx-enterprise-4.0.3/integrated_channels/moodle/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.065500 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.065500 edx-enterprise-4.0.3/integrated_channels/moodle/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/moodle/transmitters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.069500 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.069500 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.069500 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/exporters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/exporters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.069500 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0009_sapsuccessfactorsenterprisecustomerconfiguration_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.069500 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/sap_success_factors/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17708 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.069500 edx-enterprise-4.0.3/integrated_channels/xapi/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.069500 edx-enterprise-4.0.3/integrated_channels/xapi/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.069500 edx-enterprise-4.0.3/integrated_channels/xapi/management/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.069500 edx-enterprise-4.0.3/integrated_channels/xapi/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/management/commands/send_course_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/management/commands/send_course_enrollments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.073500 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0004_auto_20190830_0710.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.073500 edx-enterprise-4.0.3/integrated_channels/xapi/statements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/statements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/statements/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/statements/learner_course_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/statements/learner_course_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/integrated_channels/xapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:37.073500 edx-enterprise-4.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/celery50.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/common_constraints.txt
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/doc.in
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/edx-platform-constraints.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/js_test.in
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/js_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/test-master.in
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/test-master.txt
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-21 16:55:37.077500 edx-enterprise-4.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4028 2023-07-21 16:54:16.000000 edx-enterprise-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.025142 edx-enterprise-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)   137642 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)   186547 2023-07-24 16:39:17.029142 edx-enterprise-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.933142 edx-enterprise-4.0.4/consent/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.933142 edx-enterprise-4.0.4/consent/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.933142 edx-enterprise-4.0.4/consent/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.933142 edx-enterprise-4.0.4/consent/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.933142 edx-enterprise-4.0.4/consent/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/migrations/0002_migrate_to_new_data_sharing_consent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/migrations/0003_historicaldatasharingconsent_history_change_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/migrations/0004_datasharingconsenttextoverrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/migrations/0005_auto_20230707_0755.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/consent/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.937142 edx-enterprise-4.0.4/edx_enterprise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)   186547 2023-07-24 16:39:16.000000 edx-enterprise-4.0.4/edx_enterprise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38935 2023-07-24 16:39:16.000000 edx-enterprise-4.0.4/edx_enterprise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:39:16.000000 edx-enterprise-4.0.4/edx_enterprise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:39:16.000000 edx-enterprise-4.0.4/edx_enterprise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-24 16:39:16.000000 edx-enterprise-4.0.4/edx_enterprise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 16:39:16.000000 edx-enterprise-4.0.4/edx_enterprise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.941142 edx-enterprise-4.0.4/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.941142 edx-enterprise-4.0.4/enterprise/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)    32944 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/admin/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30210 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/admin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/admin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/admin/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.941142 edx-enterprise-4.0.4/enterprise/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/throttles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.941142 edx-enterprise-4.0.4/enterprise/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57862 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.945142 edx-enterprise-4.0.4/enterprise/api/v1/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/base_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/coupon_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_catalog_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_course_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer_branding_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer_invite_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28693 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/pending_enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api/v1/views/plotly_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.945142 edx-enterprise-4.0.4/enterprise/api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api_client/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api_client/ecommerce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api_client/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api_client/enterprise_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/api_client/lms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.925142 edx-enterprise-4.0.4/enterprise/conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.925142 edx-enterprise-4.0.4/enterprise/conf/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.925142 edx-enterprise-4.0.4/enterprise/conf/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.945142 edx-enterprise-4.0.4/enterprise/conf/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/conf/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.945142 edx-enterprise-4.0.4/enterprise/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/config/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.949142 edx-enterprise-4.0.4/enterprise/heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/heartbeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/heartbeat/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/heartbeat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/heartbeat/throttles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/heartbeat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/heartbeat/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.925142 edx-enterprise-4.0.4/enterprise/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.925142 edx-enterprise-4.0.4/enterprise/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.949142 edx-enterprise-4.0.4/enterprise/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    41500 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.925142 edx-enterprise-4.0.4/enterprise/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.949142 edx-enterprise-4.0.4/enterprise/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   104293 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.925142 edx-enterprise-4.0.4/enterprise/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.949142 edx-enterprise-4.0.4/enterprise/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/locale/es_419/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    45236 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/locale/es_419/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.949142 edx-enterprise-4.0.4/enterprise/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.953142 edx-enterprise-4.0.4/enterprise/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/backfill_learner_role_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/bulk_update_catalog_query_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/create_enterprise_course_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/create_missing_dsc_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/email_drip_for_missing_dsc_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/fix_dsc_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/migrate_enterprise_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32481 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/monthly_impact_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/revert_enrollment_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/save_enterprise_customer_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/seed_enterprise_devstack_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/unlink_enterprise_customer_learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/update_config_last_errored_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/management/commands/update_role_assignments_with_customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.965142 edx-enterprise-4.0.4/enterprise/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0001_auto_20210111_1253.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52500 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0095_auto_20200507_1138.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0096_enterprise_catalog_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0097_auto_20200619_1130.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0098_auto_20200629_1756.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0099_auto_20200702_1537.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0101_move_data_to_saved_for_later.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0102_auto_20200708_1615.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0103_remove_marked_done.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0104_sync_query_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0105_add_branding_config_color_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0106_move_branding_config_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0107_remove_branding_config_banner_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0110_add_default_contract_discount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0112_auto_20200914_0926.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0113_auto_20200914_2054.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0114_auto_20201020_0142.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0116_auto_20201116_0400.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0116_auto_20201208_1759.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0117_auto_20201215_0258.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0124_auto_20210301_1309.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0125_add_config_for_role_assign_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0126_auto_20210308_1522.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0127_enterprisecatalogquery_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0129_enterprisecatalogquery_uuid_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0130_lms_customer_lp_search_help_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0131_auto_20210517_0924.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0132_auto_20210608_1921.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26436 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0133_auto_20210608_1931.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0136_auto_20210629_2129.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0137_enrollment_email_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0139_auto_20210803_1854.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0140_update_enrollment_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0142_auto_20210907_2059.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0143_auto_20210908_0559.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0144_auto_20211011_1030.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0145_auto_20211013_1018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0146_enterprise_customer_invite_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0147_auto_20211129_1949.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0148_auto_20211129_2114.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0150_invite_key_expiry_required.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0151_add_is_active_to_invite_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0152_add_should_inactivate_other_customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0153_add_enable_browse_and_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0156_add_is_active_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0157_make_field_nullable_before_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0158_remove_is_active_from_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0159_add_enable_learner_portal_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0163_auto_20220928_1611.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0166_auto_20221209_0819.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0167_auto_20230209_2108.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0168_auto_20230222_1621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0169_auto_20230222_1621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0170_auto_20230301_1627.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0171_auto_20230503_1413.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0172_auto_20230517_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0173_auto_20230531_1459.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/0174_auto_20230608_2041.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/migrations/unique_constraints_pending_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.965142 edx-enterprise-4.0.4/enterprise/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.925142 edx-enterprise-4.0.4/enterprise/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.925142 edx-enterprise-4.0.4/enterprise/static/enterprise/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.965142 edx-enterprise-4.0.4/enterprise/static/enterprise/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/static/enterprise/admin/enterprise_customer_catalog.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.965142 edx-enterprise-4.0.4/enterprise/static/enterprise/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/static/enterprise/bundles/main-admin.style.css
+-rw-r--r--   0 runner    (1001) docker     (123)   295145 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/static/enterprise/bundles/main.style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.965142 edx-enterprise-4.0.4/enterprise/static/enterprise/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/static/enterprise/js/course_modal.js
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/static/enterprise/js/enterprise_customer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/static/enterprise/js/enterprise_login_page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/static/enterprise/js/enterprise_selection_page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/static/enterprise/js/grant_data_sharing_permissions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/static/enterprise/js/manage_learners.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/static/enterprise/js/program_enrollment_landing_page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.925142 edx-enterprise-4.0.4/enterprise/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.969142 edx-enterprise-4.0.4/enterprise/templates/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/_data_sharing_decline_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/_data_sharing_policy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/_data_sharing_top_paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/_data_sharing_user_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/_enterprise_customer_sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.969142 edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/enterprise_course_enrollments_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/manage_learners.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/oauth_authorization_failed.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27091 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/oauth_authorization_successful.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/transmit_courses_metadata.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/enterprise_course_enrollment_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/enterprise_customer_login_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/enterprise_customer_select_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/enterprise_error_page_with_messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/enterprise_program_enrollment_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/grant_data_sharing_permissions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.969142 edx-enterprise-4.0.4/enterprise/templates/enterprise/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/templatetags/alert_messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/templatetags/course_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/templatetags/expand_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/templatetags/fa_icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.969142 edx-enterprise-4.0.4/enterprise/templates/enterprise/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templates/enterprise/widgets/segment-io-django.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.969142 edx-enterprise-4.0.4/enterprise/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/templatetags/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/tpa_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85180 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise/views_error_codes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.969142 edx-enterprise-4.0.4/enterprise_learner_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.969142 edx-enterprise-4.0.4/enterprise_learner_portal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.969142 edx-enterprise-4.0.4/enterprise_learner_portal/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.973142 edx-enterprise-4.0.4/enterprise_learner_portal/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/enterprise_learner_portal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.973142 edx-enterprise-4.0.4/integrated_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.973142 edx-enterprise-4.0.4/integrated_channels/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.973142 edx-enterprise-4.0.4/integrated_channels/api/v1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.973142 edx-enterprise-4.0.4/integrated_channels/api/v1/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/blackboard/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/blackboard/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/blackboard/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.973142 edx-enterprise-4.0.4/integrated_channels/api/v1/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/canvas/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/canvas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/canvas/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.973142 edx-enterprise-4.0.4/integrated_channels/api/v1/cornerstone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/cornerstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/cornerstone/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/cornerstone/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/cornerstone/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.973142 edx-enterprise-4.0.4/integrated_channels/api/v1/degreed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/degreed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/degreed/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/degreed/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/degreed/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.977142 edx-enterprise-4.0.4/integrated_channels/api/v1/degreed2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/degreed2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/degreed2/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/degreed2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/degreed2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.977142 edx-enterprise-4.0.4/integrated_channels/api/v1/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/logs/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/logs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/logs/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.977142 edx-enterprise-4.0.4/integrated_channels/api/v1/moodle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/moodle/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/moodle/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/moodle/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.977142 edx-enterprise-4.0.4/integrated_channels/api/v1/sap_success_factors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/sap_success_factors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/sap_success_factors/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/sap_success_factors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/sap_success_factors/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/api/v1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.977142 edx-enterprise-4.0.4/integrated_channels/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.977142 edx-enterprise-4.0.4/integrated_channels/blackboard/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40081 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.977142 edx-enterprise-4.0.4/integrated_channels/blackboard/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.981142 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.981142 edx-enterprise-4.0.4/integrated_channels/blackboard/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/blackboard/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.981142 edx-enterprise-4.0.4/integrated_channels/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.981142 edx-enterprise-4.0.4/integrated_channels/canvas/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38929 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.981142 edx-enterprise-4.0.4/integrated_channels/canvas/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.985142 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0003_delete_canvasglobalconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.989142 edx-enterprise-4.0.4/integrated_channels/canvas/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/canvas/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/catalog_service_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.989142 edx-enterprise-4.0.4/integrated_channels/cornerstone/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.989142 edx-enterprise-4.0.4/integrated_channels/cornerstone/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.989142 edx-enterprise-4.0.4/integrated_channels/cornerstone/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.993142 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0002_cornerstoneglobalconfiguration_subject_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0004_cornerstoneglobalconfiguration_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0017_alter_cornerstonelearnerdatatransmissionaudit_course_completed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.993142 edx-enterprise-4.0.4/integrated_channels/cornerstone/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/cornerstone/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.993142 edx-enterprise-4.0.4/integrated_channels/degreed/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.993142 edx-enterprise-4.0.4/integrated_channels/degreed/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.993142 edx-enterprise-4.0.4/integrated_channels/degreed/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.997142 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.997142 edx-enterprise-4.0.4/integrated_channels/degreed/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed/transmitters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.997142 edx-enterprise-4.0.4/integrated_channels/degreed2/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:16.997142 edx-enterprise-4.0.4/integrated_channels/degreed2/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.001142 edx-enterprise-4.0.4/integrated_channels/degreed2/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.001142 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0008_degreed2learnerdatatransmissionaudit_course_completed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.001142 edx-enterprise-4.0.4/integrated_channels/degreed2/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/degreed2/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.005142 edx-enterprise-4.0.4/integrated_channels/integrated_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.005142 edx-enterprise-4.0.4/integrated_channels/integrated_channel/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/channel_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.005142 edx-enterprise-4.0.4/integrated_channels/integrated_channel/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39607 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.005142 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.005142 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/remove_null_catalog_transmission_audits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.013142 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0002_learnerdatatransmissionaudit_subsection_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0005_auto_20211005_1052.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0006_contentmetadataitemtransmission_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0007_delete_learnerdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0011_contentmetadataitemtransmission_plugin_configuration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0012_alter_contentmetadataitemtransmission_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_content_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0019_merge_20220928_1842.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0021_remove_contentmetadataitemtransmission_api_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0024_genericenterprisecustomerpluginconfiguration_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32216 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20241 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.013142 edx-enterprise-4.0.4/integrated_channels/integrated_channel/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23829 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/integrated_channel/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/lms_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.013142 edx-enterprise-4.0.4/integrated_channels/moodle/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.013142 edx-enterprise-4.0.4/integrated_channels/moodle/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.013142 edx-enterprise-4.0.4/integrated_channels/moodle/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.017142 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.017142 edx-enterprise-4.0.4/integrated_channels/moodle/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/moodle/transmitters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.017142 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.017142 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.017142 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/exporters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/exporters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.021142 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0009_sapsuccessfactorsenterprisecustomerconfiguration_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.021142 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/sap_success_factors/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17708 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.021142 edx-enterprise-4.0.4/integrated_channels/xapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.021142 edx-enterprise-4.0.4/integrated_channels/xapi/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.021142 edx-enterprise-4.0.4/integrated_channels/xapi/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.021142 edx-enterprise-4.0.4/integrated_channels/xapi/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/management/commands/send_course_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/management/commands/send_course_enrollments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.025142 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0004_auto_20190830_0710.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.025142 edx-enterprise-4.0.4/integrated_channels/xapi/statements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/statements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/statements/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/statements/learner_course_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/statements/learner_course_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/integrated_channels/xapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:17.025142 edx-enterprise-4.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/celery50.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/common_constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/doc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    28799 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/edx-platform-constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/js_test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/js_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/test-master.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/test-master.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-24 16:39:17.029142 edx-enterprise-4.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4028 2023-07-24 16:37:59.000000 edx-enterprise-4.0.4/setup.py
```

### Comparing `edx-enterprise-4.0.3/CHANGELOG.rst` & `edx-enterprise-4.0.4/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[4.0.4]
+--------
+feat: remove content transmission audits without a catalog uuid
+
 [4.0.3]
 -------
 fix: changing sap transmit metadata flow to account for rate limiting
 
 [4.0.2]
 -------
 fix: removing items to delete dependency on the catalog service
```

### Comparing `edx-enterprise-4.0.3/LICENSE` & `edx-enterprise-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/PKG-INFO` & `edx-enterprise-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-enterprise
-Version: 4.0.3
+Version: 4.0.4
 Summary: Your project description goes here
 Home-page: https://github.com/openedx/edx-enterprise
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: enterprise
         ==========
@@ -90,14 +90,18 @@
         
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ----------
+        [4.0.4]
+        --------
+        feat: remove content transmission audits without a catalog uuid
+        
         [4.0.3]
         -------
         fix: changing sap transmit metadata flow to account for rate limiting
         
         [4.0.2]
         -------
         fix: removing items to delete dependency on the catalog service
```

### Comparing `edx-enterprise-4.0.3/README.rst` & `edx-enterprise-4.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/__init__.py` & `edx-enterprise-4.0.4/consent/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/admin/__init__.py` & `edx-enterprise-4.0.4/consent/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/api/permissions.py` & `edx-enterprise-4.0.4/consent/api/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/api/v1/views.py` & `edx-enterprise-4.0.4/consent/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/errors.py` & `edx-enterprise-4.0.4/consent/errors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/helpers.py` & `edx-enterprise-4.0.4/consent/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/migrations/0001_initial.py` & `edx-enterprise-4.0.4/consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/migrations/0002_migrate_to_new_data_sharing_consent.py` & `edx-enterprise-4.0.4/consent/migrations/0002_migrate_to_new_data_sharing_consent.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/migrations/0004_datasharingconsenttextoverrides.py` & `edx-enterprise-4.0.4/consent/migrations/0004_datasharingconsenttextoverrides.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/migrations/0005_auto_20230707_0755.py` & `edx-enterprise-4.0.4/consent/migrations/0005_auto_20230707_0755.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/mixins.py` & `edx-enterprise-4.0.4/consent/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/consent/models.py` & `edx-enterprise-4.0.4/consent/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/edx_enterprise.egg-info/PKG-INFO` & `edx-enterprise-4.0.4/edx_enterprise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-enterprise
-Version: 4.0.3
+Version: 4.0.4
 Summary: Your project description goes here
 Home-page: https://github.com/openedx/edx-enterprise
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: enterprise
         ==========
@@ -90,14 +90,18 @@
         
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ----------
+        [4.0.4]
+        --------
+        feat: remove content transmission audits without a catalog uuid
+        
         [4.0.3]
         -------
         fix: changing sap transmit metadata flow to account for rate limiting
         
         [4.0.2]
         -------
         fix: removing items to delete dependency on the catalog service
```

### Comparing `edx-enterprise-4.0.3/edx_enterprise.egg-info/SOURCES.txt` & `edx-enterprise-4.0.4/edx_enterprise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -506,14 +506,15 @@
 integrated_channels/integrated_channel/management/commands/__init__.py
 integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py
 integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py
 integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py
 integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py
 integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py
 integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py
+integrated_channels/integrated_channel/management/commands/remove_null_catalog_transmission_audits.py
 integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py
 integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py
 integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py
 integrated_channels/integrated_channel/management/commands/transmit_learner_data.py
 integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py
 integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py
 integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py
```

### Comparing `edx-enterprise-4.0.3/edx_enterprise.egg-info/requires.txt` & `edx-enterprise-4.0.4/edx_enterprise.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/admin/__init__.py` & `edx-enterprise-4.0.4/enterprise/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/admin/actions.py` & `edx-enterprise-4.0.4/enterprise/admin/actions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/admin/forms.py` & `edx-enterprise-4.0.4/enterprise/admin/forms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/admin/paginator.py` & `edx-enterprise-4.0.4/enterprise/admin/paginator.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/admin/utils.py` & `edx-enterprise-4.0.4/enterprise/admin/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/admin/views.py` & `edx-enterprise-4.0.4/enterprise/admin/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/__init__.py` & `edx-enterprise-4.0.4/enterprise/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/filters.py` & `edx-enterprise-4.0.4/enterprise/api/filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/pagination.py` & `edx-enterprise-4.0.4/enterprise/api/pagination.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/throttles.py` & `edx-enterprise-4.0.4/enterprise/api/throttles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/utils.py` & `edx-enterprise-4.0.4/enterprise/api/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/decorators.py` & `edx-enterprise-4.0.4/enterprise/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/fields.py` & `edx-enterprise-4.0.4/enterprise/api/v1/fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/permissions.py` & `edx-enterprise-4.0.4/enterprise/api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/serializers.py` & `edx-enterprise-4.0.4/enterprise/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/urls.py` & `edx-enterprise-4.0.4/enterprise/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/base_views.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/base_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/coupon_codes.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/coupon_codes.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_catalog_query.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_catalog_query.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_course_enrollment.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer_branding_configuration.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer_branding_configuration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer_catalog.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer_catalog.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer_invite_key.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer_invite_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer_reporting.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer_reporting.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_customer_user.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/notifications.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/notifications.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/pending_enterprise_customer_user.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/pending_enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api/v1/views/plotly_auth.py` & `edx-enterprise-4.0.4/enterprise/api/v1/views/plotly_auth.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api_client/client.py` & `edx-enterprise-4.0.4/enterprise/api_client/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api_client/discovery.py` & `edx-enterprise-4.0.4/enterprise/api_client/discovery.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api_client/ecommerce.py` & `edx-enterprise-4.0.4/enterprise/api_client/ecommerce.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api_client/enterprise.py` & `edx-enterprise-4.0.4/enterprise/api_client/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api_client/enterprise_catalog.py` & `edx-enterprise-4.0.4/enterprise/api_client/enterprise_catalog.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/api_client/lms.py` & `edx-enterprise-4.0.4/enterprise/api_client/lms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/apps.py` & `edx-enterprise-4.0.4/enterprise/apps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/conf/locale/en/LC_MESSAGES/django.po` & `edx-enterprise-4.0.4/enterprise/conf/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/config/models.py` & `edx-enterprise-4.0.4/enterprise/config/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/constants.py` & `edx-enterprise-4.0.4/enterprise/constants.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/decorators.py` & `edx-enterprise-4.0.4/enterprise/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/errors.py` & `edx-enterprise-4.0.4/enterprise/errors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/forms.py` & `edx-enterprise-4.0.4/enterprise/forms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/heartbeat/checks.py` & `edx-enterprise-4.0.4/enterprise/heartbeat/checks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/heartbeat/exceptions.py` & `edx-enterprise-4.0.4/enterprise/heartbeat/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/heartbeat/utils.py` & `edx-enterprise-4.0.4/enterprise/heartbeat/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/heartbeat/views.py` & `edx-enterprise-4.0.4/enterprise/heartbeat/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/locale/en/LC_MESSAGES/django.po` & `edx-enterprise-4.0.4/enterprise/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/locale/en/LC_MESSAGES/djangojs.po` & `edx-enterprise-4.0.4/enterprise/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/locale/eo/LC_MESSAGES/django.po` & `edx-enterprise-4.0.4/enterprise/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/locale/eo/LC_MESSAGES/djangojs.po` & `edx-enterprise-4.0.4/enterprise/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/locale/es_419/LC_MESSAGES/django.mo` & `edx-enterprise-4.0.4/enterprise/locale/es_419/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/locale/es_419/LC_MESSAGES/django.po` & `edx-enterprise-4.0.4/enterprise/locale/es_419/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/logging.py` & `edx-enterprise-4.0.4/enterprise/logging.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/backfill_learner_role_assignments.py` & `edx-enterprise-4.0.4/enterprise/management/commands/backfill_learner_role_assignments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/bulk_update_catalog_query_id.py` & `edx-enterprise-4.0.4/enterprise/management/commands/bulk_update_catalog_query_id.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/create_enterprise_course_enrollments.py` & `edx-enterprise-4.0.4/enterprise/management/commands/create_enterprise_course_enrollments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/create_missing_dsc_records.py` & `edx-enterprise-4.0.4/enterprise/management/commands/create_missing_dsc_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/email_drip_for_missing_dsc_records.py` & `edx-enterprise-4.0.4/enterprise/management/commands/email_drip_for_missing_dsc_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py` & `edx-enterprise-4.0.4/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/fix_dsc_records.py` & `edx-enterprise-4.0.4/enterprise/management/commands/fix_dsc_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/migrate_enterprise_catalogs.py` & `edx-enterprise-4.0.4/enterprise/management/commands/migrate_enterprise_catalogs.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/monthly_impact_report.py` & `edx-enterprise-4.0.4/enterprise/management/commands/monthly_impact_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py` & `edx-enterprise-4.0.4/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/revert_enrollment_objects.py` & `edx-enterprise-4.0.4/enterprise/management/commands/revert_enrollment_objects.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/save_enterprise_customer_users.py` & `edx-enterprise-4.0.4/enterprise/management/commands/save_enterprise_customer_users.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/seed_enterprise_devstack_data.py` & `edx-enterprise-4.0.4/enterprise/management/commands/seed_enterprise_devstack_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/unlink_enterprise_customer_learners.py` & `edx-enterprise-4.0.4/enterprise/management/commands/unlink_enterprise_customer_learners.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/update_config_last_errored_at.py` & `edx-enterprise-4.0.4/enterprise/management/commands/update_config_last_errored_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/management/commands/update_role_assignments_with_customers.py` & `edx-enterprise-4.0.4/enterprise/management/commands/update_role_assignments_with_customers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/messages.py` & `edx-enterprise-4.0.4/enterprise/messages.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/middleware.py` & `edx-enterprise-4.0.4/enterprise/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0001_auto_20210111_1253.py` & `edx-enterprise-4.0.4/enterprise/migrations/0001_auto_20210111_1253.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py` & `edx-enterprise-4.0.4/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py` & `edx-enterprise-4.0.4/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py` & `edx-enterprise-4.0.4/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0095_auto_20200507_1138.py` & `edx-enterprise-4.0.4/enterprise/migrations/0095_auto_20200507_1138.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0096_enterprise_catalog_admin_role.py` & `edx-enterprise-4.0.4/enterprise/migrations/0096_enterprise_catalog_admin_role.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0097_auto_20200619_1130.py` & `edx-enterprise-4.0.4/enterprise/migrations/0097_auto_20200619_1130.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0098_auto_20200629_1756.py` & `edx-enterprise-4.0.4/enterprise/migrations/0098_auto_20200629_1756.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0099_auto_20200702_1537.py` & `edx-enterprise-4.0.4/enterprise/migrations/0099_auto_20200702_1537.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py` & `edx-enterprise-4.0.4/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0101_move_data_to_saved_for_later.py` & `edx-enterprise-4.0.4/enterprise/migrations/0101_move_data_to_saved_for_later.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0102_auto_20200708_1615.py` & `edx-enterprise-4.0.4/enterprise/migrations/0102_auto_20200708_1615.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0104_sync_query_field.py` & `edx-enterprise-4.0.4/enterprise/migrations/0104_sync_query_field.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0105_add_branding_config_color_fields.py` & `edx-enterprise-4.0.4/enterprise/migrations/0105_add_branding_config_color_fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0106_move_branding_config_colors.py` & `edx-enterprise-4.0.4/enterprise/migrations/0106_move_branding_config_colors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0107_remove_branding_config_banner_fields.py` & `edx-enterprise-4.0.4/enterprise/migrations/0107_remove_branding_config_banner_fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py` & `edx-enterprise-4.0.4/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py` & `edx-enterprise-4.0.4/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0110_add_default_contract_discount.py` & `edx-enterprise-4.0.4/enterprise/migrations/0110_add_default_contract_discount.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py` & `edx-enterprise-4.0.4/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0112_auto_20200914_0926.py` & `edx-enterprise-4.0.4/enterprise/migrations/0112_auto_20200914_0926.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0113_auto_20200914_2054.py` & `edx-enterprise-4.0.4/enterprise/migrations/0113_auto_20200914_2054.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0114_auto_20201020_0142.py` & `edx-enterprise-4.0.4/enterprise/migrations/0114_auto_20201020_0142.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py` & `edx-enterprise-4.0.4/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0116_auto_20201116_0400.py` & `edx-enterprise-4.0.4/enterprise/migrations/0116_auto_20201116_0400.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0116_auto_20201208_1759.py` & `edx-enterprise-4.0.4/enterprise/migrations/0116_auto_20201208_1759.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0117_auto_20201215_0258.py` & `edx-enterprise-4.0.4/enterprise/migrations/0117_auto_20201215_0258.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py` & `edx-enterprise-4.0.4/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py` & `edx-enterprise-4.0.4/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py` & `edx-enterprise-4.0.4/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py` & `edx-enterprise-4.0.4/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0124_auto_20210301_1309.py` & `edx-enterprise-4.0.4/enterprise/migrations/0124_auto_20210301_1309.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0125_add_config_for_role_assign_backfill.py` & `edx-enterprise-4.0.4/enterprise/migrations/0125_add_config_for_role_assign_backfill.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0126_auto_20210308_1522.py` & `edx-enterprise-4.0.4/enterprise/migrations/0126_auto_20210308_1522.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py` & `edx-enterprise-4.0.4/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0130_lms_customer_lp_search_help_text.py` & `edx-enterprise-4.0.4/enterprise/migrations/0130_lms_customer_lp_search_help_text.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0131_auto_20210517_0924.py` & `edx-enterprise-4.0.4/enterprise/migrations/0131_auto_20210517_0924.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0132_auto_20210608_1921.py` & `edx-enterprise-4.0.4/enterprise/migrations/0132_auto_20210608_1921.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0133_auto_20210608_1931.py` & `edx-enterprise-4.0.4/enterprise/migrations/0133_auto_20210608_1931.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py` & `edx-enterprise-4.0.4/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py` & `edx-enterprise-4.0.4/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0136_auto_20210629_2129.py` & `edx-enterprise-4.0.4/enterprise/migrations/0136_auto_20210629_2129.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0137_enrollment_email_update.py` & `edx-enterprise-4.0.4/enterprise/migrations/0137_enrollment_email_update.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py` & `edx-enterprise-4.0.4/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0139_auto_20210803_1854.py` & `edx-enterprise-4.0.4/enterprise/migrations/0139_auto_20210803_1854.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0140_update_enrollment_sources.py` & `edx-enterprise-4.0.4/enterprise/migrations/0140_update_enrollment_sources.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py` & `edx-enterprise-4.0.4/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0142_auto_20210907_2059.py` & `edx-enterprise-4.0.4/enterprise/migrations/0142_auto_20210907_2059.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0143_auto_20210908_0559.py` & `edx-enterprise-4.0.4/enterprise/migrations/0143_auto_20210908_0559.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0144_auto_20211011_1030.py` & `edx-enterprise-4.0.4/enterprise/migrations/0144_auto_20211011_1030.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0145_auto_20211013_1018.py` & `edx-enterprise-4.0.4/enterprise/migrations/0145_auto_20211013_1018.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0146_enterprise_customer_invite_key.py` & `edx-enterprise-4.0.4/enterprise/migrations/0146_enterprise_customer_invite_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0147_auto_20211129_1949.py` & `edx-enterprise-4.0.4/enterprise/migrations/0147_auto_20211129_1949.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0148_auto_20211129_2114.py` & `edx-enterprise-4.0.4/enterprise/migrations/0148_auto_20211129_2114.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py` & `edx-enterprise-4.0.4/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0150_invite_key_expiry_required.py` & `edx-enterprise-4.0.4/enterprise/migrations/0150_invite_key_expiry_required.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0151_add_is_active_to_invite_key.py` & `edx-enterprise-4.0.4/enterprise/migrations/0151_add_is_active_to_invite_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0152_add_should_inactivate_other_customers.py` & `edx-enterprise-4.0.4/enterprise/migrations/0152_add_should_inactivate_other_customers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0153_add_enable_browse_and_request.py` & `edx-enterprise-4.0.4/enterprise/migrations/0153_add_enable_browse_and_request.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py` & `edx-enterprise-4.0.4/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py` & `edx-enterprise-4.0.4/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0156_add_is_active_role_assignment.py` & `edx-enterprise-4.0.4/enterprise/migrations/0156_add_is_active_role_assignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0157_make_field_nullable_before_removal.py` & `edx-enterprise-4.0.4/enterprise/migrations/0157_make_field_nullable_before_removal.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0158_remove_is_active_from_role_assignment.py` & `edx-enterprise-4.0.4/enterprise/migrations/0158_remove_is_active_from_role_assignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0159_add_enable_learner_portal_offers.py` & `edx-enterprise-4.0.4/enterprise/migrations/0159_add_enable_learner_portal_offers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py` & `edx-enterprise-4.0.4/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py` & `edx-enterprise-4.0.4/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py` & `edx-enterprise-4.0.4/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0163_auto_20220928_1611.py` & `edx-enterprise-4.0.4/enterprise/migrations/0163_auto_20220928_1611.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py` & `edx-enterprise-4.0.4/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py` & `edx-enterprise-4.0.4/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0166_auto_20221209_0819.py` & `edx-enterprise-4.0.4/enterprise/migrations/0166_auto_20221209_0819.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0167_auto_20230209_2108.py` & `edx-enterprise-4.0.4/enterprise/migrations/0167_auto_20230209_2108.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0168_auto_20230222_1621.py` & `edx-enterprise-4.0.4/enterprise/migrations/0168_auto_20230222_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0169_auto_20230222_1621.py` & `edx-enterprise-4.0.4/enterprise/migrations/0169_auto_20230222_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0170_auto_20230301_1627.py` & `edx-enterprise-4.0.4/enterprise/migrations/0170_auto_20230301_1627.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0171_auto_20230503_1413.py` & `edx-enterprise-4.0.4/enterprise/migrations/0171_auto_20230503_1413.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0172_auto_20230517_1550.py` & `edx-enterprise-4.0.4/enterprise/migrations/0172_auto_20230517_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0173_auto_20230531_1459.py` & `edx-enterprise-4.0.4/enterprise/migrations/0173_auto_20230531_1459.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/0174_auto_20230608_2041.py` & `edx-enterprise-4.0.4/enterprise/migrations/0174_auto_20230608_2041.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/migrations/unique_constraints_pending_users.py` & `edx-enterprise-4.0.4/enterprise/migrations/unique_constraints_pending_users.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/models.py` & `edx-enterprise-4.0.4/enterprise/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/roles_api.py` & `edx-enterprise-4.0.4/enterprise/roles_api.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/rules.py` & `edx-enterprise-4.0.4/enterprise/rules.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/settings/test.py` & `edx-enterprise-4.0.4/enterprise/settings/test.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/signals.py` & `edx-enterprise-4.0.4/enterprise/signals.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/static/enterprise/admin/enterprise_customer_catalog.js` & `edx-enterprise-4.0.4/enterprise/static/enterprise/admin/enterprise_customer_catalog.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/static/enterprise/bundles/main.style.css` & `edx-enterprise-4.0.4/enterprise/static/enterprise/bundles/main.style.css`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/static/enterprise/js/course_modal.js` & `edx-enterprise-4.0.4/enterprise/static/enterprise/js/course_modal.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/static/enterprise/js/enterprise_customer.js` & `edx-enterprise-4.0.4/enterprise/static/enterprise/js/enterprise_customer.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/static/enterprise/js/enterprise_login_page.js` & `edx-enterprise-4.0.4/enterprise/static/enterprise/js/enterprise_login_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/static/enterprise/js/enterprise_selection_page.js` & `edx-enterprise-4.0.4/enterprise/static/enterprise/js/enterprise_selection_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/static/enterprise/js/grant_data_sharing_permissions.js` & `edx-enterprise-4.0.4/enterprise/static/enterprise/js/grant_data_sharing_permissions.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/static/enterprise/js/manage_learners.js` & `edx-enterprise-4.0.4/enterprise/static/enterprise/js/manage_learners.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/static/enterprise/js/program_enrollment_landing_page.js` & `edx-enterprise-4.0.4/enterprise/static/enterprise/js/program_enrollment_landing_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/tasks.py` & `edx-enterprise-4.0.4/enterprise/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/_data_sharing_decline_modal.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/_data_sharing_decline_modal.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/_data_sharing_top_paragraph.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/_data_sharing_top_paragraph.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/_data_sharing_user_input.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/_data_sharing_user_input.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/_enterprise_customer_sidebar.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/_enterprise_customer_sidebar.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/manage_learners.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/manage_learners.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/oauth_authorization_failed.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/oauth_authorization_failed.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/oauth_authorization_successful.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/oauth_authorization_successful.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/admin/transmit_courses_metadata.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/admin/transmit_courses_metadata.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/base.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/base.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/enterprise_course_enrollment_page.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/enterprise_course_enrollment_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/enterprise_customer_login_page.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/enterprise_customer_login_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/enterprise_customer_select_form.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/enterprise_customer_select_form.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/enterprise_program_enrollment_page.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/enterprise_program_enrollment_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/grant_data_sharing_permissions.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/grant_data_sharing_permissions.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/templatetags/course_modal.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/templatetags/course_modal.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templates/enterprise/widgets/segment-io-django.html` & `edx-enterprise-4.0.4/enterprise/templates/enterprise/widgets/segment-io-django.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/templatetags/enterprise.py` & `edx-enterprise-4.0.4/enterprise/templatetags/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/tpa_pipeline.py` & `edx-enterprise-4.0.4/enterprise/tpa_pipeline.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/urls.py` & `edx-enterprise-4.0.4/enterprise/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/utils.py` & `edx-enterprise-4.0.4/enterprise/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/validators.py` & `edx-enterprise-4.0.4/enterprise/validators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/views.py` & `edx-enterprise-4.0.4/enterprise/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise/views_error_codes.txt` & `edx-enterprise-4.0.4/enterprise/views_error_codes.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise_learner_portal/api/v1/serializers.py` & `edx-enterprise-4.0.4/enterprise_learner_portal/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise_learner_portal/api/v1/views.py` & `edx-enterprise-4.0.4/enterprise_learner_portal/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/enterprise_learner_portal/utils.py` & `edx-enterprise-4.0.4/enterprise_learner_portal/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/serializers.py` & `edx-enterprise-4.0.4/integrated_channels/api/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/blackboard/serializers.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/blackboard/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/blackboard/views.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/blackboard/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/canvas/serializers.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/canvas/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/canvas/views.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/canvas/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/cornerstone/serializers.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/cornerstone/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/cornerstone/views.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/cornerstone/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/degreed/serializers.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/degreed/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/degreed/views.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/degreed/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/degreed2/serializers.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/degreed2/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/degreed2/views.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/degreed2/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/logs/serializers.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/logs/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/logs/urls.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/logs/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/logs/views.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/logs/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/mixins.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/moodle/serializers.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/moodle/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/moodle/views.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/moodle/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/sap_success_factors/serializers.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/sap_success_factors/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/sap_success_factors/views.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/sap_success_factors/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/urls.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/api/v1/views.py` & `edx-enterprise-4.0.4/integrated_channels/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/admin/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/apps.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/apps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/client.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/exporters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/exporters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/models.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/transmitters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/transmitters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/blackboard/views.py` & `edx-enterprise-4.0.4/integrated_channels/blackboard/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/admin/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/client.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/exporters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/exporters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0001_initial.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/models.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/transmitters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/transmitters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/utils.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/canvas/views.py` & `edx-enterprise-4.0.4/integrated_channels/canvas/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/catalog_service_utils.py` & `edx-enterprise-4.0.4/integrated_channels/catalog_service_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/admin/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/client.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/exporters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/exporters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0001_initial.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/models.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/transmitters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/transmitters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/utils.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/cornerstone/views.py` & `edx-enterprise-4.0.4/integrated_channels/cornerstone/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/admin/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/client.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/exporters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/exporters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0001_initial.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/models.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/transmitters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed/transmitters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/degreed/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/admin/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/client.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/exporters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/exporters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0001_initial.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/models.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/transmitters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/degreed2/transmitters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/degreed2/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/admin/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/channel_settings.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/channel_settings.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/client.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/exporters/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/exporters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/exporters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/models.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/tasks.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,39 @@
             duration_seconds=duration_seconds,
             details=extra_message
         ))
 
 
 @shared_task
 @set_code_owner_attribute
+def remove_null_catalog_transmission_audits():
+    """
+    Task to remove content transmission audit records that do not contain a catalog UUID.
+    """
+    start = time.time()
+
+    _log_batch_task_start('remove_null_catalog_transmission_audits', None, None, None)
+
+    deleted_null_catalog_uuids = ContentMetadataItemTransmission.objects.filter(
+        enterprise_customer_catalog_uuid=None
+    ).delete()
+
+    duration_seconds = time.time() - start
+    _log_batch_task_finish(
+        'remove_null_catalog_transmission_audits',
+        channel_code=None,
+        job_user_id=None,
+        integrated_channel_full_config=None,
+        duration_seconds=duration_seconds,
+        extra_message=f"{deleted_null_catalog_uuids[0]} transmission audits with no catalog UUIDs removed"
+    )
+
+
+@shared_task
+@set_code_owner_attribute
 def remove_duplicate_transmission_audits():
     """
     Task to remove duplicate transmission audits, keeping the most recently modified one.
     """
     start = time.time()
     _log_batch_task_start('remove_duplicate_transsmision_audits', None, None, None)
     unique_transmissions = ContentMetadataItemTransmission.objects.values_list(
```

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/transmitters/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/transmitters/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/transmitters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/integrated_channel/transmitters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/integrated_channel/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/lms_utils.py` & `edx-enterprise-4.0.4/integrated_channels/lms_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/admin/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/client.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/exporters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/exporters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0001_initial.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/models.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/transmitters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/moodle/transmitters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/moodle/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/admin/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/client.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/constants.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/constants.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/exporters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/exporters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/exporters/utils.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/models.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/transmitters/content_metadata.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/sap_success_factors/transmitters/learner_data.py` & `edx-enterprise-4.0.4/integrated_channels/sap_success_factors/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/utils.py` & `edx-enterprise-4.0.4/integrated_channels/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/admin/__init__.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/client.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/management/commands/send_course_completions.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/management/commands/send_course_completions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/management/commands/send_course_enrollments.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/management/commands/send_course_enrollments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0001_initial.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/models.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/statements/base.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/statements/base.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/statements/learner_course_completion.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/statements/learner_course_completion.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/statements/learner_course_enrollment.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/statements/learner_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/integrated_channels/xapi/utils.py` & `edx-enterprise-4.0.4/integrated_channels/xapi/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/requirements/base.in` & `edx-enterprise-4.0.4/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/requirements/ci.txt` & `edx-enterprise-4.0.4/requirements/ci.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    make upgrade
 #
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via tox
-platformdirs==3.2.0
+platformdirs==3.9.1
     # via virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via tox
 py==1.11.0
     # via tox
 six==1.16.0
     # via tox
 tomli==2.0.1
     # via tox
@@ -26,9 +26,9 @@
     # via
     #   -c requirements/common_constraints.txt
     #   -c requirements/constraints.txt
     #   -r requirements/ci.in
     #   tox-battery
 tox-battery==0.6.1
     # via -r requirements/ci.in
-virtualenv==20.21.0
+virtualenv==20.24.1
     # via tox
```

### Comparing `edx-enterprise-4.0.3/requirements/common_constraints.txt` & `edx-enterprise-4.0.4/requirements/common_constraints.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+
 # A central location for most common version constraints
 # (across edx repos) for pip-installation.
 #
 # Similar to other constraint files this file doesn't install any packages.
 # It specifies version constraints that will be applied if a package is needed.
 # When pinning something here, please provide an explanation of why it is a good
 # idea to pin this package across all edx repos, Ideally, link to other information
```

### Comparing `edx-enterprise-4.0.3/requirements/constraints.txt` & `edx-enterprise-4.0.4/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/requirements/dev.in` & `edx-enterprise-4.0.4/requirements/dev.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.3/requirements/dev.txt` & `edx-enterprise-4.0.4/requirements/dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,66 +20,73 @@
     #   kombu
 aniso8601==9.0.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-tincan-py35
-asgiref==3.6.0
+asgiref==3.7.2
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   django
     #   django-countries
 asn1crypto==1.5.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   oscrypto
     #   snowflake-connector-python
-astroid==2.15.3
+astroid==2.15.6
     # via
     #   pylint
     #   pylint-celery
 attrs==23.1.0
     # via
     #   -r requirements/test.txt
     #   pytest
 babel==2.12.1
     # via
     #   -r requirements/doc.txt
     #   pydata-sphinx-theme
     #   sphinx
+backports-zoneinfo[tzdata]==0.2.1
+    # via
+    #   -r requirements/doc.txt
+    #   -r requirements/test-master.txt
+    #   -r requirements/test.txt
+    #   celery
+    #   kombu
 beautifulsoup4==4.12.2
     # via
     #   -r requirements/doc.txt
     #   pydata-sphinx-theme
 billiard==4.1.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   celery
-bleach[css]==6.0.0
+bleach==6.0.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   readme-renderer
 build==0.10.0
     # via pip-tools
 celery==5.3.1
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
@@ -97,15 +104,15 @@
 charset-normalizer==2.0.12
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   requests
     #   snowflake-connector-python
-click==8.1.5
+click==8.1.6
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   celery
     #   click-didyoumean
     #   click-log
@@ -125,27 +132,27 @@
     # via edx-lint
 click-plugins==1.1.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   celery
-click-repl==0.2.0
+click-repl==0.3.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   celery
 code-annotations==1.3.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-lint
-coverage[toml]==7.2.3
+coverage[toml]==7.2.7
     # via
     #   -r requirements/test.txt
     #   pytest-cov
 cryptography==38.0.4
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
@@ -159,21 +166,21 @@
     # via -r requirements/test.txt
 defusedxml==0.7.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   djangorestframework-xml
-diff-cover==7.5.0
+diff-cover==7.7.0
     # via -r requirements/test.txt
 dill==0.3.6
     # via pylint
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-django==3.2.18
+django==3.2.20
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   django-config-models
     #   django-crum
@@ -211,15 +218,15 @@
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields==0.6
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
-django-filter==23.1
+django-filter==23.2
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
 django-ipware==4.0.2
     # via
     #   -r requirements/doc.txt
@@ -227,15 +234,15 @@
     #   -r requirements/test.txt
 django-model-utils==4.3.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-rbac
-django-multi-email-field==0.6.2
+django-multi-email-field==0.7.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
 django-object-actions==4.1.0
     # via
     #   -r requirements/doc.txt
@@ -250,15 +257,15 @@
 django-waffle==3.0.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.12.4
+djangorestframework==3.14.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   django-config-models
     #   drf-jwt
     #   edx-drf-extensions
@@ -279,91 +286,85 @@
     #   sphinx
 drf-jwt==1.19.2
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-drf-extensions
-edx-django-utils==5.4.0
+edx-django-utils==5.5.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   django-config-models
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==8.6.0
+edx-drf-extensions==8.8.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-rbac
-edx-i18n-tools==0.9.2
+edx-i18n-tools==1.0.0
     # via -r requirements/dev.in
 edx-lint==5.3.4
     # via -r requirements/dev.in
 edx-opaque-keys[django]==2.3.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
-edx-rest-api-client==5.5.0
+edx-rest-api-client==5.5.2
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
 edx-tincan-py35==1.0.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
-factory-boy==3.2.1
+factory-boy==3.3.0
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.txt
-faker==18.4.0
+faker==19.2.0
     # via
     #   -r requirements/test.txt
     #   factory-boy
-filelock==3.11.0
+filelock==3.12.2
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   snowflake-connector-python
     #   tox
     #   virtualenv
 freezegun==0.3.14
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.txt
-future==0.18.3
-    # via
-    #   -r requirements/doc.txt
-    #   -r requirements/test-master.txt
-    #   -r requirements/test.txt
-    #   pyjwkest
 idna==3.4
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   requests
     #   snowflake-connector-python
 imagesize==1.4.1
     # via
     #   -r requirements/doc.txt
     #   sphinx
-importlib-metadata==6.4.1
+importlib-metadata==6.8.0
     # via
     #   -r requirements/doc.txt
     #   sphinx
 iniconfig==2.0.0
     # via
     #   -r requirements/test.txt
     #   pytest
@@ -393,27 +394,27 @@
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   celery
 lazy-object-proxy==1.9.0
     # via astroid
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   jinja2
 mccabe==0.7.0
     # via pylint
 mock==3.0.5
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.txt
-newrelic==8.8.0
+newrelic==8.8.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-django-utils
 oscrypto==1.3.0
     # via
@@ -428,15 +429,15 @@
     #   -r requirements/test.txt
     #   build
     #   pydata-sphinx-theme
     #   pytest
     #   snowflake-connector-python
     #   sphinx
     #   tox
-path==16.6.0
+path==16.7.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-i18n-tools
     #   path-py
 path-py==12.5.0
@@ -456,33 +457,31 @@
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
 pillow==9.5.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
-pip-tools==7.0.0
-    # via
-    #   -c requirements/constraints.txt
-    #   -r requirements/dev.in
+pip-tools==7.1.0
+    # via -r requirements/dev.in
 pkginfo==1.9.6
     # via twine
-platformdirs==3.2.0
+platformdirs==3.9.1
     # via
     #   pylint
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   -r requirements/test.txt
     #   diff-cover
     #   pytest
     #   tox
 polib==1.2.0
     # via edx-i18n-tools
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   click-repl
 psutil==5.9.5
     # via
@@ -491,77 +490,70 @@
     #   -r requirements/test.txt
     #   edx-django-utils
 py==1.11.0
     # via
     #   -r requirements/test.txt
     #   pytest
     #   tox
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   pgpy
 pycodestyle==2.10.0
     # via -r requirements/dev.in
 pycparser==2.21
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   cffi
-pycryptodomex==3.17
+pycryptodomex==3.18.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
-    #   pyjwkest
     #   snowflake-connector-python
 pydata-sphinx-theme==0.13.3
     # via
     #   -r requirements/doc.txt
     #   sphinx-book-theme
 pydocstyle==6.3.0
     # via -r requirements/dev.in
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   accessible-pygments
     #   diff-cover
     #   doc8
     #   pydata-sphinx-theme
     #   readme-renderer
     #   sphinx
-pyjwkest==1.4.2
-    # via
-    #   -r requirements/doc.txt
-    #   -r requirements/test-master.txt
-    #   -r requirements/test.txt
-    #   edx-drf-extensions
-pyjwt[crypto]==2.6.0
+pyjwt[crypto]==2.7.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
-pylint==2.17.2
+pylint==2.17.4
     # via
     #   edx-lint
     #   pylint-celery
     #   pylint-django
     #   pylint-plugin-utils
 pylint-celery==0.3
     # via edx-lint
 pylint-django==2.5.3
     # via edx-lint
-pylint-plugin-utils==0.7
+pylint-plugin-utils==0.8.2
     # via
     #   pylint-celery
     #   pylint-django
 pymongo==3.13.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
@@ -583,23 +575,24 @@
     # via build
 pytest==6.2.5
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.txt
     #   pytest-cov
     #   pytest-django
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r requirements/test.txt
 pytest-django==4.5.2
     # via -r requirements/test.txt
 python-dateutil==2.8.2
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
+    #   celery
     #   edx-drf-extensions
     #   faker
     #   freezegun
 python-slugify==8.0.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
@@ -607,42 +600,41 @@
     #   code-annotations
 pytz==2022.7.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   babel
-    #   celery
     #   django
+    #   djangorestframework
     #   edx-tincan-py35
     #   snowflake-connector-python
 pyyaml==6.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   code-annotations
     #   edx-i18n-tools
-readme-renderer==37.3
+readme-renderer==40.0
     # via -r requirements/doc.txt
-requests==2.28.2
+requests==2.31.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-drf-extensions
     #   edx-rest-api-client
-    #   pyjwkest
     #   requests-toolbelt
     #   responses
     #   slumber
     #   snowflake-connector-python
     #   sphinx
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 responses==0.10.15
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.txt
 restructuredtext-lint==1.4.0
     # via
@@ -661,40 +653,44 @@
     #   edx-drf-extensions
 six==1.16.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   bleach
-    #   click-repl
     #   edx-drf-extensions
     #   edx-lint
     #   edx-rbac
     #   freezegun
     #   mock
-    #   pyjwkest
     #   python-dateutil
     #   responses
     #   tox
 slumber==0.7.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   edx-rest-api-client
 snowballstemmer==2.2.0
     # via
     #   -r requirements/doc.txt
     #   pydocstyle
     #   sphinx
-snowflake-connector-python==3.0.2
+snowflake-connector-python==3.0.4
+    # via
+    #   -r requirements/doc.txt
+    #   -r requirements/test-master.txt
+    #   -r requirements/test.txt
+sortedcontainers==2.4.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
+    #   snowflake-connector-python
 soupsieve==2.4.1
     # via
     #   -r requirements/doc.txt
     #   beautifulsoup4
 sphinx==5.3.0
     # via
     #   -c requirements/common_constraints.txt
@@ -723,21 +719,21 @@
     # via
     #   -r requirements/doc.txt
     #   sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via
     #   -r requirements/doc.txt
     #   sphinx
-sqlparse==0.4.3
+sqlparse==0.4.4
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   django
-stevedore==5.0.0
+stevedore==5.1.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   code-annotations
     #   doc8
     #   edx-django-utils
@@ -750,100 +746,104 @@
     #   -r requirements/test.txt
 text-unidecode==1.3
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   python-slugify
-tinycss2==1.1.1
-    # via
-    #   -r requirements/doc.txt
-    #   -r requirements/test-master.txt
-    #   -r requirements/test.txt
-    #   bleach
 toml==0.10.2
     # via
     #   -r requirements/test.txt
     #   pytest
 tomli==2.0.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   build
     #   coverage
     #   doc8
+    #   pip-tools
     #   pylint
     #   pyproject-hooks
     #   tox
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via pylint
 tox==3.28.0
     # via
     #   -c requirements/common_constraints.txt
     #   -c requirements/constraints.txt
     #   -r requirements/dev.in
     #   tox-battery
 tox-battery==0.6.1
     # via -r requirements/dev.in
 tqdm==4.65.0
     # via twine
 twine==1.11.0
     # via -r requirements/dev.in
-typing-extensions==4.5.0
+typing-extensions==4.7.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
+    #   asgiref
     #   astroid
     #   django-countries
+    #   faker
+    #   kombu
     #   pydata-sphinx-theme
     #   pylint
     #   snowflake-connector-python
+tzdata==2023.3
+    # via
+    #   -r requirements/doc.txt
+    #   -r requirements/test-master.txt
+    #   -r requirements/test.txt
+    #   backports-zoneinfo
+    #   celery
 unicodecsv==0.14.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   requests
     #   snowflake-connector-python
 vine==5.0.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   amqp
     #   celery
     #   kombu
-virtualenv==20.21.0
+virtualenv==20.24.1
     # via tox
 wcwidth==0.2.6
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   prompt-toolkit
 webencodings==0.5.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test-master.txt
     #   -r requirements/test.txt
     #   bleach
-    #   tinycss2
 wheel==0.40.0
     # via
     #   -r requirements/dev.in
     #   pip-tools
 wrapt==1.15.0
     # via astroid
-zipp==3.15.0
+zipp==3.16.2
     # via
     #   -r requirements/doc.txt
     #   importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `edx-enterprise-4.0.3/requirements/doc.txt` & `edx-enterprise-4.0.4/requirements/doc.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,43 +12,48 @@
     # via
     #   -r requirements/test-master.txt
     #   kombu
 aniso8601==9.0.1
     # via
     #   -r requirements/test-master.txt
     #   edx-tincan-py35
-asgiref==3.6.0
+asgiref==3.7.2
     # via
     #   -r requirements/test-master.txt
     #   django
     #   django-countries
 asn1crypto==1.5.1
     # via
     #   -r requirements/test-master.txt
     #   oscrypto
     #   snowflake-connector-python
 babel==2.12.1
     # via
     #   pydata-sphinx-theme
     #   sphinx
+backports-zoneinfo[tzdata]==0.2.1
+    # via
+    #   -r requirements/test-master.txt
+    #   celery
+    #   kombu
 beautifulsoup4==4.12.2
     # via pydata-sphinx-theme
 billiard==4.1.0
     # via
     #   -r requirements/test-master.txt
     #   celery
-bleach[css]==6.0.0
+bleach==6.0.0
     # via
     #   -r requirements/test-master.txt
     #   readme-renderer
 celery==5.3.1
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test-master.txt
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   -r requirements/test-master.txt
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
     # via
     #   -r requirements/test-master.txt
@@ -56,15 +61,15 @@
     #   pynacl
     #   snowflake-connector-python
 charset-normalizer==2.0.12
     # via
     #   -r requirements/test-master.txt
     #   requests
     #   snowflake-connector-python
-click==8.1.5
+click==8.1.6
     # via
     #   -r requirements/test-master.txt
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   code-annotations
@@ -73,15 +78,15 @@
     # via
     #   -r requirements/test-master.txt
     #   celery
 click-plugins==1.1.1
     # via
     #   -r requirements/test-master.txt
     #   celery
-click-repl==0.2.0
+click-repl==0.3.0
     # via
     #   -r requirements/test-master.txt
     #   celery
 code-annotations==1.3.0
     # via -r requirements/test-master.txt
 cryptography==38.0.4
     # via
@@ -91,15 +96,15 @@
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
 defusedxml==0.7.1
     # via
     #   -r requirements/test-master.txt
     #   djangorestframework-xml
-django==3.2.18
+django==3.2.20
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/test-master.txt
     #   django-config-models
     #   django-crum
     #   django-fernet-fields
     #   django-filter
@@ -120,36 +125,36 @@
 django-crum==0.7.9
     # via
     #   -r requirements/test-master.txt
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields==0.6
     # via -r requirements/test-master.txt
-django-filter==23.1
+django-filter==23.2
     # via -r requirements/test-master.txt
 django-ipware==4.0.2
     # via -r requirements/test-master.txt
 django-model-utils==4.3.1
     # via
     #   -r requirements/test-master.txt
     #   edx-rbac
-django-multi-email-field==0.6.2
+django-multi-email-field==0.7.0
     # via -r requirements/test-master.txt
 django-object-actions==4.1.0
     # via -r requirements/test-master.txt
 django-simple-history==3.0.0
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/test-master.txt
 django-waffle==3.0.0
     # via
     #   -r requirements/test-master.txt
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.12.4
+djangorestframework==3.14.0
     # via
     #   -r requirements/test-master.txt
     #   django-config-models
     #   drf-jwt
     #   edx-drf-extensions
 djangorestframework-xml==2.0.0
     # via -r requirements/test-master.txt
@@ -163,131 +168,122 @@
     #   readme-renderer
     #   restructuredtext-lint
     #   sphinx
 drf-jwt==1.19.2
     # via
     #   -r requirements/test-master.txt
     #   edx-drf-extensions
-edx-django-utils==5.4.0
+edx-django-utils==5.5.0
     # via
     #   -r requirements/test-master.txt
     #   django-config-models
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==8.6.0
+edx-drf-extensions==8.8.0
     # via
     #   -r requirements/test-master.txt
     #   edx-rbac
 edx-opaque-keys[django]==2.3.0
     # via
     #   -r requirements/test-master.txt
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/test-master.txt
-edx-rest-api-client==5.5.0
+edx-rest-api-client==5.5.2
     # via -r requirements/test-master.txt
 edx-tincan-py35==1.0.0
     # via -r requirements/test-master.txt
-filelock==3.11.0
+filelock==3.12.2
     # via
     #   -r requirements/test-master.txt
     #   snowflake-connector-python
-future==0.18.3
-    # via
-    #   -r requirements/test-master.txt
-    #   pyjwkest
 idna==3.4
     # via
     #   -r requirements/test-master.txt
     #   requests
     #   snowflake-connector-python
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.4.1
+importlib-metadata==6.8.0
     # via sphinx
 jinja2==3.1.2
     # via
     #   -r requirements/test-master.txt
     #   code-annotations
     #   sphinx
 jsondiff==2.0.0
     # via -r requirements/test-master.txt
 jsonfield==3.1.0
     # via -r requirements/test-master.txt
 kombu==5.3.1
     # via
     #   -r requirements/test-master.txt
     #   celery
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   -r requirements/test-master.txt
     #   jinja2
-newrelic==8.8.0
+newrelic==8.8.1
     # via
     #   -r requirements/test-master.txt
     #   edx-django-utils
 oscrypto==1.3.0
     # via
     #   -r requirements/test-master.txt
     #   snowflake-connector-python
 packaging==23.1
     # via
     #   -r requirements/test-master.txt
     #   pydata-sphinx-theme
     #   snowflake-connector-python
     #   sphinx
-path==16.6.0
+path==16.7.1
     # via
     #   -r requirements/test-master.txt
     #   path-py
 path-py==12.5.0
     # via -r requirements/test-master.txt
 pbr==5.11.1
     # via
     #   -r requirements/test-master.txt
     #   stevedore
 pgpy==0.6.0
     # via -r requirements/test-master.txt
 pillow==9.5.0
     # via -r requirements/test-master.txt
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via
     #   -r requirements/test-master.txt
     #   click-repl
 psutil==5.9.5
     # via
     #   -r requirements/test-master.txt
     #   edx-django-utils
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   -r requirements/test-master.txt
     #   pgpy
 pycparser==2.21
     # via
     #   -r requirements/test-master.txt
     #   cffi
-pycryptodomex==3.17
+pycryptodomex==3.18.0
     # via
     #   -r requirements/test-master.txt
-    #   pyjwkest
     #   snowflake-connector-python
 pydata-sphinx-theme==0.13.3
     # via sphinx-book-theme
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   accessible-pygments
     #   doc8
     #   pydata-sphinx-theme
     #   readme-renderer
     #   sphinx
-pyjwkest==1.4.2
-    # via
-    #   -r requirements/test-master.txt
-    #   edx-drf-extensions
-pyjwt[crypto]==2.6.0
+pyjwt[crypto]==2.7.0
     # via
     #   -r requirements/test-master.txt
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
 pymongo==3.13.0
@@ -301,39 +297,39 @@
 pyopenssl==22.0.0
     # via
     #   -r requirements/test-master.txt
     #   snowflake-connector-python
 python-dateutil==2.8.2
     # via
     #   -r requirements/test-master.txt
+    #   celery
     #   edx-drf-extensions
 python-slugify==8.0.1
     # via
     #   -r requirements/test-master.txt
     #   code-annotations
 pytz==2022.7.1
     # via
     #   -r requirements/test-master.txt
     #   babel
-    #   celery
     #   django
+    #   djangorestframework
     #   edx-tincan-py35
     #   snowflake-connector-python
 pyyaml==6.0
     # via
     #   -r requirements/test-master.txt
     #   code-annotations
-readme-renderer==37.3
+readme-renderer==40.0
     # via -r requirements/doc.in
-requests==2.28.2
+requests==2.31.0
     # via
     #   -r requirements/test-master.txt
     #   edx-drf-extensions
     #   edx-rest-api-client
-    #   pyjwkest
     #   slumber
     #   snowflake-connector-python
     #   sphinx
 restructuredtext-lint==1.4.0
     # via doc8
 rules==3.3
     # via -r requirements/test-master.txt
@@ -341,27 +337,29 @@
     # via
     #   -r requirements/test-master.txt
     #   edx-drf-extensions
 six==1.16.0
     # via
     #   -r requirements/test-master.txt
     #   bleach
-    #   click-repl
     #   edx-drf-extensions
     #   edx-rbac
-    #   pyjwkest
     #   python-dateutil
 slumber==0.7.1
     # via
     #   -r requirements/test-master.txt
     #   edx-rest-api-client
 snowballstemmer==2.2.0
     # via sphinx
-snowflake-connector-python==3.0.2
+snowflake-connector-python==3.0.4
     # via -r requirements/test-master.txt
+sortedcontainers==2.4.0
+    # via
+    #   -r requirements/test-master.txt
+    #   snowflake-connector-python
 soupsieve==2.4.1
     # via beautifulsoup4
 sphinx==5.3.0
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/doc.in
     #   pydata-sphinx-theme
@@ -376,46 +374,49 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlparse==0.4.3
+sqlparse==0.4.4
     # via
     #   -r requirements/test-master.txt
     #   django
-stevedore==5.0.0
+stevedore==5.1.0
     # via
     #   -r requirements/test-master.txt
     #   code-annotations
     #   doc8
     #   edx-django-utils
     #   edx-opaque-keys
 testfixtures==7.1.0
     # via -r requirements/test-master.txt
 text-unidecode==1.3
     # via
     #   -r requirements/test-master.txt
     #   python-slugify
-tinycss2==1.1.1
-    # via
-    #   -r requirements/test-master.txt
-    #   bleach
 tomli==2.0.1
     # via doc8
-typing-extensions==4.5.0
+typing-extensions==4.7.1
     # via
     #   -r requirements/test-master.txt
+    #   asgiref
     #   django-countries
+    #   kombu
     #   pydata-sphinx-theme
     #   snowflake-connector-python
+tzdata==2023.3
+    # via
+    #   -r requirements/test-master.txt
+    #   backports-zoneinfo
+    #   celery
 unicodecsv==0.14.1
     # via -r requirements/test-master.txt
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   -r requirements/test-master.txt
     #   requests
     #   snowflake-connector-python
 vine==5.0.0
     # via
     #   -r requirements/test-master.txt
@@ -426,10 +427,9 @@
     # via
     #   -r requirements/test-master.txt
     #   prompt-toolkit
 webencodings==0.5.1
     # via
     #   -r requirements/test-master.txt
     #   bleach
-    #   tinycss2
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-metadata
```

### Comparing `edx-enterprise-4.0.3/requirements/edx-platform-constraints.txt` & `edx-enterprise-4.0.4/requirements/edx-platform-constraints.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,102 +2,105 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    make upgrade
 #
 acid-xblock==0.2.1
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 aiohttp==3.8.4
     # via geoip2
 aiosignal==1.3.1
     # via aiohttp
 algoliasearch==2.6.3
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/bundled.in
     # via kombu
 analytics-python==1.4.post1
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 aniso8601==9.0.1
     # via edx-tincan-py35
 appdirs==1.4.4
     # via fs
-asgiref==3.6.0
+asgiref==3.7.2
     # via
     #   django
     #   django-countries
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
 async-timeout==4.0.2
     # via
     #   aiohttp
     #   redis
 attrs==23.1.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   aiohttp
     #   edx-ace
     #   jsonschema
     #   lti-consumer-xblock
     #   openedx-blockstore
     #   openedx-events
+    #   referencing
 babel==2.11.0
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   enmerkar
     #   enmerkar-underscore
 backoff==1.10.0
     # via analytics-python
-backports-zoneinfo==0.2.1
-    # via icalendar
+backports-zoneinfo[tzdata]==0.2.1
+    # via
+    #   celery
+    #   icalendar
+    #   kombu
 beautifulsoup4==4.12.2
     # via pynliner
     # via celery
 bleach[css]==6.0.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-enterprise
     #   lti-consumer-xblock
     #   openedx-django-wiki
     #   ora2
     #   xblock-drag-and-drop-v2
     #   xblock-poll
 boto==2.39.0
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
-    #   edxval
+    #   -r requirements/edx/kernel.in
 boto3==1.7.0
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   django-ses
     #   fs-s3fs
     #   ora2
 botocore==1.10.84
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   boto3
     #   s3transfer
 bridgekeeper==0.9
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   django-celery-results
     #   django-user-tasks
     #   edx-celeryutils
     #   edx-enterprise
     #   event-tracking
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   -r requirements/edx/paver.txt
     #   elasticsearch
     #   py2neo
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
@@ -111,15 +114,15 @@
     # via
     #   -c requirements/edx/../constraints.txt
     #   -r requirements/edx/paver.txt
     #   aiohttp
     #   requests
     #   snowflake-connector-python
 chem==1.2.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
     # via
     #   -c requirements/edx/../constraints.txt
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   code-annotations
@@ -131,55 +134,52 @@
     # via celery
     # via celery
 code-annotations==1.3.0
     # via
     #   edx-enterprise
     #   edx-toggles
 codejail-includes==1.0.0
-    # via -r requirements/edx/base.in
-contextlib2==21.6.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 coreapi==2.3.3
     # via drf-yasg
 coreschema==0.0.4
     # via
     #   coreapi
     #   drf-yasg
 crowdsourcehinter-xblock==0.6
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/bundled.in
 cryptography==38.0.4
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   django-fernet-fields
     #   djfernet
     #   edx-enterprise
     #   jwcrypto
     #   optimizely-sdk
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
     #   social-auth-core
-cssutils==2.6.0
+cssutils==2.7.1
     # via pynliner
 defusedxml==0.7.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   djangorestframework-xml
     #   ora2
     #   python3-openid
-    #   python3-saml
     #   social-auth-core
-deprecated==1.2.13
+deprecated==1.2.14
     # via jwcrypto
-django==3.2.18
+django==3.2.20
     # via
     #   -c requirements/edx/../common_constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   django-appconf
     #   django-celery-results
     #   django-classy-tags
     #   django-config-models
     #   django-cors-headers
     #   django-crum
     #   django-fernet-fields
@@ -208,14 +208,15 @@
     #   edx-completion
     #   edx-django-release-util
     #   edx-django-sites-extensions
     #   edx-django-utils
     #   edx-drf-extensions
     #   edx-enterprise
     #   edx-event-bus-kafka
+    #   edx-event-bus-redis
     #   edx-i18n-tools
     #   edx-milestones
     #   edx-name-affirmation
     #   edx-organizations
     #   edx-proctoring
     #   edx-rbac
     #   edx-search
@@ -234,72 +235,68 @@
     #   openedx-blockstore
     #   openedx-django-pyfs
     #   openedx-django-wiki
     #   openedx-events
     #   openedx-filters
     #   ora2
     #   outcome-surveys
+    #   skill-tagging
     #   super-csv
     #   xss-utils
 django-appconf==1.0.5
-    # via
-    #   -r requirements/edx/base.in
-    #   django-statici18n
+    # via django-statici18n
 django-cache-memoize==0.1.10
-django-celery-results==2.5.0
-    # via -r requirements/edx/base.in
+django-celery-results==2.5.1
+    # via -r requirements/edx/kernel.in
 django-classy-tags==4.0.0
     # via django-sekizai
 django-config-models==2.3.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-enterprise
     #   edx-name-affirmation
     #   lti-consumer-xblock
-django-cors-headers==3.14.0
-    # via -r requirements/edx/base.in
+django-cors-headers==4.2.0
+    # via -r requirements/edx/kernel.in
 django-countries==7.5.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-enterprise
 django-crum==0.7.9
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-django-utils
     #   edx-enterprise
     #   edx-proctoring
     #   edx-rbac
     #   edx-toggles
     #   super-csv
 django-environ==0.10.0
     # via openedx-blockstore
 django-fernet-fields==0.6
+django-filter==23.2
     # via
-    #   -r requirements/edx/base.in
-    #   edx-enterprise
-django-filter==23.1
-    # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-enterprise
     #   learner-pathway-progress
     #   lti-consumer-xblock
     #   openedx-blockstore
 django-ipware==4.0.2
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-enterprise
     #   edx-proctoring
-django-js-asset==2.0.0
+django-js-asset==2.1.0
     # via django-mptt
 django-method-override==1.0.4
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 django-model-utils==4.3.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   django-user-tasks
     #   edx-bulk-grades
     #   edx-celeryutils
     #   edx-completion
     #   edx-enterprise
     #   edx-milestones
     #   edx-name-affirmation
@@ -308,77 +305,80 @@
     #   edx-rbac
     #   edx-submissions
     #   edx-when
     #   edxval
     #   learner-pathway-progress
     #   ora2
     #   outcome-surveys
+    #   skill-tagging
     #   super-csv
 django-mptt==0.14.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   openedx-django-wiki
-django-multi-email-field==0.6.2
-django-mysql==4.9.0
-    # via -r requirements/edx/base.in
+django-multi-email-field==0.7.0
+django-mysql==4.11.0
+    # via -r requirements/edx/kernel.in
 django-oauth-toolkit==1.3.2
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
 django-object-actions==4.1.0
 django-pipeline==2.1.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 django-ratelimit==4.0.0
-    # via -r requirements/edx/base.in
-django-sekizai==4.0.0
+    # via -r requirements/edx/kernel.in
+django-sekizai==4.1.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   openedx-django-wiki
-django-ses==3.3.0
-    # via -r requirements/edx/base.in
+django-ses==3.5.0
+    # via -r requirements/edx/bundled.in
 django-simple-history==3.0.0
     # via
     #   -c requirements/edx/../common_constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-enterprise
     #   edx-name-affirmation
     #   edx-organizations
     #   edx-proctoring
     #   learner-pathway-progress
     #   ora2
-django-splash==1.2.1
-    # via -r requirements/edx/base.in
+django-splash==1.3.0
+    # via -r requirements/edx/kernel.in
 django-statici18n==2.3.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
+    #   lti-consumer-xblock
     #   xblock-drag-and-drop-v2
-django-storages==1.8
+django-storages==1.9.1
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edxval
 django-user-tasks==3.0.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 django-waffle==3.0.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-django-utils
     #   edx-drf-extensions
     #   edx-enterprise
     #   edx-proctoring
     #   edx-toggles
     #   openedx-blockstore
 django-webpack-loader==0.7.0
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-proctoring
-djangorestframework==3.12.4
+djangorestframework==3.14.0
     # via
-    #   -r requirements/edx/base.in
+    #   -c requirements/edx/../constraints.txt
+    #   -r requirements/edx/kernel.in
     #   django-config-models
     #   django-user-tasks
     #   drf-jwt
     #   drf-nested-routers
     #   drf-yasg
     #   edx-api-doc-tools
     #   edx-completion
@@ -391,105 +391,111 @@
     #   learner-pathway-progress
     #   openedx-blockstore
     #   ora2
     #   super-csv
 djangorestframework-xml==2.0.0
 djfernet==0.8.1
     # via edxval
-docopt==0.6.2
-    # via -r requirements/edx/base.in
 docutils==0.19
-    # via botocore
+    # via
+    #   -c requirements/edx/../constraints.txt
+    #   botocore
 done-xblock==2.0.5
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/bundled.in
 drf-jwt==1.19.2
     # via edx-drf-extensions
 drf-nested-routers==0.93.4
     # via openedx-blockstore
 drf-yasg==1.21.5
-    # via edx-api-doc-tools
+    # via
+    #   -c requirements/edx/../constraints.txt
+    #   edx-api-doc-tools
 edx-ace==1.6.1
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 edx-api-doc-tools==1.6.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-name-affirmation
     #   openedx-blockstore
 edx-auth-backends==4.1.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   openedx-blockstore
-edx-braze-client==0.1.6
-    # via -r requirements/edx/base.in
+edx-braze-client==0.1.7
+    # via -r requirements/edx/bundled.in
 edx-bulk-grades==1.0.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   staff-graded-xblock
 edx-ccx-keys==1.2.1
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 edx-celeryutils==1.2.2
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-name-affirmation
     #   super-csv
 edx-codejail==3.3.3
-    # via -r requirements/edx/base.in
-edx-completion==4.2.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
+edx-completion==4.2.1
+    # via -r requirements/edx/kernel.in
 edx-django-release-util==1.2.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
+    #   edxval
     #   openedx-blockstore
 edx-django-sites-extensions==4.0.0
-    # via -r requirements/edx/base.in
-edx-django-utils==5.4.0
+    # via -r requirements/edx/kernel.in
+edx-django-utils==5.5.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   django-config-models
     #   edx-drf-extensions
     #   edx-enterprise
     #   edx-event-bus-kafka
+    #   edx-event-bus-redis
     #   edx-name-affirmation
     #   edx-rest-api-client
     #   edx-toggles
     #   edx-when
     #   event-tracking
     #   learner-pathway-progress
     #   openedx-blockstore
     #   ora2
     #   outcome-surveys
     #   super-csv
-edx-drf-extensions==8.6.0
+edx-drf-extensions==8.8.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-completion
     #   edx-enterprise
     #   edx-name-affirmation
     #   edx-organizations
     #   edx-proctoring
     #   edx-rbac
     #   edx-when
     #   edxval
     #   learner-pathway-progress
-edx-enterprise==3.61.11
+edx-enterprise==4.0.2
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   learner-pathway-progress
-edx-event-bus-kafka==3.9.6
-    # via -r requirements/edx/base.in
-edx-i18n-tools==0.9.2
+edx-event-bus-kafka==5.1.0
+    # via -r requirements/edx/kernel.in
+edx-event-bus-redis==0.3.1
+    # via -r requirements/edx/kernel.in
+edx-i18n-tools==1.0.0
     # via ora2
 edx-milestones==0.4.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 edx-name-affirmation==2.3.5
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 edx-opaque-keys[django]==2.3.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   -r requirements/edx/paver.txt
     #   edx-bulk-grades
     #   edx-ccx-keys
     #   edx-completion
     #   edx-drf-extensions
     #   edx-enterprise
     #   edx-milestones
@@ -499,292 +505,296 @@
     #   edx-when
     #   learner-pathway-progress
     #   lti-consumer-xblock
     #   openedx-events
     #   ora2
     #   outcome-surveys
 edx-organizations==6.11.1
-    # via -r requirements/edx/base.in
-edx-proctoring==4.15.0
+    # via -r requirements/edx/kernel.in
+edx-proctoring==4.16.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-proctoring-proctortrack
 edx-proctoring-proctortrack==1.0.5
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 edx-rbac==1.7.0
-edx-rest-api-client==5.5.0
+edx-rest-api-client==5.5.2
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-enterprise
     #   edx-proctoring
-edx-search==3.5.0
-    # via -r requirements/edx/base.in
-edx-sga==0.21.1
-    # via -r requirements/edx/base.in
-edx-submissions==3.5.4
+edx-search==3.6.0
+    # via -r requirements/edx/kernel.in
+edx-sga==0.22.0
+    # via -r requirements/edx/bundled.in
+edx-submissions==3.5.6
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   ora2
 edx-tincan-py35==1.0.0
 edx-toggles==5.0.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-completion
     #   edx-event-bus-kafka
+    #   edx-event-bus-redis
     #   edx-name-affirmation
     #   edx-search
     #   edxval
     #   learner-pathway-progress
     #   ora2
 edx-token-utils==0.2.1
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 edx-user-state-client==1.3.2
-    # via -r requirements/edx/base.in
-edx-when==2.3.0
+    # via -r requirements/edx/kernel.in
+edx-when==2.4.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-proctoring
-edxval==2.2.0
-    # via -r requirements/edx/base.in
+edxval==2.3.0
+    # via -r requirements/edx/kernel.in
 elasticsearch==7.13.4
     # via
     #   -c requirements/edx/../common_constraints.txt
     #   edx-search
 enmerkar==0.7.1
     # via enmerkar-underscore
 enmerkar-underscore==2.1.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 event-tracking==2.1.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-proctoring
     #   edx-search
-fastavro==1.7.3
+fastavro==1.8.0
     # via openedx-events
-filelock==3.11.0
+filelock==3.12.2
     # via snowflake-connector-python
-frozenlist==1.3.3
+frozenlist==1.4.0
     # via
     #   aiohttp
     #   aiosignal
 fs==2.0.27
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   fs-s3fs
     #   openedx-django-pyfs
     #   xblock
 fs-s3fs==0.1.8
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   openedx-django-pyfs
 future==0.18.3
     # via pyjwkest
-geoip2==4.6.0
-    # via -r requirements/edx/base.in
+geoip2==4.7.0
+    # via -r requirements/edx/kernel.in
 glob2==0.7
-    # via -r requirements/edx/base.in
-gunicorn==20.1.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
+gunicorn==21.0.0
+    # via -r requirements/edx/kernel.in
 help-tokens==2.2.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 html5lib==1.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   ora2
-icalendar==5.0.5
-    # via -r requirements/edx/base.in
+icalendar==5.0.7
+    # via -r requirements/edx/kernel.in
 idna==3.4
     # via
     #   -r requirements/edx/paver.txt
     #   optimizely-sdk
     #   requests
     #   snowflake-connector-python
     #   yarl
-importlib-metadata==6.4.1
+importlib-metadata==6.8.0
     # via markdown
-importlib-resources==5.12.0
-    # via jsonschema
+importlib-resources==6.0.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 inflection==0.5.1
     # via drf-yasg
 interchange==2021.0.4
     # via py2neo
 ipaddress==1.0.23
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 isodate==0.6.1
     # via python3-saml
 itypes==1.2.0
     # via coreapi
 jinja2==3.1.2
     # via
     #   code-annotations
     #   coreschema
 jmespath==0.10.0
     # via
     #   boto3
     #   botocore
-joblib==1.2.0
+joblib==1.3.1
     # via nltk
 jsondiff==2.0.0
 jsonfield==3.1.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-celeryutils
     #   edx-enterprise
     #   edx-proctoring
     #   edx-submissions
     #   learner-pathway-progress
     #   lti-consumer-xblock
     #   ora2
     #   outcome-surveys
-jsonschema==4.17.3
+jsonschema==4.18.3
     # via optimizely-sdk
-jwcrypto==1.4.2
+jsonschema-specifications==2023.6.1
+    # via jsonschema
+jwcrypto==1.5.0
     # via pylti1p3
     # via celery
 laboratory==1.0.2
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 lazy==1.5
     # via
     #   -r requirements/edx/paver.txt
     #   acid-xblock
     #   lti-consumer-xblock
     #   ora2
     #   xblock
-learner-pathway-progress==1.3.3
-    # via -r requirements/edx/base.in
-levenshtein==0.20.9
-    # via python-levenshtein
+learner-pathway-progress==1.3.4
+    # via -r requirements/edx/bundled.in
 libsass==0.10.0
-    # via
-    #   -r requirements/edx/paver.txt
-    #   ora2
+    # via -r requirements/edx/paver.txt
 loremipsum==1.0.5
     # via ora2
-lti-consumer-xblock==9.0.2
-    # via -r requirements/edx/base.in
-lxml==4.9.2
+lti-consumer-xblock==9.5.5
+    # via -r requirements/edx/kernel.in
+lxml==4.9.3
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edxval
     #   lti-consumer-xblock
     #   olxcleaner
     #   openedx-calc
     #   ora2
+    #   python3-saml
     #   xblock
     #   xmlsec
 mailsnake==1.6.4
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/bundled.in
 mako==1.2.4
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   acid-xblock
     #   lti-consumer-xblock
     #   xblock-google-drive
     #   xblock-utils
 markdown==3.3.7
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   openedx-django-wiki
     #   staff-graded-xblock
     #   xblock-poll
 markey==0.8
     # via enmerkar-underscore
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   -r requirements/edx/paver.txt
     #   chem
     #   jinja2
     #   mako
     #   openedx-calc
     #   xblock
-maxminddb==2.2.0
+maxminddb==2.4.0
     # via geoip2
-mock==5.0.2
+mock==5.1.0
     # via -r requirements/edx/paver.txt
-mongodbproxy @ git+https://github.com/openedx/MongoDBProxy.git@d92bafe9888d2940f647a7b2b2383b29c752f35a
-    # via -r requirements/edx/github.in
 mongoengine==0.27.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 monotonic==1.6
     # via
     #   analytics-python
     #   py2neo
 mpmath==1.3.0
     # via sympy
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
-mysqlclient==2.1.1
+mysqlclient==2.2.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   openedx-blockstore
-newrelic==8.8.0
+newrelic==8.8.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/bundled.in
     #   edx-django-utils
 nltk==3.8.1
-    # via
-    #   -r requirements/edx/base.in
-    #   chem
-nodeenv==1.7.0
-    # via -r requirements/edx/base.in
+    # via chem
+nodeenv==1.8.0
+    # via -r requirements/edx/kernel.in
 numpy==1.22.4
     # via
     #   chem
     #   openedx-calc
     #   scipy
     #   shapely
 oauthlib==3.0.1
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   django-oauth-toolkit
     #   lti-consumer-xblock
     #   requests-oauthlib
     #   social-auth-core
 olxcleaner==0.2.1
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 openedx-blockstore==1.3.1
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 openedx-calc==3.0.1
-    # via -r requirements/edx/base.in
-openedx-django-pyfs==3.2.1
+    # via -r requirements/edx/kernel.in
+openedx-django-pyfs==3.4.0
     # via xblock
 openedx-django-require==2.0.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 openedx-django-wiki==2.0.0
-    # via -r requirements/edx/base.in
-openedx-events==7.0.0
+    # via -r requirements/edx/kernel.in
+openedx-events==8.2.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-event-bus-kafka
-openedx-filters==1.2.0
+    #   edx-event-bus-redis
+    #   skill-tagging
+openedx-filters==1.3.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   lti-consumer-xblock
+    #   skill-tagging
+openedx-mongodbproxy==0.2.0
+    # via -r requirements/edx/kernel.in
 optimizely-sdk==4.1.1
-    # via -r requirements/edx/base.in
-ora2==5.0.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/bundled.in
+ora2==5.2.1
+    # via -r requirements/edx/bundled.in
 oscrypto==1.3.0
     # via snowflake-connector-python
 outcome-surveys==2.4.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/bundled.in
 packaging==23.1
     # via
     #   drf-yasg
+    #   gunicorn
     #   py2neo
     #   snowflake-connector-python
 pansi==2020.7.3
     # via py2neo
-path==16.6.0
+path==16.7.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   -r requirements/edx/paver.txt
     #   edx-i18n-tools
     #   path-py
 path-py==12.5.0
     # via
     #   edx-enterprise
     #   ora2
@@ -793,138 +803,136 @@
     # via -r requirements/edx/paver.txt
 pbr==5.11.1
     # via
     #   -r requirements/edx/paver.txt
     #   stevedore
 pgpy==0.6.0
 piexif==1.1.3
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 pillow==9.5.0
     # via
-    #   -r requirements/edx/base.in
+    #   -c requirements/edx/../constraints.txt
+    #   -r requirements/edx/kernel.in
     #   edx-enterprise
     #   edx-organizations
+    #   edxval
 pkgutil-resolve-name==1.3.10
     # via jsonschema
 polib==1.2.0
     # via edx-i18n-tools
     # via click-repl
 psutil==5.9.5
     # via
     #   -r requirements/edx/paver.txt
     #   edx-django-utils
 py2neo==2021.2.3
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
-pyasn1==0.4.8
+    #   -r requirements/edx/bundled.in
+pyasn1==0.5.0
     # via pgpy
 pycountry==22.3.5
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 pycparser==2.21
     # via cffi
-pycryptodomex==3.17
+pycryptodomex==3.18.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-proctoring
     #   lti-consumer-xblock
     #   pyjwkest
     #   snowflake-connector-python
-pygments==2.15.0
+pygments==2.15.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/bundled.in
     #   py2neo
 pyjwkest==1.4.2
     # via
-    #   -r requirements/edx/base.in
-    #   edx-drf-extensions
+    #   -r requirements/edx/kernel.in
     #   edx-token-utils
     #   lti-consumer-xblock
-pyjwt[crypto]==2.6.0
+pyjwt[crypto]==2.7.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   drf-jwt
     #   edx-auth-backends
     #   edx-drf-extensions
     #   edx-proctoring
     #   edx-rest-api-client
     #   pylti1p3
     #   snowflake-connector-python
     #   social-auth-core
 pylatexenc==2.10
     # via olxcleaner
 pylti1p3==2.0.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
+pymemcache==4.0.0
+    # via -r requirements/edx/paver.txt
 pymongo==3.13.0
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   -r requirements/edx/paver.txt
     #   edx-opaque-keys
     #   event-tracking
-    #   mongodbproxy
     #   mongoengine
+    #   openedx-mongodbproxy
 pynacl==1.5.0
     # via edx-django-utils
 pynliner==0.8.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 pyopenssl==22.0.0
     # via
     #   -c requirements/edx/../constraints.txt
     #   optimizely-sdk
     #   snowflake-connector-python
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via
     #   chem
     #   openedx-calc
 pyrsistent==0.19.3
-    # via
-    #   jsonschema
-    #   optimizely-sdk
+    # via optimizely-sdk
 pysrt==1.1.2
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edxval
 python-dateutil==2.8.2
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   analytics-python
     #   botocore
+    #   celery
     #   edx-ace
     #   edx-drf-extensions
     #   edx-enterprise
     #   edx-proctoring
     #   icalendar
     #   olxcleaner
     #   ora2
     #   xblock
-python-levenshtein==0.20.9
-    # via -r requirements/edx/base.in
 python-memcached==1.59
     # via -r requirements/edx/paver.txt
 python-slugify==8.0.1
     # via code-annotations
 python-swiftclient==4.3.0
     # via ora2
 python3-openid==3.2.0 ; python_version >= "3"
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   social-auth-core
-python3-saml==1.9.0
-    # via
-    #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+python3-saml==1.15.0
+    # via -r requirements/edx/kernel.in
 pytz==2022.7.1
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   babel
-    #   celery
     #   django
     #   django-ses
+    #   djangorestframework
     #   drf-yasg
     #   edx-completion
     #   edx-enterprise
     #   edx-proctoring
     #   edx-submissions
     #   edx-tincan-py35
     #   event-tracking
@@ -934,33 +942,37 @@
     #   learner-pathway-progress
     #   olxcleaner
     #   openedx-blockstore
     #   ora2
     #   snowflake-connector-python
     #   xblock
 pyuca==1.2
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 pyyaml==6.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   code-annotations
     #   edx-django-release-util
     #   edx-i18n-tools
     #   xblock
 random2==1.0.1
-    # via -r requirements/edx/base.in
-rapidfuzz==2.15.1
-    # via levenshtein
+    # via -r requirements/edx/kernel.in
 recommender-xblock==2.0.1
-    # via -r requirements/edx/base.in
-redis==4.5.4
-    # via -r requirements/edx/base.in
-regex==2023.3.23
+    # via -r requirements/edx/bundled.in
+redis==4.6.0
+    # via
+    #   -r requirements/edx/kernel.in
+    #   walrus
+referencing==0.29.1
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+regex==2023.6.3
     # via nltk
-requests==2.28.2
+requests==2.31.0
     # via
     #   -r requirements/edx/paver.txt
     #   algoliasearch
     #   analytics-python
     #   coreapi
     #   django-oauth-toolkit
     #   edx-bulk-grades
@@ -978,52 +990,55 @@
     #   requests-oauthlib
     #   sailthru-client
     #   slumber
     #   snowflake-connector-python
     #   social-auth-core
 requests-oauthlib==1.3.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   social-auth-core
-ruamel-yaml==0.17.21
+rpds-py==0.8.11
+    # via
+    #   jsonschema
+    #   referencing
+ruamel-yaml==0.17.32
     # via drf-yasg
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 rules==3.3
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-enterprise
     #   edx-proctoring
 s3transfer==0.1.13
     # via boto3
 sailthru-client==2.2.3
     # via edx-ace
 scipy==1.7.3
     # via
     #   -c requirements/edx/../constraints.txt
     #   chem
     #   openedx-calc
 semantic-version==2.10.0
     # via edx-drf-extensions
 shapely==2.0.1
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
 simplejson==3.19.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   sailthru-client
     #   super-csv
     #   xblock-utils
 six==1.16.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   -r requirements/edx/paver.txt
     #   analytics-python
     #   bleach
     #   chem
-    #   click-repl
     #   codejail-includes
     #   crowdsourcehinter-xblock
     #   edx-ace
     #   edx-auth-backends
     #   edx-ccx-keys
     #   edx-codejail
     #   edx-django-release-util
@@ -1040,158 +1055,168 @@
     #   optimizely-sdk
     #   pansi
     #   paver
     #   py2neo
     #   pyjwkest
     #   python-dateutil
     #   python-memcached
+skill-tagging==0.1.0
+    # via -r requirements/edx/bundled.in
 slumber==0.7.1
     # via
     #   edx-bulk-grades
     #   edx-enterprise
     #   edx-rest-api-client
-snowflake-connector-python==3.0.2
+snowflake-connector-python==3.0.4
 social-auth-app-django==5.0.0
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-auth-backends
 social-auth-core==4.3.0
     # via
     #   -c requirements/edx/../constraints.txt
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-auth-backends
     #   social-auth-app-django
 sorl-thumbnail==12.9.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   openedx-django-wiki
 sortedcontainers==2.4.0
-    # via -r requirements/edx/base.in
+    # via
+    #   -r requirements/edx/kernel.in
+    #   snowflake-connector-python
 soupsieve==2.4.1
     # via beautifulsoup4
-sqlparse==0.4.3
+sqlparse==0.4.4
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   django
     #   openedx-blockstore
 staff-graded-xblock==2.0.1
-    # via -r requirements/edx/base.in
-stevedore==5.0.0
+    # via -r requirements/edx/bundled.in
+stevedore==5.1.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   -r requirements/edx/paver.txt
     #   code-annotations
     #   edx-ace
     #   edx-django-utils
     #   edx-enterprise
     #   edx-opaque-keys
 super-csv==3.0.1
-    # via
-    #   -r requirements/edx/base.in
-    #   edx-bulk-grades
-sympy==1.11.1
+    # via edx-bulk-grades
+sympy==1.12
     # via openedx-calc
 testfixtures==7.1.0
 text-unidecode==1.3
     # via python-slugify
 tinycss2==1.1.1
     # via bleach
 tqdm==4.65.0
     # via nltk
-typing-extensions==4.5.0
+typing-extensions==4.7.1
     # via
+    #   asgiref
     #   django-countries
+    #   kombu
     #   pylti1p3
     #   snowflake-connector-python
+tzdata==2023.3
+    # via
+    #   backports-zoneinfo
+    #   celery
 unicodecsv==0.14.1
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-enterprise
 uritemplate==4.1.1
     # via
     #   coreapi
     #   drf-yasg
-urllib3==1.26.15
+urllib3==1.26.16
     # via
+    #   -c requirements/edx/../constraints.txt
     #   -r requirements/edx/paver.txt
     #   elasticsearch
-    #   geoip2
     #   py2neo
     #   requests
     #   snowflake-connector-python
 user-util==1.0.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/kernel.in
     # via
     #   amqp
     #   celery
     #   kombu
 voluptuous==0.13.1
     # via ora2
+walrus==0.9.3
+    # via edx-event-bus-redis
 watchdog==3.0.0
     # via -r requirements/edx/paver.txt
 wcwidth==0.2.6
     # via prompt-toolkit
 web-fragments==2.0.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   crowdsourcehinter-xblock
     #   edx-sga
     #   staff-graded-xblock
     #   xblock
     #   xblock-utils
 webencodings==0.5.1
     # via
     #   bleach
     #   html5lib
     #   tinycss2
 webob==1.8.7
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   xblock
 wrapt==1.15.0
     # via
     #   -r requirements/edx/paver.txt
     #   deprecated
 xblock[django]==1.6.2
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   acid-xblock
     #   crowdsourcehinter-xblock
     #   done-xblock
     #   edx-completion
     #   edx-sga
     #   edx-user-state-client
     #   edx-when
     #   lti-consumer-xblock
     #   ora2
     #   staff-graded-xblock
     #   xblock-google-drive
     #   xblock-poll
     #   xblock-utils
-xblock-drag-and-drop-v2==3.1.2
-    # via -r requirements/edx/base.in
+xblock-drag-and-drop-v2==3.2.0
+    # via -r requirements/edx/bundled.in
 xblock-google-drive==0.3.0
-    # via -r requirements/edx/base.in
+    # via -r requirements/edx/bundled.in
 xblock-poll==1.13.0
-    # via -r requirements/edx/base.in
-xblock-utils==3.0.0
+    # via -r requirements/edx/bundled.in
+xblock-utils==3.2.0
     # via
-    #   -r requirements/edx/base.in
+    #   -r requirements/edx/kernel.in
     #   edx-sga
     #   lti-consumer-xblock
     #   staff-graded-xblock
     #   xblock-drag-and-drop-v2
     #   xblock-google-drive
 xmlsec==1.3.13
     # via python3-saml
 xss-utils==0.4.0
-    # via -r requirements/edx/base.in
-yarl==1.8.2
+    # via -r requirements/edx/kernel.in
+yarl==1.9.2
     # via aiohttp
-zipp==3.15.0
+zipp==3.16.2
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `edx-enterprise-4.0.3/requirements/js_test.txt` & `edx-enterprise-4.0.4/requirements/js_test.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,114 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    make upgrade
 #
-async-generator==1.10
-    # via trio
+annotated-types==0.5.0
+    # via pydantic
 attrs==23.1.0
     # via
     #   outcome
     #   trio
 autocommand==2.2.2
     # via jaraco-text
-certifi==2022.12.7
+certifi==2023.5.7
     # via selenium
-cheroot==9.0.0
+cheroot==10.0.0
     # via cherrypy
 cherrypy==18.8.0
     # via jasmine
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via
     #   trio
     #   trio-websocket
 glob2==0.7
     # via jasmine-core
 h11==0.14.0
     # via wsproto
 idna==3.4
     # via trio
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via jaraco-text
-inflect==6.0.4
+inflect==7.0.0
     # via jaraco-text
-jaraco-classes==3.2.3
+jaraco-classes==3.3.0
     # via -r requirements/js_test.in
-jaraco-collections==4.1.0
+jaraco-collections==4.3.0
     # via
     #   -r requirements/js_test.in
     #   cherrypy
 jaraco-context==4.3.0
     # via jaraco-text
-jaraco-functools==3.6.0
+jaraco-functools==3.8.0
     # via
     #   -r requirements/js_test.in
     #   cheroot
     #   jaraco-text
     #   tempora
 jaraco-text==3.11.1
     # via jaraco-collections
 jasmine==3.99.0
     # via -r requirements/js_test.in
 jasmine-core==3.99.0
     # via jasmine
 jinja2==2.11.3
     # via jasmine
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 more-itertools==9.1.0
     # via
     #   cheroot
     #   cherrypy
     #   jaraco-classes
     #   jaraco-functools
     #   jaraco-text
 ordereddict==1.1
     # via jasmine-core
 outcome==1.2.0
     # via trio
-portend==3.1.0
+portend==3.2.0
     # via cherrypy
-pydantic==1.10.7
+pydantic==2.0.3
     # via inflect
+pydantic-core==2.3.0
+    # via pydantic
 pysocks==1.7.1
     # via urllib3
 pytz==2023.3
     # via tempora
-pyyaml==6.0
+pyyaml==6.0.1
     # via jasmine
-selenium==4.8.3
+selenium==4.10.0
     # via jasmine
-six==1.16.0
-    # via cheroot
 sniffio==1.3.0
     # via trio
 sortedcontainers==2.4.0
     # via trio
-tempora==5.2.2
+tempora==5.5.0
     # via
     #   -r requirements/js_test.in
     #   portend
-trio==0.22.0
+trio==0.22.2
     # via
     #   selenium
     #   trio-websocket
-trio-websocket==0.10.2
+trio-websocket==0.10.3
     # via selenium
-typing-extensions==4.5.0
-    # via pydantic
-urllib3[socks]==1.26.15
+typing-extensions==4.7.1
+    # via
+    #   annotated-types
+    #   inflect
+    #   pydantic
+    #   pydantic-core
+urllib3[socks]==2.0.4
     # via selenium
 wsproto==1.2.0
     # via trio-websocket
 zc-lockfile==3.0.post1
     # via cherrypy
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `edx-enterprise-4.0.3/requirements/test-master.txt` & `edx-enterprise-4.0.4/requirements/test-master.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,35 +6,40 @@
 #
 amqp==5.1.1
     # via kombu
 aniso8601==9.0.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   edx-tincan-py35
-asgiref==3.6.0
+asgiref==3.7.2
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   django
     #   django-countries
 asn1crypto==1.5.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   oscrypto
     #   snowflake-connector-python
+backports-zoneinfo[tzdata]==0.2.1
+    # via
+    #   -c requirements/edx-platform-constraints.txt
+    #   celery
+    #   kombu
 billiard==4.1.0
     # via celery
-bleach[css]==6.0.0
+bleach==6.0.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 celery==5.3.1
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
     # via
     #   -c requirements/edx-platform-constraints.txt
@@ -42,29 +47,29 @@
     #   pynacl
     #   snowflake-connector-python
 charset-normalizer==2.0.12
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   requests
     #   snowflake-connector-python
-click==8.1.5
+click==8.1.6
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   code-annotations
     #   edx-django-utils
 click-didyoumean==0.3.0
     # via celery
 click-plugins==1.1.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   celery
-click-repl==0.2.0
+click-repl==0.3.0
     # via celery
 code-annotations==1.3.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 cryptography==38.0.4
     # via
@@ -75,15 +80,15 @@
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
 defusedxml==0.7.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   djangorestframework-xml
-django==3.2.18
+django==3.2.20
     # via
     #   -c requirements/common_constraints.txt
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
     #   django-config-models
     #   django-crum
     #   django-fernet-fields
@@ -114,28 +119,28 @@
     #   -r requirements/base.in
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields==0.6
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
-django-filter==23.1
+django-filter==23.2
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 django-ipware==4.0.2
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 django-model-utils==4.3.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
     #   edx-rbac
-django-multi-email-field==0.6.2
+django-multi-email-field==0.7.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 django-object-actions==4.1.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
@@ -146,66 +151,62 @@
     #   -r requirements/base.in
 django-waffle==3.0.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.12.4
+djangorestframework==3.14.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
     #   django-config-models
     #   drf-jwt
     #   edx-drf-extensions
 djangorestframework-xml==2.0.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 drf-jwt==1.19.2
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   edx-drf-extensions
-edx-django-utils==5.4.0
+edx-django-utils==5.5.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
     #   django-config-models
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==8.6.0
+edx-drf-extensions==8.8.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
     #   edx-rbac
 edx-opaque-keys[django]==2.3.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
-edx-rest-api-client==5.5.0
+edx-rest-api-client==5.5.2
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 edx-tincan-py35==1.0.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
-filelock==3.11.0
+filelock==3.12.2
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   snowflake-connector-python
-future==0.18.3
-    # via
-    #   -c requirements/edx-platform-constraints.txt
-    #   pyjwkest
 idna==3.4
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   requests
     #   snowflake-connector-python
 jinja2==3.1.2
     # via
@@ -217,31 +218,31 @@
     #   -r requirements/base.in
 jsonfield==3.1.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 kombu==5.3.1
     # via celery
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   jinja2
-newrelic==8.8.0
+newrelic==8.8.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   edx-django-utils
 oscrypto==1.3.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   snowflake-connector-python
 packaging==23.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   snowflake-connector-python
-path==16.6.0
+path==16.7.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   path-py
 path-py==12.5.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
@@ -253,38 +254,33 @@
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 pillow==9.5.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via click-repl
 psutil==5.9.5
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   edx-django-utils
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   pgpy
 pycparser==2.21
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   cffi
-pycryptodomex==3.17
+pycryptodomex==3.18.0
     # via
     #   -c requirements/edx-platform-constraints.txt
-    #   pyjwkest
     #   snowflake-connector-python
-pyjwkest==1.4.2
-    # via
-    #   -c requirements/edx-platform-constraints.txt
-    #   edx-drf-extensions
-pyjwt[crypto]==2.6.0
+pyjwt[crypto]==2.7.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
 pymongo==3.13.0
@@ -299,99 +295,104 @@
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   snowflake-connector-python
 python-dateutil==2.8.2
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
+    #   celery
     #   edx-drf-extensions
 python-slugify==8.0.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   code-annotations
 pytz==2022.7.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
-    #   celery
     #   django
+    #   djangorestframework
     #   edx-tincan-py35
     #   snowflake-connector-python
 pyyaml==6.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   code-annotations
-requests==2.28.2
+requests==2.31.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-    #   pyjwkest
     #   slumber
     #   snowflake-connector-python
 rules==3.3
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 semantic-version==2.10.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   edx-drf-extensions
 six==1.16.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   bleach
-    #   click-repl
     #   edx-drf-extensions
     #   edx-rbac
-    #   pyjwkest
     #   python-dateutil
 slumber==0.7.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
     #   edx-rest-api-client
-snowflake-connector-python==3.0.2
+snowflake-connector-python==3.0.4
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
-sqlparse==0.4.3
+sortedcontainers==2.4.0
+    # via
+    #   -c requirements/edx-platform-constraints.txt
+    #   snowflake-connector-python
+sqlparse==0.4.4
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   django
-stevedore==5.0.0
+stevedore==5.1.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
     #   code-annotations
     #   edx-django-utils
     #   edx-opaque-keys
 testfixtures==7.1.0
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
 text-unidecode==1.3
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   python-slugify
-tinycss2==1.1.1
-    # via
-    #   -c requirements/edx-platform-constraints.txt
-    #   bleach
-typing-extensions==4.5.0
+typing-extensions==4.7.1
     # via
     #   -c requirements/edx-platform-constraints.txt
+    #   asgiref
     #   django-countries
+    #   kombu
     #   snowflake-connector-python
+tzdata==2023.3
+    # via
+    #   -c requirements/edx-platform-constraints.txt
+    #   backports-zoneinfo
+    #   celery
 unicodecsv==0.14.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   -r requirements/base.in
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   requests
     #   snowflake-connector-python
 vine==5.0.0
     # via
     #   amqp
@@ -401,8 +402,7 @@
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   prompt-toolkit
 webencodings==0.5.1
     # via
     #   -c requirements/edx-platform-constraints.txt
     #   bleach
-    #   tinycss2
```

### Comparing `edx-enterprise-4.0.3/requirements/test.in` & `edx-enterprise-4.0.4/requirements/test.in`

 * *Files 14% similar despite different names*

```diff
@@ -9,7 +9,8 @@
 factory_boy               # Test factory framework
 freezegun                 # Time freezing library
 mock                      # mocking library
 pytest-cov                # pytest extension for code coverage statistics
 pytest-django             # pytest extension for better Django support
 responses                 # utility library for mocking out the requests library
 testfixtures              # Mock objects for unit tests and doc tests
+backports.zoneinfo
```

### Comparing `edx-enterprise-4.0.3/requirements/test.txt` & `edx-enterprise-4.0.4/requirements/test.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,35 +7,41 @@
     # via
     #   -r requirements/test-master.txt
     #   kombu
 aniso8601==9.0.1
     # via
     #   -r requirements/test-master.txt
     #   edx-tincan-py35
-asgiref==3.6.0
+asgiref==3.7.2
     # via
     #   -r requirements/test-master.txt
     #   django
     #   django-countries
 asn1crypto==1.5.1
     # via
     #   -r requirements/test-master.txt
     #   oscrypto
     #   snowflake-connector-python
 attrs==23.1.0
     # via pytest
+backports-zoneinfo[tzdata]==0.2.1
     # via
     #   -r requirements/test-master.txt
+    #   -r requirements/test.in
     #   celery
-bleach[css]==6.0.0
+    #   kombu
+    # via
+    #   -r requirements/test-master.txt
+    #   celery
+bleach==6.0.0
     # via -r requirements/test-master.txt
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test-master.txt
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   -r requirements/test-master.txt
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
     # via
     #   -r requirements/test-master.txt
@@ -65,15 +71,15 @@
     #   -r requirements/test-master.txt
     #   celery
     # via
     #   -r requirements/test-master.txt
     #   celery
 code-annotations==1.3.0
     # via -r requirements/test-master.txt
-coverage[toml]==7.2.3
+coverage[toml]==7.2.7
     # via pytest-cov
 cryptography==38.0.4
     # via
     #   -r requirements/test-master.txt
     #   django-fernet-fields
     #   pgpy
     #   pyjwt
@@ -81,15 +87,15 @@
     #   snowflake-connector-python
 ddt==1.3.1
     # via -r requirements/test.in
 defusedxml==0.7.1
     # via
     #   -r requirements/test-master.txt
     #   djangorestframework-xml
-diff-cover==7.5.0
+diff-cover==7.7.0
     # via -r requirements/test.in
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/test-master.txt
     #   django-config-models
     #   django-crum
     #   django-fernet-fields
@@ -111,86 +117,82 @@
 django-crum==0.7.9
     # via
     #   -r requirements/test-master.txt
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields==0.6
     # via -r requirements/test-master.txt
-django-filter==23.1
+django-filter==23.2
     # via -r requirements/test-master.txt
 django-ipware==4.0.2
     # via -r requirements/test-master.txt
 django-model-utils==4.3.1
     # via
     #   -r requirements/test-master.txt
     #   -r requirements/test.in
     #   edx-rbac
-django-multi-email-field==0.6.2
+django-multi-email-field==0.7.0
     # via -r requirements/test-master.txt
 django-object-actions==4.1.0
     # via -r requirements/test-master.txt
 django-simple-history==3.0.0
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/test-master.txt
 django-waffle==3.0.0
     # via
     #   -r requirements/test-master.txt
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.12.4
+djangorestframework==3.14.0
     # via
     #   -r requirements/test-master.txt
     #   django-config-models
     #   drf-jwt
     #   edx-drf-extensions
 djangorestframework-xml==2.0.0
     # via -r requirements/test-master.txt
 drf-jwt==1.19.2
     # via
     #   -r requirements/test-master.txt
     #   edx-drf-extensions
-edx-django-utils==5.4.0
+edx-django-utils==5.5.0
     # via
     #   -r requirements/test-master.txt
     #   django-config-models
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==8.6.0
+edx-drf-extensions==8.8.0
     # via
     #   -r requirements/test-master.txt
     #   edx-rbac
 edx-opaque-keys[django]==2.3.0
     # via
     #   -r requirements/test-master.txt
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/test-master.txt
-edx-rest-api-client==5.5.0
+edx-rest-api-client==5.5.2
     # via -r requirements/test-master.txt
 edx-tincan-py35==1.0.0
     # via -r requirements/test-master.txt
-factory-boy==3.2.1
+factory-boy==3.3.0
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.in
-faker==18.4.0
+faker==19.2.0
     # via factory-boy
-filelock==3.11.0
+filelock==3.12.2
     # via
     #   -r requirements/test-master.txt
     #   snowflake-connector-python
 freezegun==0.3.14
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.in
-future==0.18.3
-    # via
-    #   -r requirements/test-master.txt
-    #   pyjwkest
 idna==3.4
     # via
     #   -r requirements/test-master.txt
     #   requests
     #   snowflake-connector-python
 iniconfig==2.0.0
     # via pytest
@@ -202,82 +204,77 @@
 jsondiff==2.0.0
     # via -r requirements/test-master.txt
 jsonfield==3.1.0
     # via -r requirements/test-master.txt
     # via
     #   -r requirements/test-master.txt
     #   celery
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   -r requirements/test-master.txt
     #   jinja2
 mock==3.0.5
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.in
-newrelic==8.8.0
+newrelic==8.8.1
     # via
     #   -r requirements/test-master.txt
     #   edx-django-utils
 oscrypto==1.3.0
     # via
     #   -r requirements/test-master.txt
     #   snowflake-connector-python
 packaging==23.1
     # via
     #   -r requirements/test-master.txt
     #   pytest
     #   snowflake-connector-python
-path==16.6.0
+path==16.7.1
     # via
     #   -r requirements/test-master.txt
     #   path-py
 path-py==12.5.0
     # via -r requirements/test-master.txt
 pbr==5.11.1
     # via
     #   -r requirements/test-master.txt
     #   stevedore
 pgpy==0.6.0
     # via -r requirements/test-master.txt
 pillow==9.5.0
     # via -r requirements/test-master.txt
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   diff-cover
     #   pytest
     # via
     #   -r requirements/test-master.txt
     #   click-repl
 psutil==5.9.5
     # via
     #   -r requirements/test-master.txt
     #   edx-django-utils
 py==1.11.0
     # via pytest
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   -r requirements/test-master.txt
     #   pgpy
 pycparser==2.21
     # via
     #   -r requirements/test-master.txt
     #   cffi
-pycryptodomex==3.17
+pycryptodomex==3.18.0
     # via
     #   -r requirements/test-master.txt
-    #   pyjwkest
     #   snowflake-connector-python
-pygments==2.15.0
+pygments==2.15.1
     # via diff-cover
-pyjwkest==1.4.2
-    # via
-    #   -r requirements/test-master.txt
-    #   edx-drf-extensions
-pyjwt[crypto]==2.6.0
+pyjwt[crypto]==2.7.0
     # via
     #   -r requirements/test-master.txt
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
 pymongo==3.13.0
@@ -293,45 +290,45 @@
     #   -r requirements/test-master.txt
     #   snowflake-connector-python
 pytest==6.2.5
     # via
     #   -c requirements/constraints.txt
     #   pytest-cov
     #   pytest-django
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r requirements/test.in
 pytest-django==4.5.2
     # via -r requirements/test.in
 python-dateutil==2.8.2
     # via
     #   -r requirements/test-master.txt
+    #   celery
     #   edx-drf-extensions
     #   faker
     #   freezegun
 python-slugify==8.0.1
     # via
     #   -r requirements/test-master.txt
     #   code-annotations
 pytz==2022.7.1
     # via
     #   -r requirements/test-master.txt
-    #   celery
     #   django
+    #   djangorestframework
     #   edx-tincan-py35
     #   snowflake-connector-python
 pyyaml==6.0
     # via
     #   -r requirements/test-master.txt
     #   code-annotations
-requests==2.28.2
+requests==2.31.0
     # via
     #   -r requirements/test-master.txt
     #   edx-drf-extensions
     #   edx-rest-api-client
-    #   pyjwkest
     #   responses
     #   slumber
     #   snowflake-connector-python
 responses==0.10.15
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.in
@@ -341,62 +338,68 @@
     # via
     #   -r requirements/test-master.txt
     #   edx-drf-extensions
 six==1.16.0
     # via
     #   -r requirements/test-master.txt
     #   bleach
-    #   click-repl
     #   edx-drf-extensions
     #   edx-rbac
     #   freezegun
     #   mock
-    #   pyjwkest
     #   python-dateutil
     #   responses
 slumber==0.7.1
     # via
     #   -r requirements/test-master.txt
     #   edx-rest-api-client
-snowflake-connector-python==3.0.2
+snowflake-connector-python==3.0.4
     # via -r requirements/test-master.txt
-sqlparse==0.4.3
+sortedcontainers==2.4.0
+    # via
+    #   -r requirements/test-master.txt
+    #   snowflake-connector-python
+sqlparse==0.4.4
     # via
     #   -r requirements/test-master.txt
     #   django
-stevedore==5.0.0
+stevedore==5.1.0
     # via
     #   -r requirements/test-master.txt
     #   code-annotations
     #   edx-django-utils
     #   edx-opaque-keys
 testfixtures==7.1.0
     # via
     #   -r requirements/test-master.txt
     #   -r requirements/test.in
 text-unidecode==1.3
     # via
     #   -r requirements/test-master.txt
     #   python-slugify
-tinycss2==1.1.1
-    # via
-    #   -r requirements/test-master.txt
-    #   bleach
 toml==0.10.2
     # via pytest
 tomli==2.0.1
     # via coverage
-typing-extensions==4.5.0
+typing-extensions==4.7.1
     # via
     #   -r requirements/test-master.txt
+    #   asgiref
     #   django-countries
+    #   faker
+    #   kombu
     #   snowflake-connector-python
+tzdata==2023.3
+    # via
+    #   -r requirements/test-master.txt
+    #   backports-zoneinfo
+    #   celery
 unicodecsv==0.14.1
     # via -r requirements/test-master.txt
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   -r requirements/test-master.txt
     #   requests
     #   snowflake-connector-python
     # via
     #   -r requirements/test-master.txt
     #   amqp
@@ -406,8 +409,7 @@
     # via
     #   -r requirements/test-master.txt
     #   prompt-toolkit
 webencodings==0.5.1
     # via
     #   -r requirements/test-master.txt
     #   bleach
-    #   tinycss2
```

### Comparing `edx-enterprise-4.0.3/setup.py` & `edx-enterprise-4.0.4/setup.py`

 * *Files identical despite different names*

