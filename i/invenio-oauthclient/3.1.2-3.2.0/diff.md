# Comparing `tmp/invenio-oauthclient-3.1.2.tar.gz` & `tmp/invenio-oauthclient-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-oauthclient-3.1.2.tar", last modified: Fri Jun 23 09:35:34 2023, max compression
+gzip compressed data, was "dist/invenio-oauthclient-3.2.0.tar", last modified: Mon Jul 24 09:09:46 2023, max compression
```

## Comparing `invenio-oauthclient-3.1.2.tar` & `invenio-oauthclient-3.2.0.tar`

### file list

```diff
@@ -1,172 +1,336 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      920 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7947 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7461 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10206 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/examplesapp.rst
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7007 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/examples/
--rwxr-xr-x   0 runner    (1001) docker     (122)      169 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/app-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)       85 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/app-teardown.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/github_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/github_app_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/globus_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/globus_app_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4561 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/orcid_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/orcid_app_rest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      848 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/_compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py
--rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17979 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/cern.py
--rw-r--r--   0 runner    (1001) docker     (122)    15246 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/cern_openid.py
--rw-r--r--   0 runner    (1001) docker     (122)    11557 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/github.py
--rw-r--r--   0 runner    (1001) docker     (122)    11134 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/globus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/
--rw-r--r--   0 runner    (1001) docker     (122)     3919 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5168 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3570 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)    10486 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/openaire_aai.py
--rw-r--r--   0 runner    (1001) docker     (122)    10133 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/orcid.py
--rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     7962 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10451 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8780 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     6403 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     9562 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7862 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/postmessage.html
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/rejected.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/signup.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/rejected.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      987 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     3312 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (122)    11195 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/views/
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9194 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/views/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/views/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7947 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      939 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      346 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/run-i18n-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1303 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    17922 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/cern_openid_response_content.json
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/keycloak_realm_info.json
--rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/keycloak_token_response.json
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/keycloak_userinfo_response.json
--rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/oauth_response_content.json
--rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/orcid_bio.json
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_base_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_cern_openid.py
--rw-r--r--   0 runner    (1001) docker     (122)    11031 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_cern_openid_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)    13036 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_github.py
--rw-r--r--   0 runner    (1001) docker     (122)    14224 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_github_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)    10374 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_globus.py
--rw-r--r--   0 runner    (1001) docker     (122)    14371 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (122)     9540 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_orcid.py
--rw-r--r--   0 runner    (1001) docker     (122)     9849 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_orcid_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_examples_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     9560 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_handlers_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5072 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_handlers_ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    10261 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    17496 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    15887 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_views_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1119 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8095 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7461 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10206 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/examplesapp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7007 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      169 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/examples/app-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)       85 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/examples/app-teardown.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/examples/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/examples/github_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/examples/github_app_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/examples/globus_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/examples/globus_app_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4561 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/examples/orcid_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/examples/orcid_app_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      848 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12471 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17979 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/cern.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15246 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/cern_openid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11557 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11134 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/globus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/keycloak/
+-rw-r--r--   0 runner    (1001) docker     (122)     3919 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/keycloak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5168 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/keycloak/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3570 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/keycloak/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/keycloak/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10486 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/openaire_aai.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10133 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/orcid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7962 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8092 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/authorized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8845 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6689 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5106 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7862 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5424 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/postmessage.html
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/rejected.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/signup.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/rejected.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3764 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2473 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4988 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3917 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3963 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4626 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3936 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3777 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3777 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3966 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4614 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3814 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3779 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3905 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3774 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1998 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4602 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3774 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3973 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4641 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4481 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3901 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4015 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4046 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3955 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4600 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4524 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3777 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4683 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4113 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4002 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4378 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6291 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9766 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/views/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/invenio_oauthclient/views/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8095 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10189 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      939 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      346 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1303 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    17922 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:09:46.000000 invenio-oauthclient-3.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/data/cern_openid_response_content.json
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/data/keycloak_realm_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/data/keycloak_token_response.json
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/data/keycloak_userinfo_response.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/data/oauth_response_content.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/data/orcid_bio.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2701 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_base_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_contrib_cern_openid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11021 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_contrib_cern_openid_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13084 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_contrib_github.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14214 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_contrib_github_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_contrib_globus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14362 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_contrib_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9531 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_contrib_orcid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9840 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_contrib_orcid_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_examples_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10726 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_handlers_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7309 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_handlers_ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10293 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17486 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15877 2023-07-24 09:09:36.000000 invenio-oauthclient-3.2.0/tests/test_views_rest.py
```

### Comparing `invenio-oauthclient-3.1.2/.editorconfig` & `invenio-oauthclient-3.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/.tx/config` & `invenio-oauthclient-3.2.0/.tx/config`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
+# Copyright (C)      2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 # 1) Create message catalog:
 #    $ python setup.py extract_messages
 #    $ python setup.py init_catalog -l <lang>
@@ -18,14 +19,14 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio-oauthclient-messages]
+[o:inveniosoftware:p:invenio:r:invenio-oauthclient-messages]
 file_filter = invenio_oauthclient/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_oauthclient/translations/messages.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-oauthclient-3.1.2/AUTHORS.rst` & `invenio-oauthclient-3.2.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/CHANGES.rst` & `invenio-oauthclient-3.2.0/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 3.2.0 (released 2023-07-24)
+
+- authorize: refactor authorize/signup handlers
+- update translations
+
 Version 3.1.2 (released 2023-06-23)
 
 - client: preserve "next" URL param on login redirection
 
 Version 3.1.1 (released 2023-06-21)
 
 - client: fix user confirmation
```

### Comparing `invenio-oauthclient-3.1.2/CONTRIBUTING.rst` & `invenio-oauthclient-3.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/LICENSE` & `invenio-oauthclient-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/MANIFEST.in` & `invenio-oauthclient-3.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/PKG-INFO` & `invenio-oauthclient-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-oauthclient
-Version: 3.1.2
+Version: 3.2.0
 Summary: "Invenio module that provides OAuth web authorization support."
 Home-page: https://github.com/inveniosoftware/invenio-oauthclient
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -56,14 +56,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.2.0 (released 2023-07-24)
+        
+        - authorize: refactor authorize/signup handlers
+        - update translations
+        
         Version 3.1.2 (released 2023-06-23)
         
         - client: preserve "next" URL param on login redirection
         
         Version 3.1.1 (released 2023-06-21)
         
         - client: fix user confirmation
```

### Comparing `invenio-oauthclient-3.1.2/README.rst` & `invenio-oauthclient-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/docs/Makefile` & `invenio-oauthclient-3.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/docs/api.rst` & `invenio-oauthclient-3.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/docs/conf.py` & `invenio-oauthclient-3.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/docs/examplesapp.rst` & `invenio-oauthclient-3.2.0/docs/examplesapp.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/docs/index.rst` & `invenio-oauthclient-3.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/docs/make.bat` & `invenio-oauthclient-3.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/docs/overview.rst` & `invenio-oauthclient-3.2.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/docs/usage.rst` & `invenio-oauthclient-3.2.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/examples/app.py` & `invenio-oauthclient-3.2.0/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/examples/github_app.py` & `invenio-oauthclient-3.2.0/examples/github_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/examples/github_app_rest.py` & `invenio-oauthclient-3.2.0/examples/github_app_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/examples/globus_app.py` & `invenio-oauthclient-3.2.0/examples/globus_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/examples/globus_app_rest.py` & `invenio-oauthclient-3.2.0/examples/globus_app_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/examples/orcid_app.py` & `invenio-oauthclient-3.2.0/examples/orcid_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/examples/orcid_app_rest.py` & `invenio-oauthclient-3.2.0/examples/orcid_app_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/_compat.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/_compat.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/admin.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Views for OAuth."""
 
 from flask_admin.contrib.sqla import ModelView
-from invenio_accounts.admin import UserIdentityView, user_identity_adminview
+from invenio_accounts.admin import user_identity_adminview
 
 from .models import RemoteAccount, RemoteToken
 
 
 def _(x):
     """Identity."""
     return x
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/config.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,16 +318,14 @@
         )
     )
 
 """
 
 from invenio_oauthclient.utils import _create_registrationform
 
-from .views.client import auto_redirect_login
-
 OAUTHCLIENT_REMOTE_APPS = {}
 """Configuration of remote applications."""
 
 OAUTHCLIENT_SESSION_KEY_PREFIX = "oauth_token"
 """Session key prefix used when storing the access token for a remote app."""
 
 OAUTHCLIENT_STATE_EXPIRES = 300
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/cern.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/cern.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,16 +150,16 @@
 from invenio_db import db
 from invenio_i18n import gettext as _
 
 from invenio_oauthclient.errors import OAuthCERNRejectedAccountError
 from invenio_oauthclient.handlers.rest import response_handler
 from invenio_oauthclient.handlers.utils import require_more_than_one_external_account
 from invenio_oauthclient.models import RemoteAccount
+from invenio_oauthclient.oauth import oauth_link_external_id, oauth_unlink_external_id
 from invenio_oauthclient.proxies import current_oauthclient
-from invenio_oauthclient.utils import oauth_link_external_id, oauth_unlink_external_id
 
 warn(
     "The cern contrib is deprecated. Please use the generic keycloak instead.",
     DeprecationWarning,
 )
```

#### html2text {}

```diff
@@ -51,17 +51,17 @@
 flask_login import current_user from flask_principal import
 ( AnonymousIdentity, RoleNeed, UserNeed, identity_changed, identity_loaded, )
 from invenio_db import db from invenio_i18n import gettext as _ from
 invenio_oauthclient.errors import OAuthCERNRejectedAccountError from
 invenio_oauthclient.handlers.rest import response_handler from
 invenio_oauthclient.handlers.utils import
 require_more_than_one_external_account from invenio_oauthclient.models import
