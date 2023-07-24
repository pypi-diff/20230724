# Comparing `tmp/invenio-banners-2.1.0.tar.gz` & `tmp/invenio-banners-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-banners-2.1.0.tar", last modified: Thu Mar  2 19:47:54 2023, max compression
+gzip compressed data, was "dist/invenio-banners-2.1.1.tar", last modified: Mon Jul 24 14:16:36 2023, max compression
```

## Comparing `invenio-banners-2.1.0.tar` & `invenio-banners-2.1.1.tar`

### file list

```diff
@@ -1,90 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/administration/banners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/alembic/5e02314da32e_create_invenio_banners_db_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/alembic/e40d93d99040_create_invenio_banners_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners/records/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/resources/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners/services/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/services/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/services/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/services/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners/templates/semantic-ui/invenio_banners/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/templates/semantic-ui/invenio_banners/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/invenio_banners/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/invenio_banners.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/tests/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/tests/records/test_disable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/tests/records/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/tests/resources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/tests/resources/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 19:47:54.000000 invenio-banners-2.1.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/tests/services/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/tests/services/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/tests/test_invenio_banners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-02 19:47:51.000000 invenio-banners-2.1.0/tests/test_macro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/.tx/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/administration/banners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/alembic/5e02314da32e_create_invenio_banners_db_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/alembic/e40d93d99040_create_invenio_banners_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/resources/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/services/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/services/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners/templates/semantic-ui/invenio_banners/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/templates/semantic-ui/invenio_banners/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/invenio_banners/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/invenio_banners.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/tests/records/test_disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/tests/records/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/tests/resources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/tests/resources/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:36.000000 invenio-banners-2.1.1/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/tests/services/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/tests/services/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/tests/test_invenio_banners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-24 14:16:26.000000 invenio-banners-2.1.1/tests/test_macro.py
```

### Comparing `invenio-banners-2.1.0/.editorconfig` & `invenio-banners-2.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/.github/workflows/pypi-publish.yml` & `invenio-banners-2.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/.github/workflows/tests.yml` & `invenio-banners-2.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/CHANGES.rst` & `invenio-banners-2.1.1/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
     Invenio-Banners is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.1.1 (released 2023-07-24)
+
+- ui: remove bottom margin
+
 Version 2.1.0 (released 2023-03-02)
 
 - remove deprecated flask-babelex imports
 - install invenio-i18n explicitly
 
 Version 2.0.0 (released 2023-02-15)
```

### Comparing `invenio-banners-2.1.0/CONTRIBUTING.rst` & `invenio-banners-2.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/LICENSE` & `invenio-banners-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/MANIFEST.in` & `invenio-banners-2.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/PKG-INFO` & `invenio-banners-2.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-banners
-Version: 2.1.0
+Version: 2.1.1
 Summary: Invenio-Banners is a module used to create and show banners with useful messages to users.
 Home-page: https://github.com/inveniosoftware/invenio-banners
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -41,14 +41,18 @@
         
             Invenio-Banners is free software; you can redistribute it and/or modify
             it under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.1 (released 2023-07-24)
+        
+        - ui: remove bottom margin
+        
         Version 2.1.0 (released 2023-03-02)
         
         - remove deprecated flask-babelex imports
         - install invenio-i18n explicitly
         
         Version 2.0.0 (released 2023-02-15)
```

### Comparing `invenio-banners-2.1.0/README.rst` & `invenio-banners-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/docs/Makefile` & `invenio-banners-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/docs/conf.py` & `invenio-banners-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/docs/index.rst` & `invenio-banners-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/docs/make.bat` & `invenio-banners-2.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/administration/banners.py` & `invenio-banners-2.1.1/invenio_banners/administration/banners.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/alembic/5e02314da32e_create_invenio_banners_db_table.py` & `invenio-banners-2.1.1/invenio_banners/alembic/5e02314da32e_create_invenio_banners_db_table.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/alembic/e40d93d99040_create_invenio_banners_branch.py` & `invenio-banners-2.1.1/invenio_banners/alembic/e40d93d99040_create_invenio_banners_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/config.py` & `invenio-banners-2.1.1/invenio_banners/config.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/ext.py` & `invenio-banners-2.1.1/invenio_banners/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/proxies.py` & `invenio-banners-2.1.1/invenio_banners/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/records/models.py` & `invenio-banners-2.1.1/invenio_banners/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/resources/config.py` & `invenio-banners-2.1.1/invenio_banners/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/resources/errors.py` & `invenio-banners-2.1.1/invenio_banners/resources/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/resources/resource.py` & `invenio-banners-2.1.1/invenio_banners/resources/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/services/config.py` & `invenio-banners-2.1.1/invenio_banners/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/services/errors.py` & `invenio-banners-2.1.1/invenio_banners/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/services/permissions.py` & `invenio-banners-2.1.1/invenio_banners/services/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/services/results.py` & `invenio-banners-2.1.1/invenio_banners/services/results.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/services/schemas.py` & `invenio-banners-2.1.1/invenio_banners/services/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/services/service.py` & `invenio-banners-2.1.1/invenio_banners/services/service.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/templates/semantic-ui/invenio_banners/banner.html` & `invenio-banners-2.1.1/invenio_banners/templates/semantic-ui/invenio_banners/banner.html`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/invenio_banners/utils.py` & `invenio-banners-2.1.1/invenio_banners/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """Get active banner for the current URL path request."""
     url_path = request.path
     return BannerModel.get_active(url_path)
 
 
 def style_category(category):
     """Return predefined Semantic-UI classes for each banner category."""
-    style_class = "ui {} flashed top attached manage mb-0 message"
+    style_class = "ui {} flashed top attached manage m-0 message"
     if category == "warning":
         style_class = style_class.format("warning")
     elif category == "other":
         style_class = style_class.format("grey")
     else:
         style_class = style_class.format("info")
     return style_class
```

