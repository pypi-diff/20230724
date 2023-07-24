# Comparing `tmp/django-webidoidc-provider-0.1.6.tar.gz` & `tmp/django-webidoidc-provider-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-webidoidc-provider-0.1.6.tar", last modified: Tue May 18 15:28:23 2021, max compression
+gzip compressed data, was "django-webidoidc-provider-1.0.1.tar", last modified: Mon Jul 24 19:49:58 2023, max compression
```

## Comparing `django-webidoidc-provider-0.1.6.tar` & `django-webidoidc-provider-1.0.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)      874 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1484 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/django_webidoidc_provider.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/django_webidoidc_provider.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/django_webidoidc_provider.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/django_webidoidc_provider.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/django_webidoidc_provider.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3622 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/django_webidoidc_provider.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1091 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/django_webidoidc_provider.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      210 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1671 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     7309 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     9351 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/models.py
--rw-rw-rw-   0 root         (0) root         (0)      136 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/compat.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/static/oidc_provider/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/static/oidc_provider/js/
--rw-rw-rw-   0 root         (0) root         (0)     3989 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/static/oidc_provider/js/sha256.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3765 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/pl/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     2465 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/pl/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3852 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     2962 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/fr/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2915 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/es/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      421 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    17674 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/
--rw-rw-rw-   0 root         (0) root         (0)     5665 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/claims.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)    11734 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/endpoints/authorize.py
--rw-rw-rw-   0 root         (0) root         (0)     4389 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/endpoints/register.py
--rw-rw-rw-   0 root         (0) root         (0)    10823 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/endpoints/token.py
--rw-rw-rw-   0 root         (0) root         (0)     4123 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/endpoints/introspection.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7348 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/errors.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/
--rw-rw-rw-   0 root         (0) root         (0)      696 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/authorize.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/register.py
--rw-rw-rw-   0 root         (0) root         (0)     6411 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/token.py
--rw-rw-rw-   0 root         (0) root         (0)     4120 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/dpop.py
--rw-rw-rw-   0 root         (0) root         (0)     5537 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/oauth2.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2021-05-18 15:28:21.000000 django-webidoidc-provider-0.1.6/oidc_provider/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2739 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1987 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/templates/accounts/
--rw-rw-rw-   0 root         (0) root         (0)      239 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/templates/accounts/login.html
--rw-rw-rw-   0 root         (0) root         (0)       83 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/templates/accounts/logout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/app/
--rw-rw-rw-   0 root         (0) root         (0)    11813 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/app/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/app/urls.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      801 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0025_user_field_codetoken.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0005_token_refresh_token.py
--rw-rw-rw-   0 root         (0) root         (0)     2324 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0018_hybridflow_and_clientattrs.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0003_code_nonce.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0004_remove_userinfo.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0008_rsakey.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0027_token_token_type.py
--rw-rw-rw-   0 root         (0) root         (0)      373 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0028_access_token_text_field.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0006_unique_user_client.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0019_auto_20161005_1552.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0014_client_jwt_alg.py
--rw-rw-rw-   0 root         (0) root         (0)     2625 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0017_auto_20160811_1954.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0022_auto_20170331_1626.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0020_client__post_logout_redirect_uris.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0015_change_client_code.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0012_auto_20160405_2041.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0026_client_multiple_response_types.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0024_auto_20180327_1959.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0010_code_is_authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0007_auto_20160111_1844.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0013_auto_20160407_1912.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0011_client_client_type.py
--rw-rw-rw-   0 root         (0) root         (0)     5120 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      738 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0023_client_owner.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0021_refresh_token_not_unique.py
--rw-rw-rw-   0 root         (0) root         (0)     7082 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0016_userconsent_and_verbosenames.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0002_userconsent.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/migrations/0009_auto_20160202_1945.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      608 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/management/commands/creatersakey.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/oidc_provider/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)       45 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/templates/oidc_provider/error.html
--rw-rw-rw-   0 root         (0) root         (0)      519 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/templates/oidc_provider/authorize.html
--rw-rw-rw-   0 root         (0) root         (0)      732 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/templates/oidc_provider/hidden_inputs.html
--rw-rw-rw-   0 root         (0) root         (0)     1919 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/templates/oidc_provider/check_session_iframe.html
--rw-rw-rw-   0 root         (0) root         (0)      869 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2021-05-18 15:28:08.000000 django-webidoidc-provider-0.1.6/oidc_provider/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1091 2021-05-18 15:28:23.000000 django-webidoidc-provider-0.1.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.244283 django-webidoidc-provider-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-07-24 19:49:58.244283 django-webidoidc-provider-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2248 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.232282 django-webidoidc-provider-1.0.1/django_webidoidc_provider.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-07-24 19:49:58.000000 django-webidoidc-provider-1.0.1/django_webidoidc_provider.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3622 2023-07-24 19:49:58.000000 django-webidoidc-provider-1.0.1/django_webidoidc_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 19:49:58.000000 django-webidoidc-provider-1.0.1/django_webidoidc_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 19:49:58.000000 django-webidoidc-provider-1.0.1/django_webidoidc_provider.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-24 19:49:58.000000 django-webidoidc-provider-1.0.1/django_webidoidc_provider.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-24 19:49:58.000000 django-webidoidc-provider-1.0.1/django_webidoidc_provider.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.232282 django-webidoidc-provider-1.0.1/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/compat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.232282 django-webidoidc-provider-1.0.1/oidc_provider/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5664 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/claims.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.232282 django-webidoidc-provider-1.0.1/oidc_provider/lib/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11734 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/endpoints/authorize.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/endpoints/introspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4389 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/endpoints/register.py
+-rw-rw-rw-   0 root         (0) root         (0)    10823 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/endpoints/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     7348 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.236282 django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/authorize.py
+-rw-rw-rw-   0 root         (0) root         (0)     5442 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     4120 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/dpop.py
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/oauth2.py
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/register.py
+-rw-rw-rw-   0 root         (0) root         (0)     6411 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/token.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.228282 django-webidoidc-provider-1.0.1/oidc_provider/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.228282 django-webidoidc-provider-1.0.1/oidc_provider/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.236282 django-webidoidc-provider-1.0.1/oidc_provider/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2915 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.228282 django-webidoidc-provider-1.0.1/oidc_provider/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.236282 django-webidoidc-provider-1.0.1/oidc_provider/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2962 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3852 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.228282 django-webidoidc-provider-1.0.1/oidc_provider/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.236282 django-webidoidc-provider-1.0.1/oidc_provider/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2465 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3765 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.236282 django-webidoidc-provider-1.0.1/oidc_provider/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.236282 django-webidoidc-provider-1.0.1/oidc_provider/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/management/commands/creatersakey.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.240282 django-webidoidc-provider-1.0.1/oidc_provider/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0002_userconsent.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0003_code_nonce.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0004_remove_userinfo.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0005_token_refresh_token.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0006_unique_user_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0007_auto_20160111_1844.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0008_rsakey.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0009_auto_20160202_1945.py
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0010_code_is_authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0011_client_client_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0012_auto_20160405_2041.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0013_auto_20160407_1912.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0014_client_jwt_alg.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0015_change_client_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     7082 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0016_userconsent_and_verbosenames.py
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0017_auto_20160811_1954.py
+-rw-rw-rw-   0 root         (0) root         (0)     2324 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0018_hybridflow_and_clientattrs.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0019_auto_20161005_1552.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0020_client__post_logout_redirect_uris.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0021_refresh_token_not_unique.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0022_auto_20170331_1626.py
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0023_client_owner.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0024_auto_20180327_1959.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0025_user_field_codetoken.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0026_client_multiple_response_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0027_token_token_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/0028_access_token_text_field.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9350 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7309 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.228282 django-webidoidc-provider-1.0.1/oidc_provider/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.228282 django-webidoidc-provider-1.0.1/oidc_provider/static/oidc_provider/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.240282 django-webidoidc-provider-1.0.1/oidc_provider/static/oidc_provider/js/
+-rw-rw-rw-   0 root         (0) root         (0)     3989 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/static/oidc_provider/js/sha256.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.228282 django-webidoidc-provider-1.0.1/oidc_provider/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.240282 django-webidoidc-provider-1.0.1/oidc_provider/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/templates/oidc_provider/authorize.html
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/templates/oidc_provider/check_session_iframe.html
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/templates/oidc_provider/error.html
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/templates/oidc_provider/hidden_inputs.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.244283 django-webidoidc-provider-1.0.1/oidc_provider/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.244283 django-webidoidc-provider-1.0.1/oidc_provider/tests/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/tests/app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/tests/app/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    11829 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/tests/app/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/tests/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.228282 django-webidoidc-provider-1.0.1/oidc_provider/tests/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:49:58.244283 django-webidoidc-provider-1.0.1/oidc_provider/tests/templates/accounts/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/tests/templates/accounts/login.html
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/tests/templates/accounts/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)     1189 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-24 19:49:55.000000 django-webidoidc-provider-1.0.1/oidc_provider/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    17672 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/oidc_provider/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2023-07-24 19:49:58.244283 django-webidoidc-provider-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-24 19:49:38.000000 django-webidoidc-provider-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-webidoidc-provider-0.1.6/setup.cfg` & `django-webidoidc-provider-1.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [semantic_release]
 version_source = tag
 version_variable = oidc_provider/version.py:__version__
 commit_parser = commit_parser.parse
 
 [tool:pytest]