-RemoteAccount from invenio_oauthclient.proxies import current_oauthclient from
-invenio_oauthclient.utils import oauth_link_external_id,
-oauth_unlink_external_id warn( "The cern contrib is deprecated. Please use the
+RemoteAccount from invenio_oauthclient.oauth import oauth_link_external_id,
+oauth_unlink_external_id from invenio_oauthclient.proxies import
+current_oauthclient warn( "The cern contrib is deprecated. Please use the
 generic keycloak instead.", DeprecationWarning, )
 OAUTHCLIENT_CERN_HIDDEN_GROUPS = ( "All Exchange People", "CERN Users", "cern-
 computing-postmasters", "cern-nice2000-postmasters", "CMF FrontEnd Users",
 "CMF_NSC_259_NSU", "Domain Users", "GP Apply Favorites Redirection", "GP Apply
 NoAdmin", "info-terminalservices", "info-terminalservices-members", "IT Web
 IT", "NICE Deny Enforce Password-protected Screensaver", "NICE Enforce
 Password-protected Screensaver", "NICE LightWeight Authentication WS Users",
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/cern_openid.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/cern_openid.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,16 @@
 from invenio_i18n import gettext as _
 from jwt import decode
 
 from invenio_oauthclient.errors import OAuthCERNRejectedAccountError
 from invenio_oauthclient.handlers.rest import response_handler
 from invenio_oauthclient.handlers.utils import require_more_than_one_external_account
 from invenio_oauthclient.models import RemoteAccount
+from invenio_oauthclient.oauth import oauth_link_external_id, oauth_unlink_external_id
 from invenio_oauthclient.proxies import current_oauthclient
-from invenio_oauthclient.utils import oauth_link_external_id, oauth_unlink_external_id
 
 OAUTHCLIENT_CERN_OPENID_REFRESH_TIMEDELTA = timedelta(minutes=-5)
 """Default interval for refreshing CERN extra data (e.g. groups).
 
 False value disabled the refresh.
 """
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/github.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 )
 from invenio_oauthclient.handlers.rest import (
     oauth_resp_remote_error_handler,
     response_handler,
 )
 from invenio_oauthclient.handlers.utils import require_more_than_one_external_account
 from invenio_oauthclient.models import RemoteAccount
-from invenio_oauthclient.utils import oauth_link_external_id, oauth_unlink_external_id
+from invenio_oauthclient.oauth import oauth_link_external_id, oauth_unlink_external_id
 
 
 class GitHubOAuthSettingsHelper(OAuthSettingsHelper):
     """Default configuration for GitHub OAuth provider."""
 
     def __init__(
         self,
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/globus.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/globus.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 from invenio_oauthclient import current_oauthclient
 from invenio_oauthclient.contrib.settings import OAuthSettingsHelper
 from invenio_oauthclient.errors import OAuthResponseError
 from invenio_oauthclient.handlers.rest import response_handler
 from invenio_oauthclient.handlers.utils import require_more_than_one_external_account
 from invenio_oauthclient.models import RemoteAccount
-from invenio_oauthclient.utils import oauth_link_external_id, oauth_unlink_external_id
+from invenio_oauthclient.oauth import oauth_link_external_id, oauth_unlink_external_id
 
 
 class GlobusOAuthSettingsHelper(OAuthSettingsHelper):
     """Default configuration for Globus OAuth provider."""
 
     def __init__(
         self,
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/__init__.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/handlers.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/keycloak/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from flask_login import current_user
 from invenio_db import db
 
 from invenio_oauthclient import current_oauthclient
 from invenio_oauthclient.handlers.rest import response_handler
 from invenio_oauthclient.handlers.utils import require_more_than_one_external_account
 from invenio_oauthclient.models import RemoteAccount
-from invenio_oauthclient.utils import oauth_link_external_id, oauth_unlink_external_id
+from invenio_oauthclient.oauth import oauth_link_external_id, oauth_unlink_external_id
 
 from .helpers import get_user_info
 
 
 def info_serializer_handler(remote, resp, token_user_info, user_info=None, **kwargs):
     """Serialize the account info response object.
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/helpers.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/keycloak/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/settings.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/keycloak/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/openaire_aai.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/openaire_aai.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 from invenio_oauthclient import current_oauthclient
 from invenio_oauthclient.contrib.keycloak import KeycloakSettingsHelper
 from invenio_oauthclient.contrib.settings import OAuthSettingsHelper
 from invenio_oauthclient.handlers.rest import response_handler
 from invenio_oauthclient.handlers.utils import require_more_than_one_external_account
 from invenio_oauthclient.models import RemoteAccount
-from invenio_oauthclient.utils import oauth_link_external_id, oauth_unlink_external_id
+from invenio_oauthclient.oauth import oauth_link_external_id, oauth_unlink_external_id
 
 
 class OpenAIREAuthSettingsHelper(OAuthSettingsHelper):
     """Default configuration for OpenAIRE OAuth provider."""
 
     def __init__(
         self,
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/orcid.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/orcid.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 from invenio_db import db
 
 from invenio_oauthclient import current_oauthclient
 from invenio_oauthclient.contrib.settings import OAuthSettingsHelper
 from invenio_oauthclient.handlers.rest import response_handler
 from invenio_oauthclient.handlers.utils import require_more_than_one_external_account
 from invenio_oauthclient.models import RemoteAccount
-from invenio_oauthclient.utils import oauth_link_external_id, oauth_unlink_external_id
+from invenio_oauthclient.oauth import oauth_link_external_id, oauth_unlink_external_id
 
 
 class ORCIDOAuthSettingsHelper(OAuthSettingsHelper):
     """Default configuration for ORCID OAuth provider."""
 
     def __init__(
         self,
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/settings.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/contrib/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/errors.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/ext.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/__init__.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,37 +8,36 @@
 
 """Handlers for customizing oauthclient endpoints."""
 
 from .rest import authorized_default_handler as authorized_default_handler_rest
 from .rest import authorized_signup_handler as authorized_signup_handler_rest
 from .rest import disconnect_handler as disconnect_handler_rest
 from .rest import signup_handler as signup_handler_rest
-from .ui import (
-    authorized_default_handler,
-    authorized_signup_handler,
-    disconnect_handler,
-    oauth2_handle_error,
-)
-from .ui import oauth_resp_remote_error_handler as oauth_error_handler
-from .ui import signup_handler
-from .utils import (
-    authorized_handler,
+from .token import (
     get_session_next_url,
-    make_handler,
     make_token_getter,
     oauth1_token_setter,
     oauth2_token_setter,
     oauth_logout_handler,
     response_token_setter,
     set_session_next_url,
     token_delete,
     token_getter,
     token_session_key,
     token_setter,
 )
+from .ui import (
+    authorized_default_handler,
+    authorized_signup_handler,
+    disconnect_handler,
+    oauth2_handle_error,
+)
+from .ui import oauth_resp_remote_error_handler as oauth_error_handler
+from .ui import signup_handler
+from .utils import authorized_handler, make_handler
 
 __all__ = (
     "authorized_default_handler_rest",
     "authorized_default_handler",
     "authorized_handler",
     "authorized_signup_handler_rest",
     "authorized_signup_handler",
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/base.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/authorized.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,302 +1,209 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015-2019 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
-"""Handlers for customizing oauthclient endpoints."""
+"""Authorize handlers."""
 
-from flask import current_app, session
+from flask import current_app, g, session
 from flask_login import current_user
-from invenio_accounts.models import Role
-from invenio_accounts.proxies import current_datastore
 from invenio_db import db
 
 from ..errors import (
     OAuthClientAlreadyAuthorized,
-    OAuthClientMustRedirectLogin,
     OAuthClientMustRedirectSignup,
     OAuthClientTokenNotFound,
     OAuthClientTokenNotSet,
     OAuthClientUnAuthorized,
     OAuthClientUserNotRegistered,
 )
-from ..models import RemoteAccount
+from ..oauth import oauth_authenticate, oauth_get_user, oauth_register
 from ..proxies import current_oauthclient
 from ..signals import (
     account_info_received,
     account_setup_committed,
     account_setup_received,
 )
-from ..utils import (
-    create_csrf_disabled_registrationform,
-    fill_form,
-    oauth_authenticate,
-    oauth_get_user,
-    oauth_register,
-)
-from .utils import (
+from ..utils import create_csrf_disabled_registrationform, fill_form
+from .token import (
     get_session_next_url,
-    require_more_than_one_external_account,
     response_token_setter,
     token_getter,
     token_session_key,
     token_setter,
 )
+from .utils import create_or_update_roles
 
 
-def _role_needs_update(role_obj, new_role_dict):
-    """Checks if role needs to be updated."""
-    if role_obj.name != new_role_dict.get(
-        "name"
-    ) or role_obj.description != new_role_dict.get("description"):
-        return True
-    return False
-
-
-def create_or_update_groups(account_groups):
-    """Creates the roles based on the groups provided."""
-    roles_id = []
-    for group in account_groups:
-        existing_role = current_datastore.find_role_by_id(group["id"])
-        if existing_role and existing_role.is_managed:
-            current_app.logger.exception(
-                f'Error while syncing roles: A managed role with id: ${group["id"]} already exists'
-            )
-            continue
-        existing_role_by_name = current_datastore.find_role(group["name"])
-        if existing_role_by_name and existing_role_by_name.is_managed:
-            current_app.logger.exception(
-                f'Error while syncing roles: A managed role with name: ${group["name"]} already exists'
-            )
-            continue
-        if not existing_role:
-            role = current_datastore.create_role(
-                id=group["id"],
-                name=group.get("name"),
-                description=group.get("description"),
-                is_managed=False,
-            )
-            roles_id.append(role.id)
-        elif existing_role and _role_needs_update(existing_role, group):
-            role_to_update = Role(
-                id=group["id"],
-                name=group.get("name"),
-                description=group.get("description"),
-                is_managed=False,
-            )
-            role = current_datastore.update_role(role_to_update)
-            roles_id.append(role.id)
-        else:
-            roles_id.append(existing_role.id)
-
-    current_datastore.commit()
-
-    return roles_id
-
-
-#
-# Handlers
-#
-def base_authorized_signup_handler(resp, remote, *args, **kwargs):
-    """Handle sign-in/up functionality.
+def authorized_handler(resp, remote, *args, **kwargs):
+    """Handle user login after OAuth authorize step.
 
-    :param remote: The remote application.
     :param resp: The response of the `authorized` endpoint.
-    :returns: Redirect response.
+    :param remote: The remote application.
+    :returns: The URL to go next after login
     """
+    # Validate the response and set token in the user session. This must happen
+    # first to make sure that the response payload is valid.
+    # Returned token is None when anonymous user
+    token = response_token_setter(remote, resp)
+
+    # Set the remote in the user session to know how the user logged in.
+    # Useful on log out, so that we can logout on remote too, when needed.
+    session["OAUTHCLIENT_SESSION_REMOTE_NAME"] = remote.name
     # Remove any previously stored auto register session key
     session.pop(token_session_key(remote.name) + "_autoregister", None)
-    # We set the remote in the session to be aware of which one is being used and, on log out redirect to
-    # the correct URL set in the OAUTHCLIENT_REMOTE_APPS for each remote
-    session["OAUTHCLIENT_SESSION_REMOTE_NAME"] = remote.name
-    # Store token in session
-    # ----------------------
-    # Set token in session - token object only returned if
-    # current_user.is_authenticated().
-    token = response_token_setter(remote, resp)
+
     handlers = current_oauthclient.signup_handlers[remote.name]
-    # Needed for tests
-    if not current_user.is_authenticated:
-        # Sign-in/up user
-        # ---------------
-        account_info = handlers["info"](resp)
-        assert "external_id" in account_info
-        account_info_received.send(
-            remote, token=token, response=resp, account_info=account_info
-        )
 
+    # call user info endpoint
+    account_info = handlers["info"](resp)
+    assert "external_id" in account_info
+    account_info_received.send(remote, response=resp, account_info=account_info)
+
+    # call groups endpoint, when defined
+    group_handler = handlers.get("groups")
+    if group_handler:
+        account_groups = group_handler(resp)
+        if account_groups:
+            roles_ids = create_or_update_roles(account_groups)
+            # Set the unmanaged roles in the user session, used in other modules.
+            # Unmanaged user roles are not stored in the DB for privacy reasons:
+            # sys admins should not know the external groups of a user.
+            session["unmanaged_roles_ids"] = roles_ids
+
+    # In the normal OAuth flow, the user is not yet authenticated. However, it the user
+    # is already logged in, and goes to 'Linked accounts', clicks 'Connect' on another
+    # remote app, `authorized` will be called with the new remote.
+    is_normal_oauth_flow = not current_user.is_authenticated
+    if is_normal_oauth_flow:
+        # get the user from the DB using the current remote
         user = oauth_get_user(
             remote.consumer_key,
             account_info=account_info,
             access_token=token_getter(remote)[0],
         )
-
         if user is None:
-            # Auto sign-up if user not found
+            # User not found, this is the first login. Register the user.
+            # The registration raises an exception when the account info is not enough
+            # to register the user.
             form = create_csrf_disabled_registrationform(remote)
             form = fill_form(form, account_info["user"])
-            remote_app = current_app.config["OAUTHCLIENT_REMOTE_APPS"][remote.name]
-            precedence_mask = remote_app.get("precedence_mask")
-            signup_options = remote_app.get("signup_options")
-            user = oauth_register(
-                form,
-                account_info["user"],
-                precedence_mask=precedence_mask,
-                signup_options=signup_options,
-            )
-
-            # if registration fails ...
-            if user is None:
-                # requires extra information
+
+            try:
+                user = _register_user(resp, remote, account_info, form)
+            except OAuthClientUserNotRegistered:
+                # save in the session info to display the extra signup form to the user
                 session[token_session_key(remote.name) + "_autoregister"] = True
                 session[token_session_key(remote.name) + "_account_info"] = account_info
                 session[token_session_key(remote.name) + "_response"] = resp
                 db.session.commit()
+                # this will trigger a redirect to /signup (therefor
+                # signup_handler/extra_signup_handler funcs) and will require the user
+                # to fill in the registration form with the missing information
                 raise OAuthClientMustRedirectSignup()
 
-        group_handler = handlers.get("groups")
-        if group_handler:
-            account_groups = group_handler(resp)
-            if account_groups:
-                roles_id = create_or_update_groups(account_groups)
-                # We set the unmanaged groups in the session because they are not linked to the user in the DB
-                session["_unmanaged_groups"] = roles_id
-
-        # Authenticate user after the unmanaged groups where set in the session
         if not oauth_authenticate(
             remote.consumer_key, user, require_existing_link=False
         ):
             raise OAuthClientUnAuthorized()
-
-        # Link account
-        # ------------
-        # Need to store token in database instead of only the session when
-        # called first time.
+        # Store token in the database instead of only the session
         token = response_token_setter(remote, resp)
 
-    # Setup account
-    # -------------
-    if not token.remote_account.extra_data:
+    return _complete_authorize(resp, remote, handlers, token)
+
+
+def _register_user(resp, remote, account_info, form):
+    """Try to register the user with info got from the remote app.
+
+    :param resp: The response of the `authorized` endpoint.
+    :param remote: The remote application.
+    """
+    remote_app = current_app.config["OAUTHCLIENT_REMOTE_APPS"][remote.name]
+    precedence_mask = remote_app.get("precedence_mask")
+    signup_options = remote_app.get("signup_options")
+
+    user = oauth_register(
+        form,
+        account_info["user"],
+        precedence_mask=precedence_mask,
+        signup_options=signup_options,
+    )
+
+    if user is None:
+        # Registration failed: the account info is not enough to register the user.
+        # Save info in the session, necessary for the user registration flow with form.
+        raise OAuthClientUserNotRegistered()
+
+    return user
+
+
+def _complete_authorize(resp, remote, handlers, token):
+    """Complete authorized flow.
+
+    This happens after:
+     - A normal authorized flow.
+     - The extra signup registration, where the user needs to fill in the missing
+       information during the first login.
+    """
+    is_first_login_with_this_remote = not token.remote_account.extra_data
+    if is_first_login_with_this_remote:
+        # call the `setup` handler to get complete the first login with this remote
         account_setup = handlers["setup"](token, resp)
         account_setup_received.send(
             remote, token=token, response=resp, account_setup=account_setup
         )
         db.session.commit()
         account_setup_committed.send(remote, token=token)
     else:
         db.session.commit()
 
-    # Redirect to next
+    # Return the URL where to go next
     next_url = get_session_next_url(remote.name)
     if next_url:
         return next_url
 
 
-@require_more_than_one_external_account
-def base_disconnect_handler(remote, *args, **kwargs):
-    """Handle unlinking of remote account.
-
-    This default handler will just delete the remote account link. You may
-    wish to extend this module to perform clean-up in the remote service
-    before removing the link (e.g. removing install webhooks).
-
-    :param remote: The remote application.
-    :returns: Redirect response.
-    """
-    if not current_user.is_authenticated:
-        raise OAuthClientUnAuthorized()
-
-    with db.session.begin_nested():
-        account = RemoteAccount.get(
-            user_id=current_user.get_id(), client_id=remote.consumer_key
-        )
-        if account:
-            account.delete()
-
-    db.session.commit()
-
-
-def base_signup_handler(remote, form, *args, **kwargs):
+def extra_signup_handler(remote, form, *args, **kwargs):
     """Handle extra signup information.
 
+    Validate the extra missing information that the user inserted in the signup step,
+    after authorized. If the info inserted are enough
+
     :param remote: The remote application.
     :returns: Redirect response or the template rendered.
     """
-    # User already authenticated so move on
     if current_user.is_authenticated:
         raise OAuthClientAlreadyAuthorized()
 
     # Retrieve token from session
     oauth_token = token_getter(remote)
     if not oauth_token:
         raise OAuthClientTokenNotFound()
 
     session_prefix = token_session_key(remote.name)
 
-    # Test to see if this is coming from on authorized request
-    if not session.get(session_prefix + "_autoregister", False):
-        raise OAuthClientMustRedirectLogin()
-
+    handlers = current_oauthclient.signup_handlers[remote.name]
     if form.validate_on_submit():
-        account_info = session.get(session_prefix + "_account_info")
-        response = session.get(session_prefix + "_response")
-
-        remote_app = current_app.config["OAUTHCLIENT_REMOTE_APPS"][remote.name]
-        precedence_mask = remote_app.get("precedence_mask")
-        signup_options = remote_app.get("signup_options")
-
-        # Register user
-        user = oauth_register(
-            form,
-            account_info["user"],
-            precedence_mask=precedence_mask,
-            signup_options=signup_options,
-        )
-
-        if user is None:
-            raise OAuthClientUserNotRegistered()
-
-        # Remove session key
+        # remove the autoregister flag that marks the authorized flow
         session.pop(session_prefix + "_autoregister", None)
+        account_info = session.pop(session_prefix + "_account_info")
+        response = session.pop(session_prefix + "_response")
+
+        user = _register_user(response, remote, account_info, form)
 
         # Link account and set session data
         token = token_setter(remote, oauth_token[0], secret=oauth_token[1], user=user)
-        handlers = current_oauthclient.signup_handlers[remote.name]
-
         if token is None:
             raise OAuthClientTokenNotSet()
 
-        if not token.remote_account.extra_data:
-            account_setup = handlers["setup"](token, response)
-            account_setup_received.send(
-                remote, token=token, response=response, account_setup=account_setup
-            )
-            # Registration has been finished
-            db.session.commit()
-            account_setup_committed.send(remote, token=token)
-        else:
-            # Registration has been finished
-            db.session.commit()
-
-        # Authenticate user
+        # Authenticate user, without requiring the existence of the RemoteAccount,
+        # which is created later in the setup handler.
         if not oauth_authenticate(
             remote.consumer_key, user, require_existing_link=False
         ):
             raise OAuthClientUnAuthorized()
 
-        # Remove account info from session
-        session.pop(session_prefix + "_account_info", None)
-        session.pop(session_prefix + "_response", None)
-
-        # Redirect to next
-        next_url = get_session_next_url(remote.name)
-        if next_url:
-            return next_url
-
-    # Pre-fill form
-    account_info = session.get(session_prefix + "_account_info")
-    if not form.is_submitted():
-        fill_form(form, account_info["user"])
+        return _complete_authorize(response, remote, handlers, token)
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/rest.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/rest.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 # Copyright (C) 2015-2022 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Handlers for customizing oauthclient endpoints."""
 
-import json
 from functools import partial, wraps
+from urllib.parse import parse_qs, urlencode, urlsplit, urlunsplit
 
 from flask import (
     abort,
     current_app,
     jsonify,
     make_response,
     redirect,
     render_template,
     request,
     url_for,
 )
+from flask_login import current_user
 from invenio_db import db
-from six.moves.urllib.parse import parse_qs, urlencode, urlsplit, urlunsplit
 
 from ..errors import (
     AlreadyLinkedError,
     OAuthClientAlreadyAuthorized,
     OAuthClientError,
     OAuthClientMustRedirectLogin,
     OAuthClientMustRedirectSignup,
@@ -35,20 +35,18 @@
     OAuthClientUnAuthorized,
     OAuthClientUserNotRegistered,
     OAuthError,
     OAuthRejectedRequestError,
 )
 from ..proxies import current_oauthclient
 from ..utils import create_csrf_disabled_registrationform, fill_form
-from .base import (
-    base_authorized_signup_handler,
-    base_disconnect_handler,
-    base_signup_handler,
-)
-from .utils import response_token_setter
+from .authorized import authorized_handler, extra_signup_handler
+from .base import base_disconnect_handler
+from .decorators import can_extra_signup
+from .token import response_token_setter
 
 
 def response_handler_postmessage(remote, url, payload=None):
     """Postmessage response handler."""
     return render_template("invenio_oauthclient/postmessage.html", payload=payload)
 
 
@@ -204,15 +202,15 @@
     """Handle sign-in/up functionality.
 
     :param remote: The remote application.
     :param resp: The response.
     :returns: Redirect response.
     """
     remote_app_config = current_app.config["OAUTHCLIENT_REST_REMOTE_APPS"][remote.name]
-    next_url = base_authorized_signup_handler(resp, remote, *args, **kwargs)
+    next_url = authorized_handler(resp, remote, *args, **kwargs)
     response_payload = dict(message="Successfully authorized.", code=200)
     if next_url:
         response_payload["next_url"] = next_url
 
     return response_handler(
         remote, remote_app_config["authorized_redirect_url"], payload=response_payload
     )
@@ -242,37 +240,40 @@
             message="Successfully disconnected.",
             code=200,
         ),
     )
 
 
 @oauth_remote_error_handler
+@can_extra_signup
 def signup_handler(remote, *args, **kwargs):
     """Handle extra signup information.
 
     :param remote: The remote application.
     :returns: Redirect response or the template rendered.
     """
     remote_app_config = current_app.config["OAUTHCLIENT_REST_REMOTE_APPS"][remote.name]
-    try:
-        form = create_csrf_disabled_registrationform(remote)
+    form = create_csrf_disabled_registrationform(remote)
+    if not form.is_submitted():
         data = request.form.to_dict()
         form = fill_form(form, data)
-        next_url = base_signup_handler(remote, form, *args, **kwargs)
-        if form.is_submitted():
-            response_payload = dict(message="Successfully signed up.", code=200)
-            if next_url:
-                response_payload["next_url"] = next_url
-            return jsonify(response_payload)
         return response_handler(
             remote,
             remote_app_config["signup_redirect_url"],
             payload=dict(
                 form=form.to_dict(),
                 remote=remote.name,
                 app_title=remote_app_config.get("title", ""),
                 app_description=remote_app_config.get("description", ""),
                 app_icon=remote_app_config.get("icon", None),
             ),
         )
-    except OAuthClientUnAuthorized:
-        abort(401)
+    else:
+        try:
+            next_url = extra_signup_handler(remote, form, *args, **kwargs)
+        except OAuthClientUnAuthorized:
+            abort(401)
+
+        response_payload = dict(message="Successfully signed up.", code=200)
+        if next_url:
+            response_payload["next_url"] = next_url
+        return jsonify(response_payload)
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/ui.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/handlers/ui.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,24 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Handlers for customizing oauthclient endpoints."""
 
 from functools import partial, wraps
 
-from flask import current_app, flash, redirect, render_template, request, url_for
+from flask import (
+    current_app,
+    flash,
+    redirect,
+    render_template,
+    request,
+    session,
+    url_for,
+)
+from flask_login import current_user
 from invenio_db import db
 from invenio_i18n import gettext as _
 
 from ..errors import (
     AlreadyLinkedError,
     OAuthClientAlreadyAuthorized,
     OAuthClientError,
@@ -23,21 +32,19 @@
     OAuthClientTokenNotFound,
     OAuthClientTokenNotSet,
     OAuthClientUnAuthorized,
     OAuthClientUserNotRegistered,
     OAuthError,
     OAuthRejectedRequestError,
 )
-from ..utils import create_registrationform
-from .base import (
-    base_authorized_signup_handler,
-    base_disconnect_handler,
-    base_signup_handler,
-)
-from .utils import response_token_setter
+from ..utils import create_registrationform, fill_form
+from .authorized import authorized_handler, extra_signup_handler
+from .base import base_disconnect_handler
+from .decorators import can_extra_signup
+from .token import response_token_setter, token_session_key
 
 
 def _oauth_error_handler(remote, f, *args, **kwargs):
     """Function to handle exceptions."""
     try:
         return f(remote, *args, **kwargs)
     except OAuthClientError as e:
@@ -130,15 +137,15 @@
 def authorized_signup_handler(resp, remote, *args, **kwargs):
     """Handle sign-in/up functionality.
 
     :param remote: The remote application.
     :param resp: The response.
     :returns: Redirect response.
     """
-    next_url = base_authorized_signup_handler(resp, remote, *args, **kwargs)
+    next_url = authorized_handler(resp, remote, *args, **kwargs)
     # Redirect to next
     if next_url:
         return redirect(next_url)
     return redirect(url_for("invenio_oauthclient_settings.index"))
 
 
 @oauth_remote_error_handler
@@ -153,45 +160,58 @@
     :returns: Redirect response.
     """
     base_disconnect_handler(remote, *args, **kwargs)
     return redirect(url_for("invenio_oauthclient_settings.index"))
 
 
 @oauth_remote_error_handler
+@can_extra_signup
 def signup_handler(remote, *args, **kwargs):
     """Handle extra signup information.
 
+    The info in the request.form is used to fill in the user registration form.
+    When the form does not validate (e.g. missing user e-mail), it is displayed
+    to the user, who needs to fill in the missing info and submit it.
+    This method is also called when the user has filled in the form and click on
+    btn submit.
+
     :param remote: The remote application.
     :returns: Redirect response or the template rendered.
     """
-    try:
-        form = create_registrationform(request.form, oauth_remote_app=remote)
-        next_url = base_signup_handler(remote, form, *args, **kwargs)
-        if form.is_submitted() and not form.errors:
-            if next_url:
-                return redirect(next_url)
-            else:
-                return redirect("/")
+    form = create_registrationform(request.form, oauth_remote_app=remote)
+    if not form.is_submitted():
+        session_prefix = token_session_key(remote.name)
+        account_info = session.get(session_prefix + "_account_info")
+        # Pre-fill form
+        fill_form(form, account_info["user"])
         return render_template(
             current_app.config["OAUTHCLIENT_SIGNUP_TEMPLATE"],
             form=form,
             remote=remote,
             app_title=current_app.config["OAUTHCLIENT_REMOTE_APPS"][remote.name].get(
                 "title", ""
             ),
             app_description=current_app.config["OAUTHCLIENT_REMOTE_APPS"][
                 remote.name
             ].get("description", ""),
             app_icon=current_app.config["OAUTHCLIENT_REMOTE_APPS"][remote.name].get(
                 "icon", None
             ),
         )
-    except OAuthClientUnAuthorized:
-        # Redirect the user after registration (which doesn't include the
-        # activation), waiting for user to confirm his email.
-        return redirect(url_for("security.login"))
+    elif not form.errors:
+        try:
+            next_url = extra_signup_handler(remote, form, *args, **kwargs)
+        except OAuthClientUnAuthorized:
+            # Redirect the user after registration (which doesn't include the
+            # activation), waiting for user to confirm his email.
+            return redirect(url_for("security.login"))
+
+        if next_url:
+            return redirect(next_url)
+        else:
+            return redirect("/")
 
 
 def oauth2_handle_error(remote, resp, error_code, error_uri, error_description):
     """Handle errors during exchange of one-time code for an access tokens."""
     flash(_("Authorization with remote service failed."))
     return redirect("/")
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/utils.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/views/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,291 +2,307 @@
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
-"""Handlers for customizing oauthclient endpoints."""
+"""Client blueprint used to handle OAuth callbacks."""
 
-from functools import partial, wraps
-
-import six
-from flask import abort, current_app, session
-from flask_login import current_user
+from flask import Blueprint, abort, current_app, redirect, request, session, url_for
+from flask_oauthlib.client import OAuthException
+from invenio_accounts.views import login as base_login
 from invenio_db import db
-from werkzeug.utils import import_string
+from itsdangerous import BadData
 
-from ..errors import OAuthClientError, OAuthRejectedRequestError, OAuthResponseError
-from ..models import RemoteAccount, RemoteToken
+from .._compat import _create_identifier
+from ..errors import OAuthRemoteNotFound
+from ..handlers import set_session_next_url
+from ..handlers.rest import response_handler
 from ..proxies import current_oauthclient
+from ..utils import get_safe_redirect_target, serializer
 
+blueprint = Blueprint(
+    "invenio_oauthclient",
+    __name__,
+    url_prefix="/oauth",
+    static_folder="../static",
+    template_folder="../templates",
+)
+
+
+rest_blueprint = Blueprint(
+    "invenio_oauthclient",
+    __name__,
+    url_prefix="/oauth",
+    static_folder="../static",
+    template_folder="../templates",
+)
+
+
+@blueprint.record_once
+def post_ext_init(state):
+    """Setup blueprint."""
+    app = state.app
 
-#
-# Token handling
-#
-def get_session_next_url(remote_app):
-    """Return redirect url stored in session.
-
-    :param remote_app: The remote application.
-    :returns: The redirect URL.
-    """
-    return session.get("%s_%s" % (token_session_key(remote_app), "next_url"))
-
-
-def set_session_next_url(remote_app, url):
-    """Store redirect url in session for security reasons.
-
-    :param remote_app: The remote application.
-    :param url: the redirect URL.
-    """
-    session["%s_%s" % (token_session_key(remote_app), "next_url")] = url
-
-
-def token_session_key(remote_app):
-    """Generate a session key used to store the token for a remote app.
+    app.config.setdefault(
+        "OAUTHCLIENT_SITENAME", app.config.get("THEME_SITENAME", "Invenio")
+    )
+    app.config.setdefault(
+        "OAUTHCLIENT_BASE_TEMPLATE",
+        app.config.get("BASE_TEMPLATE", "invenio_oauthclient/base.html"),
+    )
+    app.config.setdefault(
+        "OAUTHCLIENT_COVER_TEMPLATE",
+        app.config.get("COVER_TEMPLATE", "invenio_oauthclient/base_cover.html"),
+    )
+    app.config.setdefault(
+        "OAUTHCLIENT_SETTINGS_TEMPLATE",
+        app.config.get("SETTINGS_TEMPLATE", "invenio_oauthclient/settings/base.html"),
+    )
 
-    :param remote_app: The remote application.
-    :returns: The session key.
-    """
-    return "%s_%s" % (current_app.config["OAUTHCLIENT_SESSION_KEY_PREFIX"], remote_app)
 
+@blueprint.route("/login")
+def auto_redirect_login(*args, **kwargs):
+    """Handles automatic redirect to external auth service.
+
+    The login endpoint will redirect automatically to the external
+    auth service is the following conditions are met:
+
+    * local login is disabled
+    * redirect to external login is enabled
+    * only one external auth service is configured
+
+    This function should be set as value of the invenio-accounts
+    config var ``ACCOUNTS_LOGIN_VIEW_FUNCTION``. It should be defined in
+    the Invenio application configuration to ensure that is correctly loaded.
+    """
+    local_login_enabled = current_app.config.get("ACCOUNTS_LOCAL_LOGIN_ENABLED", False)
+    auto_redirect_enabled = current_app.config.get(
+        "OAUTHCLIENT_AUTO_REDIRECT_TO_EXTERNAL_LOGIN", False
+    )
+    would_redirect = auto_redirect_enabled and not local_login_enabled
+    remote_apps = list(current_oauthclient.oauth.remote_apps)
 
-def response_token_setter(remote, resp):
-    """Extract token from response and set it for the user.
+    if would_redirect and len(remote_apps) == 1:
+        redirect_args = {
+            # if local login is disabled and we only have one OAuth2 remote app
+            # configured, we forward directly to that
+            "remote_app": remote_apps[0],
+        }
+        next_url = request.args.get("next")
+        if next_url:
+            redirect_args["next"] = next_url
+        url = url_for("invenio_oauthclient.login", **redirect_args)
+        return redirect(url)
 
-    :param remote: The remote application.
-    :param resp: The response.
-    :raises invenio_oauthclient.errors.OAuthClientError: If authorization with
-        remote service failed.
-    :raises invenio_oauthclient.errors.OAuthResponseError: In case of bad
-        authorized request.
-    :returns: The token.
-    """
-    if resp is None:
-        raise OAuthRejectedRequestError("User rejected request.", remote, resp)
     else:
-        if "access_token" in resp:
-            return oauth2_token_setter(remote, resp)
-        elif "oauth_token" in resp and "oauth_token_secret" in resp:
-            return oauth1_token_setter(remote, resp)
-        elif "error" in resp:
-            # Only OAuth2 specifies how to send error messages
-            raise OAuthClientError(
-                "Authorization with remote service failed.",
-                remote,
-                resp,
-            )
-    raise OAuthResponseError("Bad OAuth authorized request", remote, resp)
-
-
-def oauth1_token_setter(remote, resp, token_type="", extra_data=None):
-    """Set an OAuth1 token.
+        return base_login(*args, **kwargs)
 
-    :param remote: The remote application.
-    :param resp: The response.
-    :param token_type: The token type. (Default: ``''``)
-    :param extra_data: Extra information. (Default: ``None``)
-    :returns: A :class:`invenio_oauthclient.models.RemoteToken` instance.
-    """
-    return token_setter(
-        remote,
-        resp["oauth_token"],
-        secret=resp["oauth_token_secret"],
-        extra_data=extra_data,
-        token_type=token_type,
-    )
 
+def _login(remote_app, authorized_view_name):
+    """Send user to remote application for authentication."""
+    oauth = current_oauthclient.oauth
+    if remote_app not in oauth.remote_apps:
+        raise OAuthRemoteNotFound()
 
-def oauth2_token_setter(remote, resp, token_type="", extra_data=None):
-    """Set an OAuth2 token.
+    # Get redirect target in safe manner.
+    next_param = get_safe_redirect_target(arg="next")
 
-    The refresh_token can be used to obtain a new access_token after
-    the old one is expired. It is saved in the database for long term use.
-    A refresh_token will be present only if `access_type=offline` is included
-    in the authorization code request.
-
-    :param remote: The remote application.
-    :param resp: The response.
-    :param token_type: The token type. (Default: ``''``)
-    :param extra_data: Extra information. (Default: ``None``)
-    :returns: A :class:`invenio_oauthclient.models.RemoteToken` instance.
-    """
-    return token_setter(
-        remote,
-        resp["access_token"],
-        secret="",
-        token_type=token_type,
-        extra_data=extra_data,
+    # Redirect URI - must be registered in the remote service.
+    callback_url = url_for(
+        authorized_view_name, remote_app=remote_app, _external=True, _scheme="https"
     )
 
+    # Create a JSON Web Token that expires after OAUTHCLIENT_STATE_EXPIRES
+    # seconds.
+    state_token = serializer.dumps(
+        {
+            "app": remote_app,
+            "next": next_param,
+            "sid": _create_identifier(),
+        }
+    )
+    return oauth.remote_apps[remote_app].authorize(
+        callback=callback_url,
+        state=state_token,
+    )
 
-def token_setter(remote, token, secret="", token_type="", extra_data=None, user=None):
-    """Set token for user.
-
-    :param remote: The remote application.
-    :param token: The token to set.
-    :param token_type: The token type. (Default: ``''``)
-    :param extra_data: Extra information. (Default: ``None``)
-    :param user: The user owner of the remote token. If it's not defined,
-        the current user is used automatically. (Default: ``None``)
-    :returns: A :class:`invenio_oauthclient.models.RemoteToken` instance or
-        ``None``.
-    """
-    session[token_session_key(remote.name)] = (token, secret)
-    user = user or current_user
-
-    # Save token if user is not anonymous (user exists but can be not active at
-    # this moment)
-    if not user.is_anonymous:
-        uid = user.id
-        cid = remote.consumer_key
-
-        # Check for already existing token
-        t = RemoteToken.get(uid, cid, token_type=token_type)
 
-        if t:
-            t.update_token(token, secret)
-        else:
-            t = RemoteToken.create(
-                uid, cid, token, secret, token_type=token_type, extra_data=extra_data
+@blueprint.route("/login/<remote_app>/")
+def login(remote_app):
+    """Send user to remote application for authentication."""
+    try:
+        return _login(remote_app, ".authorized")
+    except OAuthRemoteNotFound:
+        return abort(404)
+
+
+@rest_blueprint.route("/login/<remote_app>/")
+def rest_login(remote_app):
+    """Send user to remote application for authentication."""
+    try:
+        return _login(remote_app, ".rest_authorized")
+    except OAuthRemoteNotFound:
+        abort(404)
+
+
+def _authorized(remote_app=None):
+    """Authorized handler callback."""
+    if remote_app not in current_oauthclient.handlers:
+        return abort(404)
+
+    state_token = request.args.get("state")
+
+    # Verify state parameter
+    assert state_token
+    # Checks authenticity and integrity of state and decodes the value.
+    state = serializer.loads(state_token)
+    # Verify that state is for this session, app and that next parameter
+    # have not been modified.
+    assert state["sid"] == _create_identifier()
+    assert state["app"] == remote_app
+    # Store next URL
+    set_session_next_url(remote_app, state["next"])
+
+    handler = current_oauthclient.handlers[remote_app]()
+    return handler
+
+
+@blueprint.route("/authorized/<remote_app>/")
+def authorized(remote_app=None):
+    """Authorized handler callback."""
+    try:
+        return _authorized(remote_app)
+    except OAuthRemoteNotFound:
+        return abort(404)
+    except (AssertionError, BadData):
+        if current_app.config.get("OAUTHCLIENT_STATE_ENABLED", True) or (
+            not (current_app.debug or current_app.testing)
+        ):
+            abort(403)
+    except OAuthException as e:
+        if e.type == "invalid_response":
+            current_app.logger.warning(
+                "{message} ({data})".format(message=e.message, data=e.data)
             )
-        return t
-    return None
-
+            abort(500)
+        else:
+            raise
 
-def token_getter(remote, token=""):
-    """Retrieve OAuth access token.
 
-    Used by flask-oauthlib to get the access token when making requests.
+@rest_blueprint.route("/authorized/<remote_app>/")
+def rest_authorized(remote_app=None):
+    """Authorized handler callback."""
+    try:
+        return _authorized(remote_app)
+    except OAuthRemoteNotFound:
+        abort(404)
+    except (AssertionError, BadData) as e:
+        current_app.logger.error(str(e))
+        if current_app.config.get("OAUTHCLIENT_STATE_ENABLED", True) or (
+            not (current_app.debug or current_app.testing)
+        ):
+            return response_handler(
+                None,
+                current_app.config["OAUTHCLIENT_REST_DEFAULT_ERROR_REDIRECT_URL"],
+                payload=dict(message="Invalid state.", code=403),
+            )
+    except OAuthException as e:
+        current_app.logger.error(str(e))
+        if e.type == "invalid_response":
+            return response_handler(
+                None,
+                current_app.config["OAUTHCLIENT_REST_DEFAULT_ERROR_REDIRECT_URL"],
+                payload=dict(message="Invalid response.", code=500),
+            )
+        else:
+            raise
 
-    :param remote: The remote application.
-    :param token: Type of token to get. Data passed from ``oauth.request()`` to
-        identify which token to retrieve. (Default: ``''``)
-    :returns: The token.
-    """
-    session_key = token_session_key(remote.name)
 
-    if session_key not in session and current_user.is_authenticated:
-        # Fetch key from token store if user is authenticated, and the key
-        # isn't already cached in the session.
-        remote_token = RemoteToken.get(
-            current_user.get_id(),
-            remote.consumer_key,
-            token_type=token,
-        )
+def _signup(remote_app):
+    """Extra signup step."""
+    if remote_app not in current_oauthclient.signup_handlers:
+        raise OAuthRemoteNotFound()
+    return current_oauthclient.signup_handlers[remote_app]["view"]()
 
-        if remote_token is None:
-            return None
 
-        # Store token and secret in session
-        session[session_key] = remote_token.token()
+@blueprint.route("/signup/<remote_app>/", methods=["GET", "POST"])
+def signup(remote_app):
+    """Extra signup step.
 
-    return session.get(session_key, None)
+    GET: automatically called when OAuthClientMustRedirectSignup exception triggered
+    during authorized handler execution: the info retrieved from the remote
+    app are not sufficient to register the user.
+    POST: called when the registration form is submitted by the user.
+    """
+    try:
+        res = _signup(remote_app)
+        return abort(404) if res is None else res
+    except OAuthRemoteNotFound:
+        return abort(404)
 
 
-def token_delete(remote, token=""):
-    """Remove OAuth access tokens from session.
+@rest_blueprint.route("/signup/<remote_app>/", methods=["GET", "POST"])
+def rest_signup(remote_app):
+    """Extra signup step.
 
-    :param remote: The remote application.
-    :param token: Type of token to get. Data passed from ``oauth.request()``
-        to identify which token to retrieve. (Default: ``''``)
-    :returns: The token.
+    GET: automatically called when OAuthClientMustRedirectSignup exception triggered
+    during authorized handler execution: the info retrieved from the remote
+    app are not sufficient to register the user.
+    POST: called when the registration form is submitted by the user.
     """
-    session_key = token_session_key(remote.name)
-    return session.pop(session_key, None)
+    try:
+        res = _signup(remote_app)
+        return abort(404) if res is None else res
+    except OAuthRemoteNotFound:
+        abort(404)
 
 
-def oauth_logout_handler(sender_app, user=None):
-    """Remove all access tokens from session on logout."""
-    oauth = current_oauthclient.oauth
-    for remote in oauth.remote_apps.values():
-        token_delete(remote)
+def _disconnect(remote_app):
+    """Extra signup step."""
+    if remote_app not in current_oauthclient.signup_handlers:
+        raise OAuthRemoteNotFound()
+    ret = current_oauthclient.disconnect_handlers[remote_app]()
     db.session.commit()
+    return ret
 
 
-#
-# Helpers
-#
-def make_handler(f, remote, with_response=True):
-    """Make a handler for authorized and disconnect callbacks.
+@blueprint.route("/disconnect/<remote_app>/")
+def disconnect(remote_app):
+    """Disconnect user from remote application.
 
-    :param f: Callable or an import path to a callable
+    Removes application as well as associated information.
     """
-    if isinstance(f, six.string_types):
-        f = import_string(f)
-
-    @wraps(f)
-    def inner(*args, **kwargs):
-        if with_response:
-            return f(args[0], remote, *args[1:], **kwargs)
-        else:
-            return f(remote, *args, **kwargs)
-
-    return inner
+    try:
+        return _disconnect(remote_app)
+    except OAuthRemoteNotFound:
+        abort(404)
 
 
-def make_token_getter(remote):
-    """Make a token getter for a remote application."""
-    return partial(token_getter, remote)
+@rest_blueprint.route("/disconnect/<remote_app>/")
+def rest_disconnect(remote_app):
+    """Disconnect user from remote application.
 
-
-def authorized_handler(f, authorized_response):
-    """Handles an OAuth callback.
-
-    As authorized_handler is deprecated in favor of authorized_response,
-    it's has to be wrapped with handler which will be executed
-    at the proper time.
+    Removes application as well as associated information.
     """
+    try:
+        return _disconnect(remote_app)
+    except OAuthRemoteNotFound:
+        abort(404)
 
-    @wraps(f)
-    def decorated(*args, **kwargs):
-        data = authorized_response()
-        return f(*((data,) + args), **kwargs)
-
-    return decorated
 
+@blueprint.route("/logout")
+def post_logout():
+    """Client logout view.
 
-def require_more_than_one_external_account(f):
-    """Require that the user has more than one external account for login.
-
-    If the user only has one linked external account and no means for logging
-    in via local credentials, the decorated function won't be executed.
-    This decorator is useful for disconnect handlers, to prevent users from
-    disconnecting their last potential means of authentication.
+    This URL should be called by setting `SECURITY_POST_LOGOUT_VIEW = /oauth/logout`
     """
-
-    @wraps(f)
-    def decorated(*args, **kwargs):
-        if current_user.is_anonymous:
-            return f(*args, **kwargs)
-
-        local_login_enabled = current_app.config.get(
-            "ACCOUNTS_LOCAL_LOGIN_ENABLED", True
+    remote_name = session.pop("OAUTHCLIENT_SESSION_REMOTE_NAME", None)
+    if remote_name:
+        logout_url = current_app.config["OAUTHCLIENT_REMOTE_APPS"][remote_name].get(
+            "logout_url"
         )
-        password_set = current_user.password is not None
-        local_login_possible = local_login_enabled and password_set
-
-        remote_apps = current_app.config["OAUTHCLIENT_REMOTE_APPS"]
-        accounts = RemoteAccount.query.filter_by(user_id=current_user.get_id()).all()
-
-        # find out all of the linked external accounts for the user
-        # that are currently configured and not hidden
-        consumer_keys = set()
-        remote_apps = current_app.config["OAUTHCLIENT_REMOTE_APPS"]
-        for name, remote_app in remote_apps.items():
-            if not remote_app.get("hide", False):
-                consumer_keys.add(name)  # backcompat with v1.5.4
-                remote_app_config = current_app.config[remote_app["params"]["app_key"]]
-                consumer_keys.add(remote_app_config["consumer_key"])
-
-        linked_accounts = [acc for acc in accounts if acc.client_id in consumer_keys]
-
-        # execute the function only if local login is possible, or
-        # there's more than one linked external account
-        if local_login_possible or len(linked_accounts) > 1:
-            return f(*args, **kwargs)
-
-        else:
-            abort(400)
+        if logout_url:
+            return redirect(logout_url, code=302)
 
-    return decorated
+    return redirect("/")
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/models.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/models.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/signals.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/signals.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/_macros.html` & `invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/login_user.html` & `invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html` & `invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/signup.html` & `invenio-oauthclient-3.2.0/invenio_oauthclient/templates/invenio_oauthclient/signup.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html` & `invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html` & `invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html` & `invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html` & `invenio-oauthclient-3.2.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #}
 
 {%- extends config.OAUTHCLIENT_SETTINGS_TEMPLATE %}
 
 {% from "invenio_oauthclient/_macros.html" import form_errors, render_field %}
 
 {% block page_body %}
-<div class="ui centered grid">
+<div class="ui centered grid rel-mb-2">
   <div class="row">
   {%- block signup_panel %}
   <div>
     {%- block signup_header %}
       <div class="ui center aligned header">
         <div class="content">
           <div class="ui hidden divider"></div>
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po`

 * *Files 21% similar despite different names*

```diff
@@ -1,98 +1,132 @@
 # Translations template for invenio-oauthclient.
-# Copyright (C) 2016 CERN
+# Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-oauthclient
 # project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# 
+# Translators:
+# Alizee Pace <alizee.pace@gmail.com>, 2016
+# Tibor Simko <tibor.simko@cern.ch>, 2021
 # 
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: invenio-oauthclient 1.0.0a10\n"
+"Project-Id-Version: invenio-oauthclient 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2016-09-09 15:01+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2016\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"POT-Creation-Date: 2022-05-27 09:58+0200\n"
+"PO-Revision-Date: 2016-08-18 15:19+0000\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.3.4\n"
-"Language: cs\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"Generated-By: Babel 2.10.1\n"
+"Language: it\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
-#: invenio_oauthclient/admin.py:64
+#: invenio_oauthclient/admin.py:52
 msgid "ID"
 msgstr "ID"
 
-#: invenio_oauthclient/admin.py:65
+#: invenio_oauthclient/admin.py:53
 msgid "User ID"
-msgstr "ID uživatele"
+msgstr "ID Utente"
 
-#: invenio_oauthclient/admin.py:66
+#: invenio_oauthclient/admin.py:54
 msgid "Client ID"
-msgstr "ID klienta"
+msgstr "ID Cliente"
 
-#: invenio_oauthclient/admin.py:95
+#: invenio_oauthclient/admin.py:83
 msgid "ID Remote Account"
-msgstr "ID vzdáleného účtu"
+msgstr "ID Conto Esterno"
 
-#: invenio_oauthclient/admin.py:102 invenio_oauthclient/admin.py:108
+#: invenio_oauthclient/admin.py:90 invenio_oauthclient/admin.py:98
 msgid "User Management"
-msgstr "Správa uživatelů"
+msgstr "Gestione Utenti"
 
-#: invenio_oauthclient/handlers.py:189
-msgid "You rejected the authentication request."
-msgstr ""
+#: invenio_oauthclient/admin.py:91
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:12
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:12
+#: invenio_oauthclient/views/settings.py:47
+msgid "Linked accounts"
+msgstr "Conti legati"
 
-#: invenio_oauthclient/handlers.py:193
-msgid "External service is already linked to another account."
+#: invenio_oauthclient/admin.py:99
+msgid "Linked account tokens"
 msgstr ""
 
-#: invenio_oauthclient/handlers.py:447
-msgid "Authorization with remote service failed."
+#: invenio_oauthclient/contrib/cern.py:429
+#: invenio_oauthclient/contrib/cern_openid.py:305
+msgid "CERN account not allowed."
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:40
-msgid "Close"
-msgstr "Zavřít"
+#: invenio_oauthclient/handlers/ui.py:42
+msgid "External service is already linked to another account."
+msgstr "Il servizio esterno è già collegato a un altro conto."
+
+#: invenio_oauthclient/handlers/ui.py:47
+msgid "You rejected the authentication request."
+msgstr "Hai rifiutato la richiesta d'autenticazione."
+
+#: invenio_oauthclient/handlers/ui.py:173
+msgid "Authorization with remote service failed."
+msgstr "L'autorizzazione con il servizio esterno ha fallito."
 
-#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:58
+#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:25
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html:60
 #, python-format
 msgid "Sign in with %(title)s"
-msgstr ""
+msgstr "Registra con %(title)s"
+
+#: invenio_oauthclient/templates/invenio_oauthclient/login_user.html:21
+msgid "OR"
+msgstr "O"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:34
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:24
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:29
 #, python-format
 msgid "Sign-up with %(title)s!"
-msgstr ""
+msgstr "Accedi con %(title)s"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:35
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:25
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:32
 msgid ""
 "Fill in your details to complete your registration. You only have to do this"
 " once."
 msgstr ""
+"Completa i tuoi dettagli per finire la registrazione. Devi farlo una volta "
+"sola."
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:25
-#: invenio_oauthclient/views/settings.py:54
-msgid "Linked accounts"
-msgstr "Propojené účty"
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:33
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:45
+msgid "Complete registration"
+msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:31
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:20
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:20
 #, python-format
 msgid ""
 "Tired of entering password for %(sitename)s every time you sign in? Set up "
 "single sign-on with one or more of the services below:"
 msgstr ""
+"Non vuoi inserire la password ogni volta che accedi a %(sitename)s? "
+"Configura un accesso unico con uno o più servizi di seguito:"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:41
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:31
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:32
 msgid "Disconnect"
-msgstr "Odpojit"
+msgstr "Scollega"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:43
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:33
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:34
 msgid "Connect"
-msgstr "Připojit"
+msgstr "Collega"
+
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html:26
+msgid "Or"
+msgstr ""
 
-#: invenio_oauthclient/views/settings.py:48
+#: invenio_oauthclient/views/settings.py:38
 #, python-format
 msgid "%(icon)s Linked accounts"
-msgstr "%(icon)s Propojené účty"
+msgstr "%(icon)s Conti legati"
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/ne/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauthclient 1.0.0a10*

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 db01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 d801 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d6f 6175 7468 636c   invenio-oauthcl
-00000050: 6965 6e74 2031 2e30 2e30 6131 300a 5265  ient 1.0.0a10.Re
-00000060: 706f 7274 2d4d 7367 6964 2d42 7567 732d  port-Msgid-Bugs-
-00000070: 546f 3a20 696e 666f 4069 6e76 656e 696f  To: info@invenio
-00000080: 736f 6674 7761 7265 2e6f 7267 0a50 4f54  software.org.POT
-00000090: 2d43 7265 6174 696f 6e2d 4461 7465 3a20  -Creation-Date: 
-000000a0: 3230 3136 2d30 392d 3039 2031 353a 3031  2016-09-09 15:01
-000000b0: 2b30 3230 300a 504f 2d52 6576 6973 696f  +0200.PO-Revisio
-000000c0: 6e2d 4461 7465 3a20 5945 4152 2d4d 4f2d  n-Date: YEAR-MO-
-000000d0: 4441 2048 4f3a 4d49 2b5a 4f4e 450a 4c61  DA HO:MI+ZONE.La
-000000e0: 7374 2d54 7261 6e73 6c61 746f 723a 2046  st-Translator: F
-000000f0: 554c 4c20 4e41 4d45 203c 454d 4149 4c40  ULL NAME <EMAIL@
-00000100: 4144 4452 4553 533e 0a4c 616e 6775 6167  ADDRESS>.Languag
-00000110: 653a 2064 610a 4c61 6e67 7561 6765 2d54  e: da.Language-T
-00000120: 6561 6d3a 2044 616e 6973 6820 2868 7474  eam: Danish (htt
-00000130: 7073 3a2f 2f77 7777 2e74 7261 6e73 6966  ps://www.transif
-00000140: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
-00000150: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
-00000160: 3337 2f64 612f 290a 506c 7572 616c 2d46  37/da/).Plural-F
-00000170: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
-00000180: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
-00000190: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
-000001a0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
-000001b0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
-000001c0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
-000001d0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
-000001e0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
-000001f0: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
-00000200: 2032 2e31 322e 310a 00                    2.12.1..
+00000050: 6965 6e74 2032 2e30 2e30 0a52 6570 6f72  ient 2.0.0.Repor
+00000060: 742d 4d73 6769 642d 4275 6773 2d54 6f3a  t-Msgid-Bugs-To:
+00000070: 2069 6e66 6f40 696e 7665 6e69 6f73 6f66   info@inveniosof
+00000080: 7477 6172 652e 6f72 670a 504f 542d 4372  tware.org.POT-Cr
+00000090: 6561 7469 6f6e 2d44 6174 653a 2032 3032  eation-Date: 202
+000000a0: 322d 3035 2d32 3720 3039 3a35 382b 3032  2-05-27 09:58+02
+000000b0: 3030 0a50 4f2d 5265 7669 7369 6f6e 2d44  00.PO-Revision-D
+000000c0: 6174 653a 2032 3031 362d 3038 2d31 3820  ate: 2016-08-18 
+000000d0: 3135 3a31 392b 3030 3030 0a4c 6173 742d  15:19+0000.Last-
+000000e0: 5472 616e 736c 6174 6f72 3a20 4655 4c4c  Translator: FULL
+000000f0: 204e 414d 4520 3c45 4d41 494c 4041 4444   NAME <EMAIL@ADD
+00000100: 5245 5353 3e0a 4c61 6e67 7561 6765 3a20  RESS>.Language: 
+00000110: 6e65 0a4c 616e 6775 6167 652d 5465 616d  ne.Language-Team
+00000120: 3a20 4e65 7061 6c69 2028 6874 7470 733a  : Nepali (https:
+00000130: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
+00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
+00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
+00000160: 6e65 2f29 0a50 6c75 7261 6c2d 466f 726d  ne/).Plural-Form
+00000170: 733a 206e 706c 7572 616c 733d 323b 2070  s: nplurals=2; p
+00000180: 6c75 7261 6c3d 286e 2021 3d20 3129 3b0a  lural=(n != 1);.
+00000190: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
+000001a0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
+000001b0: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
+000001c0: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
+000001d0: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
+000001e0: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
+000001f0: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
+00000200: 3132 2e31 0a00                           12.1..
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,123 @@
 # Translations template for invenio-oauthclient.
-# Copyright (C) 2016 CERN
+# Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-oauthclient
 # project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: invenio-oauthclient 1.0.0a10\n"
+"Project-Id-Version: invenio-oauthclient 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2016-09-09 15:01+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"POT-Creation-Date: 2022-05-27 09:58+0200\n"
+"PO-Revision-Date: 2016-08-18 15:19+0000\n"
+"Language-Team: Estonian (Estonia) (https://app.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.3.4\n"
-"Language: da\n"
+"Generated-By: Babel 2.10.1\n"
+"Language: et_EE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: invenio_oauthclient/admin.py:64
+#: invenio_oauthclient/admin.py:52
 msgid "ID"
 msgstr ""
 
-#: invenio_oauthclient/admin.py:65
+#: invenio_oauthclient/admin.py:53
 msgid "User ID"
 msgstr ""
 
-#: invenio_oauthclient/admin.py:66
+#: invenio_oauthclient/admin.py:54
 msgid "Client ID"
 msgstr ""
 
-#: invenio_oauthclient/admin.py:95
+#: invenio_oauthclient/admin.py:83
 msgid "ID Remote Account"
 msgstr ""
 
-#: invenio_oauthclient/admin.py:102 invenio_oauthclient/admin.py:108
+#: invenio_oauthclient/admin.py:90 invenio_oauthclient/admin.py:98
 msgid "User Management"
 msgstr ""
 
-#: invenio_oauthclient/handlers.py:189
-msgid "You rejected the authentication request."
+#: invenio_oauthclient/admin.py:91
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:12
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:12
+#: invenio_oauthclient/views/settings.py:47
+msgid "Linked accounts"
+msgstr ""
+
+#: invenio_oauthclient/admin.py:99
+msgid "Linked account tokens"
 msgstr ""
 
-#: invenio_oauthclient/handlers.py:193
+#: invenio_oauthclient/contrib/cern.py:429
+#: invenio_oauthclient/contrib/cern_openid.py:305
+msgid "CERN account not allowed."
+msgstr ""
+
+#: invenio_oauthclient/handlers/ui.py:42
 msgid "External service is already linked to another account."
 msgstr ""
 
-#: invenio_oauthclient/handlers.py:447
-msgid "Authorization with remote service failed."
+#: invenio_oauthclient/handlers/ui.py:47
+msgid "You rejected the authentication request."
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:40
-msgid "Close"
+#: invenio_oauthclient/handlers/ui.py:173
+msgid "Authorization with remote service failed."
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:58
+#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:25
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html:60
 #, python-format
 msgid "Sign in with %(title)s"
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:34
+#: invenio_oauthclient/templates/invenio_oauthclient/login_user.html:21
+msgid "OR"
+msgstr ""
+
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:24
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:29
 #, python-format
 msgid "Sign-up with %(title)s!"
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:35
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:25
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:32
 msgid ""
 "Fill in your details to complete your registration. You only have to do this"
 " once."
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:25
-#: invenio_oauthclient/views/settings.py:54
-msgid "Linked accounts"
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:33
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:45
+msgid "Complete registration"
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:31
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:20
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:20
 #, python-format
 msgid ""
 "Tired of entering password for %(sitename)s every time you sign in? Set up "
 "single sign-on with one or more of the services below:"
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:41
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:31
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:32
 msgid "Disconnect"
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:43
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:33
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:34
 msgid "Connect"
 msgstr ""
 
-#: invenio_oauthclient/views/settings.py:48
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html:26
+msgid "Or"
+msgstr ""
+
+#: invenio_oauthclient/views/settings.py:38
 #, python-format
 msgid "%(icon)s Linked accounts"
 msgstr ""
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauthclient 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 09:58+0200\n"
 "PO-Revision-Date: 2016-08-18 15:19+0000\n"
 "Last-Translator: chriz_uniba <christina.zeller@uni-bamberg.de>, 2022\n"
 "Language: de\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/"
 "de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauthclient 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 09:58+0200\n"
 "PO-Revision-Date: 2016-08-18 15:19+0000\n"
 "Last-Translator: chriz_uniba <christina.zeller@uni-bamberg.de>, 2022\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/de/)\n"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauthclient 1.0.0a10*

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 dc01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 dd01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d6f 6175 7468 636c   invenio-oauthcl
-00000050: 6965 6e74 2031 2e30 2e30 6131 300a 5265  ient 1.0.0a10.Re
-00000060: 706f 7274 2d4d 7367 6964 2d42 7567 732d  port-Msgid-Bugs-
-00000070: 546f 3a20 696e 666f 4069 6e76 656e 696f  To: info@invenio
-00000080: 736f 6674 7761 7265 2e6f 7267 0a50 4f54  software.org.POT
-00000090: 2d43 7265 6174 696f 6e2d 4461 7465 3a20  -Creation-Date: 
-000000a0: 3230 3136 2d30 392d 3039 2031 353a 3031  2016-09-09 15:01
-000000b0: 2b30 3230 300a 504f 2d52 6576 6973 696f  +0200.PO-Revisio
-000000c0: 6e2d 4461 7465 3a20 5945 4152 2d4d 4f2d  n-Date: YEAR-MO-
-000000d0: 4441 2048 4f3a 4d49 2b5a 4f4e 450a 4c61  DA HO:MI+ZONE.La
-000000e0: 7374 2d54 7261 6e73 6c61 746f 723a 2046  st-Translator: F
-000000f0: 554c 4c20 4e41 4d45 203c 454d 4149 4c40  ULL NAME <EMAIL@
-00000100: 4144 4452 4553 533e 0a4c 616e 6775 6167  ADDRESS>.Languag
-00000110: 653a 2065 730a 4c61 6e67 7561 6765 2d54  e: es.Language-T
-00000120: 6561 6d3a 2053 7061 6e69 7368 2028 6874  eam: Spanish (ht
-00000130: 7470 733a 2f2f 7777 772e 7472 616e 7369  tps://www.transi
-00000140: 6665 782e 636f 6d2f 696e 7665 6e69 6f73  fex.com/invenios
-00000150: 6f66 7477 6172 652f 7465 616d 732f 3233  oftware/teams/23
-00000160: 3533 372f 6573 2f29 0a50 6c75 7261 6c2d  537/es/).Plural-
-00000170: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
-00000180: 323b 2070 6c75 7261 6c3d 286e 2021 3d20  2; plural=(n != 
-00000190: 3129 3b0a 4d49 4d45 2d56 6572 7369 6f6e  1);.MIME-Version
-000001a0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
-000001b0: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
-000001c0: 6368 6172 7365 743d 7574 662d 380a 436f  charset=utf-8.Co
-000001d0: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
-000001e0: 6e63 6f64 696e 673a 2038 6269 740a 4765  ncoding: 8bit.Ge
-000001f0: 6e65 7261 7465 642d 4279 3a20 4261 6265  nerated-By: Babe
-00000200: 6c20 322e 3132 2e31 0a00                 l 2.12.1..
+00000050: 6965 6e74 2032 2e30 2e30 0a52 6570 6f72  ient 2.0.0.Repor
+00000060: 742d 4d73 6769 642d 4275 6773 2d54 6f3a  t-Msgid-Bugs-To:
+00000070: 2069 6e66 6f40 696e 7665 6e69 6f73 6f66   info@inveniosof
+00000080: 7477 6172 652e 6f72 670a 504f 542d 4372  tware.org.POT-Cr
+00000090: 6561 7469 6f6e 2d44 6174 653a 2032 3032  eation-Date: 202
+000000a0: 322d 3035 2d32 3720 3039 3a35 382b 3032  2-05-27 09:58+02
+000000b0: 3030 0a50 4f2d 5265 7669 7369 6f6e 2d44  00.PO-Revision-D
+000000c0: 6174 653a 2032 3031 362d 3038 2d31 3820  ate: 2016-08-18 
+000000d0: 3135 3a31 392b 3030 3030 0a4c 6173 742d  15:19+0000.Last-
+000000e0: 5472 616e 736c 6174 6f72 3a20 4655 4c4c  Translator: FULL
+000000f0: 204e 414d 4520 3c45 4d41 494c 4041 4444   NAME <EMAIL@ADD
+00000100: 5245 5353 3e0a 4c61 6e67 7561 6765 3a20  RESS>.Language: 
+00000110: 7277 0a4c 616e 6775 6167 652d 5465 616d  rw.Language-Team
+00000120: 3a20 4b69 6e79 6172 7761 6e64 6120 2868  : Kinyarwanda (h
+00000130: 7474 7073 3a2f 2f61 7070 2e74 7261 6e73  ttps://app.trans
+00000140: 6966 6578 2e63 6f6d 2f69 6e76 656e 696f  ifex.com/invenio
+00000150: 736f 6674 7761 7265 2f74 6561 6d73 2f32  software/teams/2
+00000160: 3335 3337 2f72 772f 290a 506c 7572 616c  3537/rw/).Plural
+00000170: 2d46 6f72 6d73 3a20 6e70 6c75 7261 6c73  -Forms: nplurals
+00000180: 3d32 3b20 706c 7572 616c 3d28 6e20 213d  =2; plural=(n !=
+00000190: 2031 293b 0a4d 494d 452d 5665 7273 696f   1);.MIME-Versio
+000001a0: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
+000001b0: 7970 653a 2074 6578 742f 706c 6169 6e3b  ype: text/plain;
+000001c0: 2063 6861 7273 6574 3d75 7466 2d38 0a43   charset=utf-8.C
+000001d0: 6f6e 7465 6e74 2d54 7261 6e73 6665 722d  ontent-Transfer-
+000001e0: 456e 636f 6469 6e67 3a20 3862 6974 0a47  Encoding: 8bit.G
+000001f0: 656e 6572 6174 6564 2d42 793a 2042 6162  enerated-By: Bab
+00000200: 656c 2032 2e31 322e 310a 00              el 2.12.1..
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,123 @@
 # Translations template for invenio-oauthclient.
-# Copyright (C) 2016 CERN
+# Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-oauthclient
 # project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: invenio-oauthclient 1.0.0a10\n"
+"Project-Id-Version: invenio-oauthclient 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2016-09-09 15:01+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"POT-Creation-Date: 2022-05-27 09:58+0200\n"
+"PO-Revision-Date: 2016-08-18 15:19+0000\n"
+"Language-Team: Spanish (Cuba) (https://app.transifex.com/inveniosoftware/teams/23537/es_CU/)\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.3.4\n"
-"Language: es\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Generated-By: Babel 2.10.1\n"
+"Language: es_CU\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
-#: invenio_oauthclient/admin.py:64
+#: invenio_oauthclient/admin.py:52
 msgid "ID"
 msgstr ""
 
-#: invenio_oauthclient/admin.py:65
+#: invenio_oauthclient/admin.py:53
 msgid "User ID"
 msgstr ""
 
-#: invenio_oauthclient/admin.py:66
+#: invenio_oauthclient/admin.py:54
 msgid "Client ID"
 msgstr ""
 
-#: invenio_oauthclient/admin.py:95
+#: invenio_oauthclient/admin.py:83
 msgid "ID Remote Account"
 msgstr ""
 
-#: invenio_oauthclient/admin.py:102 invenio_oauthclient/admin.py:108
+#: invenio_oauthclient/admin.py:90 invenio_oauthclient/admin.py:98
 msgid "User Management"
 msgstr ""
 
-#: invenio_oauthclient/handlers.py:189
-msgid "You rejected the authentication request."
+#: invenio_oauthclient/admin.py:91
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:12
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:12
+#: invenio_oauthclient/views/settings.py:47
+msgid "Linked accounts"
+msgstr ""
+
+#: invenio_oauthclient/admin.py:99
+msgid "Linked account tokens"
 msgstr ""
 
-#: invenio_oauthclient/handlers.py:193
+#: invenio_oauthclient/contrib/cern.py:429
+#: invenio_oauthclient/contrib/cern_openid.py:305
+msgid "CERN account not allowed."
+msgstr ""
+
+#: invenio_oauthclient/handlers/ui.py:42
 msgid "External service is already linked to another account."
 msgstr ""
 
-#: invenio_oauthclient/handlers.py:447
-msgid "Authorization with remote service failed."
+#: invenio_oauthclient/handlers/ui.py:47
+msgid "You rejected the authentication request."
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:40
-msgid "Close"
+#: invenio_oauthclient/handlers/ui.py:173
+msgid "Authorization with remote service failed."
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:58
+#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:25
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html:60
 #, python-format
 msgid "Sign in with %(title)s"
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:34
+#: invenio_oauthclient/templates/invenio_oauthclient/login_user.html:21
+msgid "OR"
+msgstr ""
+
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:24
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:29
 #, python-format
 msgid "Sign-up with %(title)s!"
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:35
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:25
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:32
 msgid ""
 "Fill in your details to complete your registration. You only have to do this"
 " once."
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:25
-#: invenio_oauthclient/views/settings.py:54
-msgid "Linked accounts"
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:33
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:45
+msgid "Complete registration"
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:31
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:20
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:20
 #, python-format
 msgid ""
 "Tired of entering password for %(sitename)s every time you sign in? Set up "
 "single sign-on with one or more of the services below:"
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:41
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:31
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:32
 msgid "Disconnect"
 msgstr ""
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:43
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:33
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:34
 msgid "Connect"
 msgstr ""
 
-#: invenio_oauthclient/views/settings.py:48
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html:26
+msgid "Or"
+msgstr ""
+
+#: invenio_oauthclient/views/settings.py:38
 #, python-format
 msgid "%(icon)s Linked accounts"
 msgstr ""
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,75 +1,75 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: invenio-oauthclient 1.0.0a10\n"
+"Project-Id-Version: invenio-oauthclient 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2016-09-09 15:01+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2016\n"
-"Language: fr\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/"
-"fr/)\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"POT-Creation-Date: 2022-05-27 09:58+0200\n"
+"PO-Revision-Date: 2016-08-18 15:19+0000\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
+"Language: it\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/"
+"teams/23537/it/)\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
+"1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "%(icon)s Linked accounts"
-msgstr "%(icon)s Comptes liés"
+msgstr "%(icon)s Conti legati"
 
 msgid "Authorization with remote service failed."
-msgstr "Echec de l'autorisation du service externe."
+msgstr "L'autorizzazione con il servizio esterno ha fallito."
 
 msgid "Client ID"
-msgstr "ID de Client"
-
-msgid "Close"
-msgstr "Fermer"
+msgstr "ID Cliente"
 
 msgid "Connect"
-msgstr "Connexion"
+msgstr "Collega"
 
 msgid "Disconnect"
-msgstr "Déconnexion"
+msgstr "Scollega"
 
 msgid "External service is already linked to another account."
-msgstr "Le service externe est déjà lié à un autre compte."
+msgstr "Il servizio esterno è già collegato a un altro conto."
 
 msgid ""
 "Fill in your details to complete your registration. You only have to do this "
 "once."
 msgstr ""
-"Remplissez vos informations pour compléter votre inscription. Vous n'aurez à "
-"faire ceci qu'une fois."
+"Completa i tuoi dettagli per finire la registrazione. Devi farlo una volta "
+"sola."
 
 msgid "ID"
 msgstr "ID"
 
 msgid "ID Remote Account"
-msgstr "ID du Compte Externe"
+msgstr "ID Conto Esterno"
 
 msgid "Linked accounts"
-msgstr "Comptes liés"
+msgstr "Conti legati"
+
+msgid "OR"
+msgstr "O"
 
 msgid "Sign in with %(title)s"
-msgstr "Inscription avec %(title)s"
+msgstr "Registra con %(title)s"
 
 msgid "Sign-up with %(title)s!"
-msgstr "Connexion avec %(title)s!"
+msgstr "Accedi con %(title)s"
 
 msgid ""
 "Tired of entering password for %(sitename)s every time you sign in? Set up "
 "single sign-on with one or more of the services below:"
 msgstr ""
-"Vous n'avez pas envie d'entrer votre mot de passe pour %(sitename)s à chaque "
-"fois que vous vous connectez? Etablissez une connexion unique avec un ou "
-"plusieurs des services ci-dessous:"
+"Non vuoi inserire la password ogni volta che accedi a %(sitename)s? "
+"Configura un accesso unico con uno o più servizi di seguito:"
 
 msgid "User ID"
-msgstr "ID d'Utilisateur"
+msgstr "ID Utente"
 
 msgid "User Management"
-msgstr "Gestion Utilisateur"
+msgstr "Gestione Utenti"
 
 msgid "You rejected the authentication request."
-msgstr "Vous avez rejeté la demande d'authentification."
+msgstr "Hai rifiutato la richiesta d'autenticazione."
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hu/LC_MESSAGES/messages.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,133 @@
 # Translations template for invenio-oauthclient.
-# Copyright (C) 2016 CERN
+# Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-oauthclient
 # project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# 
+# Translators:
+# Andrea Dömötör, 2022
+# Dorottya Szemigán, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: invenio-oauthclient 1.0.0a10\n"
+"Project-Id-Version: invenio-oauthclient 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2016-09-09 15:01+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2016\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"POT-Creation-Date: 2022-05-27 09:58+0200\n"
+"PO-Revision-Date: 2016-08-18 15:19+0000\n"
+"Last-Translator: Dorottya Szemigán, 2022\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.3.4\n"
-"Language: fr\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Generated-By: Babel 2.10.1\n"
+"Language: hu\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: invenio_oauthclient/admin.py:64
+#: invenio_oauthclient/admin.py:52
 msgid "ID"
 msgstr "ID"
 
-#: invenio_oauthclient/admin.py:65
+#: invenio_oauthclient/admin.py:53
 msgid "User ID"
-msgstr "ID d'Utilisateur"
+msgstr "Felhasználói azonosító"
 
-#: invenio_oauthclient/admin.py:66
+#: invenio_oauthclient/admin.py:54
 msgid "Client ID"
-msgstr "ID de Client"
+msgstr "Kliens ID"
 
-#: invenio_oauthclient/admin.py:95
+#: invenio_oauthclient/admin.py:83
 msgid "ID Remote Account"
-msgstr "ID du Compte Externe"
+msgstr "ID Távolsági Felhasználói fiók"
 
-#: invenio_oauthclient/admin.py:102 invenio_oauthclient/admin.py:108
+#: invenio_oauthclient/admin.py:90 invenio_oauthclient/admin.py:98
 msgid "User Management"
-msgstr "Gestion Utilisateur"
+msgstr "Felhasználók kezelése"
 
-#: invenio_oauthclient/handlers.py:189
-msgid "You rejected the authentication request."
-msgstr "Vous avez rejeté la demande d'authentification."
+#: invenio_oauthclient/admin.py:91
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:12
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:12
+#: invenio_oauthclient/views/settings.py:47
+msgid "Linked accounts"
+msgstr "Kapcsolódó fiókok"
+
+#: invenio_oauthclient/admin.py:99
+msgid "Linked account tokens"
+msgstr "Kapcsolt fióktokenek"
+
+#: invenio_oauthclient/contrib/cern.py:429
+#: invenio_oauthclient/contrib/cern_openid.py:305
+msgid "CERN account not allowed."
+msgstr "A CERN fiók nem engedélyezett."
 
-#: invenio_oauthclient/handlers.py:193
+#: invenio_oauthclient/handlers/ui.py:42
 msgid "External service is already linked to another account."
-msgstr "Le service externe est déjà lié à un autre compte."
+msgstr ""
+"A külső szolgáltatás már kapcsolva van egy másik felhasználói fiókhoz."
 
-#: invenio_oauthclient/handlers.py:447
-msgid "Authorization with remote service failed."
-msgstr "Echec de l'autorisation du service externe."
+#: invenio_oauthclient/handlers/ui.py:47
+msgid "You rejected the authentication request."
+msgstr "Ön elutasította a hitelesítési kérést."
 
-#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:40
-msgid "Close"
-msgstr "Fermer"
+#: invenio_oauthclient/handlers/ui.py:173
+msgid "Authorization with remote service failed."
+msgstr "A távolsági szolgáltatás engedélyezése meghiúsult."
 
-#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:58
+#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:25
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html:60
 #, python-format
 msgid "Sign in with %(title)s"
-msgstr "Inscription avec %(title)s"
+msgstr "Belépés ezzel: %(title)s"
+
+#: invenio_oauthclient/templates/invenio_oauthclient/login_user.html:21
+msgid "OR"
+msgstr "VAGY"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:34
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:24
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:29
 #, python-format
 msgid "Sign-up with %(title)s!"
-msgstr "Connexion avec %(title)s!"
+msgstr "Regisztráció ezzel: %(title)s!"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:35
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:25
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:32
 msgid ""
 "Fill in your details to complete your registration. You only have to do this"
 " once."
 msgstr ""
-"Remplissez vos informations pour compléter votre inscription. Vous n'aurez à"
-" faire ceci qu'une fois."
+"Töltse ki az adatokat a regisztráció befejezéséhez! Ezt csak egyszer kell "
+"megtennie."
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:25
-#: invenio_oauthclient/views/settings.py:54
-msgid "Linked accounts"
-msgstr "Comptes liés"
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:33
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:45
+msgid "Complete registration"
+msgstr "Regisztráció befejezése"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:31
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:20
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:20
 #, python-format
 msgid ""
 "Tired of entering password for %(sitename)s every time you sign in? Set up "
 "single sign-on with one or more of the services below:"
 msgstr ""
-"Vous n'avez pas envie d'entrer votre mot de passe pour %(sitename)s à chaque"
-" fois que vous vous connectez? Etablissez une connexion unique avec un ou "
-"plusieurs des services ci-dessous:"
+"Elege van, hogy a %(sitename)s felhasználónévhez mindig jelszavat írjon be? "
+"Állítson be egyszerű belépést az alábbi szolgáltatás(ok) segítségével:"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:41
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:31
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:32
 msgid "Disconnect"
-msgstr "Déconnexion"
+msgstr "Kapcsolat bontása"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:43
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:33
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:34
 msgid "Connect"
-msgstr "Connexion"
+msgstr "Kapcsolódás"
+
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html:26
+msgid "Or"
+msgstr "Vagy"
 
-#: invenio_oauthclient/views/settings.py:48
+#: invenio_oauthclient/views/settings.py:38
 #, python-format
 msgid "%(icon)s Linked accounts"
-msgstr "%(icon)s Comptes liés"
+msgstr "%(icon)s kapcsolt fiók"
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,74 +1,86 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: invenio-oauthclient 1.0.0a10\n"
+"Project-Id-Version: invenio-oauthclient 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2016-09-09 15:01+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2016\n"
-"Language: it\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/it/)\n"
+"POT-Creation-Date: 2022-05-27 09:58+0200\n"
+"PO-Revision-Date: 2016-08-18 15:19+0000\n"
+"Last-Translator: Dorottya Szemigán, 2022\n"
+"Language: hu\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/"
+"teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "%(icon)s Linked accounts"
-msgstr "%(icon)s Conti legati"
+msgstr "%(icon)s kapcsolt fiók"
 
 msgid "Authorization with remote service failed."
-msgstr "L'autorizzazione con il servizio esterno ha fallito."
+msgstr "A távolsági szolgáltatás engedélyezése meghiúsult."
+
+msgid "CERN account not allowed."
+msgstr "A CERN fiók nem engedélyezett."
 
 msgid "Client ID"
-msgstr "ID Cliente"
+msgstr "Kliens ID"
 
-msgid "Close"
-msgstr "Chiudi"
+msgid "Complete registration"
+msgstr "Regisztráció befejezése"
 
 msgid "Connect"
-msgstr "Collega"
+msgstr "Kapcsolódás"
 
 msgid "Disconnect"
-msgstr "Scollega"
+msgstr "Kapcsolat bontása"
 
 msgid "External service is already linked to another account."
-msgstr "Il servizio esterno è già collegato a un altro conto."
+msgstr "A külső szolgáltatás már kapcsolva van egy másik felhasználói fiókhoz."
 
 msgid ""
 "Fill in your details to complete your registration. You only have to do this "
 "once."
 msgstr ""
-"Completa i tuoi dettagli per finire la registrazione. Devi farlo una volta "
-"sola."
+"Töltse ki az adatokat a regisztráció befejezéséhez! Ezt csak egyszer kell "
+"megtennie."
 
 msgid "ID"
 msgstr "ID"
 
 msgid "ID Remote Account"
-msgstr "ID Conto Esterno"
+msgstr "ID Távolsági Felhasználói fiók"
+
+msgid "Linked account tokens"
+msgstr "Kapcsolt fióktokenek"
 
 msgid "Linked accounts"
-msgstr "Conti legati"
+msgstr "Kapcsolódó fiókok"
+
+msgid "OR"
+msgstr "VAGY"
+
+msgid "Or"
+msgstr "Vagy"
 
 msgid "Sign in with %(title)s"
-msgstr "Registra con %(title)s"
+msgstr "Belépés ezzel: %(title)s"
 
 msgid "Sign-up with %(title)s!"
-msgstr "Accedi con %(title)s"
+msgstr "Regisztráció ezzel: %(title)s!"
 
 msgid ""
 "Tired of entering password for %(sitename)s every time you sign in? Set up "
 "single sign-on with one or more of the services below:"
 msgstr ""
-"Non vuoi inserire la password ogni volta che accedi a %(sitename)s? "
-"Configura un accesso unico con uno o più servizi di seguito:"
+"Elege van, hogy a %(sitename)s felhasználónévhez mindig jelszavat írjon be? "
+"Állítson be egyszerű belépést az alábbi szolgáltatás(ok) segítségével:"
 
 msgid "User ID"
-msgstr "ID Utente"
+msgstr "Felhasználói azonosító"
 
 msgid "User Management"
-msgstr "Gestione Utenti"
+msgstr "Felhasználók kezelése"
 
 msgid "You rejected the authentication request."
-msgstr "Hai rifiutato la richiesta d'autenticazione."
+msgstr "Ön elutasította a hitelesítési kérést."
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/tr/LC_MESSAGES/messages.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,133 @@
 # Translations template for invenio-oauthclient.
-# Copyright (C) 2016 CERN
+# Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-oauthclient
 # project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# 
+# Translators:
+# Berat Aldemir <berataldemir@gmail.com>, 2020
+# Ben Translation and Interpreting Services <info@bentercume.com>, 2021
 # 
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: invenio-oauthclient 1.0.0a10\n"
+"Project-Id-Version: invenio-oauthclient 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2016-09-09 15:01+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2016\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"POT-Creation-Date: 2022-05-27 09:58+0200\n"
+"PO-Revision-Date: 2016-08-18 15:19+0000\n"
+"Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2021\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.3.4\n"
-"Language: it\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Generated-By: Babel 2.10.1\n"
+"Language: tr\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: invenio_oauthclient/admin.py:64
+#: invenio_oauthclient/admin.py:52
 msgid "ID"
 msgstr "ID"
 
-#: invenio_oauthclient/admin.py:65
+#: invenio_oauthclient/admin.py:53
 msgid "User ID"
-msgstr "ID Utente"
+msgstr "Kullanıcı Kimliği"
 
-#: invenio_oauthclient/admin.py:66
+#: invenio_oauthclient/admin.py:54
 msgid "Client ID"
-msgstr "ID Cliente"
+msgstr "İstemci Kimliği"
 
-#: invenio_oauthclient/admin.py:95
+#: invenio_oauthclient/admin.py:83
 msgid "ID Remote Account"
-msgstr "ID Conto Esterno"
+msgstr "ID Uzak Hesap"
 
-#: invenio_oauthclient/admin.py:102 invenio_oauthclient/admin.py:108
+#: invenio_oauthclient/admin.py:90 invenio_oauthclient/admin.py:98
 msgid "User Management"
-msgstr "Gestione Utenti"
+msgstr "Kullanıcı Yönetimi"
 
-#: invenio_oauthclient/handlers.py:189
-msgid "You rejected the authentication request."
-msgstr "Hai rifiutato la richiesta d'autenticazione."
+#: invenio_oauthclient/admin.py:91
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:12
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:12
+#: invenio_oauthclient/views/settings.py:47
+msgid "Linked accounts"
+msgstr "Bağlı hesaplar"
 
-#: invenio_oauthclient/handlers.py:193
+#: invenio_oauthclient/admin.py:99
+msgid "Linked account tokens"
+msgstr "Bağlı hesap belirteçleri"
+
+#: invenio_oauthclient/contrib/cern.py:429
+#: invenio_oauthclient/contrib/cern_openid.py:305
+msgid "CERN account not allowed."
+msgstr "CERN hesabına izin verilmemekte."
+
+#: invenio_oauthclient/handlers/ui.py:42
 msgid "External service is already linked to another account."
-msgstr "Il servizio esterno è già collegato a un altro conto."
+msgstr "Harici hizmet zaten başka bir hesaba bağlı."
 
-#: invenio_oauthclient/handlers.py:447
-msgid "Authorization with remote service failed."
-msgstr "L'autorizzazione con il servizio esterno ha fallito."
+#: invenio_oauthclient/handlers/ui.py:47
+msgid "You rejected the authentication request."
+msgstr "Kimlik doğrulama isteğini reddettiniz."
 
-#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:40
-msgid "Close"
-msgstr "Chiudi"
+#: invenio_oauthclient/handlers/ui.py:173
+msgid "Authorization with remote service failed."
+msgstr "Uzak hizmet yetkilendirmesi başarısız oldu."
 
-#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:58
+#: invenio_oauthclient/templates/invenio_oauthclient/_macros.html:25
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html:60
 #, python-format
 msgid "Sign in with %(title)s"
-msgstr "Registra con %(title)s"
+msgstr "%(title)s ile oturum açın"
+
+#: invenio_oauthclient/templates/invenio_oauthclient/login_user.html:21
+msgid "OR"
+msgstr "VEYA"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:34
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:24
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:29
 #, python-format
 msgid "Sign-up with %(title)s!"
-msgstr "Accedi con %(title)s"
+msgstr "%(title)s ile kayıt olun !"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:35
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:25
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:32
 msgid ""
 "Fill in your details to complete your registration. You only have to do this"
 " once."
 msgstr ""
-"Completa i tuoi dettagli per finire la registrazione. Devi farlo una volta "
-"sola."
+"Kaydınızı tamamlamak için bilgilerinizi girin. Bunu yalnızca bir kez "
+"yapmanız gerekli."
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:25
-#: invenio_oauthclient/views/settings.py:54
-msgid "Linked accounts"
-msgstr "Conti legati"
+#: invenio_oauthclient/templates/invenio_oauthclient/signup.html:33
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html:45
+msgid "Complete registration"
+msgstr "Kayıt işlemini tamamlayın"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:31
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:20
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:20
 #, python-format
 msgid ""
 "Tired of entering password for %(sitename)s every time you sign in? Set up "
 "single sign-on with one or more of the services below:"
 msgstr ""
-"Non vuoi inserire la password ogni volta che accedi a %(sitename)s? "
-"Configura un accesso unico con uno o più servizi di seguito:"
+"%(sitename)s için her oturum açtığınızda şifre girmekten bıktınız mı? "
+"Aşağıdaki hizmetlerden bir veya daha fazlasıyla tek oturum açma (SSO) "
+"ayarlayın:"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:41
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:31
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:32
 msgid "Disconnect"
-msgstr "Scollega"
+msgstr "Bağlantıyı kes"
 
-#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:43
+#: invenio_oauthclient/templates/invenio_oauthclient/settings/index.html:33
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html:34
 msgid "Connect"
-msgstr "Collega"
+msgstr "Bağlan"
+
+#: invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html:26
+msgid "Or"
+msgstr "Veya"
 
-#: invenio_oauthclient/views/settings.py:48
+#: invenio_oauthclient/views/settings.py:38
 #, python-format
 msgid "%(icon)s Linked accounts"
-msgstr "%(icon)s Conti legati"
+msgstr "%(icon)s Bağlı hesaplar"
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/messages.pot` & `invenio-oauthclient-3.2.0/invenio_oauthclient/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/views/client.py` & `invenio-oauthclient-3.2.0/tests/test_handlers_rest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,296 +1,321 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2016-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
-"""Client blueprint used to handle OAuth callbacks."""
-
-from flask import Blueprint, abort, current_app, redirect, request, session, url_for
-from flask_oauthlib.client import OAuthException
-from invenio_accounts.views import login as base_login
-from invenio_db import db
-from itsdangerous import BadData
-
-from .._compat import _create_identifier
-from ..errors import OAuthRemoteNotFound
-from ..handlers import set_session_next_url
-from ..handlers.rest import response_handler
-from ..proxies import current_oauthclient
-from ..utils import get_safe_redirect_target, serializer
-
-blueprint = Blueprint(
-    "invenio_oauthclient",
-    __name__,
-    url_prefix="/oauth",
-    static_folder="../static",
-    template_folder="../templates",
-)
+"""Test handlers."""
 
+from turtle import pd
 
-rest_blueprint = Blueprint(
-    "invenio_oauthclient",
-    __name__,
-    url_prefix="/oauth",
-    static_folder="../static",
-    template_folder="../templates",
+import pytest
+from flask import session, url_for
+from flask_login import current_user
+from flask_oauthlib.client import OAuth as FlaskOAuth
+from flask_security import login_user, logout_user
+from flask_security.confirmable import _security
+from helpers import check_response_redirect_url_args
+from invenio_accounts.models import Role
+from invenio_accounts.proxies import current_datastore
+from werkzeug.routing import BuildError
+
+from invenio_oauthclient import InvenioOAuthClientREST, current_oauthclient
+from invenio_oauthclient.errors import AlreadyLinkedError
+from invenio_oauthclient.handlers import token_session_key, token_setter
+from invenio_oauthclient.handlers.rest import (
+    authorized_signup_handler,
+    disconnect_handler,
+    oauth_resp_remote_error_handler,
+    response_handler_postmessage,
+    signup_handler,
 )
+from invenio_oauthclient.models import RemoteToken
+from invenio_oauthclient.oauth import oauth_authenticate
+from invenio_oauthclient.views.client import rest_blueprint
 
-
-@blueprint.record_once
-def post_ext_init(state):
-    """Setup blueprint."""
-    app = state.app
-
-    app.config.setdefault(
-        "OAUTHCLIENT_SITENAME", app.config.get("THEME_SITENAME", "Invenio")
-    )
-    app.config.setdefault(
-        "OAUTHCLIENT_BASE_TEMPLATE",
-        app.config.get("BASE_TEMPLATE", "invenio_oauthclient/base.html"),
-    )
-    app.config.setdefault(
-        "OAUTHCLIENT_COVER_TEMPLATE",
-        app.config.get("COVER_TEMPLATE", "invenio_oauthclient/base_cover.html"),
-    )
-    app.config.setdefault(
-        "OAUTHCLIENT_SETTINGS_TEMPLATE",
-        app.config.get("SETTINGS_TEMPLATE", "invenio_oauthclient/settings/base.html"),
-    )
-
-
-@blueprint.route("/login")
-def auto_redirect_login(*args, **kwargs):
-    """Handles automatic redirect to external auth service.
-
-    The login endpoint will redirect automatically to the external
-    auth service is the following conditions are met:
-
-    * local login is disabled
-    * redirect to external login is enabled
-    * only one external auth service is configured
-
-    This function should be set as value of the invenio-accounts
-    config var ``ACCOUNTS_LOGIN_VIEW_FUNCTION``. It should be defined in
-    the Invenio application configuration to ensure that is correctly loaded.
-    """
-    local_login_enabled = current_app.config.get("ACCOUNTS_LOCAL_LOGIN_ENABLED", False)
-    auto_redirect_enabled = current_app.config.get(
-        "OAUTHCLIENT_AUTO_REDIRECT_TO_EXTERNAL_LOGIN", False
-    )
-    would_redirect = auto_redirect_enabled and not local_login_enabled
-    remote_apps = list(current_oauthclient.oauth.remote_apps)
-
-    if would_redirect and len(remote_apps) == 1:
-        redirect_args = {
-            # if local login is disabled and we only have one OAuth2 remote app
-            # configured, we forward directly to that
-            "remote_app": remote_apps[0],
-        }
-        next_url = request.args.get("next")
-        if next_url:
-            redirect_args["next"] = next_url
-        url = url_for("invenio_oauthclient.login", **redirect_args)
-        return redirect(url)
-
-    else:
-        return base_login(*args, **kwargs)
+REMOTE_APPS = ["github", "orcid", "globus"]
 
 
-def _login(remote_app, authorized_view_name):
-    """Send user to remote application for authentication."""
+@pytest.fixture(scope="function")
+def remote(request, app_rest):
+    """Fixture to return a remote app by name."""
     oauth = current_oauthclient.oauth
-    if remote_app not in oauth.remote_apps:
-        raise OAuthRemoteNotFound()
+    return oauth.remote_apps[request.param]
 
-    # Get redirect target in safe manner.
-    next_param = get_safe_redirect_target(arg="next")
-
-    # Redirect URI - must be registered in the remote service.
-    callback_url = url_for(
-        authorized_view_name, remote_app=remote_app, _external=True, _scheme="https"
-    )
 
-    # Create a JSON Web Token that expires after OAUTHCLIENT_STATE_EXPIRES
-    # seconds.
-    state_token = serializer.dumps(
+@pytest.mark.parametrize("remote", REMOTE_APPS, indirect=["remote"])
+def test_authorized_signup_handler(remote, app_rest, models_fixture):
+    """Test authorized signup handler."""
+    datastore = app_rest.extensions["invenio-accounts"].datastore
+    user = datastore.find_user(email="existing@inveniosoftware.org")
+    existing_email = "existing@inveniosoftware.org"
+
+    example_response = {"access_token": "test_access_token"}
+    example_account_info = {
+        "user": {
+            "email": existing_email,
+        },
+        "external_id": "1234",
+        "external_method": "test_method",
+    }
+
+    # Mock remote app's handler
+    current_oauthclient.signup_handlers[remote.name] = {
+        "setup": lambda token, resp: None,
+        "info": lambda resp: example_account_info,
+    }
+
+    # Authenticate user
+    oauth_authenticate("dev", user)
+
+    # Mock next url
+    next_url = "/test/redirect"
+    session[token_session_key(remote.name) + "_next_url"] = next_url
+
+    # Check user is redirected to next_url
+    expected_url_args = {
+        "message": "Successfully authorized.",
+        "code": 200,
+        "next_url": next_url,
+    }
+    resp = authorized_signup_handler(example_response, remote)
+    check_response_redirect_url_args(resp, expected_url_args)
+
+
+@pytest.mark.parametrize("remote", REMOTE_APPS, indirect=["remote"])
+def test_groups_handler(remote, app_rest, models_fixture):
+    """Test group handler."""
+    datastore = app_rest.extensions["invenio-accounts"].datastore
+    existing_email = "existing@inveniosoftware.org"
+    user = datastore.find_user(email=existing_email)
+    example_groups = [
         {
-            "app": remote_app,
-            "next": next_param,
-            "sid": _create_identifier(),
-        }
+            "id": "rdm-developers",
+            "name": "rdm-developers",
+            "description": "People contributing to RDM.",
+        },
+        {
+            "id": "existing-group-id",
+            "name": "new-group-name",
+            "description": "A previously existing group with a changed name",
+        },
+    ]
+
+    example_response = {"access_token": "test_access_token"}
+    example_account_info = {
+        "user": {
+            "email": existing_email,
+        },
+        "external_id": "1234",
+        "external_method": "test_method",
+    }
+
+    # prepare previously existing role in the db
+    assert 0 == Role.query.count()
+    current_datastore.create_role(
+        id=example_groups[1]["id"],
+        name="previous-group-name",
+        description=example_groups[1]["description"],
+        is_managed=False,
     )
-    return oauth.remote_apps[remote_app].authorize(
-        callback=callback_url,
-        state=state_token,
+    current_datastore.commit()
+
+    # Mock remote app's handler
+    current_oauthclient.signup_handlers[remote.name] = {
+        "info": lambda resp: example_account_info,
+        "groups": lambda resp: example_groups,
+    }
+
+    _security.confirmable = True
+    _security.login_without_confirmation = False
+    user.confirmed_at = None
+
+    authorized_signup_handler(example_response, remote)
+
+    # Assert that the new group is created
+    roles = Role.query.all()
+    assert 2 == len(roles)
+
+    role = Role.query.filter(Role.id == example_groups[0]["id"]).one()
+    assert role.id == example_groups[0]["id"]
+    assert role.name == example_groups[0]["name"]
+    assert role.description == example_groups[0]["description"]
+
+    # Assert that existing group is updated
+    role = Role.query.filter(Role.id == example_groups[1]["id"]).one()
+    assert role.id == example_groups[1]["id"]
+    assert role.name == "new-group-name"
+    assert role.description == example_groups[1]["description"]
+
+
+@pytest.mark.parametrize("remote", REMOTE_APPS, indirect=["remote"])
+def test_unauthorized_signup(remote, app_rest, models_fixture):
+    """Test unauthorized redirect on signup callback handler."""
+    datastore = app_rest.extensions["invenio-accounts"].datastore
+    existing_email = "existing@inveniosoftware.org"
+    user = datastore.find_user(email=existing_email)
+
+    example_response = {"access_token": "test_access_token"}
+    example_account_info = {
+        "user": {
+            "email": existing_email,
+        },
+        "external_id": "1234",
+        "external_method": "test_method",
+    }
+
+    # Mock remote app's handler
+    current_oauthclient.signup_handlers[remote.name] = {
+        "info": lambda resp: example_account_info,
+    }
+
+    _security.confirmable = True
+    _security.login_without_confirmation = False
+    user.confirmed_at = None
+
+    expected_url_args = {"message": "Unauthorized.", "code": 401}
+    resp = authorized_signup_handler(example_response, remote)
+    check_response_redirect_url_args(resp, expected_url_args)
+
+
+@pytest.mark.parametrize("remote", REMOTE_APPS, indirect=["remote"])
+def test_signup_handler(remote, app_rest, models_fixture):
+    """Test signup handler."""
+    datastore = app_rest.extensions["invenio-accounts"].datastore
+    existing_email = "existing@inveniosoftware.org"
+    user = datastore.find_user(email=existing_email)
+    # Already authenticated
+    login_user(user)
+    assert current_user.is_authenticated
+    resp1 = signup_handler(remote)
+    expected_url_args = {"message": "Successfully signed up.", "code": 200}
+    check_response_redirect_url_args(resp1, expected_url_args)
+    logout_user()
+    assert not current_user.is_authenticated
+
+    # No OAuth token
+    resp2 = signup_handler(remote)
+    expected_url_args = {"message": "Token not found.", "code": 400}
+
+    check_response_redirect_url_args(resp2, expected_url_args)
+
+    # Not coming from authorized request
+    token = RemoteToken.create(user.id, "testkey", "mytoken", "mysecret")
+    token_setter(remote, token, "mysecret")
+    with pytest.raises(BuildError):
+        signup_handler(remote)
+
+
+@pytest.mark.parametrize("remote", REMOTE_APPS, indirect=["remote"])
+def test_already_linked_exception(remote, app_rest):
+    """Test error when service is already linked to another account."""
+
+    @oauth_resp_remote_error_handler
+    def mock_handler(resp, remote):
+        raise AlreadyLinkedError(None, None)
+
+    resp = mock_handler(None, remote)
+    expected_url_args = {
+        "message": "External service is already linked to another account.",
+        "code": 400,
+    }
+    check_response_redirect_url_args(resp, expected_url_args)
+
+
+@pytest.mark.parametrize("remote", REMOTE_APPS, indirect=["remote"])
+def test_unauthorized_disconnect(remote, app_rest):
+    """Test disconnect handler when user is not authenticated."""
+
+    def mock_unauthorized():
+        return "Unauthorized"
+
+    app_rest.login_manager.unauthorized = mock_unauthorized
+    resp = disconnect_handler(remote)
+    expected_url_args = {"message": "Unauthorized.", "code": 401}
+    check_response_redirect_url_args(resp, expected_url_args)
+
+
+@pytest.mark.parametrize("remote_name", REMOTE_APPS)
+def test_dummy_handler(remote_name, base_app):
+    """Test dummy handler."""
+
+    signup_handler = base_app.config["OAUTHCLIENT_REST_REMOTE_APPS"][remote_name][
+        "signup_handler"
+    ]
+
+    # Force usage of dummy handlers
+    base_app.config["OAUTHCLIENT_REST_REMOTE_APPS"][remote_name]["signup_handler"] = {}
+
+    # Initialize InvenioOAuth
+    FlaskOAuth(base_app)
+    InvenioOAuthClientREST(base_app)
+    base_app.register_blueprint(rest_blueprint)
+
+    # Try to sign-up client
+    base_app.test_client().get(
+        url_for(
+            "invenio_oauthclient.rest_signup", remote_app=remote_name, next="/someurl/"
+        )
     )
 
+    base_app.config["OAUTHCLIENT_REST_REMOTE_APPS"][remote_name][
+        "signup_handler"
+    ] = signup_handler
+
+
+@pytest.mark.parametrize("remote_name", REMOTE_APPS)
+def test_response_handler(remote_name, base_app):
+    """Test response handler."""
+
+    def mock_response_handler(remote, url, payload):
+        return remote.name
+
+    # Force usage of dummy handlers
+    base_app.config["OAUTHCLIENT_REST_REMOTE_APPS"][remote_name][
+        "response_handler"
+    ] = mock_response_handler
+
+    # Initialize InvenioOAuth
+    FlaskOAuth(base_app)
+    InvenioOAuthClientREST(base_app)
+    base_app.register_blueprint(rest_blueprint)
+
+    # Try to sign-up client
+    response = base_app.test_client().get(
+        url_for("invenio_oauthclient.rest_signup", remote_app=remote_name)
+    )
+    assert remote_name in str(response.data)
 
-@blueprint.route("/login/<remote_app>/")
-def login(remote_app):
-    """Send user to remote application for authentication."""
-    try:
-        return _login(remote_app, ".authorized")
-    except OAuthRemoteNotFound:
-        return abort(404)
-
-
-@rest_blueprint.route("/login/<remote_app>/")
-def rest_login(remote_app):
-    """Send user to remote application for authentication."""
-    try:
-        return _login(remote_app, ".rest_authorized")
-    except OAuthRemoteNotFound:
-        abort(404)
-
-
-def _authorized(remote_app=None):
-    """Authorized handler callback."""
-    if remote_app not in current_oauthclient.handlers:
-        return abort(404)
-
-    state_token = request.args.get("state")
-
-    # Verify state parameter
-    assert state_token
-    # Checks authenticity and integrity of state and decodes the value.
-    state = serializer.loads(state_token)
-    # Verify that state is for this session, app and that next parameter
-    # have not been modified.
-    assert state["sid"] == _create_identifier()
-    assert state["app"] == remote_app
-    # Store next URL
-    set_session_next_url(remote_app, state["next"])
-
-    handler = current_oauthclient.handlers[remote_app]()
-    return handler
-
-
-@blueprint.route("/authorized/<remote_app>/")
-def authorized(remote_app=None):
-    """Authorized handler callback."""
-    try:
-        return _authorized(remote_app)
-    except OAuthRemoteNotFound:
-        return abort(404)
-    except (AssertionError, BadData):
-        if current_app.config.get("OAUTHCLIENT_STATE_ENABLED", True) or (
-            not (current_app.debug or current_app.testing)
-        ):
-            abort(403)
-    except OAuthException as e:
-        if e.type == "invalid_response":
-            current_app.logger.warning(
-                "{message} ({data})".format(message=e.message, data=e.data)
-            )
-            abort(500)
-        else:
-            raise
-
-
-@rest_blueprint.route("/authorized/<remote_app>/")
-def rest_authorized(remote_app=None):
-    """Authorized handler callback."""
-    try:
-        return _authorized(remote_app)
-    except OAuthRemoteNotFound:
-        abort(404)
-    except (AssertionError, BadData) as e:
-        current_app.logger.error(str(e))
-        if current_app.config.get("OAUTHCLIENT_STATE_ENABLED", True) or (
-            not (current_app.debug or current_app.testing)
-        ):
-            return response_handler(
-                None,
-                current_app.config["OAUTHCLIENT_REST_DEFAULT_ERROR_REDIRECT_URL"],
-                payload=dict(message="Invalid state.", code=403),
-            )
-    except OAuthException as e:
-        current_app.logger.error(str(e))
-        if e.type == "invalid_response":
-            return response_handler(
-                None,
-                current_app.config["OAUTHCLIENT_REST_DEFAULT_ERROR_REDIRECT_URL"],
-                payload=dict(message="Invalid response.", code=500),
-            )
-        else:
-            raise
-
-
-def _signup(remote_app):
-    """Extra signup step."""
-    if remote_app not in current_oauthclient.signup_handlers:
-        raise OAuthRemoteNotFound()
-    return current_oauthclient.signup_handlers[remote_app]["view"]()
-
-
-@blueprint.route("/signup/<remote_app>/", methods=["GET", "POST"])
-def signup(remote_app):
-    """Extra signup step."""
-    try:
-        res = _signup(remote_app)
-        return abort(404) if res is None else res
-    except OAuthRemoteNotFound:
-        return abort(404)
-
-
-@rest_blueprint.route("/signup/<remote_app>/", methods=["GET", "POST"])
-def rest_signup(remote_app):
-    """Extra signup step."""
-    try:
-        res = _signup(remote_app)
-        return abort(404) if res is None else res
-    except OAuthRemoteNotFound:
-        abort(404)
-
-
-def _disconnect(remote_app):
-    """Extra signup step."""
-    if remote_app not in current_oauthclient.signup_handlers:
-        raise OAuthRemoteNotFound()
-    ret = current_oauthclient.disconnect_handlers[remote_app]()
-    db.session.commit()
-    return ret
-
-
-@blueprint.route("/disconnect/<remote_app>/")
-def disconnect(remote_app):
-    """Disconnect user from remote application.
-
-    Removes application as well as associated information.
-    """
-    try:
-        return _disconnect(remote_app)
-    except OAuthRemoteNotFound:
-        abort(404)
-
-
-@rest_blueprint.route("/disconnect/<remote_app>/")
-def rest_disconnect(remote_app):
-    """Disconnect user from remote application.
-
-    Removes application as well as associated information.
-    """
-    try:
-        return _disconnect(remote_app)
-    except OAuthRemoteNotFound:
-        abort(404)
-
-
-@blueprint.route("/logout")
-def post_logout():
-    """Client logout view.
-
-    This URL should be called by setting `SECURITY_POST_LOGOUT_VIEW = /oauth/logout`
-    """
-    remote_name = session.pop("OAUTHCLIENT_SESSION_REMOTE_NAME", None)
-    if remote_name:
-        logout_url = current_app.config["OAUTHCLIENT_REMOTE_APPS"][remote_name].get(
-            "logout_url"
-        )
-        if logout_url:
-            return redirect(logout_url, code=302)
 
-    return redirect("/")
+@pytest.mark.parametrize("remote", REMOTE_APPS, indirect=["remote"])
+def test_response_handler_with_postmessage(remote, base_app):
+    """Test response handler with postmessage."""
+
+    # Force usage of dummy handlers
+    base_app.config["OAUTHCLIENT_REST_REMOTE_APPS"][remote.name][
+        "response_handler"
+    ] = response_handler_postmessage
+
+    # Initialize InvenioOAuth
+    FlaskOAuth(base_app)
+    InvenioOAuthClientREST(base_app)
+    # The `rest_blueprint` is already registered indirectly by the
+    # `remote` fixture
+
+    datastore = base_app.extensions["invenio-accounts"].datastore
+    existing_email = "existing@inveniosoftware.org"
+    user = datastore.find_user(email=existing_email)
+    # Already authenticated
+    login_user(user)
+
+    assert current_user.is_authenticated
+
+    response = signup_handler(remote)
+    expected_message = "Successfully signed up."
+    expected_status = "200"
+
+    assert expected_message in response
+    assert expected_status in response
+    assert "window.opener.postMessage" in response
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient/views/settings.py` & `invenio-oauthclient-3.2.0/invenio_oauthclient/views/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Account settings blueprint for oauthclient."""
 
 from operator import itemgetter
 
-import six
 from flask import Blueprint, current_app, render_template, request
 from flask_breadcrumbs import register_breadcrumb
 from flask_login import current_user, login_required
 from flask_menu import register_menu
 from invenio_i18n import lazy_gettext as _
 from invenio_theme.proxies import current_theme_icons
 from speaklater import make_lazy_string
@@ -52,15 +51,15 @@
     """List linked accounts."""
     oauth = current_oauthclient.oauth
 
     services = []
     service_map = {}
     i = 0
 
-    for appid, conf in six.iteritems(current_app.config["OAUTHCLIENT_REMOTE_APPS"]):
+    for appid, conf in current_app.config["OAUTHCLIENT_REMOTE_APPS"].items():
         if not conf.get("hide", False):
             services.append(
                 dict(
                     appid=appid,
                     title=conf["title"],
                     icon=conf.get("icon", None),
                     description=conf.get("description", None),
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/PKG-INFO` & `invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-oauthclient
-Version: 3.1.2
+Version: 3.2.0
 Summary: "Invenio module that provides OAuth web authorization support."
 Home-page: https://github.com/inveniosoftware/invenio-oauthclient
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -56,14 +56,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.2.0 (released 2023-07-24)
+        
+        - authorize: refactor authorize/signup handlers
+        - update translations
+        
         Version 3.1.2 (released 2023-06-23)
         
         - client: preserve "next" URL param on login redirection
         
         Version 3.1.1 (released 2023-06-21)
         
         - client: fix user confirmation
```

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/entry_points.txt` & `invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/requires.txt` & `invenio-oauthclient-3.2.0/invenio_oauthclient.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/requirements-devel.txt` & `invenio-oauthclient-3.2.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/run-tests.sh` & `invenio-oauthclient-3.2.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/setup.cfg` & `invenio-oauthclient-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/tests/conftest.py` & `invenio-oauthclient-3.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/tests/data/keycloak_realm_info.json` & `invenio-oauthclient-3.2.0/tests/data/keycloak_realm_info.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/tests/data/keycloak_token_response.json` & `invenio-oauthclient-3.2.0/tests/data/keycloak_token_response.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/tests/data/oauth_response_content.json` & `invenio-oauthclient-3.2.0/tests/data/oauth_response_content.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/tests/data/orcid_bio.json` & `invenio-oauthclient-3.2.0/tests/data/orcid_bio.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/tests/helpers.py` & `invenio-oauthclient-3.2.0/tests/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """OAuth client test utility functions."""
 
 import json
 from inspect import isfunction
+from urllib.parse import parse_qs, urlencode, urlparse
 
 import httpretty
-import six
 from mock import MagicMock
-from six.moves.urllib_parse import parse_qs, urlencode, urlparse
 
 from invenio_oauthclient._compat import _create_identifier
 from invenio_oauthclient.views.client import serializer
 
 
 def get_state(app="test"):
     """Get state."""
@@ -40,15 +39,15 @@
     """Mock the oauth remote get response."""
     oauth.remote_apps[remote_app].get = MagicMock(return_value=data)
 
 
 def check_redirect_location(resp, loc):
     """Check response redirect location."""
     assert resp._status_code == 302
-    if isinstance(loc, six.string_types):
+    if isinstance(loc, str):
         assert resp.headers["Location"] == loc
     elif isfunction(loc):
         assert loc(resp.headers["Location"])
 
 
 def check_response_redirect_url(response, expected_url):
     """Check response redirect url."""
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_admin.py` & `invenio-oauthclient-3.2.0/tests/test_admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # This file is part of Invenio.
 # Copyright (C) 2016-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Views for OAuth."""
+
 from flask import url_for
 from flask_admin import Admin
 from invenio_db import db
 
 from invenio_oauthclient import InvenioOAuthClient
 from invenio_oauthclient.admin import (
     remote_account_adminview,
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_app.py` & `invenio-oauthclient-3.2.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/tests/test_base_handlers.py` & `invenio-oauthclient-3.2.0/tests/test_base_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """Test handlers."""
 
 import pytest
 
 from invenio_oauthclient.errors import OAuthResponseError
 from invenio_oauthclient.handlers import response_token_setter, token_getter
 from invenio_oauthclient.models import RemoteToken
-from invenio_oauthclient.utils import oauth_authenticate
+from invenio_oauthclient.oauth import oauth_authenticate
 
 
 def test_token_setter(app, remote):
     """Test token setter on response from OAuth server."""
 
     # OAuth1
     resp_oauth1 = {
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_contrib_cern_openid.py` & `invenio-oauthclient-3.2.0/tests/test_contrib_cern_openid.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test case for CERN oauth remote app."""
 
 import os
+from urllib.parse import parse_qs, urlparse
 
 import pytest
 from flask import g, session, url_for
 from flask_security import login_user, logout_user
 from flask_security.utils import hash_password
 from helpers import get_state, mock_remote_get, mock_response
-from six.moves.urllib_parse import parse_qs, urlparse
 
 from invenio_oauthclient.contrib.cern_openid import (
     OAUTHCLIENT_CERN_OPENID_SESSION_KEY,
     account_info,
     disconnect_handler,
     fetch_extra_data,
     get_dict_from_response,
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_contrib_cern_openid_rest.py` & `invenio-oauthclient-3.2.0/tests/test_contrib_cern_openid_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test case for CERN oauth remote app_rest."""
 
 import os
 from datetime import timedelta
+from urllib.parse import parse_qs, urlparse
 
 import pytest
 from flask import current_app, g, session, url_for
 from flask_login import current_user
 from flask_security import login_user, logout_user
 from flask_security.utils import hash_password
 from helpers import (
     check_response_redirect_url_args,
     get_state,
     mock_remote_get,
     mock_response,
 )
-from six.moves.urllib_parse import parse_qs, urlparse
 
 from invenio_oauthclient.contrib.cern_openid import (
     OAUTHCLIENT_CERN_OPENID_SESSION_KEY,
     account_info_rest,
     disconnect_rest_handler,
     fetch_extra_data,
     get_dict_from_response,
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_contrib_github.py` & `invenio-oauthclient-3.2.0/tests/test_contrib_github.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test case for github oauth remote app."""
 
 from collections import namedtuple
+from urllib.parse import parse_qs, urlparse
 
 import mock
 import pytest
 from flask import session, url_for
 from flask_login import current_user
 from flask_security import login_user
 from flask_security.utils import hash_password
 from helpers import check_redirect_location, mock_response
 from invenio_accounts.models import User
 from invenio_db import db
-from six.moves.urllib_parse import parse_qs, urlparse
 
 from invenio_oauthclient._compat import _create_identifier
 from invenio_oauthclient.contrib.github import authorized
 from invenio_oauthclient.errors import OAuthResponseError
 from invenio_oauthclient.models import RemoteAccount, RemoteToken, UserIdentity
 from invenio_oauthclient.views.client import serializer
 
@@ -118,19 +118,19 @@
             assert (
                 1
                 == UserIdentity.query.filter_by(
                     method="github", id_user=user.id, id="githubuser"
                 ).count()
             )
 
-            # set a password for the user
+            # set a local password for the user
             user.password = hash_password("1234")
             db.session.commit()
 
-            # Disconnect again
+            # Disconnect again, it works because the user can login with local psw
             resp = c.get(url_for("invenio_oauthclient.disconnect", remote_app="github"))
             assert resp.status_code == 302
 
             user = User.query.filter_by(email=example_email).one()
             assert (
                 0
                 == UserIdentity.query.filter_by(
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_contrib_github_rest.py` & `invenio-oauthclient-3.2.0/tests/test_contrib_github_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test case for github oauth remote app."""
 
 from collections import namedtuple
+from urllib.parse import parse_qs, urlparse
 
 import mock
 import pytest
 from flask import url_for
 from flask_login import current_user
 from flask_security import login_user
 from flask_security.utils import hash_password
 from helpers import (
     check_redirect_location,
     check_response_redirect_url_args,
     mock_response,
 )
 from invenio_accounts.models import User
 from invenio_db import db
-from six.moves.urllib_parse import parse_qs, urlparse
 
 from invenio_oauthclient import current_oauthclient
 from invenio_oauthclient._compat import _create_identifier
 from invenio_oauthclient.contrib.github import authorized_rest
 from invenio_oauthclient.errors import OAuthResponseError
 from invenio_oauthclient.models import RemoteAccount, RemoteToken, UserIdentity
 from invenio_oauthclient.views.client import serializer
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_contrib_globus.py` & `invenio-oauthclient-3.2.0/tests/test_contrib_globus.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test case for globus oauth remote app."""
 
 import json
+from urllib.parse import parse_qs, urlparse
 
 import pytest
 from flask import session, url_for
 from flask_login import current_user
 from flask_oauthlib.client import OAuthResponse
 from flask_security import login_user
 from flask_security.utils import hash_password
 from helpers import mock_remote_get, mock_response
 from invenio_accounts.models import User
 from invenio_db import db
-from six.moves.urllib_parse import parse_qs, urlparse
 
 from invenio_oauthclient._compat import _create_identifier
 from invenio_oauthclient.errors import OAuthResponseError
 from invenio_oauthclient.models import RemoteAccount, RemoteToken, UserIdentity
 from invenio_oauthclient.views.client import serializer
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_contrib_keycloak.py` & `invenio-oauthclient-3.2.0/tests/test_contrib_keycloak.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 # Copyright (C) 2020-2021 TU Wien.
 #
 # Invenio-Keycloak is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Tests for the Keycloak OAuth remote_app."""
 
+from urllib.parse import parse_qs, urlparse
+
 import httpretty
 import jwt
 import pytest
 from flask import session, url_for
 from flask_login import current_user, login_user
 from flask_security.utils import hash_password
 from helpers import get_state, mock_keycloak
 from invenio_accounts.models import User
 from invenio_db import db
-from six.moves.urllib_parse import parse_qs, urlparse
 
 from invenio_oauthclient.contrib.keycloak.helpers import (
     _format_public_key,
     get_user_info,
 )
 from invenio_oauthclient.errors import OAuthError
 from invenio_oauthclient.models import UserIdentity
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_contrib_orcid.py` & `invenio-oauthclient-3.2.0/tests/test_contrib_orcid.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test case for ORCID oauth remote app."""
 
+from urllib.parse import parse_qs, urlparse
+
 import httpretty
 from flask import session, url_for
 from flask_login import current_user
 from flask_security import login_user
 from flask_security.utils import hash_password
 from helpers import get_state, mock_response
 from invenio_accounts.models import User
 from invenio_db import db
-from six.moves.urllib_parse import parse_qs, urlparse
 
 from invenio_oauthclient.contrib.orcid import account_info
 from invenio_oauthclient.handlers import token_session_key
 from invenio_oauthclient.models import RemoteAccount, RemoteToken, UserIdentity
 
 
 def test_account_info(app, example_orcid):
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_contrib_orcid_rest.py` & `invenio-oauthclient-3.2.0/tests/test_contrib_orcid_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test case for ORCID oauth remote app."""
 
+from urllib.parse import parse_qs, urlparse
+
 import httpretty
 from flask import session, url_for
 from flask_login import current_user
 from flask_security import login_user
 from flask_security.utils import hash_password
 from helpers import check_response_redirect_url_args, get_state, mock_response
 from invenio_accounts.models import User
 from invenio_db import db
-from six.moves.urllib_parse import parse_qs, urlparse
 
 from invenio_oauthclient.contrib.orcid import account_info
 from invenio_oauthclient.handlers import token_session_key
 from invenio_oauthclient.models import RemoteAccount, RemoteToken, UserIdentity
 
 
 def test_account_info(app_rest, example_orcid):
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_examples_app.py` & `invenio-oauthclient-3.2.0/tests/test_examples_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/tests/test_models.py` & `invenio-oauthclient-3.2.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.2/tests/test_utils.py` & `invenio-oauthclient-3.2.0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,36 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test utils."""
 
 import sys
+from urllib.parse import quote_plus
 
 import pytest
 from flask_security.confirmable import _security
 from invenio_db import db
-from six.moves.urllib.parse import quote_plus
 
 from invenio_oauthclient.errors import AlreadyLinkedError
 from invenio_oauthclient.models import RemoteAccount, RemoteToken
+from invenio_oauthclient.oauth import (
+    _get_external_id,
+    oauth_authenticate,
+    oauth_get_user,
+    oauth_link_external_id,
+    oauth_unlink_external_id,
+)
 from invenio_oauthclient.proxies import current_oauthclient
 from invenio_oauthclient.utils import (
-    _get_external_id,
     create_csrf_disabled_registrationform,
     create_registrationform,
     fill_form,
     filter_user_info,
     get_safe_redirect_target,
-    oauth_authenticate,
-    oauth_get_user,
-    oauth_link_external_id,
-    oauth_unlink_external_id,
     obj_or_import_string,
     patch_dictionary,
     rebuild_access_tokens,
 )
 
 
 def test_utilities(app, models_fixture):
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_views.py` & `invenio-oauthclient-3.2.0/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test case for views."""
 
 import time
+from urllib.parse import parse_qs, urlparse
 
 import pytest
 from flask import url_for
 from flask_oauthlib.client import OAuth as FlaskOAuth
 from flask_security import login_user
 from helpers import check_response_redirect_url
 from invenio_accounts.testutils import login_user_via_session
 from invenio_db import db
 from itsdangerous import TimedJSONWebSignatureSerializer
 from mock import MagicMock
 from simplejson import JSONDecodeError
-from six.moves.urllib_parse import parse_qs, urlparse
 
 from invenio_oauthclient import InvenioOAuthClient
 from invenio_oauthclient._compat import _create_identifier
 from invenio_oauthclient.handlers import token_getter
 from invenio_oauthclient.models import RemoteAccount, RemoteToken
 from invenio_oauthclient.views.client import blueprint as blueprint_client
 from invenio_oauthclient.views.client import serializer
```

### Comparing `invenio-oauthclient-3.1.2/tests/test_views_rest.py` & `invenio-oauthclient-3.2.0/tests/test_views_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test case for views."""
 
 import time
+from urllib.parse import parse_qs, urlparse
 
 import pytest
 from flask import url_for
 from flask_oauthlib.client import OAuth as FlaskOAuth
 from helpers import check_response_redirect_url, check_response_redirect_url_args
 from invenio_accounts.testutils import login_user_via_session
 from invenio_db import db
 from itsdangerous import TimedJSONWebSignatureSerializer
 from mock import MagicMock
 from simplejson import JSONDecodeError
-from six.moves.urllib_parse import parse_qs, urlparse
 
 from invenio_oauthclient import InvenioOAuthClientREST
 from invenio_oauthclient._compat import _create_identifier
 from invenio_oauthclient.handlers import token_getter
 from invenio_oauthclient.models import RemoteToken
 from invenio_oauthclient.views.client import rest_blueprint, serializer
```

