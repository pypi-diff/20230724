# Comparing `tmp/invenio-cli-1.0.9.tar.gz` & `tmp/invenio-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-cli-1.0.9.tar", last modified: Fri Oct 21 16:02:27 2022, max compression
+gzip compressed data, was "dist/invenio-cli-1.1.0.tar", last modified: Mon Jul 24 13:22:05 2023, max compression
```

## Comparing `invenio-cli-1.0.9.tar` & `invenio-cli-1.1.0.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5252 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2525 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7429 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10043 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6991 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli/
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2858 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/assets.py
--rw-r--r--   0 runner    (1001) docker     (121)     6098 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4885 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5876 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/assets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     8650 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3374 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     6226 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/local.py
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     9122 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)    11617 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/services_health.py
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/steps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2401 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6619 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3572 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/cookiecutter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/docker_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/env.py
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/process.py
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/rdm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5252 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      837 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1727 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     8006 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)    11814 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/test_local.py
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/test_requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/test_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/tests/commands/testpkg/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/testpkg/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/helpers/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/helpers/test_cookiecutter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/helpers/test_dockerhelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/helpers/test_env.py
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/helpers/test_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/invenio_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/invenio_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/cli/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/cli/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/cli/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/cli/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/cli/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/invenio_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/services_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/commands/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/invenio_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/helpers/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/helpers/cookiecutter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/helpers/docker_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/helpers/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/helpers/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/helpers/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/invenio_cli/helpers/rdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/invenio_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-24 13:22:04.000000 invenio-cli-1.1.0/invenio_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/invenio_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:04.000000 invenio-cli-1.1.0/invenio_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 13:22:04.000000 invenio-cli-1.1.0/invenio_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:04.000000 invenio-cli-1.1.0/invenio_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 13:22:04.000000 invenio-cli-1.1.0/invenio_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 13:22:04.000000 invenio-cli-1.1.0/invenio_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/commands/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1727 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/commands/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/commands/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/commands/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/commands/test_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/commands/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/tests/commands/testpkg/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/commands/testpkg/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:05.000000 invenio-cli-1.1.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/helpers/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/helpers/test_cookiecutter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/helpers/test_dockerhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/helpers/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/helpers/test_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-24 13:21:51.000000 invenio-cli-1.1.0/tests/test_cli.py
```

### Comparing `invenio-cli-1.0.9/.editorconfig` & `invenio-cli-1.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/CONTRIBUTING.rst` & `invenio-cli-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/LICENSE` & `invenio-cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/MANIFEST.in` & `invenio-cli-1.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/PKG-INFO` & `invenio-cli-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-cli
-Version: 1.0.9
+Version: 1.1.0
 Summary: "Invenio module to ease the creation and management of applications."
 Home-page: https://github.com/inveniosoftware/invenio-cli
 Author: CERN & Northwestern University
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019-2020 CERN.
@@ -99,23 +99,72 @@
         
             # Get more help
             $ invenio-cli --help
         
         Further documentation is available on https://invenio-cli.readthedocs.io/
         
         ..
-            Copyright (C) 2019-2021 CERN.
+            Copyright (C) 2019-2023 CERN.
             Copyright (C) 2019-2021 Northwestern University.
         
             Invenio-Cli is free software; you can redistribute it and/or modify
             it under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.1.0 (released 2023-07-24)
+        
+        - add compatibility for docker compose v2
+        - consider command errors when using install command and fail
+        
+        Version 1.0.21 (released 2023-05-18)
+        
+        - deps: support docker < 7 for compatibility with urllib3 v2
+        
+        Version 1.0.20 (released 2023-03-134)
+        
+        - setup: add queues initialisation to steps
+        
+        Version 1.0.19 (released 2023-03-10)
+        
+        - global: remove fail message on warning (i.e. soft failures)
+        
+        Version 1.0.18 (released 2023-02-07)
+        
+        - containerize: fix translation commands instance path
+        
+        Version 1.0.17 (released 2023-01-30)
+        
+        - requirements: check node version depending on app-rdm version
+        
+        Version 1.0.16 (released 2023-01-30)
+        
+        - bump cookiecutter to v11.0
+        
+        Version 1.0.15 (released 2023-01-13)
+        
+        - Setup: fix empty translation folder failing
+        
+        Version 1.0.14 (released 2023-01-09)
+        
+        - Add app-rdm fixtures to setup
+        
+        Version 1.0.13 (released 2022-11-14)
+        
+        - Allow compilation command to fail in case of missing catalogs.
+        
+        Version 1.0.12 (released 2022-10-28)
+        
+        - Adds support for translations (i18n) management commands.
+        
+        Version 1.0.11 (released 2022-10-24)
+        
+        - Add support for InvenioILS
+        
         Version 1.0.8 (released 2022-10-13)
         
         - Fix issue when checking for services to be up
           and running correctly.
         
         Version 1.0.7 (released 2022-10-10)
```

### Comparing `invenio-cli-1.0.9/README.rst` & `invenio-cli-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/docs/Makefile` & `invenio-cli-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/docs/conf.py` & `invenio-cli-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/docs/index.rst` & `invenio-cli-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/docs/make.bat` & `invenio-cli-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/cli/assets.py` & `invenio-cli-1.1.0/invenio_cli/cli/assets.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/cli/cli.py` & `invenio-cli-1.1.0/invenio_cli/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from ..helpers.cli_config import CLIConfig
 from ..helpers.cookiecutter_wrapper import CookiecutterWrapper
 from .assets import assets
 from .containers import containers
 from .install import install
 from .packages import packages
 from .services import services
