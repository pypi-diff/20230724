# Comparing `tmp/djangoldp_account-2.3.9.tar.gz` & `tmp/djangoldp_account-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_account-2.3.9.tar", last modified: Tue Apr 12 06:24:14 2022, max compression
+gzip compressed data, was "djangoldp_account-3.0.1.tar", last modified: Mon Jul 24 19:59:25 2023, max compression
```

## Comparing `djangoldp_account-2.3.9.tar` & `djangoldp_account-3.0.1.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/
--rw-r--r--   0 root         (0) root         (0)      303 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     4971 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      155 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     8430 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      720 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      303 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/
--rw-rw-rw-   0 root         (0) root         (0)     9300 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/tests/
--rw-rw-rw-   0 root         (0) root         (0)     7440 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/tests/tests_auth_backends.py
--rw-rw-rw-   0 root         (0) root         (0)      713 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2201 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/tests/tests_update.py
--rw-rw-rw-   0 root         (0) root         (0)      738 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     9586 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9594 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/endpoints/rp_login.py
--rw-rw-rw-   0 root         (0) root         (0)     1296 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/endpoints/webfinger.py
--rw-rw-rw-   0 root         (0) root         (0)     1122 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       70 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      374 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      213 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      215 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)      329 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      929 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)      212 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/activation_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      808 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/lost_user.html
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/activate.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      112 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/logout.html
--rw-rw-rw-   0 root         (0) root         (0)     2969 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_change_done.html
--rw-rw-rw-   0 root         (0) root         (0)      170 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/registration_complete.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/templates/password/
--rw-rw-rw-   0 root         (0) root         (0)      614 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/password/email.html
--rw-rw-rw-   0 root         (0) root         (0)      877 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/registration_base.html
--rw-rw-rw-   0 root         (0) root         (0)      580 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_email_body.txt
--rw-rw-rw-   0 root         (0) root         (0)      580 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      576 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      264 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      385 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      364 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_failed.html
--rw-rw-rw-   0 root         (0) root         (0)     1346 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2446 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1142 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      584 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/mock_account.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/create_distant_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2919 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/import_csv.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/fill_user_fields.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-04-12 06:24:13.000000 djangoldp_account-2.3.9/djangoldp_account/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10465 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/de/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/de/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    14085 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/es/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     8589 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/es/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    13987 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     8349 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/fr/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    13553 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/en/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     8055 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)      551 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/static/
--rw-rw-rw-   0 root         (0) root         (0)     2675 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/static/base.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/static/registration/
--rw-rw-rw-   0 root         (0) root         (0)      624 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/static/registration/login.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/static/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)      270 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/static/oidc_provider/authorize.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/static/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/static/django_registration/registration_form.css
--rw-rw-rw-   0 root         (0) root         (0)      493 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/auth/
--rw-rw-rw-   0 root         (0) root         (0)     6749 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/auth/backends.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/auth/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/auth/solid.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/djangoldp_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0002_auto_20190917_1141.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0012_auto_20200501_1433.py
--rw-rw-rw-   0 root         (0) root         (0)      655 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0007_auto_20200130_1242.py
--rw-rw-rw-   0 root         (0) root         (0)     4931 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1239 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0010_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0014_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0016_auto_20200903_1049.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0011_auto_20200501_1420.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0009_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0003_auto_20191024_0854.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0006_auto_20200121_1321.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0013_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0005_ldpuser_default_redirect_uri.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0017_auto_20200910_1606.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0008_auto_20200130_1251.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0015_auto_20200617_1817.py
--rw-rw-rw-   0 root         (0) root         (0)      407 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0018_auto_20210223_2254.py
--rw-rw-rw-   0 root         (0) root         (0)      606 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0004_auto_20191203_0921.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.802680 djangoldp_account-3.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-24 19:59:25.802680 djangoldp_account-3.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8962 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.786680 djangoldp_account-3.0.1/djangoldp_account/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-24 19:59:22.000000 djangoldp_account-3.0.1/djangoldp_account/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/auth/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6745 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/auth/backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/auth/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     3141 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/auth/solid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/djangoldp_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9594 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/endpoints/rp_login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/endpoints/webfinger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.786680 djangoldp_account-3.0.1/djangoldp_account/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.782680 djangoldp_account-3.0.1/djangoldp_account/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     9063 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.786680 djangoldp_account-3.0.1/djangoldp_account/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7687 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    12366 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.786680 djangoldp_account-3.0.1/djangoldp_account/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     8046 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13008 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.786680 djangoldp_account-3.0.1/djangoldp_account/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7801 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    12899 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/commands/create_distant_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/commands/fill_user_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/commands/import_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/commands/mock_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     4931 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0002_auto_20190917_1141.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0003_auto_20191024_0854.py
+-rw-rw-rw-   0 root         (0) root         (0)      606 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0004_auto_20191203_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0005_ldpuser_default_redirect_uri.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0006_auto_20200121_1321.py
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0007_auto_20200130_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0008_auto_20200130_1251.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0009_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0010_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0011_auto_20200501_1420.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0012_auto_20200501_1433.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0013_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0014_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0015_auto_20200617_1817.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0016_auto_20200903_1049.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0017_auto_20200910_1606.py
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0018_auto_20210223_2254.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0019_auto_20221031_1426.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9600 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/static/
+-rw-rw-rw-   0 root         (0) root         (0)     2675 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/static/base.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/static/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/static/django_registration/registration_form.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/static/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/static/oidc_provider/authorize.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/static/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/static/registration/login.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.798680 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_email_body.txt
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_failed.html
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/registration_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/registration_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.798680 djangoldp_account-3.0.1/djangoldp_account/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.798680 djangoldp_account-3.0.1/djangoldp_account/templates/password/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/password/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.802680 djangoldp_account-3.0.1/djangoldp_account/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/activate.html
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/activation_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/lost_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_change_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/registration_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.802680 djangoldp_account-3.0.1/djangoldp_account/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      814 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     7461 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/tests/tests_auth_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     2201 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/tests/tests_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     9436 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-24 19:59:25.000000 djangoldp_account-3.0.1/djangoldp_account.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5027 2023-07-24 19:59:25.000000 djangoldp_account-3.0.1/djangoldp_account.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 19:59:25.000000 djangoldp_account-3.0.1/djangoldp_account.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-24 19:59:25.000000 djangoldp_account-3.0.1/djangoldp_account.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-24 19:59:25.000000 djangoldp_account-3.0.1/djangoldp_account.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-24 19:59:25.802680 djangoldp_account-3.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account.egg-info/SOURCES.txt` & `djangoldp_account-3.0.1/djangoldp_account.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 djangoldp_account/migrations/0012_auto_20200501_1433.py
 djangoldp_account/migrations/0013_auto_20200505_1733.py
 djangoldp_account/migrations/0014_auto_20200610_1323.py
 djangoldp_account/migrations/0015_auto_20200617_1817.py
 djangoldp_account/migrations/0016_auto_20200903_1049.py
 djangoldp_account/migrations/0017_auto_20200910_1606.py
 djangoldp_account/migrations/0018_auto_20210223_2254.py
+djangoldp_account/migrations/0019_auto_20221031_1426.py
 djangoldp_account/migrations/__init__.py
 djangoldp_account/static/base.css
 djangoldp_account/static/django_registration/registration_form.css
 djangoldp_account/static/oidc_provider/authorize.css
 djangoldp_account/static/registration/login.css
 djangoldp_account/templates/base.html
 djangoldp_account/templates/django_registration/activation_complete.html
```

### Comparing `djangoldp_account-2.3.9/README.md` & `djangoldp_account-3.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 ## Synopsis
 
 This module is an add-on for Django that provides WebID-OIDC accounts management. It plays two roles:
 - The Relying Party
 - The Authentification provider
 
 ## Requirements