### Comparing `invenio-banners-2.1.0/invenio_banners.egg-info/PKG-INFO` & `invenio-banners-2.1.1/invenio_banners.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-banners
-Version: 2.1.0
+Version: 2.1.1
 Summary: Invenio-Banners is a module used to create and show banners with useful messages to users.
 Home-page: https://github.com/inveniosoftware/invenio-banners
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -41,14 +41,18 @@
         
             Invenio-Banners is free software; you can redistribute it and/or modify
             it under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.1 (released 2023-07-24)
+        
+        - ui: remove bottom margin
+        
         Version 2.1.0 (released 2023-03-02)
         
         - remove deprecated flask-babelex imports
         - install invenio-i18n explicitly
         
         Version 2.0.0 (released 2023-02-15)
```

### Comparing `invenio-banners-2.1.0/invenio_banners.egg-info/SOURCES.txt` & `invenio-banners-2.1.1/invenio_banners.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 README.rst
 babel.ini
 pyproject.toml
 requirements-devel.txt
 run-tests.sh
 setup.cfg
 setup.py
+.github/workflows/i18n-pull.yml
+.github/workflows/i18n-push.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/tests.yml
+.tx/config
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changes.rst
 docs/conf.py
 docs/configuration.rst
 docs/contributing.rst
```

### Comparing `invenio-banners-2.1.0/invenio_banners.egg-info/entry_points.txt` & `invenio-banners-2.1.1/invenio_banners.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/run-tests.sh` & `invenio-banners-2.1.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/setup.cfg` & `invenio-banners-2.1.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -53,14 +53,33 @@
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
 universal = 1
 
+[compile_catalog]
+directory = invenio_banners/translations/
+use-fuzzy = True
+
+[extract_messages]
+copyright_holder = CERN
+msgid_bugs_address = info@inveniosoftware.org
+mapping-file = babel.ini
+output-file = invenio_banners/translations/messages.pot
+add-comments = NOTE
+
+[init_catalog]
+input-file = invenio_banners/translations/messages.pot
+output-dir = invenio_banners/translations/
+
+[update_catalog]
+input-file = invenio_banners/translations/messages.pot
+output-dir = invenio_banners/translations/
+
 [pydocstyle]
 add_ignore = D401
 
 [isort]
 profile = black
 
 [tool:pytest]
```

### Comparing `invenio-banners-2.1.0/tests/conftest.py` & `invenio-banners-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/tests/records/test_disable.py` & `invenio-banners-2.1.1/tests/records/test_disable.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/tests/records/test_models.py` & `invenio-banners-2.1.1/tests/records/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/tests/resources/conftest.py` & `invenio-banners-2.1.1/tests/resources/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/tests/resources/test_resources.py` & `invenio-banners-2.1.1/tests/resources/test_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/tests/services/conftest.py` & `invenio-banners-2.1.1/tests/services/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/tests/services/test_services.py` & `invenio-banners-2.1.1/tests/services/test_services.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/tests/test_invenio_banners.py` & `invenio-banners-2.1.1/tests/test_invenio_banners.py`

 * *Files identical despite different names*

### Comparing `invenio-banners-2.1.0/tests/test_macro.py` & `invenio-banners-2.1.1/tests/test_macro.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,27 +47,27 @@
     html = template.render()
     one_line = html.replace("\n", "").replace(" ", "")
     assert one_line == "<html><body></body></html>"
 
     # add one banner
     EXPECTED_MSG = "Test banner info message"
     EXPECTED_CATEGORY = "info"
-    EXPECTED_STYLE = "ui info flashed top attached manage mb-0 message"
+    EXPECTED_STYLE = "ui info flashed top attached manage m-0 message"
     banner = _create_banner(EXPECTED_MSG, EXPECTED_CATEGORY)
     style = style_category(banner.category)
 
     html = template.render()
     assert EXPECTED_MSG in html
     assert style.endswith(EXPECTED_STYLE)
     assert style in html
 
     # change message and category
     EXPECTED_MSG = "Test banner warning message"
     EXPECTED_CATEGORY = "warning"
-    EXPECTED_STYLE = "ui warning flashed top attached manage mb-0 message"
+    EXPECTED_STYLE = "ui warning flashed top attached manage m-0 message"
 
     banner.message = EXPECTED_MSG
     banner.category = EXPECTED_CATEGORY
     db.session.commit()
 
     style = style_category(banner.category)
```