+from .translations import translations
 from .utils import handle_process_response, pass_cli_config, run_steps
 
 
 @click.group()
 @click.version_option()
 @click.pass_context
 def invenio_cli(ctx):
@@ -40,14 +41,15 @@
 
 
 invenio_cli.add_command(assets)
 invenio_cli.add_command(containers)
 invenio_cli.add_command(install)
 invenio_cli.add_command(packages)
 invenio_cli.add_command(services)
+invenio_cli.add_command(translations)
 
 
 @invenio_cli.command("check-requirements")
 @click.option(
     "--development",
     "-d",
     default=False,
@@ -82,15 +84,15 @@
     """Python shell command."""
     Commands.pyshell(debug=debug)
 
 
 @invenio_cli.command()
 @click.argument(
     "flavour",
-    type=click.Choice(["RDM"], case_sensitive=False),
+    type=click.Choice(["RDM", "ILS"], case_sensitive=False),
     default="RDM",
     required=False,
 )
 @click.option(
     "-t", "--template", required=False, help="Cookiecutter path or git url to template"
 )
 @click.option(
@@ -122,15 +124,15 @@
     }
     cookiecutter_wrapper = CookiecutterWrapper(flavour, **cookiecutter_kwargs)
 
     try:
         click.secho("Running cookiecutter...", fg="green")
         project_dir = cookiecutter_wrapper.cookiecutter()
 
-        click.secho("Writing invenio-invenio_cli config file...", fg="green")
+        click.secho("Writing invenio-cli config files...", fg="green")
         saved_replay = cookiecutter_wrapper.get_replay()
         CLIConfig.write(project_dir, flavour, saved_replay)
 
         click.secho("Creating logs directory...", fg="green")
         os.mkdir(Path(project_dir) / "logs")
 
     except Exception as e:
```

### Comparing `invenio-cli-1.0.9/invenio_cli/cli/containers.py` & `invenio-cli-1.1.0/invenio_cli/cli/containers.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/cli/install.py` & `invenio-cli-1.1.0/invenio_cli/cli/install.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/cli/packages.py` & `invenio-cli-1.1.0/invenio_cli/cli/packages.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/cli/services.py` & `invenio-cli-1.1.0/invenio_cli/cli/services.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/cli/utils.py` & `invenio-cli-1.1.0/invenio_cli/cli/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,13 +41,10 @@
         exit(1)
     elif response.warning:
         if response.error:
             msg = f"Errors: {response.error}"
         if response.output:
             msg = f"Output: {response.output}"
 
-        if fail_message:
-            msg = fail_message + "\n" + msg
-
         click.secho(msg, fg="yellow")
     elif response.output:
         click.secho(message=response.output, fg="green")
```

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/__init__.py` & `invenio-cli-1.1.0/invenio_cli/commands/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 from .commands import Commands
 from .containers import ContainersCommands
 from .install import InstallCommands
 from .local import LocalCommands
 from .packages import PackagesCommands
 from .requirements import RequirementsCommands
 from .services import ServicesCommands
+from .translations import TranslationsCommands
 from .upgrade import UpgradeCommands
 
 __all__ = (
     "AssetsCommands",
     "Commands",
     "ContainersCommands",
     "InstallCommands",
     "LocalCommands",
     "PackagesCommands",
     "RequirementsCommands",
     "ServicesCommands",
+    "TranslationsCommands",
     "UpgradeCommands",
 )
```

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/assets.py` & `invenio-cli-1.1.0/invenio_cli/commands/assets.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/commands.py` & `invenio-cli-1.1.0/invenio_cli/commands/commands.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/containers.py` & `invenio-cli-1.1.0/invenio_cli/commands/containers.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 #
 # Invenio-Cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module to ease the creation and management of applications."""
 
 from ..helpers.docker_helper import DockerHelper
+from ..helpers.rdm import rdm_version
 from .packages import PackagesCommands
 from .services import ServicesCommands
 from .steps import FunctionStep
+from .translations import TranslationsCommands
 
 
 class ContainersCommands(ServicesCommands):
     """Containerized environment CLI commands."""
 
     def __init__(self, cli_config, docker_helper=None):
         """Constructor."""
@@ -137,14 +139,43 @@
             FunctionStep(
                 func=self.cli_config.update_services_setup,
                 args={"is_setup": True},
                 message="Updating service setup status (True)...",
             ),
         ]
 
+        if rdm_version()[0] >= 10:
+            steps.extend(
+                [
+                    FunctionStep(
+                        func=self.docker_helper.execute_cli_command,
+                        args={
+                            "project_shortname": project_shortname,
+                            "command": "invenio rdm-records custom-fields init",
+                        },
+                        message="Creating custom fields for records...",
+                    ),
+                    FunctionStep(
+                        func=self.docker_helper.execute_cli_command,
+                        args={
+                            "project_shortname": project_shortname,
+                            "command": "invenio communities custom-fields init",
+                        },
+                        message="Creating custom fields for communities...",
+                    ),
+                ]
+            )
+
+        if rdm_version()[0] >= 11:
+            steps.extend(self.rdm_fixtures(project_shortname))
+            steps.extend(self.translations(project_shortname))
+
+        if rdm_version()[0] >= 12:
+            steps.extend(self.declare_queues(project_shortname))
+
         return steps
 
     def demo(self, project_shortname):
         """Steps to demo records into the instance."""
         steps = [
             FunctionStep(
                 func=self.docker_helper.execute_cli_command,
@@ -154,29 +185,86 @@
                 },
                 message="Creating demo records...",
             )
         ]
 
         return steps
 