-
-* djangoldp~=0.5
-* validators~=0.12
-* pyoic~=0.15
-* django-webidoidc-provider==0.1
+* djangoldp~=3.0
+* django_registration~=3.4
+* validators~=0.20
+* oic~=1.6
+* django-webidoidc-provider~=1.0
+* djangorestframework>=3.14
 
 ## Installation
 
 1. Install this module and all its dependencies
 
 ```
 pip install djangoldp_account
@@ -64,20 +65,26 @@
 
 ```python
 REGISTRATION_FIELDS = ('username', 'email', 'password1', 'password2')
 ```
 
 This will be sufficient to change the user fields on display on the form. If you want to customise the form (for example by [adding a model relationship to the user](https://stackoverflow.com/questions/14726725/python-django-django-registration-add-an-extra-field/14879316#14879316)), then you can override the setting `REGISTRATION_USER_FORM` to replace it altogether. The form you supply should extend `djangoldp_account.forms.LDPUserForm` or at minimum `django_registration.forms.RegistrationForm`
 
-```
+```yaml
 REGISTRATION_USER_FORM: "djangoldp_hiphopcommunity.forms.HipHopUserForm"
 ```
 
 In either case, at a minimum the registration form fields must include the fields `('username', 'email', 'password1', 'password2')`
 
+the setting `REGISTRATION_TEMPLATE_PATH` changes the path of the template serving the form, e.g.
+
+```yaml
+REGISTRATION_TEMPLATE_PATH: "hiphopcommunity/registration_form.html"
+```
+
 Visit http://127.0.0.1:8000/auth/register/ to access the registration form
 
 ### Enabling account activation without mail
 
 Optionally, you can also enable the user account activation without sending the activation mail, by setting:
 
 ```yaml
@@ -238,7 +245,16 @@
         #... Your Middlewares ...
         'django.middleware.locale.LocaleMiddleware',
 ]
 
 USE_L10N = True
 ```
 
+## ACCOUNT DEFAULT PICTURE
+
+There is a way to set a profile picture in the account section of every created user by default, and it is using the following settings key:
+
+```
+ACCOUNT_DEFAULT_PICTURE = 'https://example.com/profile.jpg'
+```
+
+That allows to avoid having an empty picture client side.
```

### Comparing `djangoldp_account-2.3.9/setup.cfg` & `djangoldp_account-3.0.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [metadata]
 name = djangoldp_account
 version = attr: djangoldp_account.__version__
 url = http://git.happy-dev.fr/startinblox/djangoldp_account
 author = Startin'blox
-author_email = jblemee@happy-dev.fr
+author_email = tech@startinblox.com
 description = djangoldp package for account and chat data models
 license = MIT
 
 [options]
 include_package_data = True
 packages = find:
 install_requires = 
-	djangoldp~=2.1
-	django_registration~=3.0.1
-	validators~=0.12
-	oic~=0.15
-	django-webidoidc-provider>=0.1.0
-	djangorestframework>=3.12
+	djangoldp~=3.0
+	django_registration~=3.4
+	validators~=0.20
+	oic~=1.6
+	django-webidoidc-provider~=1.0
+	djangorestframework>=3.14
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
 
 [semantic_release]
 version_source = tag
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/views.py` & `djangoldp_account-3.0.1/djangoldp_account/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.http import HttpResponse, JsonResponse, HttpResponseRedirect, HttpResponseNotFound
 from django.views import View
 from django.contrib.auth import get_user_model
-from django.contrib.auth.views import LoginView, SuccessURLAllowedHostsMixin
+from django.contrib.auth.views import LoginView, RedirectURLMixin
 from django.shortcuts import redirect, render
 from django.urls import reverse, reverse_lazy
 from django.utils.http import (
-    is_safe_url, urlsafe_base64_decode,
+    url_has_allowed_host_and_scheme, urlsafe_base64_decode,
 )
 from django.contrib.auth import authenticate, get_user_model, login
 from django_registration import signals
 from django_registration.backends.activation.views import RegistrationView
 from djangoldp_account import settings
 from django.conf import settings as django_settings
 
@@ -33,15 +33,15 @@
     return userinfo(request, *args, **kwargs)
 
 
 def check_user(request, *args, **kwargs):
     '''Returns user if they are authenticated with this server, else 404'''
     response = HttpResponse({}, status=200)
     if request.method in ['GET', 'HEAD', 'OPTIONS']:
-        response['Access-Control-Allow-Origin'] = request.META.get('HTTP_ORIGIN')
+        response['Access-Control-Allow-Origin'] = request.headers.get('origin')
         response["Access-Control-Allow-Headers"] = \
             oidc_settings.get('OIDC_ACCESS_CONTROL_ALLOW_HEADERS')
         response["Access-Control-Allow-Credentials"] = 'true'
         response["Access-Control-Expose-Headers"] = "Location, User"
     if request.method == 'OPTIONS':
         return response
 
@@ -50,15 +50,15 @@
         if 'Authorization' in request.headers:
             response_body['Authorization'] = request.headers['Authorization']
 
         if 'Dpop' in request.headers:
             response_body['dpop'] = request.headers['Dpop']
 
         response = JsonResponse(settings.userinfo(response_body, request.user))
-        response['Access-Control-Allow-Origin'] = request.META.get('HTTP_ORIGIN')
+        response['Access-Control-Allow-Origin'] = request.headers.get('origin')
         response["Access-Control-Allow-Headers"] = \
             oidc_settings.get('OIDC_ACCESS_CONTROL_ALLOW_HEADERS')
         response["Access-Control-Expose-Headers"] = "Location, User"
         response["Access-Control-Allow-Credentials"] = 'true'
 
         try:
             response['User'] = request.user.webid()
@@ -139,25 +139,27 @@
         next = request.POST.get('next')
 
         _set_default_redirect_uri(request.user, next)
 
         return return_value
 
 
-class LDPAccountRegistrationView(SuccessURLAllowedHostsMixin, RegistrationView):
+class LDPAccountRegistrationView(RedirectURLMixin, RegistrationView):
     """
     Extension of django-registration's RegistrationView for managing user's default_redirect_uri
     """
+    template_name = getattr(django_settings, 'REGISTRATION_TEMPLATE_PATH', 'django_registration/registration_form.html')
+
     def get_redirect_url(self):
         """Return the user-originating redirect URL if it's safe."""
         redirect_to = self.request.POST.get(
             'next',
             self.request.GET.get('next', '')
         )