-django_settings_module = oidc_provider.tests.settings
+DJANGO_SETTINGS_MODULE = oidc_provider.tests.settings
 python_files = test_*.py
 flake8-max-line-length = 100
 flake8-ignore = 
 	.git ALL
 	__pycache__ ALL
 	.ropeproject ALL
 	migrations/* ALL
```

### Comparing `django-webidoidc-provider-0.1.6/README.md` & `django-webidoidc-provider-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 # Django OpenID Connect Provider
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/django-oidc-provider.svg)](https://pypi.python.org/pypi/django-oidc-provider)
 [![PyPI Versions](https://img.shields.io/pypi/v/django-oidc-provider.svg)](https://pypi.python.org/pypi/django-oidc-provider)
 [![Documentation Status](https://readthedocs.org/projects/django-oidc-provider/badge/?version=master)](http://django-oidc-provider.readthedocs.io/)
 [![Travis](https://travis-ci.org/juanifioren/django-oidc-provider.svg?branch=master)](https://travis-ci.org/juanifioren/django-oidc-provider)
 
-## About OpenID
+## About OpenID Connect
 
 OpenID Connect is a simple identity layer on top of the OAuth 2.0 protocol, which allows computing clients to verify the identity of an end-user based on the authentication performed by an authorization server, as well as to obtain basic profile information about the end-user in an interoperable and REST-like manner. Like [Google](https://developers.google.com/identity/protocols/OpenIDConnect) for example.
 
+## About Solid OpenID Connect
+
+The primary divergence of django-webid-oidc-provider from its parent package [django-oidc-provider](https://github.com/juanifioren/django-oidc-provider/blob/master/docs/index.rst) is the support of Solid OIDC. Solid OpenID Connect is a draft specification which extends OIDC for use with decentralised applications, in particular applications using [Solid](https://solidproject.org).
+
+* See the specification here: [https://solid.github.io/authentication-panel/solid-oidc/](https://solid.github.io/authentication-panel/solid-oidc/)
+* See the Primer which accompanies the specification here: [https://solid.github.io/authentication-panel/solid-oidc-primer/](https://solid.github.io/authentication-panel/solid-oidc-primer/)
+
 ## About the package
 
 `django-oidc-provider` can help you providing out of the box all the endpoints, data and logic needed to add OpenID Connect (and OAuth2) capabilities to your Django projects.
 
-Support for Python 3 and 2. Also latest versions of django.
+Support for Python 3.11 and Django 4.2, improves performance.
 
 [Read documentation for more info.](http://django-oidc-provider.readthedocs.org/)
 
 [Do you want to contribute? Please read this.](http://django-oidc-provider.readthedocs.io/en/latest/sections/contribute.html)
```

### Comparing `django-webidoidc-provider-0.1.6/django_webidoidc_provider.egg-info/SOURCES.txt` & `django-webidoidc-provider-1.0.1/django_webidoidc_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/django_webidoidc_provider.egg-info/PKG-INFO` & `django-webidoidc-provider-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-webidoidc-provider
-Version: 0.1.6
+Version: 1.0.1
 Summary: WEBID - OIDC Provider implementation for Django.
 Home-page: https://git.startinblox.com/djangoldp-packages/django-webidoidc-provider
 Author: Juan Ignacio Fiorentino + Startin'blox Team
 Author-email: support@startinblox.com
 License: MIT License
-Description: https://git.startinblox.com/djangoldp-packages/django-webidoidc-provider
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+https://git.startinblox.com/djangoldp-packages/django-webidoidc-provider
```

### Comparing `django-webidoidc-provider-0.1.6/setup.py` & `django-webidoidc-provider-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/LICENSE` & `django-webidoidc-provider-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/settings.py` & `django-webidoidc-provider-1.0.1/oidc_provider/settings.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/models.py` & `django-webidoidc-provider-1.0.1/oidc_provider/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import base64
 import binascii
 from hashlib import md5, sha256
 import json
 
 from django.db import models
 from django.utils import timezone
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.conf import settings
 
 
 CLIENT_TYPE_CHOICES = [
     ('confidential', 'Confidential'),
     ('public', 'Public'),
 ]
```

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/static/oidc_provider/js/sha256.min.js` & `django-webidoidc-provider-1.0.1/oidc_provider/static/oidc_provider/js/sha256.min.js`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/locale/pl/LC_MESSAGES/django.po` & `django-webidoidc-provider-1.0.1/oidc_provider/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/locale/pl/LC_MESSAGES/django.mo` & `django-webidoidc-provider-1.0.1/oidc_provider/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/locale/fr/LC_MESSAGES/django.po` & `django-webidoidc-provider-1.0.1/oidc_provider/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/locale/fr/LC_MESSAGES/django.mo` & `django-webidoidc-provider-1.0.1/oidc_provider/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/locale/es/LC_MESSAGES/django.po` & `django-webidoidc-provider-1.0.1/oidc_provider/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/views.py` & `django-webidoidc-provider-1.0.1/oidc_provider/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,15 +432,15 @@
 
 class RegisterView(View):
 
     @method_decorator(csrf_exempt)
     def dispatch(self, request, *args, **kwargs):
         response = super(RegisterView, self).dispatch(request, *args, **kwargs)
         if settings.get('OIDC_REGISTRATION_ENDPOINT_ALLOW_HTTP_ORIGIN'):
-            response["Access-Control-Allow-Origin"] = request.META.get('HTTP_ORIGIN')
+            response["Access-Control-Allow-Origin"] = request.headers.get('origin')
             response["Access-Control-Allow-Methods"] = "POST"
             response["Access-Control-Allow-Headers"] = \
                 settings.get('OIDC_ACCESS_CONTROL_ALLOW_HEADERS')
         return response
 
     def post(self, request, *args, **kwargs):
```

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/claims.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/claims.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from oidc_provider import settings
 
 
 STANDARD_CLAIMS = {
     'name': '',
     'given_name': '',
```

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/endpoints/authorize.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/endpoints/authorize.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/endpoints/register.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/endpoints/register.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/endpoints/token.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/endpoints/token.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/endpoints/introspection.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/endpoints/introspection.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/errors.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/errors.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/authorize.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/authorize.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/token.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/token.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/dpop.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/dpop.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/common.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 import django
 from django.http import HttpResponse
 from django.utils.cache import patch_vary_headers
 
 from oidc_provider import settings
 
 
-if django.VERSION >= (1, 11):
-    from django.urls import reverse
-else:
-    from django.core.urlresolvers import reverse
+from django.urls import reverse
 
 
 def redirect(uri):
     """
     Custom Response object for redirecting to a Non-HTTP url scheme.
     """
     response = HttpResponse('', status=302)
@@ -164,24 +161,24 @@
 
 
 def cors_allow_any(request, response):
     """
     Add headers to permit CORS requests from any origin, with or without credentials,
     with any headers.
     """
-    origin = request.META.get('HTTP_ORIGIN')
+    origin = request.headers.get('origin')
     if not origin:
         return response
 
     # From the CORS spec: The string "*" cannot be used for a resource that supports credentials.
     response['Access-Control-Allow-Origin'] = origin
     patch_vary_headers(response, ['Origin'])
     response['Access-Control-Allow-Credentials'] = 'true'
     response["Access-Control-Expose-Headers"] = "Location, User"
 
     if request.method == 'OPTIONS':
-        if 'HTTP_ACCESS_CONTROL_REQUEST_HEADERS' in request.META:
+        if 'access-control-request-headers' in request.headers:
             response['Access-Control-Allow-Headers'] \
-                = request.META['HTTP_ACCESS_CONTROL_REQUEST_HEADERS']
+                = request.headers['access-control-request-headers']
         response['Access-Control-Allow-Methods'] = 'GET, POST, OPTIONS'
 
     return response
```

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/lib/utils/oauth2.py` & `django-webidoidc-provider-1.0.1/oidc_provider/lib/utils/oauth2.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """
     Get the access token using Authorization Request Header Field method.
     Or try getting via GET.
     See: http://tools.ietf.org/html/rfc6750#section-2.1
 
     Return a string.
     """
-    auth_header = request.META.get('HTTP_AUTHORIZATION', '')
+    auth_header = request.headers.get('authorization', '')
 
     if re.compile(r'^[Bb]earer\s{1}.+$').match(auth_header):
         access_token = auth_header.split()[1]
     else:
         access_token = request.GET.get('access_token', '')
 
     return access_token
@@ -33,15 +33,15 @@
     """
     Get client credentials using HTTP Basic Authentication method.
     Or try getting parameters via POST.
     See: http://tools.ietf.org/html/rfc6750#section-2.1
 
     Return a tuple `(client_id, client_secret)`.
     """
-    auth_header = request.META.get('HTTP_AUTHORIZATION', '')
+    auth_header = request.headers.get('authorization', '')
 
     if re.compile(r'^Basic\s{1}.+$').match(auth_header):
         b64_user_pass = auth_header.split()[1]
         try:
             user_pass = b64decode(b64_user_pass).decode('utf-8').split(':')
             client_id, client_secret = tuple(user_pass)
         except Exception:
```

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/admin.py` & `django-webidoidc-provider-1.0.1/oidc_provider/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from hashlib import sha224
 from random import randint
 from uuid import uuid4
 
 from django.forms import ModelForm
 from django.contrib import admin
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from oidc_provider.models import Client, Code, Token, RSAKey
 
 
 class ClientForm(ModelForm):
 
     class Meta:
```

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/tests/settings.py` & `django-webidoidc-provider-1.0.1/oidc_provider/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/tests/runner.py` & `django-webidoidc-provider-1.0.1/oidc_provider/tests/runner.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/tests/app/utils.py` & `django-webidoidc-provider-1.0.1/oidc_provider/tests/app/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import string
 import base64
 import time
 import uuid
 import json
 import jwt
 import logging
+from math import floor
 from jwt.utils import to_base64url_uint
 
 import Cryptodome
 from Cryptodome.PublicKey import (RSA, ECC)
 from Cryptodome.Hash import SHA256
 from Cryptodome.Signature import pkcs1_15
 
@@ -253,15 +254,15 @@
     }
 
     # claim something
     payload = {
         "htu": htu,
         "htm": htm,
         "jti": str(uuid.uuid4()),
-        "iat": int(round(time.time() * 1000))
+        "iat": int(floor(time.time()))
     }
 
     # build a signed JWT
     return jwt.encode(payload, signing_key.export_key(format="PEM"), algorithm=headers["alg"], headers=headers)
 
 
 def is_code_valid(url, user, client):
```

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0025_user_field_codetoken.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0025_user_field_codetoken.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0018_hybridflow_and_clientattrs.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0018_hybridflow_and_clientattrs.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0008_rsakey.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0008_rsakey.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0027_token_token_type.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0027_token_token_type.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0019_auto_20161005_1552.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0019_auto_20161005_1552.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0014_client_jwt_alg.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0014_client_jwt_alg.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0017_auto_20160811_1954.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0017_auto_20160811_1954.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0022_auto_20170331_1626.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0022_auto_20170331_1626.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0020_client__post_logout_redirect_uris.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0020_client__post_logout_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0015_change_client_code.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0015_change_client_code.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0026_client_multiple_response_types.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0026_client_multiple_response_types.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0024_auto_20180327_1959.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0024_auto_20180327_1959.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0007_auto_20160111_1844.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0007_auto_20160111_1844.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0013_auto_20160407_1912.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0013_auto_20160407_1912.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0011_client_client_type.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0011_client_client_type.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0001_initial.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0023_client_owner.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0023_client_owner.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0021_refresh_token_not_unique.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0021_refresh_token_not_unique.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0016_userconsent_and_verbosenames.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0016_userconsent_and_verbosenames.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0002_userconsent.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0002_userconsent.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/migrations/0009_auto_20160202_1945.py` & `django-webidoidc-provider-1.0.1/oidc_provider/migrations/0009_auto_20160202_1945.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/management/commands/creatersakey.py` & `django-webidoidc-provider-1.0.1/oidc_provider/management/commands/creatersakey.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/templates/oidc_provider/authorize.html` & `django-webidoidc-provider-1.0.1/oidc_provider/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/templates/oidc_provider/hidden_inputs.html` & `django-webidoidc-provider-1.0.1/oidc_provider/templates/oidc_provider/hidden_inputs.html`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/templates/oidc_provider/check_session_iframe.html` & `django-webidoidc-provider-1.0.1/oidc_provider/templates/oidc_provider/check_session_iframe.html`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/oidc_provider/middleware.py` & `django-webidoidc-provider-1.0.1/oidc_provider/middleware.py`

 * *Files identical despite different names*

### Comparing `django-webidoidc-provider-0.1.6/PKG-INFO` & `django-webidoidc-provider-1.0.1/django_webidoidc_provider.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-webidoidc-provider
-Version: 0.1.6
+Version: 1.0.1
 Summary: WEBID - OIDC Provider implementation for Django.
 Home-page: https://git.startinblox.com/djangoldp-packages/django-webidoidc-provider
 Author: Juan Ignacio Fiorentino + Startin'blox Team
 Author-email: support@startinblox.com
 License: MIT License
-Description: https://git.startinblox.com/djangoldp-packages/django-webidoidc-provider
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+https://git.startinblox.com/djangoldp-packages/django-webidoidc-provider
```