+    def declare_queues(self, project_shortname):
+        """Steps to declare the MQ queues required for statistics, etc."""
+        steps = [
+            FunctionStep(
+                func=self.docker_helper.execute_cli_command,
+                args={
+                    "project_shortname": project_shortname,
+                    "command": "invenio queues declare",
+                },
+                message="Declaring queues...",
+            )
+        ]
+        return steps
+
     def fixtures(self, project_shortname):
         """Steps to set up the required fixtures for the instance."""
         steps = [
             FunctionStep(
                 func=self.docker_helper.execute_cli_command,
                 args={
                     "project_shortname": project_shortname,
                     "command": "invenio rdm-records fixtures",
                 },
-                message="Creating fixtures...",
+                message="Creating records fixtures...",
+            )
+        ]
+
+        return steps
+
+    def rdm_fixtures(self, project_shortname):
+        """Steps to set up the rdm fixtures for the instance."""
+        steps = [
+            FunctionStep(
+                func=self.docker_helper.execute_cli_command,
+                args={
+                    "project_shortname": project_shortname,
+                    "command": "invenio rdm fixtures",
+                },
+                message="Creating rdm fixtures...",
             )
         ]
 
         return steps
 
+    def translations(self, project_shortname):
+        """Steps to compile translations for the instance."""
+        commands = TranslationsCommands(
+            project_path=self.cli_config.get_project_dir(),
+            # we use INVENIO_INSTANCE_PATH that is set in the Dockerfile as
+            # config.instance_path is set only in development `install` command
+            instance_path="${INVENIO_INSTANCE_PATH}",
+        )
+        cmd = commands.compile(
+            # instance path inside the container
+            directory="${INVENIO_INSTANCE_PATH}/translations",
+            symlink=False,
+        )
+        cmd = cmd[0].cmd  # extract compilation command
+        cmd = " ".join(cmd)  # convert to string
+
+        return [
+            FunctionStep(
+                func=self.docker_helper.execute_cli_command,
+                args={
+                    "project_shortname": project_shortname,
+                    "command": cmd,
+                },
+                message="Compiling message catalog...",
+                skippable=True,
+            ),
+        ]
+
     def setup(self, force, demo_data=True, stop=False, services=True):
         """Return the steps to setup containerize services.
 
         :param force: Remove existing content (db, indices, etc.).
         :param demo_data: Include demo records.
         :param stop: Stop services after setup.
         """
```

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/install.py` & `invenio-cli-1.1.0/invenio_cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/local.py` & `invenio-cli-1.1.0/invenio_cli/commands/local.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Copyright (C) 2022 Graz University of Technology.
 #
 # Invenio-Cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module to ease the creation and management of applications."""
 
+import os
 import signal
 from distutils.dir_util import copy_tree
 from os import environ
 from pathlib import Path
 from subprocess import Popen as popen
 
 import click
@@ -41,80 +42,82 @@
             target_path = project_dir / relative_path
             filesystem.force_symlink(target_path, file_path)
 
     def _copy_statics_and_assets(self):
         """Copy project's statics and assets into instance dir."""
         click.secho("Copying project statics and assets...", fg="green")
 
-        static = "static"
-        src_dir = self.cli_config.get_project_dir() / static
-        src_dir = str(src_dir)  # copy_tree below doesn't accept Path objects
-        dst_dir = self.cli_config.get_instance_path() / static
-        dst_dir = str(dst_dir)
-        # using it for a different purpose then intended but very useful
-        copy_tree(src_dir, dst_dir)
-
-        assets = "assets"
-        src_dir = self.cli_config.get_project_dir() / assets
-        src_dir = str(src_dir)
-        dst_dir = self.cli_config.get_instance_path() / assets
-        dst_dir = str(dst_dir)
-        # The full path to the files that were copied is returned
-        copied_files = copy_tree(src_dir, dst_dir)
-        return copied_files
+        # static and assets folders do not exist in non-RDM contexts
+        rdm_static_dir_exists = os.path.exists("static")
+        rdm_assets_dir_exists = os.path.exists("assets")
+
+        if rdm_static_dir_exists:
+            static = "static"
+            src_dir = self.cli_config.get_project_dir() / static
+            src_dir = str(src_dir)  # copy_tree below doesn't accept Path objects
+            dst_dir = self.cli_config.get_instance_path() / static
+            dst_dir = str(dst_dir)
+            # using it for a different purpose then intended but very useful
+            copy_tree(src_dir, dst_dir)
+
+        if rdm_assets_dir_exists:
+            assets = "assets"
+            src_dir = self.cli_config.get_project_dir() / assets
+            src_dir = str(src_dir)
+            dst_dir = self.cli_config.get_instance_path() / assets
+            dst_dir = str(dst_dir)
+            # The full path to the files that were copied is returned
+            return copy_tree(src_dir, dst_dir)
+        return []
+
+    def _statics(self):
+        # Symlink the instance's statics and assets
+        copied_files = self._copy_statics_and_assets()
+        self._symlink_assets_templates(copied_files)
+        return ProcessResponse(
+            output="Assets and statics updated.",
+            status_code=0,
+        )
 
     def update_statics_and_assets(self, force, flask_env="production", log_file=None):
         """High-level command to update less/js/images/... files.
 
         Needed here (parent) because is used by Assets and Install commands.
         """
         # Commands
-        prefix = ["pipenv", "run"]
-        collect_cmd = prefix + ["invenio", "collect", "--verbose"]
-        clean_create_cmd = prefix + ["invenio", "webpack", "clean", "create"]
-        create_cmd = prefix + ["invenio", "webpack", "create"]
-        install_cmd = prefix + ["invenio", "webpack", "install"]
-        build_cmd = prefix + ["invenio", "webpack", "build"]
+        prefix = ["pipenv", "run", "invenio"]
 
-        with env(FLASK_ENV=flask_env):
-            # Collect into statics/ and assets/ folder
-            click.secho("Collecting statics and assets...", fg="green")
-            run_interactive(
-                collect_cmd, env={"PIPENV_VERBOSITY": "-1"}, log_file=log_file
-            )
-            if force:
-                run_interactive(
-                    clean_create_cmd, env={"PIPENV_VERBOSITY": "-1"}, log_file=log_file
-                )
-
-                # Installs in assets/node_modules/
-                click.secho("Installing JS dependencies...", fg="green")
-                run_interactive(
-                    install_cmd, env={"PIPENV_VERBOSITY": "-1"}, log_file=log_file
-                )
-            else:
-                run_interactive(
-                    create_cmd, env={"PIPENV_VERBOSITY": "-1"}, log_file=log_file
-                )
-
-            # Symlink the instance's statics and assets
-            copied_files = self._copy_statics_and_assets()
-            self._symlink_assets_templates(copied_files)
-
-            # Build project
-            click.secho("Building assets...", fg="green")
-            run_interactive(
-                build_cmd, env={"PIPENV_VERBOSITY": "-1"}, log_file=log_file
-            )
+        ops = [prefix + ["collect", "--verbose"]]
 
-        # FIXME: Refactor above to make use of proper error handling.
-        return ProcessResponse(
-            output="Assets and statics updated.",
-            status_code=0,
-        )
+        if force:
+            ops.append(prefix + ["webpack", "clean", "create"])
+            ops.append(prefix + ["webpack", "install"])
+        else:
+            ops.append(prefix + ["webpack", "create"])
+        ops.append(self._statics)
+        ops.append(prefix + ["webpack", "build"])
+        # Keep the same messages for some of the operations for backward compatibility
+        messages = {
+            "build": "Building assets...",
+            "install": "Installing JS dependencies...",
+        }
+
+        with env(FLASK_ENV=flask_env):
+            for op in ops:
+                if callable(op):
+                    response = op()
+                else:
+                    if op[-1] in messages:
+                        click.secho(messages[op[-1]], fg="green")
+                    response = run_interactive(
+                        op, env={"PIPENV_VERBOSITY": "-1"}, log_file=log_file
+                    )
+                if response.status_code != 0:
+                    break
+        return response
 
     def run(self, host, port, debug=True, services=True, celery_log_file=None):
         """Run development server and celery queue."""
 
         def signal_handler(sig, frame):
             click.secho("Stopping server and worker...", fg="green")
             server.terminate()
```

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/packages.py` & `invenio-cli-1.1.0/invenio_cli/commands/packages.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/requirements.py` & `invenio-cli-1.1.0/invenio_cli/commands/requirements.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2020-2021 CERN.
 # Copyright (C) 2021 TU Wien.