-        url_is_safe = is_safe_url(
+        url_is_safe = url_has_allowed_host_and_scheme(
             url=redirect_to,
             allowed_hosts=self.get_success_url_allowed_hosts(),
             require_https=self.request.is_secure(),
         )
         return redirect_to if url_is_safe else ''
 
     def get_context_data(self, **kwargs):
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/tests/tests_auth_backends.py` & `djangoldp_account-3.0.1/djangoldp_account/tests/tests_auth_backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from oidc_provider.views import TokenView, JwksView
 from oidc_provider.lib.utils.token import create_code
 from oidc_provider.tests.app.utils import create_fake_client, FAKE_NONCE, create_fake_dpop_proof
 
 from djangoldp_account.models import LDPUser
 from djangoldp_account.tests.models import OwnedResource
 
-
+#TODO: catch warnings
 class AuthBackendTestCase(APITestCase):
     def setUp(self):
         call_command('creatersakey')
         self.client = APIClient()
         self.user = LDPUser.objects.create(email='{}@test.co.uk'.format(str(uuid.uuid4())), first_name='Test',
                                            last_name='Test', username=str(uuid.uuid4()))
         self.factory = RequestFactory()
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/tests/models.py` & `djangoldp_account-3.0.1/djangoldp_account/tests/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/tests/tests_update.py` & `djangoldp_account-3.0.1/djangoldp_account/tests/tests_update.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/tests/runner.py` & `djangoldp_account-3.0.1/djangoldp_account/tests/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # create a test configuration
 config = {
     # add the packages to the reference list
     'ldppackages': ['djangoldp_account', 'djangoldp_account.tests'],
 
     # required values for server
     'server': {
+        'SECRET_KEY': "$r&)p-4k@h5b!1yrft6&q%j)_p$lxqh6#)jeeu0z1iag&y&wdu",
         'JABBER_DEFAULT_HOST': ''
     }
 }
 
 ldpsettings = LDPSettings(config)
 django_settings.configure(ldpsettings)
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/models.py` & `djangoldp_account-3.0.1/djangoldp_account/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import re, unicodedata
 import uuid
+
 from urllib.parse import urlparse
 from django.conf import settings
 from django.core.mail import send_mail
 from django.core.validators import RegexValidator
 from django.contrib.auth.models import AbstractUser
 from django.db import models
 from django.template import loader
 from django.db.models.signals import post_save, pre_save
 from django.dispatch import receiver
 from django.urls import reverse_lazy
 from django.utils.deconstruct import deconstructible
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from importlib import import_module
 from djangoldp.models import Model
 from djangoldp.permissions import LDPPermissions
-from djangoldp_account.permissions import LDPUserPermissions
+from djangoldp_account.permissions import IPOpenPermissions
 
 
 djangoldp_modules = list(settings.DJANGOLDP_PACKAGES)
 user_fields = ['@id', 'first_name', 'groups', 'last_name', 'username', 'email', 'account', 'chatProfile', 'name']
 
 if 'djangoldp_uploader' in settings.DJANGOLDP_PACKAGES:
     user_fields += ['uploadURL']
@@ -39,30 +40,30 @@
 s_fields = []
 s_fields.extend(user_fields)
 s_fields.extend(user_nested_fields)
 
 
 @deconstructible
 class UsernameValidator(RegexValidator):
-    regex = r'^[\w.+-]+$'
+    regex = r'^[\w._-]+$'
     message = _(
         "Entre un nom d'utilisateur valide. Il ne peut contenir que des lettres, "
-        'des chiffres, et les caractères ./+/-/_'
+        'des chiffres, et les caractères ./-/_'
     )
     flags = re.UNICODE
 
 
 class LDPUser(AbstractUser, Model):
     slug = models.SlugField(unique=True, blank=True, null=True)
     username_validator = UsernameValidator()
     username = models.CharField(
         _('username'),
         max_length=150,
         unique=True,
-        help_text=_('Requiert 150 caractères ou moins. Seulement des lettres, chiffres et les caractères ./+/-/_'),
+        help_text=_('Requiert 150 caractères ou moins. Seulement des lettres, chiffres et les caractères ./-/_'),
         validators=[username_validator],
         error_messages={
             'unique': _("Ce nom d'utilisateur est déjà pris."),
         },
     )
     email = models.EmailField(
         _('email address'),
@@ -79,16 +80,16 @@
     class Meta:
         depth = 1
         verbose_name = _('user')
         verbose_name_plural = _('users')
         rdf_type = 'foaf:user'
         lookup_field = 'slug'
         container_path = 'users'
-        owner_field = 'urlid'
-        permission_classes = getattr(settings, 'USER_PERMISSION_CLASSES', [LDPUserPermissions])
+        owner_urlid_field = 'urlid'
+        permission_classes = getattr(settings, 'USER_PERMISSION_CLASSES', [IPOpenPermissions])
         nested_fields = user_nested_fields
         serializer_fields = s_fields
         empty_containers = user_empty_containers
         anonymous_perms = getattr(settings, 'USER_ANONYMOUS_PERMISSIONS', [])
         authenticated_perms = getattr(settings, 'USER_AUTHENTICATED_PERMISSIONS', ['inherit'])
         owner_perms = getattr(settings, 'USER_OWNER_PERMISSIONS', ['inherit'])
 
@@ -96,15 +97,15 @@
         return self.get_full_name()
     
     def uploadURL(self):
         return {"@id": settings.BASE_URL + "/upload/"}
 
     def webid(self):
         # remote user
-        if self.urlid is not None and urlparse(self.urlid).netloc != urlparse(settings.BASE_URL).netloc:
+        if Model.is_external(self.urlid):
             webid = self.urlid
         else:
             webid = '{0}{1}'.format(settings.BASE_URL, reverse_lazy('ldpuser-detail', kwargs={'slug': self.slug}))
         return webid
 
     def save(self, *args, **kwargs):
         if self.username == "hubl-workaround-493":
@@ -133,26 +134,26 @@
     def __str__(self):
         return self.urlid
 
 
 class Account(Model):
     user = models.OneToOneField(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
     slug = models.SlugField(unique=True)
-    picture = models.URLField(blank=True, null=True)
+    picture = models.URLField(blank=True, null=True, default=getattr(settings, 'ACCOUNT_DEFAULT_PICTURE', None))
     issuer = models.URLField(blank=True, null=True)
 
     class Meta:
         auto_author = 'user'
         permissions = (
             ('control_account', 'Control'),
         )
         lookup_field = 'slug'
         owner_field = 'user'
-        permission_classes = getattr(settings, 'USER_PERMISSION_CLASSES', [LDPPermissions])
-        anonymous_perms = getattr(settings, 'USER_ANONYMOUS_PERMISSIONS', ['view'])
+        permission_classes = getattr(settings, 'USER_PERMISSION_CLASSES', [IPOpenPermissions])
+        anonymous_perms = getattr(settings, 'USER_ANONYMOUS_PERMISSIONS', [])
         authenticated_perms = getattr(settings, 'USER_AUTHENTICATED_PERMISSIONS', ['inherit'])
         owner_perms = getattr(settings, 'USER_OWNER_PERMISSIONS', ['inherit'])
 
     def __str__(self):
         return '{} ({})'.format(self.user.get_full_name(), self.user.username)
 
 
@@ -164,16 +165,16 @@
     class Meta:
         auto_author = 'user'
         permissions = (
             ('control_chatprofile', 'Control'),
         )
         lookup_field = 'slug'
         owner_field = 'user'
-        permission_classes = getattr(settings, 'USER_PERMISSION_CLASSES', [LDPPermissions])
-        anonymous_perms = getattr(settings, 'USER_ANONYMOUS_PERMISSIONS', ['view'])
+        permission_classes = getattr(settings, 'USER_PERMISSION_CLASSES', [IPOpenPermissions])
+        anonymous_perms = getattr(settings, 'USER_ANONYMOUS_PERMISSIONS', [])
         authenticated_perms = getattr(settings, 'USER_AUTHENTICATED_PERMISSIONS', ['inherit'])
         owner_perms = getattr(settings, 'USER_OWNER_PERMISSIONS', ['inherit'])
 
     def __str__(self):
         return '{} (jabberID: {})'.format(self.user.get_full_name(), self.jabberID)
 
 
@@ -225,15 +226,15 @@
 @receiver(post_save, sender=settings.AUTH_USER_MODEL)
 def create_account(sender, instance, created, **kwargs):
     if not Model.is_external(instance):
         if created:
             Account.objects.create(user=instance, slug=instance.username)
             chat_profile = ChatProfile.objects.create(user=instance, slug=instance.username)
             if isinstance(getattr(settings, 'JABBER_DEFAULT_HOST', False), str):
-                chat_profile.jabberID = '{}@{}'.format(instance.username, settings.JABBER_DEFAULT_HOST)
+                chat_profile.jabberID = '{}@{}'.format(instance.username + uuid.uuid4().hex[:7], settings.JABBER_DEFAULT_HOST)
                 chat_profile.save()
         else:
             try:
                 instance.account.slug = instance.username
                 instance.account.save()
                 instance.chatProfile.slug = instance.username
                 instance.chatProfile.save()
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/endpoints/rp_login.py` & `djangoldp_account-3.0.1/djangoldp_account/endpoints/rp_login.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/endpoints/webfinger.py` & `djangoldp_account-3.0.1/djangoldp_account/endpoints/webfinger.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_form.html` & `djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/templates/registration/lost_user.html` & `djangoldp_account-3.0.1/djangoldp_account/templates/registration/lost_user.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/templates/registration/login.html` & `djangoldp_account-3.0.1/djangoldp_account/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/templates/oidc_provider/authorize.html` & `djangoldp_account-3.0.1/djangoldp_account/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/templates/password/email.html` & `djangoldp_account-3.0.1/djangoldp_account/templates/password/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/templates/base.html` & `djangoldp_account-3.0.1/djangoldp_account/templates/base.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_email_body.txt` & `djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_email_body.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_complete.html` & `djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/registration_form.html` & `djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/admin.py` & `djangoldp_account-3.0.1/djangoldp_account/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from django.contrib.auth.admin import UserAdmin
 from django.contrib.auth.forms import UserChangeForm
 from djangoldp.admin import DjangoLDPUserAdmin
 from djangoldp_account.models import LDPUser
 from .models import Account, ChatProfile
 
 
+@admin.register(Account, ChatProfile)
 class EmptyAdmin(admin.ModelAdmin):
     def get_model_perms(self, request):
         return {}
 
 
 class LDPUserChangeForm(UserChangeForm):
     class Meta(UserChangeForm.Meta):
@@ -24,27 +25,25 @@
 
 class ChatProfileInline(admin.StackedInline):
     model = ChatProfile
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink', 'slug')
     extra = 0
 
 
+@admin.register(LDPUser)
 class LDPUserAdmin(DjangoLDPUserAdmin):
     exclude = ('is_backlink', 'allow_create_backlink')
     form = LDPUserChangeForm
 
-    inlines = DjangoLDPUserAdmin.inlines + [
+    inlines = DjangoLDPUserAdmin.inlines + (
         AccountInline,
         ChatProfileInline
-    ]
+    )
 
     fieldsets = DjangoLDPUserAdmin.fieldsets + (
         (None, {'fields': ('default_redirect_uri',)}),
     )
     add_fieldsets = DjangoLDPUserAdmin.add_fieldsets + (
-        (None, {'fields': ('email',)}),
+        (None, {'fields': ('email', 'first_name', 'last_name')}),
     )
 
 
-admin.site.register(LDPUser, LDPUserAdmin)
-admin.site.register(Account, EmptyAdmin)
-admin.site.register(ChatProfile, EmptyAdmin)
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/djangoldp_urls.py` & `djangoldp_account-3.0.1/djangoldp_account/djangoldp_urls.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """djangoldp project URL Configuration"""
 
 from pydoc import locate
 from django.conf import settings
-from django.conf.urls import url, include
+from django.urls import path, re_path, include
 from django.contrib.auth.models import Group
 from django.views.decorators.csrf import csrf_exempt
 
 from djangoldp.permissions import LDPPermissions
 from djangoldp.views import LDPViewSet
 from djangoldp_account.forms import LDPUserForm
 from .models import ChatProfile, Account
@@ -18,32 +18,32 @@
 Group._meta.authenticated_perms = getattr(settings, 'GROUP_AUTHENTICATED_PERMISSIONS', ['inherit'])
 Group._meta.owner_perms = getattr(settings, 'GROUP_OWNER_PERMISSIONS', ['inherit'])
 
 user_form_override = getattr(settings, 'REGISTRATION_USER_FORM', None)
 user_form = LDPUserForm if user_form_override is None else locate(user_form_override)
 
 urlpatterns = [
-    url(r'^groups/',
+    path('groups/',
         LDPViewSet.urls(model=Group, fields=['@id', 'name', 'user_set'],
                         permission_classes=getattr(settings, 'GROUP_PERMISSION_CLASSES', [LDPPermissions]),
         )
     ),
-    url(r'^auth/register/$',
+    path('auth/register/',
         LDPAccountRegistrationView.as_view(
             form_class=user_form
         ),
         name='django_registration_register',
     ),
-    url(r'^auth/login/$', LDPAccountLoginView.as_view(),name='login'),
-    url(r'^auth/', include('django_registration.backends.activation.urls')),
-    url(r'^auth/', include('django.contrib.auth.urls')),
-    url(r'^accounts/', LDPViewSet.urls(model=Account, permission_classes=[LDPPermissions], model_prefix='pk_lookup',
+    path('auth/login/', LDPAccountLoginView.as_view(),name='login'),
+    path('auth/', include('django_registration.backends.activation.urls')),
+    path('auth/', include('django.contrib.auth.urls')),
+    path('accounts/', LDPViewSet.urls(model=Account, permission_classes=[LDPPermissions], model_prefix='pk_lookup',
                                        lookup_field='pk')),
-    url(r'^chat-profile/', LDPViewSet.urls(model=ChatProfile, permission_classes=[LDPPermissions],
+    path('chat-profile/', LDPViewSet.urls(model=ChatProfile, permission_classes=[LDPPermissions],
                                            model_prefix='pk_lookup', lookup_field='pk')),
-    url(r'^oidc/login/callback/?$', RPLoginCallBackView.as_view(), name='oidc_login_callback'),
-    url(r'^oidc/login/?$', RPLoginView.as_view(), name='oidc_login'),
-    url(r'^userinfo/?$', csrf_exempt(userinfocustom)),
-    url(r'^check-user/?$', csrf_exempt(check_user)),
-    url(r'^redirect-default/$', RedirectView.as_view(),name='redirect-default'),
-    url(r'^', include('oidc_provider.urls', namespace='oidc_provider'))
+    re_path(r'^oidc/login/callback/?$', RPLoginCallBackView.as_view(), name='oidc_login_callback'),
+    re_path(r'^oidc/login/?$', RPLoginView.as_view(), name='oidc_login'),
+    re_path(r'^userinfo/?$', csrf_exempt(userinfocustom)),
+    re_path(r'^check-user/?$', csrf_exempt(check_user)),
+    path('redirect-default/', RedirectView.as_view(),name='redirect-default'),
+    path('', include('oidc_provider.urls', namespace='oidc_provider'))
 ]
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/errors.py` & `djangoldp_account-3.0.1/djangoldp_account/errors.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/management/commands/mock_account.py` & `djangoldp_account-3.0.1/djangoldp_account/management/commands/mock_account.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/management/commands/create_distant_admin.py` & `djangoldp_account-3.0.1/djangoldp_account/management/commands/create_distant_admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/management/commands/import_csv.py` & `djangoldp_account-3.0.1/djangoldp_account/management/commands/import_csv.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/management/commands/fill_user_fields.py` & `djangoldp_account-3.0.1/djangoldp_account/management/commands/fill_user_fields.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/factories.py` & `djangoldp_account-3.0.1/djangoldp_account/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/locale/es/LC_MESSAGES/django.mo` & `djangoldp_account-3.0.1/djangoldp_account/locale/es/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -138,27 +138,17 @@
 
 msgid "Enregistrement du compte pour %(sitename)s"
 msgstr "Registro de la cuenta para %(sitename)s"
 
 msgid "Enregistrer un compte"
 msgstr "Registrar una cuenta"
 
-msgid ""
-"Entre un nom d'utilisateur valide. Il ne peut contenir que des lettres, des "
-"chiffres, et les caractères ./+/-/_"
-msgstr ""
-"Ingresa un nombre de usuario válido. Solo puede contener letras, números y "
-"los caracteres ./+/-/_"
-
 msgid "Envoyer"
 msgstr "Envíar"
 
-msgid "Envoyer un e-mail d'activation"
-msgstr "Enviar un correo electrónico de activación"
-
 msgid "Envoyez-moi les instructions !"
 msgstr "¡Envíame las instrucciones!"
 
 msgid ""
 "Indique ton adresse e-mail ci-dessous et nous t'enverrons des instructions "
 "par e-mail pour en définir un nouveau."
 msgstr ""
@@ -207,21 +197,14 @@
 
 msgid "Perdu"
 msgstr "Perdido"
 
 msgid "Refuser"
 msgstr "Rechazar"
 
-msgid ""
-"Requiert 150 caractères ou moins. Seulement des lettres, chiffres et les "
-"caractères ./+/-/_"
-msgstr ""
-"Requiere 150 caracteres o menos. Solo letras, números y los caracteres ./+/-/"
-"_"
-
 msgid "Réinitialiser le mot de passe sur %(site_name)s"
 msgstr "Reset password on %(site_name)s"
 
 msgid "S'inscrire !"
 msgstr "¡Inscríbete!"
 
 msgid "Se connecter"
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/locale/fr/LC_MESSAGES/django.po` & `djangoldp_account-3.0.1/djangoldp_account/locale/en/LC_MESSAGES/django.po`

 * *Files 22% similar despite different names*

```diff
@@ -4,100 +4,104 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-12-03 09:55+0000\n"
+"POT-Creation-Date: 2022-10-17 19:04+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: djangoldp_account/models.py:43
+#: models.py:49
+#, fuzzy
+#| msgid ""
+#| "Entre un nom d'utilisateur valide. Il ne peut contenir que des lettres, "
+#| "des chiffres, et les caractères ./-/_"
 msgid ""
 "Entre un nom d'utilisateur valide. Il ne peut contenir que des lettres, des "
-"chiffres, et les caractères ./+/-/_"
+"chiffres, et les caractères ./-/_"
 msgstr ""
-"Entre un nom d'utilisateur valide. Il ne peut contenir que des lettres, des "
-"chiffres, et les caractères ./+/-/_"
+"Enter a valid username. It can only contain letters, numbers, and the "
+"characters ./-/_."
 
-#: djangoldp_account/models.py:53
+#: models.py:59
 msgid "username"
-msgstr ""
+msgstr "username"
 
-#: djangoldp_account/models.py:56
+#: models.py:62
+#, fuzzy
+#| msgid ""
+#| "Requiert 150 caractères ou moins. Seulement des lettres, chiffres et les "
+#| "caractères ./-/_"
 msgid ""
 "Requiert 150 caractères ou moins. Seulement des lettres, chiffres et les "
-"caractères ./+/-/_"
+"caractères ./-/_"
 msgstr ""
-"Requiert 150 caractères ou moins. Seulement des lettres, chiffres et les "
-"caractères ./+/-/_"
+"Requires 150 characters or less. Only letters, numbers and the characters ./"
+"-/_."
 
-#: djangoldp_account/models.py:59
+#: models.py:65
 msgid "Ce nom d'utilisateur est déjà pris."
-msgstr "Ce nom d'utilisateur est déjà pris."
+msgstr "This username is already taken."
 
-#: djangoldp_account/models.py:63
+#: models.py:69
 msgid "email address"
-msgstr ""
+msgstr "email address"
 
-#: djangoldp_account/models.py:68
+#: models.py:74
 msgid "Un utilisateur avec cette adresse mail existe déjà."
-msgstr "Un utilisateur avec cette adresse mail existe déjà."
+msgstr "A user with this email address already exists."
 
-#: djangoldp_account/models.py:76
+#: models.py:82
 msgid "user"
-msgstr ""
+msgstr "user"
 
-#: djangoldp_account/models.py:77
+#: models.py:83
 msgid "users"
-msgstr ""
+msgstr "users"
 
-#: djangoldp_account/models.py:195
-#, fuzzy
-#| msgid "Activation du compte sur"
+#: models.py:216
 msgid "Création de compte sur "
-msgstr "Activation du compte sur "
+msgstr "Account creation on "
 
-#: djangoldp_account/models.py:196
-#, fuzzy
-#| msgid "Un compte a été créé pour toi"
+#: models.py:217
 msgid "Compte créé sur "
-msgstr "Compte créé sur"
+msgstr "Account created on "
 
-#: djangoldp_account/templates/django_registration/activation_complete.html:3
+#: templates/django_registration/activation_complete.html:3
 msgid "Activation terminée"
-msgstr "Activation terminée"
+msgstr "Activation complete"
 
-#: djangoldp_account/templates/django_registration/activation_complete.html:6
+#: templates/django_registration/activation_complete.html:6
 msgid "Merci, l'activation est terminée !"
-msgstr "Merci, l'activation est terminée !"
+msgstr "Thank you, the activation is finished!"
 
-#: djangoldp_account/templates/django_registration/activation_complete.html:8
+#: templates/django_registration/activation_complete.html:8
 #, python-format
 msgid ""
 "\n"
 "            Tu peux maintenant te <a href='%(auth_login_url)s'>connecter</a> "
 "en utilisant le nom d'utilisateur et le mot de passe\n"
 "            que tu as définis lors de ton enregistrement.\n"
 "        "
 msgstr ""
 "\n"
-"            Tu peux maintenant te <a href='%(auth_login_url)s'>connecter</a> "
-"en utilisant le nom d'utilisateur et le mot de passe\n"
-"            que tu as définis lors de ton enregistrement.\n"
+"           Now you can <a href='%(auth_login_url)s'>connect</a> using the "
+"username and password\n"
+"           that you defined when you registered.\n"
 "        "
 
-#: djangoldp_account/templates/django_registration/activation_email_body.txt:3
+#: templates/django_registration/activation_email_body.txt:3
 #, python-format
 msgid ""
 "\n"
 "Tu (ou une autre personne se faisant passer pour toi) as demandé à "
 "enregistrer un compte sur %(sitename)s.\n"
 "Si ce n'était pas toi, ignore cet e-mail et ton adresse s'effacera de notre "
 "banque de données.\n"
@@ -108,291 +112,291 @@
 "\n"
 "http://%(siteurl)s%(activation_key_url)s\n"
 "\n"
 "Bonne journée,\n"
 "l'équipe %(sitename)s\n"
 msgstr ""
 "\n"
-"Tu (ou une autre personne se faisant passer pour toi) as demandé à "
-"enregistrer un compte sur %(sitename)s.\n"
-"Si ce n'était pas toi, ignore cet e-mail et ton adresse s'effacera de notre "
-"banque de données.\n"
-"\n"
-"Pour activer ce compte, tu peux cliquer sur le lien suivant dans un délai "
-"de \n"
-"%(expiration_days)s jours :\n"
+"You (or another person pretending to be you) have asked to register an "
+"account on %(sitename)s.\n"
+"If it wasn't you, ignore this email and your address will be deleted from "
+"our database.\n"
+"\n"
+"To activate this account, you can click on the following link within a delay "
+"of \n"
+"%(expiration_days)s days :\n"
 "\n"
 "http://%(siteurl)s%(activation_key_url)s\n"
 "\n"
-"Bonne journée,\n"
-"l'équipe %(sitename)s\n"
+"Have a nice day.\n"
+"The team %(sitename)s\n"
 
-#: djangoldp_account/templates/django_registration/activation_email_subject.txt:1
+#: templates/django_registration/activation_email_subject.txt:1
 #, python-format
 msgid "Enregistrement du compte pour %(sitename)s"
-msgstr "Enregistrement du compte pour %(sitename)s"
+msgstr "Account registration for %(sitename)s"
 
-#: djangoldp_account/templates/django_registration/activation_failed.html:3
+#: templates/django_registration/activation_failed.html:3
 msgid "Echec de l'activation"
-msgstr "Echec de l'activation"
+msgstr "Failed activation"
 
-#: djangoldp_account/templates/django_registration/activation_failed.html:5
+#: templates/django_registration/activation_failed.html:5
 msgid "Échec de l'activation de l'utilisateur."
-msgstr "Échec de l'activation de l'utilisateur."
+msgstr "User activation failed."
 
-#: djangoldp_account/templates/django_registration/activation_failed.html:6
+#: templates/django_registration/activation_failed.html:6
 msgid "Contacte ton administrateur pour plus d'informations."
-msgstr "Contacte ton administrateur pour plus d'informations."
+msgstr "Contact your administrator for more information."
 
-#: djangoldp_account/templates/django_registration/registration_closed.html:3
+#: templates/django_registration/registration_closed.html:3
 msgid "Inscription terminée"
-msgstr "Inscription terminée"
+msgstr "Registration closed"
 
-#: djangoldp_account/templates/django_registration/registration_closed.html:5
+#: templates/django_registration/registration_closed.html:5
 msgid "L'inscription est fermée pour ce site."
-msgstr "L'inscription est fermée pour ce site."
+msgstr "Registration is closed for this site."
 
-#: djangoldp_account/templates/django_registration/registration_complete.html:3
+#: templates/django_registration/registration_complete.html:3
 msgid "E-mail d'activation envoyé"
-msgstr "E-mail d'activation envoyé"
+msgstr "Activation e-mail sent"
 
-#: djangoldp_account/templates/django_registration/registration_complete.html:5
+#: templates/django_registration/registration_complete.html:5
 msgid "Un e-mail d'activation a été envoyé."
-msgstr "Un e-mail d'activation a été envoyé."
+msgstr "An activation e-mail has been sent."
 
-#: djangoldp_account/templates/django_registration/registration_complete.html:6
+#: templates/django_registration/registration_complete.html:6
 msgid "Vérifie ta boite mail et clique sur le lien pour activer ton compte."
-msgstr "Vérifie ta boite mail et clique sur le lien pour activer ton compte."
+msgstr "Check your mailbox and click on the link to activate your account."
 
-#: djangoldp_account/templates/django_registration/registration_form.html:5
+#: templates/django_registration/registration_form.html:5
 msgid "Enregistrer un compte"
-msgstr "Enregistrer un compte"
+msgstr "Register an account"
 
-#: djangoldp_account/templates/django_registration/registration_form.html:16
-msgid "Envoyer un e-mail d'activation"
-msgstr "Envoyer un e-mail d'activation"
+#: templates/django_registration/registration_form.html:16
+#, fuzzy
+#| msgid "Envoyer un e-mail d'activation"
+msgid "Envoyer un e-mail d\\"
+msgstr "Send an activation e-mail"
 
-#: djangoldp_account/templates/oidc_provider/authorize.html:6
+#: templates/oidc_provider/authorize.html:6
 msgid "Demande d'accès aux informations"
-msgstr "Demande d'accès aux informations"
+msgstr "Information access request"
 
-#: djangoldp_account/templates/oidc_provider/authorize.html:17
+#: templates/oidc_provider/authorize.html:17
 msgid "Demande d'autorisation"
-msgstr "Demande d'autorisation"
+msgstr "Request for authorization"
 
-#: djangoldp_account/templates/oidc_provider/authorize.html:20
-#: djangoldp_account/templates/oidc_provider/authorize.html:22
+#: templates/oidc_provider/authorize.html:20
+#: templates/oidc_provider/authorize.html:22
 msgid "Le client"
-msgstr "Le client"
+msgstr "The client"
 
-#: djangoldp_account/templates/oidc_provider/authorize.html:20
+#: templates/oidc_provider/authorize.html:20
 msgid "voudrait accéder à ces informations te concernant :"
-msgstr "voudrait accéder à ces informations te concernant :"
+msgstr "would like to access this information about you :"
 
-#: djangoldp_account/templates/oidc_provider/authorize.html:22
+#: templates/oidc_provider/authorize.html:22
 msgid "voudrait accéder à ton compte."
-msgstr "voudrait accéder à ton compte."
+msgstr "would like to access your account."
 
-#: djangoldp_account/templates/oidc_provider/authorize.html:33
+#: templates/oidc_provider/authorize.html:33
 msgid "Refuser"
-msgstr "Refuser"
+msgstr "Decline"
 
-#: djangoldp_account/templates/oidc_provider/authorize.html:34
+#: templates/oidc_provider/authorize.html:34
 msgid "Autoriser"
-msgstr "Autoriser"
+msgstr "Authorize"
 
-#: djangoldp_account/templates/password/email.html:7
+#: templates/password/email.html:7
 msgid "Un compte a été créé pour toi"
-msgstr "Un compte a été créé pour toi"
+msgstr "An account has been created for you"
 
-#: djangoldp_account/templates/password/email.html:8
+#: templates/password/email.html:8
 msgid "Crée ton mot de passe en "
-msgstr "Crée ton mot de passe en "
+msgstr "Create your password by "
 
-#: djangoldp_account/templates/password/email.html:8
+#: templates/password/email.html:8
 msgid "suivant ce lien."
-msgstr "suivant ce lien."
+msgstr "following this link."
 
-#: djangoldp_account/templates/password/email.html:14
+#: templates/password/email.html:14
 msgid "Ne réponds pas directement à cet e-mail, à la place rends-toi sur"
-msgstr "Ne réponds pas directement à cet e-mail, à la place rends-toi sur"
+msgstr "Don't reply directly to this e-mail, but go to"
 
-#: djangoldp_account/templates/registration/activate.html:6
+#: templates/registration/activate.html:6
 msgid "Échec de l'activation du compte."
-msgstr "Échec de l'activation du compte."
+msgstr "Account activation failed."
 
-#: djangoldp_account/templates/registration/activation_complete.html:5
+#: templates/registration/activation_complete.html:5
 msgid "Ton compte est maintenant activé."
-msgstr "Ton compte est maintenant activé."
+msgstr "Your account is now activated."
 
-#: djangoldp_account/templates/registration/activation_email.txt:2
+#: templates/registration/activation_email.txt:2
 msgid "Active ton compte sur"
-msgstr "Active ton compte sur"
+msgstr "Activate your account on"
 
-#: djangoldp_account/templates/registration/activation_email.txt:6
+#: templates/registration/activation_email.txt:6
 #, python-format
 msgid "Ce lien est valide pendant %(expiration_days)s jours."
-msgstr "Ce lien est valide pendant %(expiration_days)s jours."
+msgstr "This link is valid for %(expiration_days)s days."
 
-#: djangoldp_account/templates/registration/activation_email_subject.txt:1
+#: templates/registration/activation_email_subject.txt:1
 msgid "Activation du compte sur"
-msgstr "Activation du compte sur"
+msgstr "Account activation on"
 
-#: djangoldp_account/templates/registration/login.html:6
-#: djangoldp_account/templates/registration/login.html:44
-#: djangoldp_account/templates/registration/login.html:58
-#: djangoldp_account/templates/registration/password_reset_complete.html:8
+#: templates/registration/login.html:6 templates/registration/login.html:44
+#: templates/registration/login.html:58
+#: templates/registration/password_reset_complete.html:8
 msgid "Se connecter"
-msgstr "Se connecter"
+msgstr "Login"
 
-#: djangoldp_account/templates/registration/login.html:18
+#: templates/registration/login.html:18
 msgid ""
 "\n"
 "                        Ton compte n'a pas accès à cette page. \n"
 "                        Pour continuer, connecte-toi avec un compte qui y a "
 "accès.\n"
 "                    "
 msgstr ""
 "\n"
-"                        Ton compte n'a pas accès à cette page. \n"
-"                        Pour continuer, connecte-toi avec un compte qui y a "
-"accès.\n"
+"                        Your account does not have access to this page. \n"
+"                        To continue, log in with an account that has "
+"access.\n"
 "                    "
 
-#: djangoldp_account/templates/registration/login.html:24
+#: templates/registration/login.html:24
 msgid "Connecte-toi pour voir cette page."
-msgstr "Connecte-toi pour voir cette page."
+msgstr "Login to see this page."
 
-#: djangoldp_account/templates/registration/login.html:32
+#: templates/registration/login.html:32
 msgid ""
 "Ton nom d'utilisateur et ton mot de passe ne correspondent pas. Réessaye."
-msgstr ""
-"Ton nom d'utilisateur et ton mot de passe ne correspondent pas. Réessaye."
+msgstr "Your username and password do not match. Please try again."
 
-#: djangoldp_account/templates/registration/login.html:37
+#: templates/registration/login.html:37
 msgid "Nom d'utilisateur ou e-mail:"
-msgstr "Nom d'utilisateur ou e-mail:"
+msgstr "Username or e-mail:"
 
-#: djangoldp_account/templates/registration/login.html:47
-#: djangoldp_account/templates/registration/password_reset_form.html:6
+#: templates/registration/login.html:47
+#: templates/registration/password_reset_form.html:6
 msgid "Mot de passe oublié ?"
-msgstr "Mot de passe oublié ?"
+msgstr "Forgot your password?"
 
-#: djangoldp_account/templates/registration/login.html:52
+#: templates/registration/login.html:52
 msgid "Se connecter avec un autre fournisseur d'identité"
-msgstr "Se connecter avec un autre fournisseur d'identité"
+msgstr "Connect with another identity provider"
 
-#: djangoldp_account/templates/registration/login.html:56
+#: templates/registration/login.html:56
 msgid "Webfinger :"
 msgstr "Webfinger :"
 
-#: djangoldp_account/templates/registration/login.html:66
+#: templates/registration/login.html:66
 msgid "Tu n'as pas encore de compte ?"
-msgstr "Tu n'as pas encore de compte ?"
+msgstr "Don't you have an account yet?"
 
-#: djangoldp_account/templates/registration/login.html:67
+#: templates/registration/login.html:67
 msgid "S'inscrire !"
-msgstr "S'inscrire !"
+msgstr "Register!"
 
-#: djangoldp_account/templates/registration/logout.html:5
+#: templates/registration/logout.html:5
 msgid "Déconnecté"
-msgstr "Déconnecté"
+msgstr "Logged off"
 
-#: djangoldp_account/templates/registration/lost_user.html:6
+#: templates/registration/lost_user.html:6
 msgid "Perdu"
-msgstr "Perdu"
+msgstr "Lost"
 
-#: djangoldp_account/templates/registration/lost_user.html:16
+#: templates/registration/lost_user.html:16
 msgid ""
 "\n"
 "                    Désolé, nous n'avons pas trouvé de page où te rediriger. "
 "Navigue manuellement \n"
 "                    vers ton application préférée.\n"
 "                "
 msgstr ""
 "\n"
-"                    Désolé, nous n'avons pas trouvé de page où te rediriger. "
-"Navigue manuellement \n"
-"                    vers ton application préférée.\n"
-"                "
+"                    Sorry, we couldn't find a page to redirect you to. "
+"Navigate manually\n"
+"                    to your favorite app.\n"
+" "
 
-#: djangoldp_account/templates/registration/lost_user.html:22
+#: templates/registration/lost_user.html:22
 msgid ""
 "\n"
 "                    Si tu n'es pas sûr, contacte un administrateur système.\n"
 "                "
 msgstr ""
 "\n"
-"                    Si tu n'es pas sûr, contacte un administrateur système.\n"
+"                    If you're not sure, contact a system administrator.\n"
 "                "
 
-#: djangoldp_account/templates/registration/password_change_done.html:5
+#: templates/registration/password_change_done.html:5
 msgid "Mot de passe modifié"
-msgstr "Mot de passe modifié"
+msgstr "Password updated"
 
-#: djangoldp_account/templates/registration/password_change_form.html:9
-#: djangoldp_account/templates/registration/password_reset_confirm.html:12
-#: djangoldp_account/templates/registration/registration_form.html:9
+#: templates/registration/password_change_form.html:9
+#: templates/registration/password_reset_confirm.html:12
+#: templates/registration/registration_form.html:9
 msgid "Envoyer"
-msgstr "Envoyer"
+msgstr "Send"
 
-#: djangoldp_account/templates/registration/password_reset_complete.html:6
+#: templates/registration/password_reset_complete.html:6
 msgid "Mot de passe réinitialisé avec succès"
-msgstr "Mot de passe réinitialisé avec succès"
+msgstr "Password successfully reset"
 
-#: djangoldp_account/templates/registration/password_reset_confirm.html:17
+#: templates/registration/password_reset_confirm.html:17
 msgid "Échec de la réinitialisation du mot de passe"
-msgstr "Échec de la réinitialisation du mot de passe"
+msgstr "Failure to reset the password"
 
-#: djangoldp_account/templates/registration/password_reset_done.html:3
+#: templates/registration/password_reset_done.html:3
 msgid "E-mail envoyé"
-msgstr "E-mail envoyé"
+msgstr "E-mail sent"
 
-#: djangoldp_account/templates/registration/password_reset_done.html:5
+#: templates/registration/password_reset_done.html:5
 msgid "Vérifie ta boite mail."
-msgstr "Vérifie ta boite mail."
+msgstr "Check your mailbox."
 
-#: djangoldp_account/templates/registration/password_reset_done.html:6
+#: templates/registration/password_reset_done.html:6
 msgid ""
 "Nous t'avons envoyé des instructions pour définir ton mot de passe. Tu "
 "devrais recevoir cet e-mail dans peu de temps !"
 msgstr ""
-"Nous t'avons envoyé des instructions pour définir ton mot de passe. Tu "
-"devrais recevoir cet e-mail dans peu de temps !"
+"We have sent you instructions on how to set your password. You should be "
+"receiving this e-mail shortly!"
 
-#: djangoldp_account/templates/registration/password_reset_email.html:2
+#: templates/registration/password_reset_email.html:2
 #, python-format
 msgid "Réinitialiser le mot de passe sur %(site_name)s"
-msgstr "Réinitialiser le mot de passe sur %(site_name)s"
+msgstr "Reset password on %(site_name)s"
 
-#: djangoldp_account/templates/registration/password_reset_form.html:11
+#: templates/registration/password_reset_form.html:11
 msgid "Tu as oublié ton mot de passe ?"
-msgstr "Tu as oublié ton mot de passe ?"
+msgstr "Forgot your password?"
 
-#: djangoldp_account/templates/registration/password_reset_form.html:12
+#: templates/registration/password_reset_form.html:12
 msgid ""
 "Indique ton adresse e-mail ci-dessous et nous t'enverrons des instructions "
 "par e-mail pour en définir un nouveau."
 msgstr ""
-"Indique ton adresse e-mail ci-dessous et nous t'enverrons des instructions "
-"par e-mail pour en définir un nouveau."
+"Enter your email address below and we will send you instructions by e-mail "
+"to set up a new one."
 
-#: djangoldp_account/templates/registration/password_reset_form.html:20
+#: templates/registration/password_reset_form.html:20
 msgid "Envoyez-moi les instructions !"
-msgstr "Envoyez-moi les instructions !"
+msgstr "Send me the instructions!"
 
-#: djangoldp_account/templates/registration/password_reset_form.html:24
+#: templates/registration/password_reset_form.html:24
 msgid "Ton adresse e-mail est invalide."
-msgstr "Ton adresse e-mail est invalide."
+msgstr "Your email address is invalid."
 
-#: djangoldp_account/templates/registration/password_reset_subject.txt:3
+#: templates/registration/password_reset_subject.txt:3
 #, python-format
 msgid "Mot de passe réinitialisé sur %(site_name)s"
-msgstr "Mot de passe réinitialisé sur %(site_name)s"
+msgstr "Password reset on %(site_name)s"
 
-#: djangoldp_account/templates/registration/registration_closed.html:5
+#: templates/registration/registration_closed.html:5
 msgid "Les inscriptions sont actuellement fermées."
-msgstr "Les inscriptions sont actuellement fermées."
+msgstr "Registration is currently closed."
 
-#: djangoldp_account/templates/registration/registration_complete.html:5
+#: templates/registration/registration_complete.html:5
 msgid "Tu es désormais enregistré. Un e-mail d'activation t'a été envoyé."
-msgstr "Tu es désormais enregistré. Un e-mail d'activation t'a été envoyé."
+msgstr "You are now registered. An activation email has been sent to you."
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/locale/fr/LC_MESSAGES/django.mo` & `djangoldp_account-3.0.1/djangoldp_account/locale/fr/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -137,27 +137,17 @@
 
 msgid "Enregistrement du compte pour %(sitename)s"
 msgstr "Enregistrement du compte pour %(sitename)s"
 
 msgid "Enregistrer un compte"
 msgstr "Enregistrer un compte"
 
-msgid ""
-"Entre un nom d'utilisateur valide. Il ne peut contenir que des lettres, des "
-"chiffres, et les caractères ./+/-/_"
-msgstr ""
-"Entre un nom d'utilisateur valide. Il ne peut contenir que des lettres, des "
-"chiffres, et les caractères ./+/-/_"
-
 msgid "Envoyer"
 msgstr "Envoyer"
 
-msgid "Envoyer un e-mail d'activation"
-msgstr "Envoyer un e-mail d'activation"
-
 msgid "Envoyez-moi les instructions !"
 msgstr "Envoyez-moi les instructions !"
 
 msgid ""
 "Indique ton adresse e-mail ci-dessous et nous t'enverrons des instructions "
 "par e-mail pour en définir un nouveau."
 msgstr ""
@@ -206,21 +196,14 @@
 
 msgid "Perdu"
 msgstr "Perdu"
 
 msgid "Refuser"
 msgstr "Refuser"
 
-msgid ""
-"Requiert 150 caractères ou moins. Seulement des lettres, chiffres et les "
-"caractères ./+/-/_"
-msgstr ""
-"Requiert 150 caractères ou moins. Seulement des lettres, chiffres et les "
-"caractères ./+/-/_"
-
 msgid "Réinitialiser le mot de passe sur %(site_name)s"
 msgstr "Réinitialiser le mot de passe sur %(site_name)s"
 
 msgid "S'inscrire !"
 msgstr "S'inscrire !"
 
 msgid "Se connecter"
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/locale/en/LC_MESSAGES/django.mo` & `djangoldp_account-3.0.1/djangoldp_account/locale/en/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -104,20 +104,26 @@
 
 msgid "Ce lien est valide pendant %(expiration_days)s jours."
 msgstr "This link is valid for %(expiration_days)s days."
 
 msgid "Ce nom d'utilisateur est déjà pris."
 msgstr "This username is already taken."
 
+msgid "Compte créé sur "
+msgstr "Account created on "
+
 msgid "Connecte-toi pour voir cette page."
 msgstr "Login to see this page."
 
 msgid "Contacte ton administrateur pour plus d'informations."
 msgstr "Contact your administrator for more information."
 
+msgid "Création de compte sur "
+msgstr "Account creation on "
+
 msgid "Crée ton mot de passe en "
 msgstr "Create your password by "
 
 msgid "Demande d'accès aux informations"
 msgstr "Information access request"
 
 msgid "Demande d'autorisation"
@@ -137,27 +143,17 @@
 
 msgid "Enregistrement du compte pour %(sitename)s"
 msgstr "Account registration for %(sitename)s"
 
 msgid "Enregistrer un compte"
 msgstr "Register an account"
 
-msgid ""
-"Entre un nom d'utilisateur valide. Il ne peut contenir que des lettres, des "
-"chiffres, et les caractères ./+/-/_"
-msgstr ""
-"Enter a valid username. It can only contain letters, numbers, and the "
-"characters ./+/-/_."
-
 msgid "Envoyer"
 msgstr "Send"
 
-msgid "Envoyer un e-mail d'activation"
-msgstr "Send an activation e-mail"
-
 msgid "Envoyez-moi les instructions !"
 msgstr "Send me the instructions!"
 
 msgid ""
 "Indique ton adresse e-mail ci-dessous et nous t'enverrons des instructions "
 "par e-mail pour en définir un nouveau."
 msgstr ""
@@ -206,21 +202,14 @@
 
 msgid "Perdu"
 msgstr "Lost"
 
 msgid "Refuser"
 msgstr "Decline"
 
-msgid ""
-"Requiert 150 caractères ou moins. Seulement des lettres, chiffres et les "
-"caractères ./+/-/_"
-msgstr ""
-"Requires 150 characters or less. Only letters, numbers and the characters ./"
-"+/-/_."
-
 msgid "Réinitialiser le mot de passe sur %(site_name)s"
 msgstr "Reset password on %(site_name)s"
 
 msgid "S'inscrire !"
 msgstr "Register!"
 
 msgid "Se connecter"
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/forms.py` & `djangoldp_account-3.0.1/djangoldp_account/forms.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/static/base.css` & `djangoldp_account-3.0.1/djangoldp_account/static/base.css`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/static/registration/login.css` & `djangoldp_account-3.0.1/djangoldp_account/static/registration/login.css`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/auth/backends.py` & `djangoldp_account-3.0.1/djangoldp_account/auth/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,16 +153,16 @@
             print('error validating claims ' + str(e))
             raise AuthenticationFailed(detail='unable to validate claims', code=status.HTTP_401_UNAUTHORIZED)
 
         # validation complete, we can complete the authentication
         return self._get_or_create_then_authenticate({}, jwt['webid'])
 
     def authenticate(self, request, username=None, password=None, **kwargs):
-        if 'HTTP_AUTHORIZATION' in request.META:
-            jwt = request.META['HTTP_AUTHORIZATION']
+        if 'authorization' in request.headers:
+            jwt = request.headers['authorization']
             if jwt.lower().startswith("dpop"):
                 jwt = jwt[5:]
                 return self.validate_dpop_token(request, jwt)
 
             elif jwt.lower().startswith("bearer"):
                 jwt = jwt[7:]
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/auth/middleware.py` & `djangoldp_account-3.0.1/djangoldp_account/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/auth/solid.py` & `djangoldp_account-3.0.1/djangoldp_account/auth/solid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import uuid
-from urllib.parse import urlparse
+from urllib.parse import urlparse, unquote
 
 from django.http import Http404
 from django.core.exceptions import ObjectDoesNotExist
 from django.conf import settings
 from django.contrib.auth import login, get_user_model
 from django.utils.decorators import classonlymethod
 
@@ -21,15 +21,15 @@
         if not isinstance(claims['htu'], str):
             raise LDPLoginError('htu_claim_invalid')
 
         htu = urlparse(claims['htu'])
         request_url = urlparse(request.build_absolute_uri())
 
         # reject if the htu does not match the protocol, origin and path of the request
-        if htu.scheme != request_url.scheme or htu.hostname != request_url.hostname or htu.path != request_url.path:
+        if htu.scheme != request_url.scheme or htu.hostname != request_url.hostname or unquote(htu.path) != unquote(request_url.path):
             raise LDPLoginError('htu_claim_not_matching_request')
 
     @classonlymethod
     def check_htm_claim(cls, request, claims):
         if 'htm' not in claims or claims['htm'] != request.method:
             raise LDPLoginError('htm_claim_invalid')
```

### Comparing `djangoldp_account-2.3.9/djangoldp_account/djangoldp_settings.py` & `djangoldp_account-3.0.1/djangoldp_account/djangoldp_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0002_auto_20190917_1141.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0002_auto_20190917_1141.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0012_auto_20200501_1433.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0012_auto_20200501_1433.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0007_auto_20200130_1242.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0007_auto_20200130_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0001_initial.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0010_auto_20200501_1207.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0010_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0014_auto_20200610_1323.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0014_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0016_auto_20200903_1049.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0016_auto_20200903_1049.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0011_auto_20200501_1420.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0011_auto_20200501_1420.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0009_auto_20200429_1346.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0009_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0003_auto_20191024_0854.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0003_auto_20191024_0854.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0006_auto_20200121_1321.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0006_auto_20200121_1321.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0013_auto_20200505_1733.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0013_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0017_auto_20200910_1606.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0017_auto_20200910_1606.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0008_auto_20200130_1251.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0008_auto_20200130_1251.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0015_auto_20200617_1817.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0015_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.9/djangoldp_account/migrations/0004_auto_20191203_0921.py` & `djangoldp_account-3.0.1/djangoldp_account/migrations/0004_auto_20191203_0921.py`

 * *Files identical despite different names*

