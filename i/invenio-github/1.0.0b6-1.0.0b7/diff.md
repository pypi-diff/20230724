# Comparing `tmp/invenio-github-1.0.0b6.tar.gz` & `tmp/invenio-github-1.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-github-1.0.0b6.tar", last modified: Fri Jul 21 16:11:38 2023, max compression
+gzip compressed data, was "dist/invenio-github-1.0.0b7.tar", last modified: Mon Jul 24 09:24:01 2023, max compression
```

## Comparing `invenio-github-1.0.0b6.tar` & `invenio-github-1.0.0b7.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      973 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2509 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/.lgtm
--rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/RELEASE-NOTES.rst
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/babel.ini
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10770 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/alembic/5a5428312b2b_create_github_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/alembic/b0eaee37b545_create_github_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)    23408 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/assets/semantic-ui/js/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     3388 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/assets/semantic-ui/js/invenio_github/index.js
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/oauth/
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/oauth/handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/oauth/remote_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/receivers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/helpers.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (122)     6538 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
--rw-r--r--   0 runner    (1001) docker     (122)    15814 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/views/
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/views/badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     8272 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/views/github.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      347 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/run-i18n-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2509 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/.lgtm
+-rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5058 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/RELEASE-NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10770 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/alembic/5a5428312b2b_create_github_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/alembic/b0eaee37b545_create_github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23408 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/assets/semantic-ui/js/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     3388 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/assets/semantic-ui/js/invenio_github/index.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/oauth/
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/oauth/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/oauth/remote_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/helpers.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6538 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
+-rw-r--r--   0 runner    (1001) docker     (122)    15814 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/views/badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8272 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/views/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5058 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      347 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/setup.py
```

### Comparing `invenio-github-1.0.0b6/.github/workflows/pypi-publish.yml` & `invenio-github-1.0.0b7/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/.github/workflows/tests.yml` & `invenio-github-1.0.0b7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/.travis.yml` & `invenio-github-1.0.0b7/.travis.yml`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/AUTHORS.rst` & `invenio-github-1.0.0b7/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/CHANGES.rst` & `invenio-github-1.0.0b7/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
 Changes
 =======
 
+Version v1.0.0b7 (released 2023-07-24)
+
+- handlers: fix oauthclient import
+
 Version v1.0.0b6 (released 2023-07-21)
 
 - add github badges
 
 Version v1.0.0b5 (released 2023-07-17)
 
 - setup: enable tests
```

### Comparing `invenio-github-1.0.0b6/CONTRIBUTING.rst` & `invenio-github-1.0.0b7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/LICENSE` & `invenio-github-1.0.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/MANIFEST.in` & `invenio-github-1.0.0b7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/PKG-INFO` & `invenio-github-1.0.0b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,18 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.0b7 (released 2023-07-24)
+        
+        - handlers: fix oauthclient import
+        
         Version v1.0.0b6 (released 2023-07-21)
         
         - add github badges
         
         Version v1.0.0b5 (released 2023-07-17)
         
         - setup: enable tests
```

### Comparing `invenio-github-1.0.0b6/README.rst` & `invenio-github-1.0.0b7/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/RELEASE-NOTES.rst` & `invenio-github-1.0.0b7/RELEASE-NOTES.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/Makefile` & `invenio-github-1.0.0b7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/api.rst` & `invenio-github-1.0.0b7/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/authors.rst` & `invenio-github-1.0.0b7/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/changes.rst` & `invenio-github-1.0.0b7/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/conf.py` & `invenio-github-1.0.0b7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/contributing.rst` & `invenio-github-1.0.0b7/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/index.rst` & `invenio-github-1.0.0b7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/installation.rst` & `invenio-github-1.0.0b7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/license.rst` & `invenio-github-1.0.0b7/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/make.bat` & `invenio-github-1.0.0b7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/docs/usage.rst` & `invenio-github-1.0.0b7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/__init__.py` & `invenio-github-1.0.0b7/invenio_github/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
 from .ext import InvenioGitHub
 