+# Copyright (C) 2023 ULB Münster.
 #
 # Invenio-Cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module to ease the creation and management of applications."""
 
+import json
 import re
 import sys
 from os import listdir
 
+from ..helpers.docker_helper import DockerHelper
 from ..helpers.process import ProcessResponse, run_cmd, run_interactive
+from ..helpers.rdm import rdm_version
 from .steps import FunctionStep
 
 
 class RequirementsCommands(object):
     """Pre-requirements check."""
 
     @classmethod
@@ -105,30 +109,31 @@
         )
 
         return cls._check_version("Python", version, major, minor, patch, exact)
 
     @classmethod
     def check_docker_version(cls, major, minor=-1, patch=-1, exact=False):
         """Check the docker version."""
-        # Output comes in the form of
-        # 'Docker version 19.03.13, build 4484c46d9d\n'
+        # Use JSON Formatted output and parse it
         try:
-            result = run_cmd(["docker", "--version"])
-            version = cls._version_from_string(result.output.strip())
+            result = run_cmd(["docker", "version", "--format", "json"])
+            result_json = json.loads(result.output.strip())
+            version = cls._version_from_string(result_json["Client"]["Version"])
             return cls._check_version("Docker", version, major, minor, patch, exact)
         except Exception as err:
             return ProcessResponse(error=f"Docker not found. Got {err}.", status_code=1)
 
     @classmethod
     def check_docker_compose_version(cls, major, minor=-1, patch=-1, exact=False):
         """Check the docker compose version."""
         # Output comes in the form of
-        # 'docker-compose version 1.27.4, build 4484c46d9d\n'
+        # 'Docker Compose version v2.17.3\n'
+        docker_helper = DockerHelper("", local=False)
         try:
