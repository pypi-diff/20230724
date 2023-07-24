# Comparing `tmp/invenio-theme-2.1.2.tar.gz` & `tmp/invenio-theme-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-theme-2.1.2.tar", last modified: Wed Apr 12 09:16:33 2023, max compression
+gzip compressed data, was "dist/invenio-theme-2.1.3.tar", last modified: Mon Jul 24 14:09:42 2023, max compression
```

## Comparing `invenio-theme-2.1.2.tar` & `invenio-theme-2.1.3.tar`

### file list

```diff
@@ -1,421 +1,477 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      348 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1186 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9597 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7437 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6995 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/docs/static/
--rw-r--r--   0 runner    (1001) docker     (122)    39567 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/static/base.png
--rw-r--r--   0 runner    (1001) docker     (122)    27194 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/static/cover.png
--rw-r--r--   0 runner    (1001) docker     (122)    45698 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/static/error.png
--rw-r--r--   0 runner    (1001) docker     (122)    48992 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/static/settings.png
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)    18117 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/js/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)      733 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/js/invenio_theme/base.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/footer.scss
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/header.scss
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/theme.scss
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/type.scss
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/base.js
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js
--rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   256056 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (122)   600856 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   309728 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (122)   184912 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   266158 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot
--rw-r--r--   0 runner    (1001) docker     (122)   622572 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   323344 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (122)   193308 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   268604 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot
--rw-r--r--   0 runner    (1001) docker     (122)   639388 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   328412 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (122)   195704 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    77192 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    49064 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   253461 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot
--rw-r--r--   0 runner    (1001) docker     (122)   607720 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   309192 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (122)   182708 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.variables
--rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.variables
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.variables
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.variables
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.variables
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.overrides
--rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.variables
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.variables
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.variables
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.variables
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      992 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.variables
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.variables
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.variables
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.variables
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.variables
--rw-r--r--   0 runner    (1001) docker     (122)    14632 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.variables
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.variables
--rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.variables
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.variables
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.variables
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.variables
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.variables
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.variables
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.variables
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.variables
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.variables
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.variables
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.variables
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.variables
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.variables
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.variables
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.variables
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.variables
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.variables
--rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/footer.scss
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/header.scss
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/theme.scss
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/type.scss
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss
--rw-r--r--   0 runner    (1001) docker     (122)     5142 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3420 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/static/
--rw-r--r--   0 runner    (1001) docker     (122)    15178 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/static/apple-touch-icon-120.png
--rw-r--r--   0 runner    (1001) docker     (122)    20939 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/static/apple-touch-icon-152.png
--rw-r--r--   0 runner    (1001) docker     (122)    23315 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/static/apple-touch-icon-167.png
--rw-r--r--   0 runner    (1001) docker     (122)    25366 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/static/apple-touch-icon-180.png
--rw-r--r--   0 runner    (1001) docker     (122)    93062 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (122)     5096 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/static/images/invenio-white.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/static/images/square-placeholder.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/401.html
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/403.html
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/404.html
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/429.html
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/500.html
--rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/admin_header.html
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/admin_layout.html
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/body.html
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/frontpage.html
--rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/header.html
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/header_frontpage.html
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/header_login.html
--rw-r--r--   0 runner    (1001) docker     (122)      288 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/javascript.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/macros/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/macros/messages.html
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/macros/truncate.html
--rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/page.html
--rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/page_admin.html
--rw-r--r--   0 runner    (1001) docker     (122)     2325 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/page_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/page_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/page_settings.html
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/trackingcode.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/401.html
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/403.html
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/404.html
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/429.html
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/500.html
--rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/body.html
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (122)      846 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/frontpage.html
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/header.html
--rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html
--rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/javascript.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/macros/
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html
--rw-r--r--   0 runner    (1001) docker     (122)     4307 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/page.html
--rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1998 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/trackingcode.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5364 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5702 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5972 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5508 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6322 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5424 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2308 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6101 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5222 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5375 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5206 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5434 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6022 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5804 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5350 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5500 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     5141 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5492 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5406 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5374 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5553 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5209 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5931 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1998 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5992 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5591 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/invenio_theme/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     3952 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/invenio_theme/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9597 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18874 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-12 09:16:32.000000 invenio-theme-2.1.2/invenio_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      502 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:16:33.000000 invenio-theme-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5691 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/tests/test_invenio_theme.py
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-04-12 09:16:27.000000 invenio-theme-2.1.2/tests/test_invenio_theme_error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5765 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1186 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9691 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7437 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6995 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (122)    39567 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/static/base.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27194 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/static/cover.png
+-rw-r--r--   0 runner    (1001) docker     (122)    45698 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/static/error.png
+-rw-r--r--   0 runner    (1001) docker     (122)    48992 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/static/settings.png
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)    18117 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/js/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)      733 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/js/invenio_theme/base.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/header.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/type.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/base.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   256056 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   600856 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   309728 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   184912 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   266158 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   622572 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   323344 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   193308 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   268604 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   639388 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   328412 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   195704 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    77192 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    49064 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   253461 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   607720 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   309192 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   182708 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/
+-rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.variables
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/
+-rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      992 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.variables
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.variables
+-rw-r--r--   0 runner    (1001) docker     (122)    14632 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/header.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/type.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss
+-rw-r--r--   0 runner    (1001) docker     (122)     5142 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3420 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (122)    15178 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/static/apple-touch-icon-120.png
+-rw-r--r--   0 runner    (1001) docker     (122)    20939 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/static/apple-touch-icon-152.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23315 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/static/apple-touch-icon-167.png
+-rw-r--r--   0 runner    (1001) docker     (122)    25366 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/static/apple-touch-icon-180.png
+-rw-r--r--   0 runner    (1001) docker     (122)    93062 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     5096 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/static/images/invenio-white.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/static/images/square-placeholder.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/401.html
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/403.html
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/404.html
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/429.html
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/500.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/admin_header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/admin_layout.html
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/body.html
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/header_frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/javascript.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/macros/messages.html
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/macros/truncate.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/page.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/page_admin.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2325 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/page_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/page_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/page_settings.html
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/trackingcode.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/401.html
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/403.html
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/404.html
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/429.html
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/500.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/body.html
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (122)      846 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/javascript.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)     1526 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4307 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/page.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1998 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/trackingcode.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6411 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5364 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5702 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5972 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5508 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6322 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5424 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2308 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6101 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5257 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5259 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5222 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5375 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5217 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      587 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5278 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5270 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5206 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5217 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5434 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6022 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5804 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5350 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5500 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5141 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5492 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5406 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5415 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5553 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5209 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5964 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1998 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5992 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5777 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3952 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/invenio_theme/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9691 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    20464 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/invenio_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-24 14:09:41.000000 invenio-theme-2.1.3/invenio_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      502 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 14:09:42.000000 invenio-theme-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5691 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/tests/test_invenio_theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-07-24 14:09:30.000000 invenio-theme-2.1.3/tests/test_invenio_theme_error_handler.py
```

### Comparing `invenio-theme-2.1.2/.editorconfig` & `invenio-theme-2.1.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/.github/workflows/pypi-publish.yml` & `invenio-theme-2.1.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/.github/workflows/tests.yml` & `invenio-theme-2.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/.tx/config` & `invenio-theme-2.1.3/.tx/config`

 * *Files 14% similar despite different names*

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
 
 
 # Transifex integration
 #
@@ -21,14 +22,14 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio-theme-messages]
+[o:inveniosoftware:p:invenio:r:invenio-theme-messages]
 file_filter = invenio_theme/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_theme/translations/messages.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-theme-2.1.2/AUTHORS.rst` & `invenio-theme-2.1.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/CHANGES.rst` & `invenio-theme-2.1.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.1.3 (released 2023-07-24)
+
+- messages: add z-index
+
 Version 2.1.2 (released 2023-04-12)
 
 - add flex utility classes
 - add text sizes classes
 
 Version 2.1.1 (released 2023-04-06)
```