-__version__ = "1.0.0b6"
+__version__ = "1.0.0b7"
 
 __all__ = ("__version__", "InvenioGitHub")
```

### Comparing `invenio-github-1.0.0b6/invenio_github/alembic/5a5428312b2b_create_github_branch.py` & `invenio-github-1.0.0b7/invenio_github/alembic/5a5428312b2b_create_github_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/alembic/b0eaee37b545_create_github_tables.py` & `invenio-github-1.0.0b7/invenio_github/alembic/b0eaee37b545_create_github_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/api.py` & `invenio-github-1.0.0b7/invenio_github/api.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/assets/semantic-ui/js/invenio_github/index.js` & `invenio-github-1.0.0b7/invenio_github/assets/semantic-ui/js/invenio_github/index.js`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/config.py` & `invenio-github-1.0.0b7/invenio_github/config.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/errors.py` & `invenio-github-1.0.0b7/invenio_github/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/ext.py` & `invenio-github-1.0.0b7/invenio_github/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/models.py` & `invenio-github-1.0.0b7/invenio_github/models.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/oauth/handlers.py` & `invenio-github-1.0.0b7/invenio_github/oauth/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 """Implement OAuth client handler."""
 
 from flask import current_app, redirect, url_for
 from flask_login import current_user
 from invenio_db import db
 from invenio_oauth2server.models import Token as ProviderToken
-from invenio_oauthclient.utils import oauth_unlink_external_id
+from invenio_oauthclient import oauth_unlink_external_id
 
 from invenio_github.api import GitHubAPI
 from invenio_github.tasks import disconnect_github
 
 
 def account_setup_handler(remote, token, resp):
     """Perform post initialization."""
```

### Comparing `invenio-github-1.0.0b6/invenio_github/oauth/remote_app.py` & `invenio-github-1.0.0b7/invenio_github/oauth/remote_app.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/proxies.py` & `invenio-github-1.0.0b7/invenio_github/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/receivers.py` & `invenio-github-1.0.0b7/invenio_github/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/tasks.py` & `invenio-github-1.0.0b7/invenio_github/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/helpers.html` & `invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html` & `invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/index.html` & `invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html` & `invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/view.html` & `invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/view.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/translations/cs/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b7/invenio_github/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/translations/da/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b7/invenio_github/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/translations/de/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b7/invenio_github/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/translations/en/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b7/invenio_github/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/translations/es/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b7/invenio_github/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/translations/fr/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b7/invenio_github/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/translations/it/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b7/invenio_github/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/translations/messages.pot` & `invenio-github-1.0.0b7/invenio_github/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/utils.py` & `invenio-github-1.0.0b7/invenio_github/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/views/__init__.py` & `invenio-github-1.0.0b7/invenio_github/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/views/badge.py` & `invenio-github-1.0.0b7/invenio_github/views/badge.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/views/github.py` & `invenio-github-1.0.0b7/invenio_github/views/github.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github/webpack.py` & `invenio-github-1.0.0b7/invenio_github/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github.egg-info/PKG-INFO` & `invenio-github-1.0.0b7/invenio_github.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,18 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.0b7 (released 2023-07-24)
+        
+        - handlers: fix oauthclient import
+        
         Version v1.0.0b6 (released 2023-07-21)
         
         - add github badges
         
         Version v1.0.0b5 (released 2023-07-17)
         
         - setup: enable tests
```

### Comparing `invenio-github-1.0.0b6/invenio_github.egg-info/SOURCES.txt` & `invenio-github-1.0.0b7/invenio_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github.egg-info/entry_points.txt` & `invenio-github-1.0.0b7/invenio_github.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/invenio_github.egg-info/requires.txt` & `invenio-github-1.0.0b7/invenio_github.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/requirements-devel.txt` & `invenio-github-1.0.0b7/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/run-tests.sh` & `invenio-github-1.0.0b7/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/setup.cfg` & `invenio-github-1.0.0b7/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b6/setup.py` & `invenio-github-1.0.0b7/setup.py`

 * *Files identical despite different names*