-            result = run_cmd(["docker-compose", "--version"])
+            result = run_cmd(docker_helper.docker_compose + ["version"])
             version = cls._version_from_string(result.output.strip())
             return cls._check_version(
                 "Docker Compose", version, major, minor, patch, exact
             )
         except Exception as err:
             return ProcessResponse(
                 error=f"Docker Compose not found. Got {err}.", status_code=1
@@ -187,23 +192,31 @@
             return ProcessResponse(
                 error=f"Pipenv not found. Got {result.error}.", status_code=1
             )
 
     @classmethod
     def check_dev(cls):
         """Steps to check the development pre-requisites."""
+        if rdm_version()[0] >= 11:
+            node_version = 16
+            npm_version = 7
+        else:
+            # for backwards compatibility with v9 (LTS)
+            node_version = 14
+            npm_version = 6
+
         steps = [
             FunctionStep(
                 func=cls.check_node_version,
-                args={"major": 14, "exact": True},
+                args={"major": node_version, "exact": True},
                 message="Checking Node version...",
             ),
             FunctionStep(
                 func=cls.check_npm_version,
-                args={"major": 6, "exact": True},
+                args={"major": npm_version, "exact": True},
                 message="Checking NPM version...",
             ),
             FunctionStep(
                 func=cls.check_imagemagick_version,
                 args={"major": 0, "minor": 0},
                 message="Checking ImageMagick version...",
             ),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/services.py` & `invenio-cli-1.1.0/invenio_cli/commands/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # Invenio-Cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module to ease the creation and management of applications."""
 
 import click
 
+from invenio_cli.commands.translations import TranslationsCommands
+
 from ..helpers.docker_helper import DockerHelper
 from ..helpers.process import ProcessResponse
 from ..helpers.rdm import rdm_version
 from .commands import Commands
 from .services_health import HEALTHCHECKS, ServicesHealthCommands
 from .steps import CommandStep, FunctionStep
 
@@ -210,14 +212,21 @@
                         ],
                         env={"PIPENV_VERBOSITY": "-1"},
                         message="Creating custom fields for communities...",
                     ),
                 ]
             )
 
+        if rdm_version()[0] >= 11:
+            steps.extend(self.rdm_fixtures())
+            steps.extend(self.translations())
+
+        if rdm_version()[0] >= 12:
+            steps.extend(self.declare_queues())
+
         steps.append(
             FunctionStep(
                 func=self.cli_config.update_services_setup,
                 args={"is_setup": True},
                 message="Updating service setup status (True)...",
             ),
         )
@@ -232,27 +241,54 @@
                 env={"PIPENV_VERBOSITY": "-1"},
                 message="Creating demo records...",
             )
         ]
 
         return steps
 
+    def declare_queues(self):
+        """Steps to declare the MQ queues required for statistics, etc."""
+        command = ["pipenv", "run", "invenio", "queues", "declare"]
+        steps = [CommandStep(cmd=command, message="Declaring queues...")]
+        return steps
+
     def fixtures(self):
         """Steps to set up the required fixtures for the instance."""
         command = ["pipenv", "run", "invenio", "rdm-records", "fixtures"]
         steps = [
             CommandStep(
                 cmd=command,
                 env={"PIPENV_VERBOSITY": "-1"},
-                message="Creating fixtures...",
+                message="Creating records fixtures...",
+            )
+        ]
+
+        return steps
+
+    def rdm_fixtures(self):
+        """Steps to set up the rdm fixtures for the instance."""
+        command = ["pipenv", "run", "invenio", "rdm", "fixtures"]
+        steps = [
+            CommandStep(
+                cmd=command,
+                env={"PIPENV_VERBOSITY": "-1"},
+                message="Creating rdm fixtures...",
             )
         ]
 
         return steps
 
+    def translations(self):
+        """Steps to compile translations."""
+        commands = TranslationsCommands(
+            project_path=self.cli_config.get_project_dir(),
+            instance_path=self.cli_config.get_instance_path(),
+        )
+        return commands.compile(symlink=False)
+
     def setup(self, force, demo_data=True, stop=False, services=True):
         """Steps to setup services' containers.
 
         A check in invenio-cli's config file is done to see if one-time setup
         has been executed before.
         """
         steps = []
```

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/services_health.py` & `invenio-cli-1.1.0/invenio_cli/commands/services_health.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2020 CERN.
+# Copyright (C) 2023 ULB Münster.
 #
 # Invenio-Cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module to ease the creation and management of applications."""
 
 #####
@@ -37,15 +38,16 @@
     def postgresql_healthcheck(cls, *args, **kwargs):
         """Postgresql healthcheck."""
         filepath = kwargs["filepath"]
         verbose = kwargs["verbose"]
 
         return run_cmd(
             [
-                "docker-compose",
+                "docker",
+                "compose",
                 "--file",
                 filepath,
                 "exec",
                 "-T",
                 "db",
                 "bash",
                 "-c",
@@ -58,15 +60,16 @@
         """Mysql healthcheck."""
         filepath = kwargs["filepath"]
         verbose = kwargs["verbose"]
         password = kwargs["project_shortname"]
 
         return run_cmd(
             [
-                "docker-compose",
+                "docker",
+                "compose",
                 "--file",
                 filepath,
                 "exec",
                 "-T",
                 "db",
                 "bash",
                 "-c",
@@ -78,15 +81,16 @@
     def redis_healthcheck(cls, *args, **kwargs):
         """Redis healthcheck."""
         filepath = kwargs["filepath"]
         verbose = kwargs["verbose"]
 
         return run_cmd(
             [
-                "docker-compose",
+                "docker",
+                "compose",
                 "--file",
                 filepath,
                 "exec",
                 "-T",
                 "cache",
                 "bash",
                 "-c",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/steps.py` & `invenio-cli-1.1.0/invenio_cli/commands/steps.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/commands/upgrade.py` & `invenio-cli-1.1.0/invenio_cli/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/helpers/cli_config.py` & `invenio-cli-1.1.0/invenio_cli/helpers/cli_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -128,14 +128,22 @@
                 "`search` or `elasticsearch` field not set in .invenio file"
             )
 
     def get_file_storage(self):
         """Returns the file storage (local, s3, etc.)."""
         return self.config[CLIConfig.COOKIECUTTER_SECTION]["file_storage"]
 
+    def get_author_email(self):
+        """Returns the email of the author/owner of the project."""
+        return self.config[CLIConfig.COOKIECUTTER_SECTION]["author_email"]
+
+    def get_author_name(self):
+        """Returns the name of the author/owner of the project."""
+        return self.config[CLIConfig.COOKIECUTTER_SECTION]["author_name"]
+
     @classmethod
     def _write_private_config(cls, project_dir):
         """Write per-instance config file."""
         config_parser = ConfigParser()
         config_parser[cls.CLI_SECTION] = {}
         config_parser[cls.CLI_SECTION]["services_setup"] = str(False)
         private_config_path = project_dir / cls.PRIVATE_CONFIG_FILENAME
```