### Comparing `invenio-theme-2.1.2/CONTRIBUTING.rst` & `invenio-theme-2.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/LICENSE` & `invenio-theme-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/MANIFEST.in` & `invenio-theme-2.1.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/PKG-INFO` & `invenio-theme-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme
-Version: 2.1.2
+Version: 2.1.3
 Summary: "Invenio standard theme."
 Home-page: https://github.com/inveniosoftware/invenio-theme
 Author: Invenio Collaboration
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -48,14 +48,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.3 (released 2023-07-24)
+        
+        - messages: add z-index
+        
         Version 2.1.2 (released 2023-04-12)
         
         - add flex utility classes
         - add text sizes classes
         
         Version 2.1.1 (released 2023-04-06)
```

### Comparing `invenio-theme-2.1.2/README.rst` & `invenio-theme-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/docs/Makefile` & `invenio-theme-2.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/docs/conf.py` & `invenio-theme-2.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/docs/index.rst` & `invenio-theme-2.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/docs/make.bat` & `invenio-theme-2.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/docs/static/base.png` & `invenio-theme-2.1.3/docs/static/base.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/docs/static/cover.png` & `invenio-theme-2.1.3/docs/static/cover.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/docs/static/error.png` & `invenio-theme-2.1.3/docs/static/error.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/docs/static/settings.png` & `invenio-theme-2.1.3/docs/static/settings.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/__init__.py` & `invenio-theme-2.1.3/invenio_theme/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,10 +517,10 @@
     def settings_item_1():
         flash('Testing flashing', category='info')
         return render_template('...')
 """
 
 from .ext import InvenioTheme
 
-__version__ = "2.1.2"
+__version__ = "2.1.3"
 
 __all__ = ("__version__", "InvenioTheme")
```

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js` & `invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss` & `invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss` & `invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss` & `invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss` & `invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss` & `invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss` & `invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss` & `invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss` & `invenio-theme-2.1.3/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss` & `invenio-theme-2.1.3/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/config.py` & `invenio-theme-2.1.3/invenio_theme/config.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/ext.py` & `invenio-theme-2.1.3/invenio_theme/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/proxies.py` & `invenio-theme-2.1.3/invenio_theme/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/static/apple-touch-icon-120.png` & `invenio-theme-2.1.3/invenio_theme/static/apple-touch-icon-120.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/static/apple-touch-icon-152.png` & `invenio-theme-2.1.3/invenio_theme/static/apple-touch-icon-152.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/static/apple-touch-icon-167.png` & `invenio-theme-2.1.3/invenio_theme/static/apple-touch-icon-167.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/static/apple-touch-icon-180.png` & `invenio-theme-2.1.3/invenio_theme/static/apple-touch-icon-180.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/static/favicon.ico` & `invenio-theme-2.1.3/invenio_theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/static/images/invenio-white.svg` & `invenio-theme-2.1.3/invenio_theme/static/images/invenio-white.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/static/images/square-placeholder.png` & `invenio-theme-2.1.3/invenio_theme/static/images/square-placeholder.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/500.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/500.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/admin_header.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/admin_header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/admin_layout.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/admin_layout.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/breadcrumbs.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/footer.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/header.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/header_frontpage.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/header_frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/header_login.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/macros/messages.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/macros/messages.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/macros/truncate.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/macros/truncate.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/page.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/page.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/page_admin.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/page_admin.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/page_cover.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/page_cover.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/invenio_theme/page_settings.html` & `invenio-theme-2.1.3/invenio_theme/templates/invenio_theme/page_settings.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/footer.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/header.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
       {%- if center_text %}
         {%- set gridClass = 'centered' %}
         {%- set firstColWidth = 'twelve wide mobile six wide tablet four wide computer' %}
         {%- set secondColWidth = 'two wide tablet one wide computer' %}
       {% endif %}
 
-      <div class="ui {{ category }} flashed message">
+      <div class="ui {{ category }} flashed message m-0">
         <div class="ui middle aligned grid {{gridClass}}">
 
           <div role="alert" id="flash-message" class="{{ firstColWidth }} left aligned column">
             <p id="alert-content" style="display:none;">{{ msg }}</p>
           </div>
 
           <div class="{{ secondColWidth }} right aligned column">
```

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/page.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/page.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html` & `invenio-theme-2.1.3/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/af/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-theme 1.3.28*

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 d601 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 d801 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d74 6865 6d65 2031   invenio-theme 1
 00000050: 2e33 2e32 380a 5265 706f 7274 2d4d 7367  .3.28.Report-Msg
 00000060: 6964 2d42 7567 732d 546f 3a20 696e 666f  id-Bugs-To: info
 00000070: 4069 6e76 656e 696f 736f 6674 7761 7265  @inveniosoftware
 00000080: 2e6f 7267 0a50 4f54 2d43 7265 6174 696f  .org.POT-Creatio
 00000090: 6e2d 4461 7465 3a20 3230 3232 2d30 392d  n-Date: 2022-09-
 000000a0: 3136 2030 383a 3430 2b30 3030 300a 504f  16 08:40+0000.PO
 000000b0: 2d52 6576 6973 696f 6e2d 4461 7465 3a20  -Revision-Date: 
 000000c0: 3230 3136 2d30 382d 3235 2031 353a 3238  2016-08-25 15:28
 000000d0: 2b30 3030 300a 4c61 7374 2d54 7261 6e73  +0000.Last-Trans
 000000e0: 6c61 746f 723a 2046 554c 4c20 4e41 4d45  lator: FULL NAME
 000000f0: 203c 454d 4149 4c40 4144 4452 4553 533e   <EMAIL@ADDRESS>
-00000100: 0a4c 616e 6775 6167 653a 2061 660a 4c61  .Language: af.La
-00000110: 6e67 7561 6765 2d54 6561 6d3a 2041 6672  nguage-Team: Afr
-00000120: 696b 6161 6e73 2028 6874 7470 733a 2f2f  ikaans (https://
-00000130: 7777 772e 7472 616e 7369 6665 782e 636f  www.transifex.co
-00000140: 6d2f 696e 7665 6e69 6f73 6f66 7477 6172  m/inveniosoftwar
-00000150: 652f 7465 616d 732f 3233 3533 372f 6166  e/teams/23537/af
-00000160: 2f29 0a50 6c75 7261 6c2d 466f 726d 733a  /).Plural-Forms:
-00000170: 206e 706c 7572 616c 733d 323b 2070 6c75   nplurals=2; plu
-00000180: 7261 6c3d 286e 2021 3d20 3129 3b0a 4d49  ral=(n != 1);.MI
-00000190: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
-000001a0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-000001b0: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
-000001c0: 743d 7574 662d 380a 436f 6e74 656e 742d  t=utf-8.Content-
-000001d0: 5472 616e 7366 6572 2d45 6e63 6f64 696e  Transfer-Encodin
-000001e0: 673a 2038 6269 740a 4765 6e65 7261 7465  g: 8bit.Generate
-000001f0: 642d 4279 3a20 4261 6265 6c20 322e 3132  d-By: Babel 2.12
-00000200: 2e31 0a00                                .1..
+00000100: 0a4c 616e 6775 6167 653a 2072 770a 4c61  .Language: rw.La
+00000110: 6e67 7561 6765 2d54 6561 6d3a 204b 696e  nguage-Team: Kin
+00000120: 7961 7277 616e 6461 2028 6874 7470 733a  yarwanda (https:
+00000130: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
+00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
+00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
+00000160: 7277 2f29 0a50 6c75 7261 6c2d 466f 726d  rw/).Plural-Form
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

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/af/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/af/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: Afrikaans (https://app.transifex.com/inveniosoftware/teams/23537/af/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: af\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ar/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022\n"
 "Language: ar\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/"
 "ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
@@ -27,15 +27,15 @@
 msgid "Home"
 msgstr "الإستقبــال"
 
 msgid "Internal server error"
 msgstr "خطأ بالموزّع الدّاخلي"
 
 msgid "Invenio"
-msgstr "Invenio"
+msgstr "إنفنيو"
 
 msgid "Log in"
 msgstr "تسجيل الدّخول"
 
 msgid "Log out"
 msgstr "خروج"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ar/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/ar/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-theme
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2016
-# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022
 # Bessem Aamira <bessemamira@gmail.com>, 2022
+# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022\n"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 #: invenio_theme/config.py:102 invenio_theme/config.py:117
 #: invenio_theme/templates/invenio_theme/page.html:26
 #: invenio_theme/templates/invenio_theme/page_admin.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html:34
 msgid "Invenio"
-msgstr "Invenio"
+msgstr "إنفنيو"
 
 #: invenio_theme/ext.py:73
 msgid "Home"
 msgstr "الإستقبــال"
 
 #: invenio_theme/templates/invenio_theme/401.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/401.html:13
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/bg/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/bg/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: bg\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/bg/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/bg/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/bg/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ca/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: ca\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ca/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ca/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/ca/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/cs/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2022\n"
 "Language: cs\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/"
 "cs/)\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/cs/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/cs/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/da/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/da/LC_MESSAGES/messages.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2016\n"
 "Language: da\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/"
 "da/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/da/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/da/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2016\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/de/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/de/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
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

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/de/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/de/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: chriz_uniba <christina.zeller@uni-bamberg.de>, 2022\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/de/)\n"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/el/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/el/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: el\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/"
 "el/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/el/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/el/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/es/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/es/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
 "Language: es\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/es/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/es/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/et/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/et/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2022\n"
 "Language: et\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/et/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/et/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/et/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/teams/23537/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/teams/23537/et/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-theme 1.3.28*

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 e501 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 e301 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d74 6865 6d65 2031   invenio-theme 1
 00000050: 2e33 2e32 380a 5265 706f 7274 2d4d 7367  .3.28.Report-Msg
 00000060: 6964 2d42 7567 732d 546f 3a20 696e 666f  id-Bugs-To: info
 00000070: 4069 6e76 656e 696f 736f 6674 7761 7265  @inveniosoftware
 00000080: 2e6f 7267 0a50 4f54 2d43 7265 6174 696f  .org.POT-Creatio
 00000090: 6e2d 4461 7465 3a20 3230 3232 2d30 392d  n-Date: 2022-09-
 000000a0: 3136 2030 383a 3430 2b30 3030 300a 504f  16 08:40+0000.PO
 000000b0: 2d52 6576 6973 696f 6e2d 4461 7465 3a20  -Revision-Date: 
 000000c0: 3230 3136 2d30 382d 3235 2031 353a 3238  2016-08-25 15:28
 000000d0: 2b30 3030 300a 4c61 7374 2d54 7261 6e73  +0000.Last-Trans
 000000e0: 6c61 746f 723a 2046 554c 4c20 4e41 4d45  lator: FULL NAME
 000000f0: 203c 454d 4149 4c40 4144 4452 4553 533e   <EMAIL@ADDRESS>
-00000100: 0a4c 616e 6775 6167 653a 2065 745f 4545  .Language: et_EE
+00000100: 0a4c 616e 6775 6167 653a 2064 655f 4154  .Language: de_AT
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
-00000120: 4573 746f 6e69 616e 2028 4573 746f 6e69  Estonian (Estoni
-00000130: 6129 2028 6874 7470 733a 2f2f 7777 772e  a) (https://www.
-00000140: 7472 616e 7369 6665 782e 636f 6d2f 696e  transifex.com/in
-00000150: 7665 6e69 6f73 6f66 7477 6172 652f 7465  veniosoftware/te
-00000160: 616d 732f 3233 3533 372f 6574 5f45 452f  ams/23537/et_EE/
-00000170: 290a 506c 7572 616c 2d46 6f72 6d73 3a20  ).Plural-Forms: 
-00000180: 6e70 6c75 7261 6c73 3d32 3b20 706c 7572  nplurals=2; plur
-00000190: 616c 3d28 6e20 213d 2031 293b 0a4d 494d  al=(n != 1);.MIM
-000001a0: 452d 5665 7273 696f 6e3a 2031 2e30 0a43  E-Version: 1.0.C
-000001b0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000001c0: 742f 706c 6169 6e3b 2063 6861 7273 6574  t/plain; charset
-000001d0: 3d75 7466 2d38 0a43 6f6e 7465 6e74 2d54  =utf-8.Content-T
-000001e0: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
-000001f0: 3a20 3862 6974 0a47 656e 6572 6174 6564  : 8bit.Generated
-00000200: 2d42 793a 2042 6162 656c 2032 2e31 322e  -By: Babel 2.12.
-00000210: 310a 00                                  1..
+00000120: 4765 726d 616e 2028 4175 7374 7269 6129  German (Austria)
+00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
+00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
+00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
+00000160: 732f 3233 3533 372f 6465 5f41 542f 290a  s/23537/de_AT/).
+00000170: 506c 7572 616c 2d46 6f72 6d73 3a20 6e70  Plural-Forms: np
+00000180: 6c75 7261 6c73 3d32 3b20 706c 7572 616c  lurals=2; plural
+00000190: 3d28 6e20 213d 2031 293b 0a4d 494d 452d  =(n != 1);.MIME-
+000001a0: 5665 7273 696f 6e3a 2031 2e30 0a43 6f6e  Version: 1.0.Con
+000001b0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000001c0: 706c 6169 6e3b 2063 6861 7273 6574 3d75  plain; charset=u
+000001d0: 7466 2d38 0a43 6f6e 7465 6e74 2d54 7261  tf-8.Content-Tra
+000001e0: 6e73 6665 722d 456e 636f 6469 6e67 3a20  nsfer-Encoding: 
+000001f0: 3862 6974 0a47 656e 6572 6174 6564 2d42  8bit.Generated-B
+00000200: 793a 2042 6162 656c 2032 2e31 322e 310a  y: Babel 2.12.1.
+00000210: 00                                       .
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: Estonian (Estonia) (https://app.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: et_EE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/fa/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: fa\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/fa/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/fa/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/fa/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/teams/23537/fa/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/fr/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
 "Language: fr\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/"
 "fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/fr/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/fr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/gl/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-theme 1.3.28*

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 000000b0: 2d52 6576 6973 696f 6e2d 4461 7465 3a20  -Revision-Date: 
 000000c0: 3230 3136 2d30 382d 3235 2031 353a 3238  2016-08-25 15:28
 000000d0: 2b30 3030 300a 4c61 7374 2d54 7261 6e73  +0000.Last-Trans
 000000e0: 6c61 746f 723a 2046 554c 4c20 4e41 4d45  lator: FULL NAME
 000000f0: 203c 454d 4149 4c40 4144 4452 4553 533e   <EMAIL@ADDRESS>
 00000100: 0a4c 616e 6775 6167 653a 2067 6c0a 4c61  .Language: gl.La
 00000110: 6e67 7561 6765 2d54 6561 6d3a 2047 616c  nguage-Team: Gal
-00000120: 6963 6961 6e20 2868 7474 7073 3a2f 2f77  ician (https://w
-00000130: 7777 2e74 7261 6e73 6966 6578 2e63 6f6d  ww.transifex.com
+00000120: 6963 6961 6e20 2868 7474 7073 3a2f 2f61  ician (https://a
+00000130: 7070 2e74 7261 6e73 6966 6578 2e63 6f6d  pp.transifex.com
 00000140: 2f69 6e76 656e 696f 736f 6674 7761 7265  /inveniosoftware
 00000150: 2f74 6561 6d73 2f32 3335 3337 2f67 6c2f  /teams/23537/gl/
 00000160: 290a 506c 7572 616c 2d46 6f72 6d73 3a20  ).Plural-Forms: 
 00000170: 6e70 6c75 7261 6c73 3d32 3b20 706c 7572  nplurals=2; plur
 00000180: 616c 3d28 6e20 213d 2031 293b 0a4d 494d  al=(n != 1);.MIM
 00000190: 452d 5665 7273 696f 6e3a 2031 2e30 0a43  E-Version: 1.0.C
 000001a0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/gl/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: Persian (Iran) (https://app.transifex.com/inveniosoftware/teams/23537/fa_IR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: gl\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: fa_IR\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: invenio_theme/config.py:102 invenio_theme/config.py:117
 #: invenio_theme/templates/invenio_theme/page.html:26
 #: invenio_theme/templates/invenio_theme/page_admin.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html:34
 msgid "Invenio"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/hr/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/hr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: hr\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hr/)\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/hr/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/no/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: hr\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Language: no\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_theme/config.py:102 invenio_theme/config.py:117
 #: invenio_theme/templates/invenio_theme/page.html:26
 #: invenio_theme/templates/invenio_theme/page_admin.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html:34
 msgid "Invenio"
 msgstr ""
 
 #: invenio_theme/ext.py:73
 msgid "Home"
-msgstr "Početna stranica"
+msgstr "Hovedsiden"
 
 #: invenio_theme/templates/invenio_theme/401.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/401.html:13
 msgid "Unauthorized"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/401.html:14
@@ -90,25 +90,25 @@
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:17
 msgid "Toggle navigation"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/admin_header.html:72
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:72
 msgid "Logout"
-msgstr "Odjavi se"
+msgstr "Logg ut"
 
 #: invenio_theme/templates/invenio_theme/footer.html:22
 #, python-format
 msgid "Powered by <a href=\"%(link)s\">Invenio</a>"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header.html:38
 #: invenio_theme/templates/semantic-ui/invenio_theme/header.html:46
 msgid "Search"
-msgstr "Pretraži"
+msgstr "Søk"
 
 #: invenio_theme/templates/invenio_theme/header_frontpage.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html:32
 msgid "Type and press enter to search"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header_login.html:12
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/hu/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Andrea Dömötör, 2022\n"
 "Language: hu\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/hu/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/hu/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/it/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/it/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
 "Language: it\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/it/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/it/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/it/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ja/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/ja/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: ja\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ja/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ja/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ja\n"
+"Language: zh_TW\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: invenio_theme/config.py:102 invenio_theme/config.py:117
 #: invenio_theme/templates/invenio_theme/page.html:26
 #: invenio_theme/templates/invenio_theme/page_admin.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html:34
 msgid "Invenio"
 msgstr ""
 
 #: invenio_theme/ext.py:73
 msgid "Home"
-msgstr "ホーム"
+msgstr "主頁"
 
 #: invenio_theme/templates/invenio_theme/401.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/401.html:13
 msgid "Unauthorized"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/401.html:14
@@ -90,25 +90,25 @@
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:17
 msgid "Toggle navigation"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/admin_header.html:72
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:72
 msgid "Logout"
-msgstr "ログアウト"
+msgstr "登出"
 
 #: invenio_theme/templates/invenio_theme/footer.html:22
 #, python-format
 msgid "Powered by <a href=\"%(link)s\">Invenio</a>"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header.html:38
 #: invenio_theme/templates/semantic-ui/invenio_theme/header.html:46
 msgid "Search"
-msgstr "検索"
+msgstr "搜尋"
 
 #: invenio_theme/templates/invenio_theme/header_frontpage.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html:32
 msgid "Type and press enter to search"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header_login.html:12
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ka/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/ka/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: ka\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ka/)\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ka/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/ka/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/lt/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/lt/LC_MESSAGES/messages.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: lt\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/lt/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/lt/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/lt/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/messages.pot` & `invenio-theme-2.1.3/invenio_theme/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/no/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/no/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: no\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/no/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/no/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/ro/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # Translations template for invenio-theme.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-theme
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2020
+# Tibor Simko <tibor.simko@cern.ch>, 2016
+# Nicolaie Constantinescu, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Last-Translator: Nicolaie Constantinescu, 2023\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/teams/23537/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: no\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ro\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: invenio_theme/config.py:102 invenio_theme/config.py:117
 #: invenio_theme/templates/invenio_theme/page.html:26
 #: invenio_theme/templates/invenio_theme/page_admin.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html:34
 msgid "Invenio"
 msgstr ""
 
 #: invenio_theme/ext.py:73
 msgid "Home"
-msgstr "Hovedsiden"
+msgstr ""
 
 #: invenio_theme/templates/invenio_theme/401.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/401.html:13
 msgid "Unauthorized"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/401.html:14
@@ -90,40 +91,40 @@
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:17
 msgid "Toggle navigation"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/admin_header.html:72
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:72
 msgid "Logout"
-msgstr "Logg ut"
+msgstr "Logout"
 
 #: invenio_theme/templates/invenio_theme/footer.html:22
 #, python-format
 msgid "Powered by <a href=\"%(link)s\">Invenio</a>"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header.html:38
 #: invenio_theme/templates/semantic-ui/invenio_theme/header.html:46
 msgid "Search"
-msgstr "Søk"
+msgstr "Caută"
 
 #: invenio_theme/templates/invenio_theme/header_frontpage.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html:32
 msgid "Type and press enter to search"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header_login.html:12
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:15
 msgid "Log in"
-msgstr ""
+msgstr "Log in"
 
 #: invenio_theme/templates/invenio_theme/header_login.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:19
 msgid "Sign up"
-msgstr ""
+msgstr "Sign up"
 
 #: invenio_theme/templates/invenio_theme/header_login.html:30
 #: invenio_theme/templates/invenio_theme/header_login.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:44
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:52
 msgid "Log out"
 msgstr ""
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/pl/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: pl\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/"
 "pl/)\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/pl/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/pl/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/pt/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: pt\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/"
 "teams/23537/pt/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/pt/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/pt/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/teams/23537/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pt\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ro/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-theme 1.3.28\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-09-16 08:40+0000\n"
-"PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language: ro\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/ro/)\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
-"2:1));\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Search"
-msgstr "Caută"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ro/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/ja/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # Translations template for invenio-theme.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-theme
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2016
+# Tibor Simko <tibor.simko@cern.ch>, 2020
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/teams/23537/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ro\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
+"Language: ja\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: invenio_theme/config.py:102 invenio_theme/config.py:117
 #: invenio_theme/templates/invenio_theme/page.html:26
 #: invenio_theme/templates/invenio_theme/page_admin.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html:34
 msgid "Invenio"
 msgstr ""
 
 #: invenio_theme/ext.py:73
 msgid "Home"
-msgstr ""
+msgstr "ホーム"
 
 #: invenio_theme/templates/invenio_theme/401.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/401.html:13
 msgid "Unauthorized"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/401.html:14
@@ -90,25 +90,25 @@
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:17
 msgid "Toggle navigation"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/admin_header.html:72
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:72
 msgid "Logout"
-msgstr ""
+msgstr "ログアウト"
 
 #: invenio_theme/templates/invenio_theme/footer.html:22
 #, python-format
 msgid "Powered by <a href=\"%(link)s\">Invenio</a>"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header.html:38
 #: invenio_theme/templates/semantic-ui/invenio_theme/header.html:46
 msgid "Search"
-msgstr "Caută"
+msgstr "検索"
 
 #: invenio_theme/templates/invenio_theme/header_frontpage.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html:32
 msgid "Type and press enter to search"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header_login.html:12
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ru/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: ru\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ru/)\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/ru/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/uk/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # Translations template for invenio-theme.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-theme
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2020
+# Tibor Simko <tibor.simko@cern.ch>, 2016
+# Vasyl Ostrovskyi <vasyusya@yahoo.com>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Last-Translator: Vasyl Ostrovskyi <vasyusya@yahoo.com>, 2023\n"
+"Language-Team: Ukrainian (https://app.transifex.com/inveniosoftware/teams/23537/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ru\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Language: uk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: invenio_theme/config.py:102 invenio_theme/config.py:117
 #: invenio_theme/templates/invenio_theme/page.html:26
 #: invenio_theme/templates/invenio_theme/page_admin.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html:34
 msgid "Invenio"
 msgstr ""
 
 #: invenio_theme/ext.py:73
 msgid "Home"
-msgstr "Главная страница"
+msgstr "Головна сторінка"
 
 #: invenio_theme/templates/invenio_theme/401.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/401.html:13
 msgid "Unauthorized"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/401.html:14
@@ -54,15 +55,15 @@
 #: invenio_theme/templates/semantic-ui/invenio_theme/403.html:14
 msgid "You do not have sufficient permissions to view this page."
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/404.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/404.html:13
 msgid "Page not found"
-msgstr "Страница не найдена"
+msgstr ""
 
 #: invenio_theme/templates/invenio_theme/404.html:14
 #: invenio_theme/templates/semantic-ui/invenio_theme/404.html:14
 msgid "The page you are looking for could not be found."
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/429.html:13
@@ -90,52 +91,52 @@
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:17
 msgid "Toggle navigation"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/admin_header.html:72
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:72
 msgid "Logout"
-msgstr "Выход"
+msgstr "Вийти"
 
 #: invenio_theme/templates/invenio_theme/footer.html:22
 #, python-format
 msgid "Powered by <a href=\"%(link)s\">Invenio</a>"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header.html:38
 #: invenio_theme/templates/semantic-ui/invenio_theme/header.html:46
 msgid "Search"
-msgstr "Искать"
+msgstr "Пошук"
 
 #: invenio_theme/templates/invenio_theme/header_frontpage.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html:32
 msgid "Type and press enter to search"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header_login.html:12
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:15
 msgid "Log in"
-msgstr ""
+msgstr "Увійти"
 
 #: invenio_theme/templates/invenio_theme/header_login.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:19
 msgid "Sign up"
-msgstr ""
+msgstr "Зареєструватись"
 
 #: invenio_theme/templates/invenio_theme/header_login.html:30
 #: invenio_theme/templates/invenio_theme/header_login.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:44
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:52
 msgid "Log out"
-msgstr ""
+msgstr "Вийти"
 
 #: invenio_theme/templates/invenio_theme/page_settings.html:19
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html:25
 msgid "Settings"
-msgstr ""
+msgstr "Налаштування"
 
 #: invenio_theme/templates/invenio_theme/macros/truncate.html:12
 msgid "Show more"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/macros/truncate.html:13
 msgid "Show less"
@@ -150,16 +151,16 @@
 
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:75
 msgid "Skip to main"
 msgstr ""
 
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html:17
 msgid "My account"
-msgstr ""
+msgstr "Мій обліковий запис"
 
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html:21
 msgid "Account settings"
 msgstr ""
 
 #: invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html:33
 msgid "Close"
-msgstr ""
+msgstr "Закрити"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/rw/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/ne/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-theme 1.3.28*

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 d801 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 d301 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d74 6865 6d65 2031   invenio-theme 1
 00000050: 2e33 2e32 380a 5265 706f 7274 2d4d 7367  .3.28.Report-Msg
 00000060: 6964 2d42 7567 732d 546f 3a20 696e 666f  id-Bugs-To: info
 00000070: 4069 6e76 656e 696f 736f 6674 7761 7265  @inveniosoftware
 00000080: 2e6f 7267 0a50 4f54 2d43 7265 6174 696f  .org.POT-Creatio
 00000090: 6e2d 4461 7465 3a20 3230 3232 2d30 392d  n-Date: 2022-09-
 000000a0: 3136 2030 383a 3430 2b30 3030 300a 504f  16 08:40+0000.PO
 000000b0: 2d52 6576 6973 696f 6e2d 4461 7465 3a20  -Revision-Date: 
 000000c0: 3230 3136 2d30 382d 3235 2031 353a 3238  2016-08-25 15:28
 000000d0: 2b30 3030 300a 4c61 7374 2d54 7261 6e73  +0000.Last-Trans
 000000e0: 6c61 746f 723a 2046 554c 4c20 4e41 4d45  lator: FULL NAME
 000000f0: 203c 454d 4149 4c40 4144 4452 4553 533e   <EMAIL@ADDRESS>
-00000100: 0a4c 616e 6775 6167 653a 2072 770a 4c61  .Language: rw.La
-00000110: 6e67 7561 6765 2d54 6561 6d3a 204b 696e  nguage-Team: Kin
-00000120: 7961 7277 616e 6461 2028 6874 7470 733a  yarwanda (https:
-00000130: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
-00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
-00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
-00000160: 7277 2f29 0a50 6c75 7261 6c2d 466f 726d  rw/).Plural-Form
-00000170: 733a 206e 706c 7572 616c 733d 323b 2070  s: nplurals=2; p
-00000180: 6c75 7261 6c3d 286e 2021 3d20 3129 3b0a  lural=(n != 1);.
-00000190: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
-000001a0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
-000001b0: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
-000001c0: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
-000001d0: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
-000001e0: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
-000001f0: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
-00000200: 3132 2e31 0a00                           12.1..
+00000100: 0a4c 616e 6775 6167 653a 206e 650a 4c61  .Language: ne.La
+00000110: 6e67 7561 6765 2d54 6561 6d3a 204e 6570  nguage-Team: Nep
+00000120: 616c 6920 2868 7474 7073 3a2f 2f61 7070  ali (https://app
+00000130: 2e74 7261 6e73 6966 6578 2e63 6f6d 2f69  .transifex.com/i
+00000140: 6e76 656e 696f 736f 6674 7761 7265 2f74  nveniosoftware/t
+00000150: 6561 6d73 2f32 3335 3337 2f6e 652f 290a  eams/23537/ne/).
+00000160: 506c 7572 616c 2d46 6f72 6d73 3a20 6e70  Plural-Forms: np
+00000170: 6c75 7261 6c73 3d32 3b20 706c 7572 616c  lurals=2; plural
+00000180: 3d28 6e20 213d 2031 293b 0a4d 494d 452d  =(n != 1);.MIME-
+00000190: 5665 7273 696f 6e3a 2031 2e30 0a43 6f6e  Version: 1.0.Con
+000001a0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000001b0: 706c 6169 6e3b 2063 6861 7273 6574 3d75  plain; charset=u
+000001c0: 7466 2d38 0a43 6f6e 7465 6e74 2d54 7261  tf-8.Content-Tra
+000001d0: 6e73 6665 722d 456e 636f 6469 6e67 3a20  nsfer-Encoding: 
+000001e0: 3862 6974 0a47 656e 6572 6174 6564 2d42  8bit.Generated-B
+000001f0: 793a 2042 6162 656c 2032 2e31 322e 310a  y: Babel 2.12.1.
+00000200: 00                                       .
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/rw/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: Hindi (India) (https://app.transifex.com/inveniosoftware/teams/23537/hi_IN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: rw\n"
+"Language: hi_IN\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_theme/config.py:102 invenio_theme/config.py:117
 #: invenio_theme/templates/invenio_theme/page.html:26
 #: invenio_theme/templates/invenio_theme/page_admin.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html:34
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/sk/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2022\n"
 "Language: sk\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/"
 "sk/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/sk/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/sk/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2022\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/sv/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,28 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
+"Last-Translator: Rim Sharif, 2023\n"
 "Language: sv\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Account settings"
 msgstr "Kontoinställningar"
 
 msgid "Close"
-msgstr "Stänga"
+msgstr "Stäng"
 
 msgid "Error identifier"
 msgstr "Felidentifierare"
 
 msgid "Home"
 msgstr "Hem"
 
@@ -41,15 +41,15 @@
 msgid "Logout"
 msgstr "Logga ut"
 
 msgid "My account"
 msgstr "Mitt konto"
 
 msgid "Page not found"
-msgstr "sidan hittas inte"
+msgstr "Sidan hittas inte"
 
 msgid "Permission required"
 msgstr "Tillstånd krävs"
 
 msgid ""
 "Powered by\n"
 "        <a href=\"%(link)s\">Invenio</a>"
@@ -60,44 +60,44 @@
 msgid "Powered by <a href=\"%(link)s\">Invenio</a>"
 msgstr "Drivs av <a href=\"%(link)s\">Invenio</a>"
 
 msgid "Search"
 msgstr "Sök"
 
 msgid "Settings"
-msgstr "inställningar"
+msgstr "Inställningar"
 
 msgid "Show less"
 msgstr "Visa mindre"
 
 msgid "Show more"
 msgstr "Visa mer"
 
 msgid "Sign up"
-msgstr "Skriva upp"
+msgstr "Registrera konto"
 
 msgid "Skip to main"
 msgstr "Hoppa till main"
 
 msgid "The page you are looking for could not be found."
 msgstr "Sidan du letar efter kunde inte hittas."
 
 msgid "Toggle navigation"
 msgstr "Växla navigering"
 
 msgid "Too many requests"
-msgstr "För många begäran"
+msgstr "För många förfrågningar"
 
 msgid "Type and press enter to search"
 msgstr "Skriv och tryck enter för att söka"
 
 msgid "Unauthorized"
 msgstr "Obehörig"
 
 msgid "You do not have sufficient permissions to view this page."
-msgstr "Du har inte tillräckliga behörigheter för att se den här sidan."
+msgstr "Du har inte behörigheten för att se den här sidan."
 
 msgid "You have made too many consecutive requests, please try again later."
 msgstr "Du har gjort för många förfrågningar i följd, försök igen senare."
 
 msgid "You need to be authenticated to view this page."
 msgstr "Du måste vara autentiserad för att se den här sidan."
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/sv/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/sv/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 # This file is distributed under the same license as the invenio-theme
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2020
 # Sam Arbid, 2022
+# yyones, 2023
+# Rim Sharif, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Last-Translator: Rim Sharif, 2023\n"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/teams/23537/sv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
@@ -50,30 +52,30 @@
 #: invenio_theme/templates/semantic-ui/invenio_theme/403.html:13
 msgid "Permission required"
 msgstr "Tillstånd krävs"
 
 #: invenio_theme/templates/invenio_theme/403.html:14
 #: invenio_theme/templates/semantic-ui/invenio_theme/403.html:14
 msgid "You do not have sufficient permissions to view this page."
-msgstr "Du har inte tillräckliga behörigheter för att se den här sidan."
+msgstr "Du har inte behörigheten för att se den här sidan."
 
 #: invenio_theme/templates/invenio_theme/404.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/404.html:13
 msgid "Page not found"
-msgstr "sidan hittas inte"
+msgstr "Sidan hittas inte"
 
 #: invenio_theme/templates/invenio_theme/404.html:14
 #: invenio_theme/templates/semantic-ui/invenio_theme/404.html:14
 msgid "The page you are looking for could not be found."
 msgstr "Sidan du letar efter kunde inte hittas."
 
 #: invenio_theme/templates/invenio_theme/429.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/429.html:13
 msgid "Too many requests"
-msgstr "För många begäran"
+msgstr "För många förfrågningar"
 
 #: invenio_theme/templates/invenio_theme/429.html:14
 #: invenio_theme/templates/semantic-ui/invenio_theme/429.html:14
 msgid "You have made too many consecutive requests, please try again later."
 msgstr "Du har gjort för många förfrågningar i följd, försök igen senare."
 
 #: invenio_theme/templates/invenio_theme/500.html:13
@@ -116,27 +118,27 @@
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:15
 msgid "Log in"
 msgstr "Logga in"
 
 #: invenio_theme/templates/invenio_theme/header_login.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:19
 msgid "Sign up"
-msgstr "Skriva upp"
+msgstr "Registrera konto"
 
 #: invenio_theme/templates/invenio_theme/header_login.html:30
 #: invenio_theme/templates/invenio_theme/header_login.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:44
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_login.html:52
 msgid "Log out"
 msgstr "Logga ut"
 
 #: invenio_theme/templates/invenio_theme/page_settings.html:19
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html:25
 msgid "Settings"
-msgstr "inställningar"
+msgstr "Inställningar"
 
 #: invenio_theme/templates/invenio_theme/macros/truncate.html:12
 msgid "Show more"
 msgstr "Visa mer"
 
 #: invenio_theme/templates/invenio_theme/macros/truncate.html:13
 msgid "Show less"
@@ -161,8 +163,8 @@
 
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html:21
 msgid "Account settings"
 msgstr "Kontoinställningar"
 
 #: invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html:33
 msgid "Close"
-msgstr "Stänga"
+msgstr "Stäng"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/tr/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,15 +3,15 @@
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume."
 "com>, 2022\n"
 "Language: tr\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/tr/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/tr/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/tr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/uk/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,24 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-theme 1.3.28\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-09-16 08:40+0000\n"
-"PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language: uk\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/uk/)\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
-"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
-"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
-"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Home"
-msgstr "Головна сторінка"
-
-msgid "Search"
-msgstr "Пошук"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/uk/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/hr/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # Translations template for invenio-theme.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-theme
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2016
+# Tibor Simko <tibor.simko@cern.ch>, 2020
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: uk\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"Language: hr\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
 #: invenio_theme/config.py:102 invenio_theme/config.py:117
 #: invenio_theme/templates/invenio_theme/page.html:26
 #: invenio_theme/templates/invenio_theme/page_admin.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html:34
 msgid "Invenio"
 msgstr ""
 
 #: invenio_theme/ext.py:73
 msgid "Home"
-msgstr "Головна сторінка"
+msgstr "Početna stranica"
 
 #: invenio_theme/templates/invenio_theme/401.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/401.html:13
 msgid "Unauthorized"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/401.html:14
@@ -90,25 +90,25 @@
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:17
 msgid "Toggle navigation"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/admin_header.html:72
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:72
 msgid "Logout"
-msgstr ""
+msgstr "Odjavi se"
 
 #: invenio_theme/templates/invenio_theme/footer.html:22
 #, python-format
 msgid "Powered by <a href=\"%(link)s\">Invenio</a>"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header.html:38
 #: invenio_theme/templates/semantic-ui/invenio_theme/header.html:46
 msgid "Search"
-msgstr "Пошук"
+msgstr "Pretraži"
 
 #: invenio_theme/templates/invenio_theme/header_frontpage.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html:32
 msgid "Type and press enter to search"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header_login.html:12
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Kalven Richie, 2022\n"
 "Language: zh_CN\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/"
 "teams/23537/zh_CN/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Kalven Richie, 2022\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-theme-2.1.3/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
 "Language: zh_TW\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/"
 "teams/23537/zh_TW/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-theme-2.1.2/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-theme-2.1.3/invenio_theme/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 # Translations template for invenio-theme.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-theme
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2020
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme 1.3.28\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-09-16 08:40+0000\n"
 "PO-Revision-Date: 2016-08-25 15:28+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2020\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: German (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/de_AT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: zh_TW\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: de_AT\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_theme/config.py:102 invenio_theme/config.py:117
 #: invenio_theme/templates/invenio_theme/page.html:26
 #: invenio_theme/templates/invenio_theme/page_admin.html:34
 #: invenio_theme/templates/semantic-ui/invenio_theme/page.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html:34
 msgid "Invenio"
 msgstr ""
 
 #: invenio_theme/ext.py:73
 msgid "Home"
-msgstr "主頁"
+msgstr ""
 
 #: invenio_theme/templates/invenio_theme/401.html:13
 #: invenio_theme/templates/semantic-ui/invenio_theme/401.html:13
 msgid "Unauthorized"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/401.html:14
@@ -90,25 +86,25 @@
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:17
 msgid "Toggle navigation"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/admin_header.html:72
 #: invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html:72
 msgid "Logout"
-msgstr "登出"
+msgstr ""
 
 #: invenio_theme/templates/invenio_theme/footer.html:22
 #, python-format
 msgid "Powered by <a href=\"%(link)s\">Invenio</a>"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header.html:38
 #: invenio_theme/templates/semantic-ui/invenio_theme/header.html:46
 msgid "Search"
-msgstr "搜尋"
+msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header_frontpage.html:29
 #: invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html:32
 msgid "Type and press enter to search"
 msgstr ""
 
 #: invenio_theme/templates/invenio_theme/header_login.html:12
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-theme-2.1.2/invenio_theme/views.py` & `invenio-theme-2.1.3/invenio_theme/views.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme/webpack.py` & `invenio-theme-2.1.3/invenio_theme/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/invenio_theme.egg-info/PKG-INFO` & `invenio-theme-2.1.3/invenio_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme
-Version: 2.1.2
+Version: 2.1.3
 Summary: "Invenio standard theme."
 Home-page: https://github.com/inveniosoftware/invenio-theme
 Author: Invenio Collaboration
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -48,14 +48,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.3 (released 2023-07-24)
+        
+        - messages: add z-index
+        
         Version 2.1.2 (released 2023-04-12)
         
         - add flex utility classes
         - add text sizes classes
         
         Version 2.1.1 (released 2023-04-06)
```

### Comparing `invenio-theme-2.1.2/invenio_theme.egg-info/SOURCES.txt` & `invenio-theme-2.1.3/invenio_theme.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -257,40 +257,64 @@
 invenio_theme/translations/ca/LC_MESSAGES/messages.po
 invenio_theme/translations/cs/LC_MESSAGES/messages.mo
 invenio_theme/translations/cs/LC_MESSAGES/messages.po
 invenio_theme/translations/da/LC_MESSAGES/messages.mo
 invenio_theme/translations/da/LC_MESSAGES/messages.po
 invenio_theme/translations/de/LC_MESSAGES/messages.mo
 invenio_theme/translations/de/LC_MESSAGES/messages.po
+invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo
+invenio_theme/translations/de_AT/LC_MESSAGES/messages.po
+invenio_theme/translations/de_DE/LC_MESSAGES/messages.mo
+invenio_theme/translations/de_DE/LC_MESSAGES/messages.po
 invenio_theme/translations/el/LC_MESSAGES/messages.mo
 invenio_theme/translations/el/LC_MESSAGES/messages.po
+invenio_theme/translations/en_AT/LC_MESSAGES/messages.mo
+invenio_theme/translations/en_AT/LC_MESSAGES/messages.po
+invenio_theme/translations/en_HU/LC_MESSAGES/messages.mo
+invenio_theme/translations/en_HU/LC_MESSAGES/messages.po
 invenio_theme/translations/es/LC_MESSAGES/messages.mo
 invenio_theme/translations/es/LC_MESSAGES/messages.po
+invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo
+invenio_theme/translations/es_CU/LC_MESSAGES/messages.po
+invenio_theme/translations/es_MX/LC_MESSAGES/messages.mo
+invenio_theme/translations/es_MX/LC_MESSAGES/messages.po
 invenio_theme/translations/et/LC_MESSAGES/messages.mo
 invenio_theme/translations/et/LC_MESSAGES/messages.po
 invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo
 invenio_theme/translations/et_EE/LC_MESSAGES/messages.po
 invenio_theme/translations/fa/LC_MESSAGES/messages.mo
 invenio_theme/translations/fa/LC_MESSAGES/messages.po
+invenio_theme/translations/fa_IR/LC_MESSAGES/messages.mo
+invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po
 invenio_theme/translations/fr/LC_MESSAGES/messages.mo
 invenio_theme/translations/fr/LC_MESSAGES/messages.po
+invenio_theme/translations/fr_CI/LC_MESSAGES/messages.mo
+invenio_theme/translations/fr_CI/LC_MESSAGES/messages.po
+invenio_theme/translations/fr_FR/LC_MESSAGES/messages.mo
+invenio_theme/translations/fr_FR/LC_MESSAGES/messages.po
 invenio_theme/translations/gl/LC_MESSAGES/messages.mo
 invenio_theme/translations/gl/LC_MESSAGES/messages.po
+invenio_theme/translations/hi_IN/LC_MESSAGES/messages.mo
+invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po
 invenio_theme/translations/hr/LC_MESSAGES/messages.mo
 invenio_theme/translations/hr/LC_MESSAGES/messages.po
 invenio_theme/translations/hu/LC_MESSAGES/messages.mo
 invenio_theme/translations/hu/LC_MESSAGES/messages.po
+invenio_theme/translations/hu_HU/LC_MESSAGES/messages.mo
+invenio_theme/translations/hu_HU/LC_MESSAGES/messages.po
 invenio_theme/translations/it/LC_MESSAGES/messages.mo
 invenio_theme/translations/it/LC_MESSAGES/messages.po
 invenio_theme/translations/ja/LC_MESSAGES/messages.mo
 invenio_theme/translations/ja/LC_MESSAGES/messages.po
 invenio_theme/translations/ka/LC_MESSAGES/messages.mo
 invenio_theme/translations/ka/LC_MESSAGES/messages.po
 invenio_theme/translations/lt/LC_MESSAGES/messages.mo
 invenio_theme/translations/lt/LC_MESSAGES/messages.po
+invenio_theme/translations/ne/LC_MESSAGES/messages.mo
+invenio_theme/translations/ne/LC_MESSAGES/messages.po
 invenio_theme/translations/no/LC_MESSAGES/messages.mo
 invenio_theme/translations/no/LC_MESSAGES/messages.po
 invenio_theme/translations/pl/LC_MESSAGES/messages.mo
 invenio_theme/translations/pl/LC_MESSAGES/messages.po
 invenio_theme/translations/pt/LC_MESSAGES/messages.mo
 invenio_theme/translations/pt/LC_MESSAGES/messages.po
 invenio_theme/translations/ro/LC_MESSAGES/messages.mo
@@ -299,18 +323,22 @@
 invenio_theme/translations/ru/LC_MESSAGES/messages.po
 invenio_theme/translations/rw/LC_MESSAGES/messages.mo
 invenio_theme/translations/rw/LC_MESSAGES/messages.po
 invenio_theme/translations/sk/LC_MESSAGES/messages.mo
 invenio_theme/translations/sk/LC_MESSAGES/messages.po
 invenio_theme/translations/sv/LC_MESSAGES/messages.mo
 invenio_theme/translations/sv/LC_MESSAGES/messages.po
+invenio_theme/translations/sv_SE/LC_MESSAGES/messages.mo
+invenio_theme/translations/sv_SE/LC_MESSAGES/messages.po
 invenio_theme/translations/tr/LC_MESSAGES/messages.mo
 invenio_theme/translations/tr/LC_MESSAGES/messages.po
 invenio_theme/translations/uk/LC_MESSAGES/messages.mo
 invenio_theme/translations/uk/LC_MESSAGES/messages.po
+invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo
+invenio_theme/translations/uk_UA/LC_MESSAGES/messages.po
 invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo
 invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po
 invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo
 invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po
 tests/conftest.py
 tests/helpers.py
 tests/test_invenio_theme.py
```

### Comparing `invenio-theme-2.1.2/requirements-devel.txt` & `invenio-theme-2.1.3/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/setup.cfg` & `invenio-theme-2.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/tests/conftest.py` & `invenio-theme-2.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/tests/helpers.py` & `invenio-theme-2.1.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/tests/test_invenio_theme.py` & `invenio-theme-2.1.3/tests/test_invenio_theme.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.1.2/tests/test_invenio_theme_error_handler.py` & `invenio-theme-2.1.3/tests/test_invenio_theme_error_handler.py`

 * *Files identical despite different names*