### Comparing `invenio-cli-1.0.9/invenio_cli/helpers/cookiecutter_wrapper.py` & `invenio-cli-1.1.0/invenio_cli/helpers/cookiecutter_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         if name.endswith(git):
             name = name[: -len(git)]
         return name
 
     def __init__(self, flavour, **kwargs):
         """Constructor.
 
-        :param flavour: "RDM" or something else: String
+        :param flavour: "RDM", "ILS" or something else: String
 
         :Keyword Arguments:
           * template: URL
           * checkout: String,
           * user_input: Boolean
           * config: String
         """
@@ -62,15 +62,23 @@
 
         if self.flavour.upper() == "RDM":
             self.template = (
                 self.template_name
                 or "https://github.com/inveniosoftware/cookiecutter-invenio-rdm.git"
             )
             self.template_name = self.extract_template_name(self.template)
-            self.checkout = self.checkout or "v10.0"
+            self.checkout = self.checkout or "v11.0"
+
+        if self.flavour.upper() == "ILS":
+            self.template = (
+                self.template_name
+                or "https://github.com/inveniosoftware/cookiecutter-invenio-ils.git"
+            )
+            self.template_name = self.extract_template_name(self.template)
+            self.checkout = self.checkout or "v1.0.0rc.1"
 
     def cookiecutter(self):
         """Wrap cookiecutter call."""
         # build actual kwargs
         cookiecutter_kwargs = {
             "template": self.template,
             # NOTE: if template is not a git url, then checkout is ignored
```

### Comparing `invenio-cli-1.0.9/invenio_cli/helpers/docker_helper.py` & `invenio-cli-1.1.0/invenio_cli/helpers/docker_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2019 CERN.
 # Copyright (C) 2019 Northwestern University.
+# Copyright (C) 2023 ULB Münster.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio CLI Docker Compose class."""
 
 import re
@@ -20,25 +21,26 @@
 
 class DockerHelper(object):
     """Utility class to interact with docker-compose."""
 
     def __init__(self, project_shortname, local=True, log_config=None):
         """Constructor."""
         super().__init__()
+        self.docker_compose = ["docker", "compose"]
         self.container_prefix = self._normalize_name(project_shortname)
         self.local = local
         self.docker_client = docker.from_env()
 
     def _normalize_name(self, project_shortname):
         """Normalize the container name according to the compose version.
 
         Docker-Compose introduced support for dash and underscore in
         version 1.21.0.
         """
-        dc_version_string = run_cmd(["docker-compose", "--version"])
+        dc_version_string = run_cmd(self.docker_compose + ["version"])
         groups = re.search(r"[0-9].[0-9]*.[0-9]*", dc_version_string.output)
         dc_version = groups.group(0)
 
         if dc_version < DOCKER_COMPOSE_VERSION_DASH:
             return re.sub(r"[^a-z0-9]", "", project_shortname)
         else:
             return project_shortname
@@ -60,16 +62,15 @@
 
     def build_images(self, pull=False, cache=True):
         """Build images.
 
         :param pull: Adds --pull to the docker-compose command.
         :param cache: Removes --no-cache to the docker-compose command.
         """
-        command = [
-            "docker-compose",
+        command = self.docker_compose + [
             "--file",
             "docker-compose.full.yml",
             "build",
         ]
         if pull:
             command.append("--pull")
         if not cache:
@@ -79,36 +80,34 @@
         return run_interactive(command)
 
     def start_containers(self, app_only=False):
         """Start containers according to the specified environment.
 
         :param app_only: Boot up only ui and api containers.
         """
-        command = [
-            "docker-compose",
+        command = self.docker_compose + [
             "--file",
             "docker-compose.yml" if self.local else "docker-compose.full.yml",
             "up",
             "-d",  # --detach not supported in 1.17.0
         ]
 
         if app_only:
             command.extend(["web-ui", "web-api"])
 
         return run_cmd(command)
 
     def stop_containers(self):
         """Stop currently running containers."""
-        command = ["docker-compose", "--file", "docker-compose.full.yml", "stop"]
+        command = self.docker_compose + ["--file", "docker-compose.full.yml", "stop"]
         return run_cmd(command)
 
     def destroy_containers(self):
         """Stop and remove all containers, volumes and images."""
-        command = [
-            "docker-compose",
+        command = self.docker_compose + [
             "--file",
             "docker-compose.full.yml",
             "down",
             "--volumes",
         ]
 
         return run_cmd(command)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-cli-1.0.9/invenio_cli/helpers/env.py` & `invenio-cli-1.1.0/invenio_cli/helpers/env.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/helpers/filesystem.py` & `invenio-cli-1.1.0/invenio_cli/helpers/filesystem.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli/helpers/process.py` & `invenio-cli-1.1.0/invenio_cli/helpers/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     full_env = environ.copy()  # Need to inherit the global one
     if env:
         for var, val in env.items():
             full_env[var] = val
 
     try:
         stdout = open(log_file, "a") if log_file else None
-        response = run(command, check=True, env=full_env, stdout=stdout, stderr=stdout)
+        _ = run(command, check=True, env=full_env, stdout=stdout, stderr=stdout)
         return ProcessResponse(output=None, error=None, status_code=0)
     except CalledProcessError as e:
         if skippable:
             return ProcessResponse(
                 output=e.stdout, error=e.stderr, status_code=0, warning=True
             )
         else:
```

### Comparing `invenio-cli-1.0.9/invenio_cli/helpers/rdm.py` & `invenio-cli-1.1.0/invenio_cli/helpers/rdm.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/invenio_cli.egg-info/PKG-INFO` & `invenio-cli-1.1.0/invenio_cli.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-cli
-Version: 1.0.9
+Version: 1.1.0
 Summary: "Invenio module to ease the creation and management of applications."
 Home-page: https://github.com/inveniosoftware/invenio-cli
 Author: CERN & Northwestern University
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019-2020 CERN.
@@ -99,23 +99,72 @@
         
             # Get more help
             $ invenio-cli --help
         
         Further documentation is available on https://invenio-cli.readthedocs.io/
         
         ..
-            Copyright (C) 2019-2021 CERN.
+            Copyright (C) 2019-2023 CERN.
             Copyright (C) 2019-2021 Northwestern University.
         
             Invenio-Cli is free software; you can redistribute it and/or modify
             it under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.1.0 (released 2023-07-24)
+        
+        - add compatibility for docker compose v2
+        - consider command errors when using install command and fail
+        
+        Version 1.0.21 (released 2023-05-18)
+        
+        - deps: support docker < 7 for compatibility with urllib3 v2
+        
+        Version 1.0.20 (released 2023-03-134)
+        
+        - setup: add queues initialisation to steps
+        
+        Version 1.0.19 (released 2023-03-10)
+        
+        - global: remove fail message on warning (i.e. soft failures)
+        
+        Version 1.0.18 (released 2023-02-07)
+        
+        - containerize: fix translation commands instance path
+        
+        Version 1.0.17 (released 2023-01-30)
+        
+        - requirements: check node version depending on app-rdm version
+        
+        Version 1.0.16 (released 2023-01-30)
+        
+        - bump cookiecutter to v11.0
+        
+        Version 1.0.15 (released 2023-01-13)
+        
+        - Setup: fix empty translation folder failing
+        
+        Version 1.0.14 (released 2023-01-09)
+        
+        - Add app-rdm fixtures to setup
+        
+        Version 1.0.13 (released 2022-11-14)
+        
+        - Allow compilation command to fail in case of missing catalogs.
+        
+        Version 1.0.12 (released 2022-10-28)
+        
+        - Adds support for translations (i18n) management commands.
+        
+        Version 1.0.11 (released 2022-10-24)
+        
+        - Add support for InvenioILS
+        
         Version 1.0.8 (released 2022-10-13)
         
         - Fix issue when checking for services to be up
           and running correctly.
         
         Version 1.0.7 (released 2022-10-10)
```

### Comparing `invenio-cli-1.0.9/invenio_cli.egg-info/SOURCES.txt` & `invenio-cli-1.1.0/invenio_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,26 +37,28 @@
 invenio_cli/cli/__init__.py
 invenio_cli/cli/assets.py
 invenio_cli/cli/cli.py
 invenio_cli/cli/containers.py
 invenio_cli/cli/install.py
 invenio_cli/cli/packages.py
 invenio_cli/cli/services.py
+invenio_cli/cli/translations.py
 invenio_cli/cli/utils.py
 invenio_cli/commands/__init__.py
 invenio_cli/commands/assets.py
 invenio_cli/commands/commands.py
 invenio_cli/commands/containers.py
 invenio_cli/commands/install.py
 invenio_cli/commands/local.py
 invenio_cli/commands/packages.py
 invenio_cli/commands/requirements.py
 invenio_cli/commands/services.py
 invenio_cli/commands/services_health.py
 invenio_cli/commands/steps.py
+invenio_cli/commands/translations.py
 invenio_cli/commands/upgrade.py
 invenio_cli/helpers/__init__.py
 invenio_cli/helpers/cli_config.py
 invenio_cli/helpers/cookiecutter_wrapper.py
 invenio_cli/helpers/docker_helper.py
 invenio_cli/helpers/env.py
 invenio_cli/helpers/filesystem.py
```

### Comparing `invenio-cli-1.0.9/run-tests.sh` & `invenio-cli-1.1.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/setup.cfg` & `invenio-cli-1.1.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
-	cookiecutter>=1.7.1,<1.8.0
+	Babel>=2.8
+	cookiecutter>=2.0.0,<2.2.0
 	click>=7.1.1,<8.2
 	click-default-group>=1.2.2,<2.0.0
-	docker>=4.1.0,<6.0.0
+	docker>=4.1.0,<7.0.0
 	pipfile>=0.0.2
 	pipenv>=2020.6.2
 	PyYAML>=5.1.2
 	pynpm>=0.1.2
-	virtualenv>=20.0.35,<=20.13.0
+	virtualenv>=20.0.35
 
 [options.extras_require]
 tests = 
 	pytest-black==0.3.9
 	pytest-invenio>=1.4.0
 	Sphinx>=4.2.0
```

### Comparing `invenio-cli-1.0.9/tests/commands/conftest.py` & `invenio-cli-1.1.0/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/tests/commands/test_commands.py` & `invenio-cli-1.1.0/tests/commands/test_commands.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/tests/commands/test_containers.py` & `invenio-cli-1.1.0/tests/commands/test_containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         ),
         call("project-shortname", "invenio roles create admin"),
         call("project-shortname", "invenio access allow superuser-access role admin"),
         call("project-shortname", "invenio index init"),
         # update_statics_and_assets call
         call("project-shortname", "invenio collect"),
         call("project-shortname", "invenio webpack create"),
-        call("project-shortname", "invenio webpack install --unsafe"),
+        call("project-shortname", "invenio webpack install"),
         call("project-shortname", "invenio webpack build"),
     ]
 
 
 @pytest.mark.skip()
 @pytest.fixture(scope="function")
 def expected_force_calls():
@@ -84,15 +84,15 @@
     p_popen.return_value = mocked_pipe
     commands = ContainersCommands(mock_cli_config, p_docker_helper())
     commands.docker_helper.execute_cli_command.reset_mock()
 
     commands.containerize(pre=False, force=False, install=False)
 
     assert (
-        call("project-shortname", "invenio webpack install --unsafe")
+        call("project-shortname", "invenio webpack install")
         not in commands.docker_helper.execute_cli_command.mock_calls
     )
 
 
 @pytest.mark.skip()
 @patch("invenio_cli.commands.containers.run_cmd")
 @patch("invenio_cli.commands.containers.DockerHelper")
@@ -152,15 +152,15 @@
     commands = ContainersCommands(mock_cli_config, p_docker_helper())
 
     commands.update_statics_and_assets(install=True)
 
     expected_execute_cli_calls = [
         call("project-shortname", "invenio collect"),
         call("project-shortname", "invenio webpack create"),
-        call("project-shortname", "invenio webpack install --unsafe"),
+        call("project-shortname", "invenio webpack install"),
         call("project-shortname", "invenio webpack build"),
     ]
     assert (
         commands.docker_helper.execute_cli_command.mock_calls
         == expected_execute_cli_calls
     )
```

### Comparing `invenio-cli-1.0.9/tests/commands/test_local.py` & `invenio-cli-1.1.0/tests/commands/test_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,41 +310,38 @@
     ]
     assert p_commands_popen.mock_calls == expected_calls
 
 
 @pytest.mark.skip()
 @patch("pynpm.package.run_npm")
 def test_link_js_module(p_run_npm, testpkg, mock_cli_config):
-
     LocalCommands(mock_cli_config).link_js_module(testpkg)
 
     expected_calls = [
         call(testpkg, "run-script", npm_bin="npm", args=("link-dist",)),
         call("instance_dir/assets", "link", npm_bin="npm", args=("testpkg",)),
     ]
 
     assert expected_calls == p_run_npm.mock_calls
 
 
 @pytest.mark.skip()
 @patch("pynpm.package.run_npm")
 def test_watch_js_module(p_run_npm, testpkg, mock_cli_config):
-
     LocalCommands(mock_cli_config).watch_js_module(testpkg, link=False)
 
     expected_calls = [
         call(testpkg, "run-script", npm_bin="npm", args=("watch",)),
     ]
     assert expected_calls == p_run_npm.mock_calls
 
 
 @pytest.mark.skip()
 @patch("pynpm.package.run_npm")
 def test_watch_js_module_w_build(p_run_npm, testpkg, mock_cli_config):
-
     LocalCommands(mock_cli_config).watch_js_module(testpkg, link=True)
 
     expected_calls = [
         call(testpkg, "run-script", npm_bin="npm", args=("link-dist",)),
         call("instance_dir/assets", "link", npm_bin="npm", args=("testpkg",)),
         call(testpkg, "run-script", npm_bin="npm", args=("watch",)),
     ]
```

### Comparing `invenio-cli-1.0.9/tests/commands/test_requirements.py` & `invenio-cli-1.1.0/tests/commands/test_requirements.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/tests/commands/test_steps.py` & `invenio-cli-1.1.0/tests/commands/test_steps.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/tests/helpers/test_cli_config.py` & `invenio-cli-1.1.0/tests/helpers/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/tests/helpers/test_cookiecutter_wrapper.py` & `invenio-cli-1.1.0/tests/helpers/test_cookiecutter_wrapper.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/tests/helpers/test_dockerhelper.py` & `invenio-cli-1.1.0/tests/helpers/test_dockerhelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2019-2020 CERN.
 # Copyright (C) 2019-2020 Northwestern University.
+# Copyright (C) 2023 ULB Münster.
 #
 # Invenio-Cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Module docker_helper tests."""
 
 from unittest.mock import patch
@@ -25,18 +26,27 @@
 
     with patch.object(DockerHelper, "_normalize_name", fake_normalize_name):
         docker_helper = DockerHelper("project-shortname", local=True)
 
     docker_helper.start_containers()
 
     p_run_cmd.run.assert_called_with(
-        ["docker-compose", "--file", "docker-compose.yml", "up", "--build", "-d"]
+        docker_helper.docker_compose
+        + ["--file", "docker-compose.yml", "up", "--build", "-d"]
     )
 
     with patch.object(DockerHelper, "_normalize_name", fake_normalize_name):
         docker_helper = DockerHelper("project-shortname", local=False)
 
     docker_helper.start_containers()
 
     p_run_cmd.run.assert_called_with(
-        ["docker-compose", "--file", "docker-compose.full.yml", "up", "--build", "-d"]
+        [
+            "docker",
+            "compose",
+            "--file",
+            "docker-compose.full.yml",
+            "up",
+            "--build",
+            "-d",
+        ]
     )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-cli-1.0.9/tests/helpers/test_env.py` & `invenio-cli-1.1.0/tests/helpers/test_env.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/tests/helpers/test_filesystem.py` & `invenio-cli-1.1.0/tests/helpers/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.9/tests/test_cli.py` & `invenio-cli-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

